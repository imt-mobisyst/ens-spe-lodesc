---
marp: true
theme: imt
paginate: true
backgroundImage: url('../style/bg-imt.svg')
---

# IMT MobiSyst
### Des systèmes mobiles autonomes pour <br /> l'échantillonnage en milieu naturel

<br />
<br />
<br />

**Noury.Bouraqadi**
**Luc.Fabresse**
**Guillaume.Lozenguez**
[@imt-nord-europe.fr](mailto:guillaume.lozenguez@imt-nord-europe.fr)

![bg](../style/bg-tittle.svg)

---
<!-- --------------------------------------------------------------- -->

![bg](../style/bg-toc.svg)

<br />

- **Nos thématiques**
- **Focus sur le projet ALPAGA**


---
<!-- --------------------------------------------------------------- -->

![bg](../style/bg-toc.svg)

<br />

- **Nos thématiques**
  - Logiciel distribué communicant
  - Prise de décision embarquée
  - Cartographie Cooperative
- Focus sur le projet ALPAGA
- Quelques résultats expérimentaux


---
<!-- --------------------------------------------------------------- -->

## Logiciel distribué communicant


![](../resources/pharos.svg)

- Protocole de communication - Distribution des connaissances / des calculs
- Développements agiles et modulaires

---
<!-- --------------------------------------------------------------- -->

## Prise de décision embarquée

**Planifier les actions à réaliser** <br /> (une politique $\Pi$)

- Tenir compte des coéquipiers
- Intégrer l'incertitude
- Être réactif aux changements

**Partie prix**

- Remise en cause perpétuelle
- Algorithme rapide, mais approché

![bg right width:90%](../resources/topo_pb.svg)


---
<!-- --------------------------------------------------------------- -->

## Cartographie coopérative

- Solution basée sur une représentation **vectorielle** de l'environnement<br />(PhD Johann Dichtl 2019)

![](../resources/car_bot.svg)

$$M= \langle Node(x, y), Edge(n1, n2, \mathit{type}) \rangle \text{ ,} \quad  \mathit{type} \in [\mathit{obstacle}, \mathit{frontier}]$$

- Modélisation légère, graphique avec une sémantique forte.

---
<!-- --------------------------------------------------------------- -->

![bg](../style/bg-toc.svg)

<br />

- Nos thématiques
- **Focus sur le projet ALPAGA**
- Quelques résultats expérimentaux


---
<!-- --------------------------------------------------------------- -->

## Genèse du projet ALPAGA

<br />

*A*eia*L* *P*latform for sampling *A*tmospheric *G*ases and *A*erosols

En collaboration entre 2 des 3 centres de l'IMT Nord-Europe.

- Système numérique
- Énergie et Environnement

Besoin de prélèvement d'échantillons de Gaz à faible et moyenne altitude.

---
<!-- --------------------------------------------------------------- -->

## ALPAGA, l'équipe

![](../resources/alpaga-team.svg)


---
<!-- --------------------------------------------------------------- -->

## Les Composés organiques volatils

**Sources :** 

![](../resources/alpaga-voc.svg)

**Mesures :**

- Équipement lourd: Spectromètre de masse
- Prélèvement in situ et analyses en laboratoire

---
<!-- --------------------------------------------------------------- -->

## Capture d'échantillon traditionnel

![](../resources/alpaga-sampling.svg)

- Évidence: utiliser un ou plusieurs drones pour faire le boulot.

---
<!-- --------------------------------------------------------------- -->

## Scenario

### 1. Mission statique

- Équiper un ou plusieurs drones de capteurs et préleveurs
- Identifier les points de mesures
- Planifier et exécuter la mission

### 2. Mission dynamique

- Identifier et reconfigurer les points de mesure en vols <br />(Exemple: suivi de panache)

---
<!-- --------------------------------------------------------------- -->

## Les Drones

#### Drone principal (station de prélèvement) + Drones Scouts (capteurs légers)

![](../resources/alpaga-drones.svg)

---
<!-- --------------------------------------------------------------- -->

## Playload - Station de prélèvement

### Dans l'idée:

![](../resources/alpaga-playload-idea.svg)

- Mise sous vide d'un volume avec Sac Tedlar
- Activation du remplissage par électrovanne

---
<!-- --------------------------------------------------------------- -->

## Playload - Station de prélèvement

### Playload sur le drone:

![](../resources/alpaga-playload-archi.svg)

---
<!-- --------------------------------------------------------------- -->

## Playload - Station de prélèvement


### Electronique misse en oeuvre:

![](../resources/alpaga-playload-elect.svg)


---
<!-- --------------------------------------------------------------- -->

## Playload - Station de prélèvement - On the drone

**Architecture logicielle:**

![](../resources/alpaga-archi.svg)

- Nodes: processus fonctionnels autonomes interconnectés

---
<!-- --------------------------------------------------------------- -->

![bg](../style/bg-toc.svg)

<br />

- Nos thématiques
- Focus sur le projet ALPAGA
- Quelques résultats expérimentaux

---
<!-- --------------------------------------------------------------- -->

## Alpaga - Premières expérimentations

### Le lieu

![](../resources/alpaga-xp1-map.svg)

---
<!-- --------------------------------------------------------------- -->

## Alpaga - Mission

![bg right](../resources/alpaga-xp1-height.svg)

1er vol:

- Système 4 cylindres
- Temps de prélèvement: $40s$<br />($2 \times 20s$, pompe puis ouverture) 
- Échantillons: 110 - 220 ml

2e vol:

- Système 3 cylindres
- Temps de prélèvement: $28s$ <br />($8s$ pompe seule puis $20s$) 
- Échantillons: 340 - 400 ml

---
<!-- --------------------------------------------------------------- -->

## Alpaga - Premières expérimentations

### Les résultats: permettre l'ajustement du système

Entre deux vols:

- Calibrage des temps de (pompe électrovannes)
- Nouveaux design de la structure tubulaire

Pour une nouvelle version:

- Changer de volume (minimiser les fuites)
- Ajouter un capteur de pression

---
<!-- --------------------------------------------------------------- -->

## Alpaga - Premières mesures

![](../resources/alpaga-xp1-results.svg)

- Les résultats sont inattendus (haut) et sans explications.

---
<!-- --------------------------------------------------------------- -->

#### Merci pour votre attention

---
<!-- --------------------------------------------------------------- -->


## Résumé.

<br />

Les robots mobiles autonomes ont gagné en maturité et diversité sur ces 10 dernières années. 
Les développeurs de plates-formes robotiques terrestres, aquatiques ou aériennes et la communauté notamment académique proposent des solutions.
Celles-ci sont accompagnées de logiciels de contrôle et de supervision qui permettent de traiter les problématiques de réalisation autonome de missions complexes. 
Dans le cadre de nos travaux, nous nous focalisons sur les architectures logicielles de contrôle et de supervision de missions, embarquées sur les robots. 
Nous ciblons en particulier leur mise en oeuvre sur des missions d'échantillonnages automatisés.
Dans cet exposé, nous traiterons en particulier de la problématique d'analyse de la qualité de l'air en utilisant un drone aérien.
Nous présenterons nos travaux en cours sur l'utilisation d'un hexacopter chargé de prélever des échantillons d'air à des fins d'analyse de Composés Organiques Volatiles (COV).
