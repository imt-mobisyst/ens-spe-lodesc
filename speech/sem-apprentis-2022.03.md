# Seminaire APPRENTIS

Organisateur: Dimitri Lefebvre

## Apprentis

ANR Flash (ANR + Régions Nords) suite à l'accident LUBRISOL.

Configuration de flotte (quel capteur sur quel robots)

## 9h Drones en Essaim pour la Surveillance des sites Industriels à Hauts Risques

François Guerin, GREAH - ULHN

**RESUME** La présentation portera sur l'instrumentation et la commande décentralisée d'une flotte de drones
pour évaluer la qualité de l'air (nature des polluants, concentration, ...) à la suite d'un accident majeur
sur un site industriel.

**CR** Suivie de panache aider de drones et caractérisation. Sujet et approche très proches de notre travaille sur ALPAGA.

Capteur:

- PMSA003: concentration en microparticules dans l'air
- BME280 : pression température humidité

- Autopilot: C++/ROS - DJI
- Drone: [squadrone](https://squadrone-system.com) 
- Simulateur de vol FlightGear (hardware in the loop)

- Communication : mesh radio 2.4 G.Hertz (porté 5-6 km)

- Protopite de cartes capteurs et perspective électronique.


## 10h Des systèmes mobiles autonomes pour l'échantillonnage en milieu naturel

Guillaume Lozenguez, Luc Fabresse, Bouraqadi Noury, IMT Lille Douai


**RESUME** Les robots mobiles autonomes ont gagné en maturité et diversité sur ces 10 dernières années. Les
développeurs de plates-formes robotiques terrestres, aquatiques ou aériennes et la communauté
notamment académique proposent des solutions. Celles-ci sont accompagnées de logiciels de contrôle
et de supervision qui permettent de traiter les problématiques de réalisation autonome de missions
complexes.
Dans le cadre de nos travaux, nous nous focalisons sur les architectures logicielles de contrôle et de
supervision de missions, embarquées sur les robots. Nous ciblons en particulier leur mise en œuvre
sur des missions d'échantillonnages automatisés. Dans cet exposé, nous traiterons en particulier de la
problématique d'analyse de la qualité de l'air en utilisant un drone aérien. Nous présenterons nos
travaux en cours sur l'utilisation d'un hexacopter chargé de prélever des échantillons d'air à des fins
d'analyse de Composés Organiques Volatiles (COV).



## 11h Architecture pour la reconfiguration des missions de surveillance

Sara Hsaini, GREAH –ULHN


**RESUME** Après un résumé sur l’état d’avancement du projet, l’architecture proposée pour étendre en ligne la
méthode d’optimisation par recherche en faisceaux sera présentée. La nouvelle architecture est basée
sur un système temps réel qui permet de reconfigurer à distance et d’une manière continue les
trajectoires des robots en prenant en considération les nouvelles tâches qui apparaissent.