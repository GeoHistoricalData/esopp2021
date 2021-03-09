---
title: Situer (1) les populations dans l’espace et dans le temps
tags: esopp, geohistoricaldata,ladehis, partie 1, historique
description: Présentation du 10 mars 2021 dans le séminaire du groupe ESOPP
---
Liens vers les autres documents : 
[Carnet de notes générales](https://hackmd.iscpif.fr/kifrM1xQQZyLSemvdOkx9A?both) -- 
[Partie 1, historique du labo](https://hackmd.io/k5x0vZDWQ7q8rwYRzrKj0Q) --
[Partie 2, travail sur les sources, Cassini](https://hackmd.io/CsCqUq7ZQQCI8GnWAB7LjQ) --
[Partie 3, outils collaboratifs, Paris](https://hackmd.io/C5W_HUx6TjOz9HXxguQhNQ) --
[Pres_2020_google](https://docs.google.com/presentation/d/1Jxqyg3TLefsDdbKPURSWT7sGq91LF03-7sv_sn2NR2I/edit?usp=sharing ) --
[Résumé_2020_google](https://docs.google.com/document/d/1ZJ6LYhT782eK6p7od7IZGjnRFJBttzkg3xakRWiAd2c/edit?usp=sharing) -- [Prefig groupe HistoireSocialePopulationEspace](https://hackmd.io/7_nk2gBlQSOFnPSObrzfsg)

---

# Situer (1) les populations dans l’espace et dans le temps

***Quelques expériences collectives de construction et d'exploitation des sources & données géo-historiques (France, 1750-2000)***

**Stéphane Baciocchi, Pascal Cristofoli et Bertrand Duménieu (LaDéHIS - CRH UMR 8558 EHESS-CNRS)**

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_Vectorisation.png)



![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/logo_soduco.png =75x) 
![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/logo_geohistoricaldata.png =75x) 

---

# Partie 0 - Introduction

Reprise ici du brouillon ESOPP (Espace) - les sources et données micro-historique et leurs références spatiales (*geohistoricaldata*). L'idée même de laboratoire (en sciences sociales)

<div style="text-align: justify; font-size: x-small"> 
L’étude du rapport entre les populations du passé, leurs pratiques sociales et l’espace géographique dans lesquelles elles se déploient et s’organisent peut s’appuyer sur des systèmes d’information géographiques (SIG), outils numériques dédiés à la représentation et l’analyse de phénomènes spatiaux.

Ils traitent des données géo-historiques modélisant les formes de l’espace et les informations sociales localisées, construites à partir du croisement de cartes et plans anciens avec les multiples traces documentaires attestant de l’insertion des pratiques individuelles dans l’espace géographique à un moment donné : localisations relatives, adresses, affectations à des unités administratives, etc.

Une partie des travaux menés au sein du présent groupe exploite ces outils pour suivre dans le temps et dans l’espace des données individuelles en grand nombre tout en raisonnant à plusieurs niveaux d’échelle et de granularité d’observation (de l’espace métropolitain aux parcelles cadastrales, des individus aux groupements de population).
Ce parti pris résolument spatial invite à constituer ou re-visiter de larges bases de données géo-historiques. Il implique des choix méthodologiques forts : des modélisations explicites et un travail nécessairement collectif et collaboratif pour produire des données ouvertes.
</div>

    Etude des phénomènes historiques, dans leurs contextes et représentations, étude des évolutions des structures et institutions, des pratiques et des phénomènes sociaux.

---

# P1 - Retour réflexif sur une succession de travaux qui ont en commun la production de référentiels géo-historique sur *l'histoire administrative et démographique de l'espace et du territoire français métropolitain*

## P1.1 Introduction : Réflexions sur plusieurs enquêtes collectives menées au sein d'un laboratoire de sciences sociales

### P1.1.1 - Un Laboratoire d'histoire et de démographie

- Le lieu de cette enquête : 
le laboratoire de démographie historique (1973-2010) et laboratoire de démographie et d'histoire sociale (2011-2021). (CRH - EHESS - CNRS)

Page de présentation du laboratoire sur le site Web institutionnel (ladehis.ehess.fr/): 

<div style="text-align: justify; font-size: small"> 
<b>En choisissant le terme de laboratoire, on a souhaité insister sur le caractère expérimental, sur la modélisation et sur la quantification</b>. Historiens et démographes travaillent au LaDéHiS avec des juristes, des sociologues, des géographes, des informaticiens et des géomaticiens. Ils restent en contact étroit avec des linguistes, des paléontologues, des mathématiciens des biologistes et des géographes.

En accord avec la vocation initiale de l'EHESS, le laboratoire s'intéresse aux problèmes, non aux disciplines qui constituent des outils mais non des fins. Historiquement, le LaDéHiS a pleinement participé aux avancées de la connaissance qu'a permises l'exploitation rationnelle des registres paroissiaux. Il s'engage désormais sur de nouveaux territoires en construisant et discutant les représentations du passé qu'il s'agisse de concepts, de catégories ou d'images et de cartes. <b>Il cherche à lier les parcours et les destins individuels aux institutions et aux agrégats statistiques censés les résumer.</b>

Il met ainsi en oeuvre un va et vient entre les données les plus diverses issues du passé, la perception et les catégories par lesquelles elles ont été exprimées à l'époque et leur interprétation présente. Il s'attache à <b>situer ces informations passées avec le maximum de précision</b> (géoréférencement) et à <b>mettre en valeur l'importance de l'espace dans le développement de la démographie et de la société</b>, particulièrement au XIXe siècle
</div>

----

#### P1.1.1.1 Démographie historique et histoire sociale - Production de "données" à partir de sources documentaires

- Histoire démographique des populations du passé
Démographie historique, Histoire de l'administration, Histoire sociale, Histoire des populations
- "Histoire quantitiative", histoire et mesure, morphologie et processus sociaux
De l'étude des données agrégées et liens statistiques à celle des données "individuelles" en grand nombre et liens "interindividuels"
- Production de "données" et la constitution d'instruments de recherche et d'outils pour la recherche

----

#### P1.1.1.2 Des travaux de recherches ancrées dans l'espace géographique

Un intêret pour l'espace dans les recherche d'histoire sociale. Spatialisation des phénomènes sociaux:
    
- Populations et espace
H. Le Bras -  les 3 Frances / Travaux Datar au niveau communal
Ex: Cartes de fécondité ? (départementales / communales / lissages)
Etudes des Migrations MG et PA
- Histoire de l'espace Parisien
Début 2000, premiers travaux SIG sur l'histoire de Paris au LDH
Séminaires et ouvrages de M. Gribaudi.

*Ce travail, mené en parallèle à ce que je vais présenter, sera abordé dans les 2ème et 3ème partie de la présentation.*
- Cartographie et géomatique
Importance de la cartographie et des cartographes (Laboratoire de Graphique de l'EHESS), puis de la géomatique et des géomaticiens (A. Vitu et F. Pirot (Centre compétence Thématique SIG) - Carlo Bertelli, Univ. Piémont) - Ecole Nationale des sciences géograpiques - Laboratoire COGIT de l'IGN) 

----

#### P1.1.1.3 Un Laboratoire de sciences sociales

L'idèe même de laboratoire :
- Produire des "données" à partie de sources documentaires dans le cadre des problématiques de recherche
- Mise au point d'outils, de dispositifs techniques
- Un lieux pour engager des travaux collectifs
- Un laboratoire marqué par la forte présence de personnels d'appui à la recherche (ingénieurs, documentalistes, cartographes)
- Un laboratoire expérimentateur et usager des outils et procédures informatiques, avec de nombreuses "collaborations" avec des informaticiens.
- Stabilité relative de la structure dans le temps long de la recherche. 

----

###  P1.1.2 L'étude de la trajectoire formée par une succession d'enquête

#### Distinction de trois moments (périodes / stades d'évolution)

- Collection *Paroisses & Communes de France* (1970-2012) - Des dictionnaires départementaux d'hitoire administrative et démographique
- Site *Cassini.ehess.fr* (1996-2012) - Un instrument à l'échelle de la France métropolitaine de la révolution à nos jours
- Groupe *Geohistoricaldata* (2009-2021) - Exploitation d'une source : la Carte générale de la France dite de Cassini

Multiples faces d'un objet particulier et délimité, mais qui des inflexions au grès de l'évolution des programmes scientifiques, des opportunités et contraintes offertes par des changements institutionnels, des évolutions technologiques et techniques (notamment informatiques), mais aussi des parcours des hommes et des femmes qui y ont participé, qui ont souhaité le faire avancer, le relancer, bifurquer.
Une lecture à posteriori de 50 ans de travaux réalisé au sein d'une équipe de recherche en constante évolution.
Lecture qui met en lumière des continuités, des contextes et des préoccupations scientifiques différents.
Une insistance sur la dernière période : pourquoi et comment travailler avec une source cartographique et produire des données géo-historiques.

####  Adopter une démarche réflexive 
- Importance du contexte socio-technique, plus particulièrement les relations avec l'informatique (contexte matériel, technique et humain) 
- sur le contexte historiographique et l'évolution des questionnements scientifiques
- sur les collaborations scientifiques et l'interdisciplinarité
- sur le contexte institutionel et financier de la recherche en SHS

####  Aborder des questions générales sur la recherche en SHS

- Travail collectif en SHS et le rapport avec les recherches et parcours individuels, relations et conflits inter-individuels ?
- Contexte historiographique et cycles scientifiques ?
- Importance et rôle des opportunités et inovations techniques dans le travail scientifique ?
- Pérénité des données ? le cumul des résultats, cumul des expériences ? Qu'est-ce qu'une enquête vivante, quand s'arrête-elle ? Temporalité du travail en SHS.

---

## P1.2 - La Collection des Dictionnaires *Paroisses & Communes de France* 1965-2012

#### Introduction

"Histoire du peuplement de la France"
Combler des manques sur l'histoire de la population: Chiffres publiés par l'INSEE à Partir de 1954 - Code géographique national : 1943.

Ambition P&C : populations contemporaines et ancien régime, ressorts administratifs. par département et par commune.

Un modèle:Dictionnaires de topographie
Etats annuels vs historique
Repérage dans les fonds documentaires. Documents : situés dans l'espace. localisation indirecte (toponymes, adresses)

----

### P1.2.1 Genèse et débuts  d'une collection.

#### Un chantier ouvert sous les auspice de Marcel Reinhard
- 1967, création de l'ERA n°68 constitué en 1967 sous la présdence de M. Reinhard ( titulaire de la chaine d’histoire de la Révolution Française de Sorbonne). J. Dupaquier Assistant de Reinhard
Les 6 dictionnaires de la région parisienne ont été réalisé avec l'aide financière du CNRS dans cette équipe

- En 1968, J. Dupaquier est désigné maitre-assistant à l'École pratique des hautes études

- 1969-1970 : Rapport du Centre de recherche Historique (EHESS)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Rapport_activite_CRH_1969_1970_DicosPetC.png)

- 1973, Création du Laboratoire de démographie historique à l'EHESS. J. Dupaquier ()
- 1974, accord du CNRS pour la publication (Lettre à Jean-Pierre Bardet)


#### Bilan d'une enquête nationale, le dictionnaire NRS . LDH, 6 janvier 1975.

#### Dictionnaires P&C, Perspectives de publications 1982-1983, Réponse aux Editions du CNRS, 1982

<div style="text-align: justify; font-size: small"> 
On pourra noter que la distribution des dictionnaires est assez dispersée sur le plan géographique. Ce phénomène résulte évidemment de la disponibilité des auteurs. Toutefois, <b>nous avons réussi à conduie avec l'aide du CNRS et de la région Rhône-Alpes unéritable action concertée</b>. A ce jour pratiquement tous les dictionnaires départementaux de cette région sont publiés. Ceci présente un grand intérêt pour l'analyse synthétique des données : il devieent possible de déplacer le cadre étroit et souvent artificiel (du moins pour l'Ancien Régime) du département et de préparer à une échelle convenable les études globales.""
</div>

----

### P1.2.2 Les dictionnaires P&C - Période 1974-2000

*Un dictionnaire est publié en 2012, mais c'est à l'initiative et avec le financement des Archives de l'Ariège. Plusieurs dictionnaire sont en état d'être publiés.*


![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/PetC_resume.png)

----

#### P1.2.2.1 Dictionnaires P&C - Fiche communale

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/DicoPetC_fichesmanuscrites.png)

#### P1.2.2.2 Dictionnaires P&C - Cartographie

G. Arbelot, Bilan de la cartographie présente dans les dictionnaires P&C, 1984
![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/dico_PetC_bilan_carto.png)

##### Mouvement communal - Exemple

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/DicoPetC_fiches_mouvementcomm.png)

----


#### P1.2.2.3 Dictionnaires P&C - Un instrument de travail

Poulat Emile. *Paroisses et communes de France*. In: Archives de sciences sociales des religions, n°56/2, 1983. pp. 191-193.
DOI : https://doi.org/10.3406/assr.1983.2297

##### Klapish-Zuber, N° spécial 50 ans du RH, cahier du CRH, 2005. 

<div style="text-align: justify; font-size: small"> 
« Le travail de préparation est long et pour partie répétitif, et il est naturel qu’il ne mobilise pas à plein temps les chercheurs. Peut-être faudra-il au total cinquante ans pour que cette gigantesque entreprise soit menée à son terme… Mais le CRH n’est-il pas précisément l’un des lieux où peut se concevoir et s’exécuter ce type de recherche, inaccessible à l’initiative individuelle ? »
</div>
<div style="text-align: justify; font-size: x-small"> 
Netter M-L, Klapisch-Zuber C. Cinquante ans d’histoire au Centre de Recherches Historiques. Les Cahiers du Centre de Recherches Historiques, 2005, p. 138 ; Disponible sur : http://ccrh.revues.org/3048.
</div>

Présentation "Rapports du CRH"


### P1.2.3 "Travailler à plusieurs"

#### P1.2.3.1 Une équipe de réalisation :

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/PetC_1996_Dordogne_credits.png =500x)

1985, Claude Motte s'occupe de la collection.

#### P1.2.3.2 Auteurs et collaborateurs
<div style="text-align: justify; font-size: small"> 
<b>J. Dupâquier et al.</b>, <i>75-Paris et Région parisienne</i>, 1974, 921 p. ; <b>F. Lebrun</b>, 49-Maine-et-Loire, 1974, 464 p. ; <b>G. Bellart et al.</b>, 62-Pas-de-Calais, 1975, 1475 p. ; <b>A. Molinier</b>, 07-Ardèche, 1976, 464 p. ; <b>R. Lemaire</b>, 60-Oise, 1976, 877 p. ; <b>A. Vitu</b>, 10-Aube, 1977, 640 p. ; <b>J.-P. Kintz</b>, 67-Bas-Rhin, 1977, 688 p. ; <b>G. Brunet et al.</b>, 01-Ain, 1978, 580 p. ; <b>M. Garden</b>, 69-Rhône, 1978, 384 p. ; <b>M.-C. Roederer</b>, 11-Aude, 1979, 560 p. ; <b>Ph. Canu</b>, 58-Nièvre, 1979, 472 p. ; <b>D. Barbero</b>, 73-Savoie, 1979, 422 p. ; <b>D. Barbero</b>, 74-Haute-Savoie, 1980, 492 p. ; <b>I. Empereur-Bissonnet</b>, 87-Haute-Vienne, 1981, 328 p. ; <b>M.-E. Martin</b>, 26-Drôme, 1982, 557 p. ; <b>Ch. Poitou</b>, 45-Loiret, 1982, 315 p. ; <b>R.-J. Bernard</b>, 48-Lozère, 1982, 313 p. ; <b>B. Bonnin et al.</b>, 38-Isère, 1983, 715 p. ; <b>R. Plessix</b>, 72-Sarthe, 1983, 492 p. ; <b>M. Boucher</b>, 51-Marne, 1984, 801 p. ; <b>Ph. Hercule</b>, 17-Charente-Maritime, 1985, 628 p. ; <b>D. Lacroix</b>, 30-Gard, 1986, 478 p. ; <b>J.-P. Pélissier</b>, 66-Pyrénées-Orientales, 1986, 375 p. ; <b>R. Sicard</b>, 84-Vaucluse, 1986, 262 p. ; <b>Ch. Lippold</b>, 19-Corrèze, 1988, 406 p. ; <b>R. Le Mée et al.</b>, 77-Seine-et-Marne, 1988, 942 p. ; <b>Cl. Motte et al.</b>, 34-Hérault, 1989, 490 p. ; <b>J.-Cl. Farcy et al.</b>, 28-Eure-et-Loir, 1990, 586 p. ; <b>Cl. Renard</b>, 35-Ille-et-Vilaine, 1990, 466 p. ; <b>H. Baldit</b>, 15-Cantal, 1991, 392 p. ; <b>S. Beauvalet-Boutouyrie, Cl. Motte</b>, 55-Meuse, 1992, 763 p. ; <b>F. Casta</b>, 20-Corse, 1993, 530 p. ; <b>C. Canu, G. Arbellot</b>, 18-Cher, 1994, 568 p. ; <b>J.-P. Kintz</b>, 68-Haut-Rhin et T. de Belfort, 1994, 660 p. ; <b>J.-P. Brun</b>, 05-Hautes-Alpes, 1995, 288 p. ; <b>G. Florenty</b>, 24-Dordogne, 1996, 884 p. ; <b>Ch. Poitou</b>, 36-Indre, 1997, 580 p. ; <b>Ch. Poitou</b>, 41-Loir-et-Cher, 1997, 591 p. ; <b>Ch. Poitou</b>, 23-Creuse, 2000, 865 p. ;</br>
<b>C. Pailhès, C. Motte</b>, 09-Ariège, 2012, 917 p. (Edité par les Archives départementales de l'Ariège).
</div>

### P1.2.4. L'informatisation des données des dictionnaires

### Des collaborations scientifiques techniques

L. Henry, Démographie et histoire
Interdisciplinarité
Relations tumultueuses entre informatique et histoire
Zysberg André, 1987, « Impact de l’informatique sur la recherche historique », Matériaux pour l’histoire de notre temps, 1987, p. 35‑37.

#### L'Objet physique "dictionnaire" est différent de la "banque" de données associée
Multiples tentatives pour constituer une "banque de donnée"
- La banque de données initiale : fiches papier
- Exemple 1976-1977 : Entreprise MATEVA - Saisie dictionnaire + Banque de données (échec)
- Travail avec le Laboratoire Informatique pour les sciences humaines (LISH-FMSH) (Fiches perforées) : banque de données Paroisses et communes de France
- Micro-ordinateurs:
Apple 2E : Dictionnaires produits entre 1985 et 1988 ; IBM: Dictionnaires produits après 1988.
- Tentatives de récupération des données des années anciennes (Stéphane Vari sur Bandes)

#### Chaine technique d'édition des derniers dictionnaires:
Micro-informatique
- Tableau Excel contenant la base de données et les colonnes formatés
- Opération de publipostage sous Word (un modèle de fiche sur Word et chargement des données Excel)
- Intégration des pages éditoriales (Introduction, cartes, bibliographie)
- Envoi du fichier Word complet à l'éditeur
- L'éditeur le retravaille avec un logiciel d'édition spécialisé (Xpress)

## P1.3 - Le site Cassini.ehess.fr (1996-2006) : Ne pas s'arréter au milieu du guêt

### P1.3.1 - En route vers le site Cassini


#### P1.3.1.1 - Des contraintes, des opportunités et des choix

##### P1.3.1.1.1 - Un changement du contexte (1985-1995)

- Tournant critique en histoire
Fin des années 1980 et Début 1990: essouflement de la démographie historique traditionnelle, et arrivée de la micro-histoire (M. Gribaudi)
En 1986, création de la revue "Histoire et Mesure".
Travaux sur l'espace de H. le Bras (diffusion, cartes de lissage, échelle communale) et sur les migrations et les réseaux (M. Gribaudi, P.-A. Rosental)
<div style="text-align: justify; font-size: small"> 
Cf. Dupâquier J. <i>Pour la démographie historique</i>. Paris, France: Presses Universitaires de France, impr. 1984, 1984. et la recension de B. Lepetit dans les annales (Annales Économies, Sociétés, Civilisations 1985;40:145).
</div>

- Des changements au LDH
Débat Lebras-INED-Dupaquier sur la natalité; 
Passage au ministère de J.-P. Bardet et passage professeur à Paris IV-Sorbonne (1987). Retraite de J. Dupâquier
Hervé Le Bras directeur du LDH en 1987, Formation doctorale "Démographie et sciences sociales" (1990-1996).
B. Lepetit, bref directeur de la collection P&C (1985) devient directeur d'études à l'EHESS (1989) et directeur du CRH en 1992. il décède en 1996. 

- L'impact de l'*Atlas de la révolution Française*
Publication de Atlas de la révolution Française (11 volumes), dont 2 volumes sur le territoire, 1 sur la démographie et 1 autre sur le réseau Routier.
*Un bilan national sur le passage de l'Ancien régime et XIXème siècle accompagné d'une production cartographique en collaboration avec le Laboratoire de Graphique.*

- L'"Abandon" de la collection par les éditions du CNRS. Finalisation des dictionnaires en chantier, mais peu de nouveaux projets.
Avec l'appui d'H. Bras, C. Motte, directrice de la rédaction P&C, recherche des financements (ex: dossier Fondation Philipp Morris en 1995) et des moyens pour "terminer" d'une manière ou d'une autre la collection.
 

##### P1.3.1.1.2 Convention EHESS-INED (1997-2003): complétion, harmonisation et publication de le base de données sur le mouvement communal depuis 1801

CD-Rom : fichiers pdf contenant l'ensemble des index et des fiches communales reliés par des liens hypertextes (nombre de pages : )

<div style="text-align: justify; font-size: small"> 
Claude Motte, I. Séguy et C. Théré, avec la coll. de D. Tixier-Basse, <i>Commune d'hier, communes d'aujourd'hui. Les communes de la France métropolitaine, 1801-2001. Dictionnaire d’histoire administrative</i>, INED, 2003, VIII + 408 pages, livre et CD Rom, Préface de G. Lang, Réalisation graphique A. Varet-Vitu, Assistance informatique A. Bringé et P. Cristofoli (Réalisation CD-Rom).</div>

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/commune_hier_communes_auj.png  )

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/mouvement_comm_dessin.png)

----

##### P1.3.1.1.3 Subvention Ministère de l'équipement (PUCA) : DVD-ROM populations depuis la révolution pour l'ensemble de la France métroplotaine

- Opportunité de compléter le recueil des chiffres de population pour la période post-révolutionnaire sur l'ensemble du territoire.
Plusieurs sources mobilisées pour harmoniser et stabiliser une base de donnée globale sur la population et le mouvement communal (fichier Ined, Liste de 1801 et ses imperfections + recensements (AD + AN + INSEE) et code géographique offciel)

- L'opportunité de la publication numérique de la Carte de Cassini par la BNF au début des années 2000

<div style="text-align: justify; font-size: small"> 
La <i>Carte Générale et Particulière de la France</i>, dite “de Cassini” prend appui sur la première triangulation géodésique du royaume [2,5], cette carte monumentale réalisée au 1:86 400e (ou “une ligne pour 100 toises”) a été divisée en 182 planches de dimensions 610x955mm. Elle dépeint le territoire français de la seconde moitié du XVIIIe siècle et décrit avec finesse et détails les lieux habités et nommés, les divers édifices religieux, les réseaux routiers principaux, la topographie et l’hydrographie du royaume de France.<br>
<br><b>La BNF publie en 2004 les 180 planches de la carte de Cassini en Couleur (dit "Exemplaire de la Reine")</b><br>
</div>

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini1999_F2_1_F0000098_BR.png  )

- Projet initial de CD-ROM ou DVD-ROM de belle facture qui se transforme en cours de travail en projet de réalisation d'un site web dynamique éditorialisé.

<div style="text-align: justify; font-size: x-small">
Motte C, Vouloir M-C. "Les villages de Cassini. Un projet de céréome". In: Genet J-P, Pennetier C, Romero Passerin d’Entrèves G, éditeurs. In: <i>Histoire et informatique III: quels CD Rom pour l’enseignement et la recherche ?</i>i> Paris, France: Publications de la Sorbonne, 1997:65-75.
</div> 

---

#### P1.3.1.2 - Les particularités de l'objet: (complexité et gros volume) suscitent l'intérêt des informaticiens et géomaticiens

##### Un objet imposant et complexe
- notamment par son caractère dynamique, 200 ans.
- Des problèmes spécifiques : enclaves, cantons urbains
    Données floue, pas sûres ou manquantes...
- Un objet imposant (40 000 communes, 37 recensements, 80 000 toponymes, 3 niveaux hiéarchiques administratifs pour la période post révolutionnaire)
- Gérer des sources éparses et contr^le des données: AD / Journal officiel / Archives nationnales / INSEE

#### Un objet multi-échelle (granularité):
- échelles géographiques, échelles temporelles
- La commune - La paroisse et travail à l'échelle de l'ensemble la France 
- liens de hiérarchie: Pouvoir passer de la donnée "individuelle" au territoire local, régional, national (canton, arrondissments, départements)
- liens entre objets : mouvement communal et "généalogies" des communes
- Gérer les disparités locales, régionnales et historiques

---

### P1.3.2 Le site cassini.ehess.fr : des villages de Cassini aux communes d'aujourd'hui

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Site_cassini_vue_generale.png )

<div style="text-align: justify; font-size: x-small">
Motte C, Vouloir M-C. Des villages Cassini aux communes d’aujourd’hui. territoires et populations, deux siècles d’évolution. [2004, version 1] [2006, version 2]. Disponible sur : http://cassini.ehess.fr/.
</div>

#### P1.3.2.1 De nouvelles tâches et collaborations 

- Apparition de la géomatique:
Entreprise générale d'infographie, IGN, ENSG
- Contexte institutionnel : Service informatique de Recherche de l'EHESS (Dirigé par HLB) :
Hébergement des serveurs - contraintes techniques
- Une entreprise pour gérer l'aspect visuel du site (CSS)
- De nouvelles compétences : Travail de traitement d'image
Découpage des planches (Exemplaire de la Reine, pliable)
Assemblage des planches et Géoréférencement

----

##### Carte originale numérisée par la BNF, feuille n°2

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini1999_F2_2_coin_HD_F0000098.png)

----

##### Carte decoupée et assemblage des morceaux à l'intérieur des feuilles et entre feuilles (feuille n°2) 

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini1999_F2_3_coinHD_recolle.png)

----

##### Assemblage des 182 feuilles de Cassini 

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_assemblage.png)

----

### P1.3.2.1 Evolution des dispositifs techniques et nouvelles possibilités
- Transformation du fichier Excel en "Base de données" : discussions homériques avec informaticiens : lever les implicites, préciser les choses

- Web dynamique (Interogation en ligne d'une base de données (MySQL) via des pages web dynamiques (PHP et JavaScript))
Opération analogue au publipostage: (Passage de 40 000 pages web potentielles (web statique) à un patron de page affichant à la demande les informations pour une commune) 

- Serveur géographique : Affichage de la Carte avec niveaux de zoom

- La question de la mise à jour des données.
Modification de données
Modifications de structure
Faire en sorte que la personne qui se charge des modification puisse utiliser les outils (Question de l'apprentissage de nouveaux outils et de la formation des personnels : choix et coûts)
Solution maintien d'une BD ACCESS, transformation en MySQL et re-chargement de la BD sur le Site.


### P1.3.2.2 Les Notices communales 

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/sitecassini_notice0.png)

----

### P1.3.2.3 Un index et une recherche à l'échelle de la France

##### Module de recherche du site Cassini

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/sitecassini_recherche.png)

----

##### Module de recherche du site Cassini

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/sitecassini_index.png)

----

### P1.3.2.3 Une entreprise collective : la page "partenaires" du Site

**Remerciements**
<div style="text-align: justify; font-size: small">
À celles et ceux qui, dès l’origine, ont accordé leur <b>soutien</b> à cette réalisation et plus spécialement :
Madame Anne-Marie Meunier, directeur financier de la recherche, EHESS ; Madame Monique Pelletier, directrice du département Cartes et Plans, BNF ;
Madame Hélène Richard, directrice du département Cartes et plans, BNF ; Monsieur Hervé Le Bras, directeur du Laboratoire de Démographie historique, EHESS ; Monsieur Alain Wauters, Inspecteur général de la construction, Conseil général des ponts et chaussées.<br>
Aux membres du <b>Comité de pilotage</b>, composé de représentants des ministères de l’Équipement, de l’Environnement et de l’Intérieur, de la BNF et de l’EHESS / CNRS, qui ont accompagné et guidé les travaux de l’équipe de réalisation.
<br><br></div>

**Institutions partenaires et entreprises prestataires**
<div style="text-align: justify; font-size: small">
<b>Partenaires scientifiques</b>: Ecole des Hautes études en sciences sociales, EHESS ; Bibliothèque nationale, BNF ; Centre national de la recherche scientifique, CNRS ; Institut national d'études démographiques, INED.<br>
<b>Partenaire financier</b>: Ministère de l’Équipement, du Logement, du Tourisme et de la Mer, DGUHC-PUCA.<br> 
<b>Entreprises prestataires</b>: Digitech International ; Société Géomod ; Société Générale d’Infographie ; Institut Géographique National, IGN-Conseil ; École Nationale des Sciences Géographiques ; Société Atelier-des-Signes.<br><br></div>

**Equipe de réalisation**
<div style="text-align: justify; font-size: small">
<b>Conception et coordination</b>: Claude Motte et Marie-Christine Vouloir, Laboratoire de Démographie historique, EHESS/CNRS, avec la participation d’Aleksandra Sarrabezolles, BNF.<br>
<b>Suivi des travaux</b>: Roland Gomez, DGUHC-PUCA<br>
<b>Préparation du fonds Cassini, légende et informations sur les feuilles</b>: Marie-Christine Vouloir<br>
<b>Constitution de la base de données</b>: Claude Motte, Pascal Cristofoli (EHESS), Anahi Morales<br>
<b>Rédaction des dossiers</b>: Monique Pelletier et Jean-Paul Saint-Aubin (Univ. Paris I) ; Claude Motte<br>
<b>Géo-référencement du fonds Cassini</b>: Claude Yvon, Frédéric Bizet, société Géomod<br>
<b>Validation du logiciel de conversion Cassini/Lambert II</b>: Dominique Lévêque, IGN-Conseil.<br>
<b>Réalisation du site et de la base de données MySQL:</b> Éric Pennors, Pierre-André Le Ny, société Générale d’Infographie ; Élodie Buard, Xavier Chaze, Sébastien Giordano, Erwann Houzay, Benoït Kiene, École nationale des sciences géographiques, IT 2e année.<br>
<b>Conception graphique</b>: Franklin Desclouds, société Atelier-des-Signe
<br></div>


----

### P1.3.2.5 Un site de référence : Wikipedia / Geoportail IGN

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/wikipedia_geoportail.png)

### P1.3.2.6 Une idée du mouvement communal à l'échelle de la france entre 1790 et 2004

##### Nombre d'évènements communaux par année

- Evenements communaux affectant les communes dans la base Cassini : création de commune, absorption d'une commune, Transferts de territoire

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cevt0Evolutions_evt_territoriaux_orig17932004..png )

- Un fond de carte actuelle pour visualiser les évènements du passé : la localisation de l'occurence des évènements communaux est réalisée à l'aide du fond de Carte des surfaces communales actuelles (Carte Geo-FLA 2013)

----

##### Localisation des communes actuelles (2013) ayant vécu des évènements communaux

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cevtall.png )
    
----

##### Communes actuelles (2013) ayant vécu des évènements communaux entre 1790-1793

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cevt1.png )
    
----

##### Communes actuelles (2013) ayant vécu des évènements communaux entre 1794-1815

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cevt2.png )
    
----

##### Communes actuelles (2013) ayant vécu des évènements communaux entre 1816-1848

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cevt3.png )
    
----

##### Communes actuelles (2013) ayant vécu des évènements communaux entre 1849-1958

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cevt4.png )
    
----

##### Communes actuelles (2013) ayant vécu des évènements communaux entre 1959-2004

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cevt5.png )
    
---

## P1.4 A la découverte de la carte de(s) Cassini (2006-2020)

### P1.4.1 introduction : De l'images à la carte numérique

#### Un glissement progressif :
- la carte comme illustration (Site BNF)
- La carte comme localisation dans l'espace (et dans le temps) (Site Cassini.ehess.fr)
- La carte comme source d'informations
-- Comment elle a été réalisé
-- Ce qui y est représenté
-- Ce que cela nous dit des territoires d'autrefois

*Le travail de saisie et les premières lectures morphologiques de la vectorisation ouvrent plusieurs questions sur :
la carte elle même, le formes et les contextes de sa production, le statut des objets représentés, etc.
les phénomènes qu’on croit pouvoir lire à travers les formes représentées,
les rapports qu’il est possible d’établir avec des autres bases de données etc.*


#### Faire connaissance avec la carte
- Site Cassini.ehess.fr 
- ANR Geopeuple (2009-2012): première plongée dans la carte et collaboration avec Laboratoire IGN-COGIT et 
- Etude des sources sur la réalisation de la Carte :
ouvrages et minutes de Cassini
- Nouvelle version de la carte de Cassini publiée par la BNF

<div style="text-align: justify; font-size: small">
François de Dainville, <i>Le Langage des géographes. Termes, Signes, Couleurs des cartes anciennes, 1500-1800</i>, Paris, Éditions A. et J. Picard & Cie, 1964, 384 p.<br>
M. Pelletier, <i>La Carte de Cassini. L’extraordinaire aventure de la Carte de France</i>, Presses de l’École nationale des Ponts et Chaussées, Paris, 1990, 263 p.<br>
M. Pelletier, <i>Les cartes des Cassini : la science au service de l'État et des régions</i> , Paris, Éd. du CTHS, 2002.<br>
</div>

----

Carte BNF 2004 :

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini1999_F2_F0000098_detail.png)

----

Carte BNF 2015 :

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini2015_F2_detail.png )

----

#### La légende de la carte de Cassini

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini_LegendeNetB_0.png)

<div style="text-align: justify; font-size: x-small"> 
J.-C. Dezauche, Tableau de la France divisé par gouvernement et provinces pour servir à l'assemblage et à l'intelligence des 180 cartes levées géométriquement par ordre du Roi. BNF. Cartes et Plans. Ge F pièce 10913 (Cité par Monique Pelletier, 2002, p. 224-225)
</div>

----

#### La réalisation de la carte de Cassini, une enquête de long terme sur le royaume de France

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_feuille_annees.png)

----

#### La réalisation de la carte de Cassini, Première carte Géométrique

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_arpenteurs.png)

---

### P1.4.2 Une plongée collective au dans le territoire retracé par la Carte de Cassini

#### P1.4.2.1 Suivre les routes de Cassini à l'écchelle de la France (2013-2015)


##### P1.4.2.1.1 Geohistoricaldata : l'expérimentation d'une saisie collaborative des sources catographique

- Programme initié à partir de 2013 par M. Gribaudi, J. Perret (IGN-COGIT) et Marc. Barthelemy (CAMS)
Travail sur l'histoire de Paris (M. Gribaudi)
Séminaire collectif sur la Morphologie (CAMS-LaDéHiS)
Suite du travail de M. Bartelemy et M. Gribaudi sur l'évolution des filaires des rues parisiennes.

<div style="text-align: justify; font-size: small"> 
Barthelemy Marc, Bordin Patricia, Berestycki Henri et Gribaudi Maurizio, 2013, « Self-organization versus top-down planning in the evolution of a city », <i>Scientific Reports</i>, 8 juillet 2013, vol. 3.<br><br>
</div>

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/paris_contexte.png )

<div style="text-align: justify; font-size: small"> 
<b>Participant assidus ou temporaires du groupe Geohistoricaldata depuis 2013</b> : N. Abadie, S. Baciocchi, M. Barthélémy, P. Bernard, C. Bertelli, O. Bonin, P. Bordin, A. Bretagnolle, J. Chadeyron, L. Clavier, L. Costa, B. Costes, P. Cristofoli, J.M. Delaveau, B. Dumenieu, S. Gomis, J. Gravier, M. Gribaudi, C. Hoarau, J.P. Hubert, I. Langlois, P.A. Le Ny, E Mermet, C. Mimieur, C. Motte, M. Pardoen, J. Perret, O. Pigez, A.M. Raimond, A.N. Regond, S. Robert, D. Shereen, T. Thevenin, A. Thomas, A. Varet-vitu, M.C. Vouloir et les participants des ateliers Cassini de Clermont-Ferrand.
</div>

----

- La promotion d'une démarche de saisie collaborative d'exploitation des sources cartographiques anciennes
le groupe de travail pluridisciplinaire GeoHistoricalData entreprend la vectorisation de l’information géographique gravée sur les cuivres de la Carte Générale et Particulière de la France, dite “de Cassini”.
- L'importance des géomaticiens et des informaticiens (administration système, programmation)
Collaboration: partager une façon de voir le travail. La carte comme source, garder la trace des opérations qui permettent de produire les données
- Des outils et une infrastructure dédiée:
Architecture serveur, logiciel libre de SIG QGIS et base de données PostgreSQL/PostGIS
- Contexte institutionnel : 
Au début et pendant quelques années Serveur informatique personnel. Accès au  Serveur EHESS (avec contraintes de sécurité), puis transport vers un serveur Huma-num.
La question et les enjeux de la maintenance informatique.

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini_routes_etapes_vectorisation_20132015.png)

----

##### P1.4.2.1.2 Vue d'ensemble et Des disparités régionales

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/SiteGeohistorical_org_vue_ensemble.png)

----

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/SiteGeohistorical_org_vue_ensemble_road.png)

----

##### P1.4.2.1.3 Des pratiques et des problématiques nouvelles 

- modéliation des données, la question et les débats autours des spécifications de saisie :
Ne pas imposer d'interprétation à priori.
Routes rouges, routes blanches, routes bordées d'arbre

- Le réseau routier et les villes
Au terme de la saisie : 112.391 km de routes,  1.133 km² de villes
Verification et correction de la topologie du réseau routier (avec 
l'extension Postgis Topology)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_routes_topology.png)

- Diffusion : Diffusion du jeu de données en Open Data
Un travail collectif : Question des crédits et de la reconnaissance du travail collectif en SHS.


<div style="text-align: justify; font-size: x-small"> 
- J. Perret, M. Gribaudi, M. Barthelemy, N. Abadie, S. Baciocchi, C. Bertelli, O. Bonin, P. Bordin, B. Costes, P. Cristofoli, B. Dumenieu, J. Gravier, J.-P. Hubert, P.-A. Le Ny, E. Mermet, C. Motte, M. Pardoen, A.-M. Raimond, S. Robert, and M.-C. Vouloir. The 18th century cassini roads and cities dataset, Harvard Dataverse, 2015. URL : https://doi.org/10.7910/DVN/28674.<br>
- J. Perret, M. Gribaudi, and M. Barthelemy. Roads and cities of 18th century france. Scientific data, 2 :150048, 2015. URL : https://doi.org/10.1038/sdata.2015.48.
</div>

##### P1.4.2.1.4 Bilan sur la saisie collaborative (dec. 2019)

###### Vue globale (Déc. 2019)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_Vectorisation.png)


###### Nombre mensuel de nouveaux objets saisis dans la base de données géo-historique (juil. 2013 - déc. 2019)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Geohist_saisie_collab_nouveaux_objets.png )

----

###### Nombre mensuel de modifications d'objets de la base de données géo-historique (juil. 2013 - déc. 2019)
![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Geohist_saisie_collab_modification_objets.png )

----

###### Nombre d'objets par type (Mars 2020)

    à faire (avec démarcation saisie complète ou non)

---

#### P1.4.3 L'édition critique de la Planche 52 (2016-2019)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_totale.png)

----

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_verso_titre.png)

----

##### P1.4.3.1 Une Vectorisation exhaustive de la Planche 52

<div style="text-align: justify; ">
Une première expérience de vectorisation exhaustive de la carte de Cassini géoréférencée a été menée sur la planche numéro 52, qui délimite un rectangle de 78 km de longueur et  48.7 km de largeur, englobant à l’ouest le Puy de Dôme et ses alentours, au centre la Limagne et Riom, Clermont-Ferrand et Issoire et à l’est Thiers et une partie des monts du Forez. Réalisé par environ 10 contributeurs à l’aide des logiciels de SIG QGIS et PostgreSQL/PostGIS, le travail collaboratif a permis d’identifier et d’extraire plus de 6 800 représentations d’entités géographiques qui forment désormais une base de données géohistorique relativement complète sur cette partie du Puy de Dôme. 
</div>

But comprendre le processus de fabrication de la carte, ce qu'elle contient. Faire une édition critique de la feuille

**Détail de la carte numérique:**

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_extrait.png )

----

##### P1.4.3.2 Des entités géographiques de nature différente

<div style="text-align: justify;">
Suivant la distinction faite par Cassini lui-même, la base de données est composée de deux catégories d’entités : <b>les entités géographiques triangulées (dénommées entités géométriques par Cassini)</b> dont les propriétés géodésiques sont partiellement documentées, et <b>les entités relatives (topographiques dans le vocabulaire de Cassini) positionnées relativement aux premières</b>. Ces entités sont analytiquement distinctes mais proviennent toutes d’une seule et unique source : les plaques de cuivre de la carte de Cassini dans lesquelles elles ont été gravées.<br><br>
</div>

cf. “Lettre du comte de Cassini  IV, adressée en 1784 aux États de Bretagne,” citée par C. Motte & M.-C. Vouloir (2007) 

<div style="text-align: justify; font-size: small">
<i>Les ingénieurs en partant de bases qui leur sont données ont cherché à déterminer, par des observations d’angles faites dans le plus grand nombre des clochers d’un canton, la position de tous les objets environnants qu’ils peuvent découvrir, et qui sont dans le cas d’être géométriquement décrits.<br> 
<b>La détermination précise n’a lieu que pour les objets qui intéressent, tels que villes, bourgs, villages et grands châteaux ; les petites chapelles, fermes et métairies, composées de trois ou quatre maisons ne peuvent se placer qu’à vue d’œil, surtout à une échelle aussi petite que la nôtre.</b><br> 
La topographie qui offre la description détaillée et scrupuleuse, non seulement des objets, mais même de la conformation du terrain, de l’élévation et du contour exact des vallées, des montagnes, des coteaux, des rivières, prés, bois,etc., est une partie de la géographie tellement étendue, si minutieuse, si longue et si coûteuse dans l’exécution, qu’elle ne peut être entreprise dans une carte générale...<br>
On n’a jamais prétendu en faire qu’un accessoire à la carte générale de la France. Pour la rendre plus agréable, <b>on y a joint, pour ainsi dire, une esquisse, une ébauche de topographie</b>.</i><br><br>
</div>

<div style="text-align: justify; font-size: x-small">
- C.-F. Cassini. <i>Description géométrique de la France</i>i>. Imprimerie Desaint. Google-Books-ID : RDReAAAAcAAJ.<br>
- F. de Dainville, "La carte de Cassini et son intérêt géographique." <i>Bulletin de l'Association de géographes français</i>, 32(251), 138-147, 1955. URL https://doi.org/10.3406/bagf.1955.8014.<br>
- J. V. Konvitz. "Redating and rethinking the cassini geodetic surveys of france, 1730–1750". <i>Cartographica : The International Journal for Geographic Information and Geovisualization</i>i>, 19(1) :1–15, 1982. URL https://doi.org/10.3138/W62K-3152-7062-5267.<br>
- C. Motte et M.-C. Vouloir, "le site cassini.ehess.fr, un instrument d’observation pour une analyse du peuplement", <i>revue du comité français de cartographie</i> n°191, 2007
</div>

----

**Principaux Triangles qui servent à la description Géométrique de la France**

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini_triangulation1.png)

<div style="text-align: justify; font-size: x-small">
Source : Carte générale de la France. Tableau d'assemblage, Nouvelle carte Qui Comprend les principaux Triangles qui servent à la description Géométrique de la France levée par ordre du Roy / Par Mess.rs Maraldi et Cassini de Thury, de l'Académie Royale des Sciences. Année 1744 ; Tracé d'après les Mesures, et gravé par Dheulland ; Aubin scripsit - (https://gallica.bnf.fr/ark:/12148/btv1b53095291n )</div>

----

**Principaux triangles de la planche 52**

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini_triangulation2.png)

<div style="text-align: justify; font-size: x-small">
Source : Carte générale de la France. Tableau d'assemblage, Nouvelle carte Qui Comprend les principaux Triangles qui servent à la description Géométrique de la France levée par ordre du Roy / Par Mess.rs Maraldi et Cassini de Thury, de l'Académie Royale des Sciences. Année 1744 ; Tracé d'après les Mesures, et gravé par Dheulland ; Aubin scripsit - (https://gallica.bnf.fr/ark:/12148/btv1b53095291n )</div>

----

**Entités géographiques triangulées (316 points rouges) et relatives (6 565 croix grises) dans la planche n°52 de la carte de Cassini (1759-1777). La triangulation de premier niveau utilisée par les géomètres est figurée en bleu**

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_verso_carte_triangulation.png)


----

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_enquete0.png)

----

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_enquete1.png)

----

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/cassini_enquete2.png)

---

##### P1.4.3.3 Index des entités géographiques présentes sur la carte

##### Le verso de la Carte 52 - Vue générale

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_verso.png)

----

##### Le verso de la Carte 52 - Index et symboles

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_verso_index.png)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_verso_symboles.png)

----

##### P1.4.3.4 Un objet hybride : Base de donnée géo-historique et un style cartographique associé

<div style="text-align: justify; font-size: x-small"> 
Le processus de construction de la carte n’étant que partiellement documenté, les données géographiques vectorielles qui en ont été extraites sont entachées de multiples incertitudes, leur forme et leur position sont nécessairement imprécises, sans compter les erreurs que contient la carte. Représenter graphiquement ces objets hybrides suppose d’élaborer une visualisation cartographique adaptée afin d’éviter une fausse impression de précision et d’exactitude des données. Pour ce faire, une possibilité consiste à reproduire un style cartographique imitant la carte ancienne, offrant de surcroît un rendu esthétique (Fig. 2). Ce style “à la Cassini” préserve les propriétés cartographiques des données vectorielles extraites de la carte : généralisation, échelle, granularité spatiale, ainsi que l’intention générale des cartographes du XVIIIe siècle [3]. Souvent négligées, ces propriétés sont pourtant des composants du style cartographique et fournissent des informations cruciales sur l’exactitude  planimétrique des entités géographiques cartographiées et les relations qu’elles entretiennent entre elles. 
</div>

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_stylecassini.png)

<div style="text-align: justify; font-size: x-small"> 
Ce résumé introduit un poster publié à la conférence internationale de cartographie, qui présente  une visualisation cartographique renouvelée de la planche n°52 de la Carte de France de Cassini (Fig. 3.a). En même temps édition critique de la planche originale, cette nouvelle carte révèle des entités géographiques jusqu’ici quasi invisibles, des configurations locales et régionales spécifiques. Elle est doublée d’un index toponymique complet facilitant la recherche de lieux au sein de la carte (Fig. 3.b). L’historiographie de la cartographie s’est fondée sur l’édition critique de cartes anciennes publiées sous forme de facsimile non géoréférencés. Nous proposons ici une approche exploitant les possibilités offertes par les SIG, en produisant des cartes numériques construites à partir de bases de données géohistoriques, qui combinent l’esthétique et la sémiologie d’un style cartographique ancien, l’analyse du processus de production de la carte et les capacités de modélisation et de représentation des SIG modernes. L’étude et l’analyse combinée de ces différentes dimensions permet de préciser notre connaissance des paysages anciens. 
Le jeu de données rassemblant les données vectorielles extraites de la planche n°52, les fichiers nécessaires à la construction de la carte numérique dans le style Cassini et les documents de composition de la carte finale sont publiés sous license ouverte sur l’entrepôt de données Harvard Dataverse [1].
</div>

<div style="text-align: justify; font-size: x-small"> 
- Abadie, Nathalie; Baciocchi, Stéphane; Boivin, Pierre; Chadeyron, Julien; Cristofoli, Pascal; Delaveau, Jean-Michel; Duménieu, Bertrand; Gomis, Stéphane; Gribaudi, Maurizio; Langlois, Isabelle; Motte, Claude; Perret, Julien; Vouloir, Marie-Christine, 2019, "A GIS reconstruction of the Cassini "Carte de France" sheet No. 52", https://doi.org/10.7910/DVN/XP8J6P, Harvard Dataverse, V1.
</div>

<div style="text-align: justify; font-size: x-small">
- C.-F. Cassini. Description géométrique de la France. Imprimerie Desaint. Google-Books-ID : RDReAAAAcAAJ.
- S. Christophe, B. Duménieu, A. Masse, C. Hoarau, J. Ory, M. Brédif, F. Lecordix, N. Mellado, J. Turbet, H. Loi, T. Hurtut, D. Vanderhaeghe, R. Vergne, and J. Thollot. Expressive map design: Ogc sld/se++ extension for expressive map styles. Proceedings of the ICA, 1:21, 2018.
</div>


---

### P1.4.4 Des communes aux paroisses, des paroisses aux communes

#### P1.4.3.1 Les "chefs lieux et clochers de Cassini"

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/exemple_clocher.png)

- Des lieux remarquables sur la carte de Cassini
Les Chefs-lieux et clochers de la carte de Cassini (Villes, bourgs, clochers, abbayes) sont signalés par des symboles et des graphies (Capitales, grosses romaines, petites romaines) différentes qui témoignent de leur statut à part.
- Du point de vue de l'élaboration de la carte, ce sont les lieux qui ont servi de base au travail des géomètres.

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Cassini_Pl52_villes_bourgs_clochers.png)

----

- Une figuration des entités "administratives" d'ancien régime.

Eric Brian (Brian 2001, p. 173) emploie le mot de "Municipalités" pour décrire la catégorie "ville, bourg ou village (ou paroisse)" utilisée par les administrateurs à la fin de l'ancien régime.

<div style="text-align: justify; font-size: small"> 
<i>"J’emploie ce mot à dessein : il renvoie à la vaste réforme voulue par Turgot et la catégorie «ville, bourg ou village» ou «ville, bourg ou paroisse» lui correspond dans l’esprit des réformateurs de l’administration monarchique de la fin du XVIIIe siècle. Il faut attendre 1790 pour que la catégorie de «commune» scelle définitivement, et sans ambiguïté du fait de sa fondation révolutionnaire, ce dont on parle déjà
depuis plusieurs décennies dans les documents qui servent aux compilations.
Dans la suite de cet article, le mot «municipalité» désigne l’unité de
comptes du contrôle général et des intendances : le plus souvent une paroisse, et dès que l’agglomération couvre plusieurs atomes paroissiaux, un
groupe d’entre elles, jusqu’à l’entièreté de Paris s’il le faut.</i></br>
</div>

Il insiste notamment (p. 180-181) sur l'effet de réalité de la nomenclature des municipalités produit par la mise en relation au cours de la décénie 1780 de trois logiques : la police du royaume, la comptabilité ecclésiastiques des âmes (enquête de La Michodière) et le repérage géodésique des points hauts (notamment des clochers).

<div style="text-align: justify; font-size: small"> 
<i>[...] ces trois logiques [...] sont à la fois mises à l’épreuve et conjuguées dans l’établissement de la nomenclature des « villes, bourgs et villages » forgée au cours des années 1780. Chaque municipalité finalement identifiée est (1) identifiée à un lieu topographique défini en longitude et en latitude, (2) le siège d’un ou plusieurs clercs qui régulièrement rassemblent leurs ouailles et tiennent le registre des naissances de la communauté, des unions et des sépultures, (3) une entité envisagée comme homogène par le représentant provincial de l’autorité royale. La conjonction de ces trois logiques dans la définition d’une même nomenclature procurait aux listes établies pour l’enquête, aux yeux d’un contemporain informé, un réalisme qu’il nous est difficile de concevoir tant il faut s’affranchir des évidences induites par les institutions administratives issues de la Révolution.</i></div>

- Paroisses, municipalités, communes (1789-1793) :
<div style="text-align: justify; font-size: small"> 
«Il y aura une municipalité dans chaque ville, bourg, paroisse ou communauté de campagne ». Décret de l’Assemblée nationale du 12 novembre 1789, repris dans l’article 7 du décret du 22 décembre 1789, Archives parlementaires, t.10, p.7.</div>
<div style="text-align: justify; font-size: small">
« L’Assemblée municipale se réunira dans le lieu où est le clocher. » Décret de l’Assemblée nationale du 20 janvier 1790, Archives parlementaires, t.11, p. 257.
</div>
<div style="text-align: justify; font-size: small">
 « Il est entendu que les villes emportent le territoire soumis à l’administration directe de leurs municipalités, et que les communautés de campagne comprennent de même tout le territoire, hameaux, toutes les maisons isolées dont les habitants sont cotisés sur le même rôle. » Art. 2 du décret de l’Assemblée nationale relatif à la Division du Royaume, des 15 janvier et 16 février 1790, Archives parlementaires, t. 11, p. 717.
 </div>
<div style="text-align: justify; font-size: small">
« La Convention décrète que toutes les dénominations de ville, bourg et village sont supprimées et que celle de commune leur est substituée. » Décret de la Convention du 10 brumaire an II (31 octobre 1793), Archives parlementaires, t. 78, p. 89.
</div>


<div style="text-align: justify; font-size: x-small"> 
(1) (Brian, 2001) : Brian, Éric. «Nouvel essai pour connaître la population du royaume. Histoire des sciences, calcul des probabilités et population de la France vers 1780», <i>Annales de démographie historique</i>, vol. no 102, no. 2, 2001, pp. 173-222.
</div>

----
#### P1.4.3.2 - Le repérage des clochers et chefs-lieux sur la carte

##### Une saisie experte et assistée ("semi-manuelle"):

- Saisie fondée sur l'iInfrastructure du projet Geohistoricaldata mise en place pour la saisie des routes de Cassini : Base de données geo Post-GIS (historicisée) et logiciel libre SIG QGIS.
- Pré-placement automatisé des points communes existantes aujourd'hui sur la coordonnée du chef lieux de la couche BD-Topo de l'IGN (Point vert)
- Pré-placement approximatif des communes disparues sur le territoire de la commune dont elles dépendent aujourd'hui (Point Rouge)
- Déplacement des "points communes" sur le symbole associé sur la carte -> il deviennent ainsi des "Points clocher" (on constate que certains de ces points n'ont pas le statut de paroisse, bourg ou ville dans la carte);
- Pour les symboles de clochers, bourgs ou villes qui ne correspondent pas à une commune, création d'un nouveau point (Point bleu) -> ce sont aussi des "Points clocher" (dont la propriété est de ne pas être devenu commune)
- Saisie manuelle du toponyme inscrit sur la carte, du type de symbole associé sur la carte et de la typographie du toponyme, et de remarques éventuelles
- Décision de prendre en compte l'ensemble des établissements relgieux signalés comme importants (Abbayes, prieurés,...) par leur symbole ou leur graphie (cp) 
- Parcours systématique de l'ensemble des planches de la carte

----

##### Le repérage des clochers et chefs-lieux sur la carte (1)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Ex_Billom1_chefs_lieux_clochers_CC1999_seule.png)

----

##### Le repérage des clochers et chefs-lieux sur la carte (2)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Ex_Billom2_chefs_lieux_clochers_CC1999.png)

----

##### Le repérage des clochers et chefs-lieux sur la carte (3) - version 2015

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Ex_Billom3_chefs_lieux_clochers_CC2015.png)

----

##### Le repérage des clochers et chefs-lieux sur la carte (4)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Ex_Billom4_chefs_lieux_clochers.png )

----

##### Clochers et chefs-lieux tenant registres paroissiaux : expérimentation sur la planche 52 

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/CarteCassiniNumerique_planche_52_verso_carte_population.png)
    
----

#### P1.4.3.3  Clochers et chefs lieux à l'échelle de la France

Le travail de repérage et de saisie a été réalisé au LaDéHiS-CRH dans la cadre des activités du groupe Geohistoricaldata par **C. Motte et M.-C. Vouloir**, avec la collaboration de S. Baciocchi, P. Cristofoli, B. Duménieux, M. Gribaudi, E. Mermet (PSIG EHESS) et J. Perret.

- La **couche des "clochers et chefs-lieux de la carte de Cassini"** est en instance de publication en données ouverte.
- De cette opération découle en outre la **capacité de faire le lien entre les paroisses d'ancien-Régime et les communes** (en terme géomatique : il s'agit d'un alignement de la base des communes avec les informations extraites de la carte que l'on considère comme un état de la situation à la fin de l'ancien régime).

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/chefsLieux_tableau_202012.png)


----

##### Chefs lieux et Clochers de Cassini relevés sur la carte de Cassini

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/clochers_france_tous.png)

----

##### Chefs-lieux et Clochers de la carte de Cassini selon le type de statut après 1789

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/clochers_france_toustypes.png)

<div style="text-align: justify; font-size: x-small"> Rappel: En vert, les chefs lieux de Cassini encore chef-lieux d'une commune actuelle ; En rouge, les chefs-lieux de Cassini qui ont été un jour chef-lieux de commune mais ne le sont plus actuellement ; En bleu : chefs-lieux de Cassini qui ne sont pas devenu chefs-lieux de commune.</div>

----

##### Chefs-lieux et Clochers de Cassini qui sont chef-lieux de communes actuellement

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/clochers_france_co.png)

----

##### Chefs-lieux et Clochers de Cassini qui ont été chef-lieux de d'anciennes communes qui n'existent plus actuellement

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/clochers_france_ac.png)

----

##### Chefs-lieux et Clochers de Cassini qui ne sont jamais devenus chefs-lieux de communes

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/clochers_france_new.png)

----

##### Abbayes relevées sur la carte de Cassini

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/clochers_france_abbaye.png)

    1 - Carte de densité des clochers (est-ce que cela change beaucoup par rapport à la densité des communes).
    Des observations locales à l'opportunité d'un résultat national
    2 - Paroisses non devenues communes, à rapprocher des cartes déjà faites sur les mouvements communaux
    

---

### P1.4.4 Les limites

#### P1.4.4.1 Les limites sur la carte de Cassini

##### Une limite telle que “relevée” sur le terrain en 1763

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_1.png )
    
----

##### Limites, frontières, bornes ?

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_2.png )
    
----

##### Limites 3 - Relevé quasi exhaustif des limites gravées sur la carte

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_3.png )
    
----

##### Limites 4 - Noeuds routiers urbains et limites territoriales

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_4.png )
    
----

##### Limites 5 - Premier inventaire critique des limites administratives “provinciales”

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_5.png )
    
----

##### Limites 6 - Souscriptions versées par diverses institutions provinciales

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_6.png )
    
----

##### Limites 7 - Minutes des planches comportant des limites ecclésiastiques

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_7.png )
    
----

##### Limites 8 - les limites et le marquage politique des territoires

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_8.png )
    
----

##### Limites 9 - La mise à jour politique des limites en 1790

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/limites_9.png )
    
----

    Frontières (surfaces) ou réseaux de "lieux".
    Disparités régionales
    Réseaux des liens nomées rattachés à un clocher?
    Voronoi pour approximer les territoires
    Histoire de la production de la Carte

#### P1.4.4.2 La carte d'Arbelot et Al. (1986) comme source spatiale pour 

G. Arbellot, J.-P. Goubert, J. Mallet, Y. Palazot, Carte des généralités, subdélégations et élections en France à la veille de la Révolution de 1789, CNRS, 1986

Réutilisation d'un travail scientifique (nécéssité d'un cumul)
Fond de carte IGN 1984

Une couche à corriger et à préciser.()

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/arbelot1.png )

    
#### P1.4.4.3 Paroisses et Subdélégations à la fin de l'ancien régime

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Arbellot_Rouen_detail.png)

##### Discordances temporelles et "communes mi-parties"

- Travail d'Arbelot et al. : Description d'une réalité de la fin de l'ancien régime à l'échelle nationale compilant des informations correspondant à des états différents sur la période 1770-1789.
- Couche cartographique Arbelot : Une source cartographique crée en 1986 sur le fond carographique IGN 1984.
- Les territoires communaux ne correspondent pas forcéments au tracés des "frontières" du passé.
- Geohistoricaldata : Reprise des informations sur le fond cartographique FLA de l'IGN 2013. Entre 1984 et 2013, des communes ont entre-temps vécu un évènement d'absoption, de création ou de suppression
- Dans la carte d'Arbelot, il existe de nombreux cas de communes dont le territoire est traversé par une frontière de subdélégation (communes mi-parties)

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Subdel_1789_communes_miparties.png )

----

**Carte des subdélégations à la fin du 18e siècle reconstituée à partir de la Carte d'Arbelot et Al. 1986**.

![image alt](https://raw.githubusercontent.com/GeoHistoricalData/esopp2021/main/images/Subdel_1789.png )
    
---

## P1.5 Bilan et transition


##### Evolution des objets matériels, du contexte soci-technique, évolutions des questions scientifiques
Evolutuion des outils et pratiques de travail
Evolution de manière d'appréhender les sources
Produire un appeillage critique nécessaire à la compréhension des données qui en sont issues.
Pérénité ? activité ? travaux collectifs.
Des savoir-faire spécialisés: informatique, géomatique

    (cartes perforées, bandes magnétiques, fichiers formats). Des graos systèmes à la micro-informatique personnelle aux serveurs.
    Humanités numériques, Sciences computationnelles, Web sémantique


##### La carte comme une source. Importance de l'ancrage dans l'espace des sources historiques. 

##### Le traitement des problématiques en histoire pose des questions à la recherche en informatique :
Comment traiter l’absence d’information, l’imprécision, le flou, ou encore la contradiction dans les systèmes informatiques ?
Comment prendre en compte efficacement la dimension temporelle dans les bases de données ?

##### Pour quoi faire ?
- Utilisation des connaissances et des outils élaborés
- Mise au point de dispositifs et d'infrastructures pour produire de manière collaborative des données géohistoriques, les diffuser et les utiliser.

---

## Partie 2 - De la carte des Cassini au Paris révolutionnaire de Verniquet (1750-1795). Deux études de cas à partir des travaux sur l’espace au laboratoire
2e partie
(SB)
Point 1. L’édition critique de la Planche 52
Point 2. Les cartes de sûreté du Paris révolutionnaire

---

## Partie 3 - Les outils développés au sein du laboratoire
3e partie
(BD)

[![hackmd-github-sync-badge](https://hackmd.io/k5x0vZDWQ7q8rwYRzrKj0Q/badge)](https://hackmd.io/k5x0vZDWQ7q8rwYRzrKj0Q)

