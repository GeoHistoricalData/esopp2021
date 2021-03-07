## Comptage des rues Révolutionnaires et des autres
** Rues non révolutionnaires lisibles**
```sql=
SELECT voie, count(voie) FROM
(
SELECT lower(c_voies_approx) as voie, c_nomruerevolutionnaire
FROM cartes_de_surete.security_cards_current_address_import
WHERE c_voies_approx NOT ILIKE '%illisible%'
) as sub
WHERE c_nomruerevolutionnaire = '--'
GROUP BY voie
ORDER BY count(voie) DESC
```


**Rues révolutionnaires lisibles**
```sql=
SELECT c_nomruerevolutionnaire, count(c_nomruerevolutionnaire) FROM
(
SELECT lower(c_voies_approx) as voie, c_nomruerevolutionnaire
FROM cartes_de_surete.security_cards_current_address_import
WHERE c_voies_approx NOT ILIKE '%illisible%'
) as sub
WHERE c_nomruerevolutionnaire != '--'
GROUP BY c_nomruerevolutionnaire
ORDER BY count(c_nomruerevolutionnaire) DESC
```

** Tous les occurences des 20 rues les plus fréquentes non révolutionnaires**
```sql=
SELECT lower(c_voies_approx)
FROM cartes_de_surete.security_cards_current_address_import
WHERE lower(c_voies_approx) IN (
  SELECT voie
  FROM (
  SELECT lower(c_voies_approx) as voie, c_nomruerevolutionnaire
  FROM cartes_de_surete.security_cards_current_address_import
  WHERE c_voies_approx NOT ILIKE '%illisible%' ) as sub
  WHERE c_nomruerevolutionnaire = '--'
  AND voie NOT ILIKE '%cours & enclos%'
  GROUP BY voie
  ORDER BY count(voie) DESC
  LIMIT 20
)
```

** Cartes par section en proportion de toutes les cartes attribuées à une section**
```sql
SELECT section_id, MAX(section_revolutionnaire[1]), COUNT(*)::double precision/175231.0 AS cards_ratio, MAX(geom) as geom 
FROM cartes_de_surete.security_cards_current_address_import 
JOIN cartes_de_surete.sections_revolutionnaires as s 
ON section_id = s.section_id::text 
GROUP BY section_id 
ORDER BY section_id
```


**Nombre de cartes émises par par section et année rapportée au nombre totale de cartes émises dans chaque section**
```sql

SELECT 100.*ncards / (SELECT count(*) FROM cartes_de_surete.cartes_de_surete_import WHERE section_id = sub.section_id)  as propcards
,date_emission, section_id, geom 
FROM 
(
  SELECT count(*) as ncards, EXTRACT(YEAR FROM rc_date::date) AS date_emission, section_id, MAX(geom) as geom 
  FROM cartes_de_surete.cartes_de_surete_import AS c
  JOIN cartes_de_surete.sections_revolutionnaires as s 
  ON section_id = s.id_section::text 
  GROUP BY EXTRACT(YEAR FROM rc_date::date), section_id 
  ORDER BY EXTRACT(YEAR FROM rc_date::date), section_id
) AS sub
WHERE ncards != 0
```


** Cumul des cartes émises par section à différentes périodes clés, rapporté au total des cartes émises dans chaque section**
```sql
-- Première période : jusqu'au 18 septembre 1792 (décret relatif aux mesures de sûreté et de tranquillité publique pour la ville de Paris)
SELECT 100.*ncards / (SELECT count(*) FROM cartes_de_surete.cartes_de_surete_import WHERE section_id = sub.section_id) as propcards, section_id, geom 
FROM ( 
  SELECT count(*) as ncards, section_id, MAX(geom) as geom
  FROM cartes_de_surete.cartes_de_surete_import AS c
  JOIN cartes_de_surete.sections_revolutionnaires as s
  ON section_id = s.id_section::text
  WHERE rc_date::date < '1792-09-19'::date
  GROUP BY section_id
) AS sub
WHERE ncards != 0 

-- Au 31 décembre 1792
SELECT 100.*ncards / (SELECT count(*) FROM cartes_de_surete.cartes_de_surete_import WHERE section_id = sub.section_id) as propcards, section_id, geom 
FROM ( 
  SELECT count(*) as ncards, section_id, MAX(geom) as geom
  FROM cartes_de_surete.cartes_de_surete_import AS c
  JOIN cartes_de_surete.sections_revolutionnaires as s
  ON section_id = s.id_section::text
  WHERE rc_date::date <= '1792-12-31'::date
  GROUP BY section_id
) AS sub
WHERE ncards != 0 


-- Au 6 octobre 1793 (15 vendémiaire an II)
SELECT 100.*ncards / (SELECT count(*) FROM cartes_de_surete.cartes_de_surete_import WHERE section_id = sub.section_id) as propcards, section_id, geom 
FROM ( 
  SELECT count(*) as ncards, section_id, MAX(geom) as geom
  FROM cartes_de_surete.cartes_de_surete_import AS c
  JOIN cartes_de_surete.sections_revolutionnaires as s
  ON section_id = s.id_section::text
  WHERE rc_date::date <= '1793-10-05'::date
  GROUP BY section_id
) AS sub
WHERE ncards != 0 

-- À la fin de l'an II - 21 septembre 1794
SELECT 100.*ncards / (SELECT count(*) FROM cartes_de_surete.cartes_de_surete_import WHERE section_id = sub.section_id) as propcards, section_id, geom 
FROM ( 
  SELECT count(*) as ncards, section_id, MAX(geom) as geom
  FROM cartes_de_surete.cartes_de_surete_import AS c
  JOIN cartes_de_surete.sections_revolutionnaires as s
  ON section_id = s.id_section::text
  WHERE rc_date::date <= '1794-09-21'::date
  GROUP BY section_id
) AS sub
WHERE ncards != 0 

-- À partir de l'an III: 1794-09-22 et +
SELECT 100.*ncards / (SELECT count(*) FROM cartes_de_surete.cartes_de_surete_import WHERE section_id = sub.section_id) as propcards, section_id, geom 
FROM ( 
  SELECT count(*) as ncards, section_id, MAX(geom) as geom
  FROM cartes_de_surete.cartes_de_surete_import AS c
  JOIN cartes_de_surete.sections_revolutionnaires as s
  ON section_id = s.id_section::text
  WHERE rc_date::date <= '1802-01-01'::date
  GROUP BY section_id
) AS sub
WHERE ncards != 0 
```


**Cartes délivrées chaque mois pour chaque façade**
```sql=

SELECT count(id), to_char(rc_date::date, 'YYYY-MM') AS ym, facade_grp_id, max(geom) as geom, max(section) as section
FROM cartes_de_surete.cards_join_facade_group jointable
JOIN cartes_de_surete.cartes_de_surete_import cards
ON jointable.card_id = cards.id
JOIN cartes_de_surete.verniquet_facades_with_sections facades_groups
ON jointable.facade_grp_id = facades_groups.gid
GROUP BY to_char(rc_date::date, 'YYYY-MM'), facade_grp_id
```

SELECT count(*) as ncards, EXTRACT(YEAR FROM rc_date::date) AS date_emission, section_id, MAX(geom) as geom FROM cartes_de_surete.cartes_de_surete_import AS c JOIN cartes_de_surete.sections_revolutionnaires as s ON section_id = s.id::text GROUP BY EXTRACT(YEAR FROM rc_date::date), section_id ORDER BY EXTRACT(YEAR FROM rc_date::date), section_id



SELECT count(*), max(clocher_nomcart) as nomcart, st_transform(st_setsrid(st_point(lon,lat),4326),2154) as geom
from cartes_de_surete.r_insee_domicile_precedent_import
where clocher_nomcart not ilike 'paris'
group by st_point(lon,lat)


SELECT coalesce(SUM(cartes),0), g.geom FROM
(
  SELECT count(*) as cartes, max(clocher_nomcart) as nomcart, st_transform(st_setsrid(st_point(lon,lat),4326),2154) as geom
  from cartes_de_surete.r_insee_domicile_precedent_import
  where clocher_nomcart not ilike 'paris'
  group by st_point(lon,lat)
) AS s
RIGHT JOIN cartes_de_surete.grid_hex_france AS g
ON ST_WITHIN(s.geom, g.geom)
GROUP BY g.geom 