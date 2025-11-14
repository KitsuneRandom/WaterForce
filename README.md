## Application de gestion de casernes de pompiers

<h3>Ce projet a été réalisé lors de ma première année en BUT informatique.</h3>
à noter : aucun dépôt git n'a été créé lors de la réalisation du projet. Ceci est donc un simple dépôt généré après sa réalisation.

<h3>Contexte du projet (donné par les professeurs responsables du projet) : </h3>
Rattachée au ministère de l'Intérieur, la Direction de la Sécurité Civile (DSC) est la structure centrale
responsable de la gestion des risques en France pour les accidents de la vie courante ou les
catastrophes majeures. Parmi ses compétences figure la gestion des services départementaux
d’incendie et de secours (SDIS) qui gère les centres d’incendie et de secours (CIS) appelés
familièrement "casernes".
Concevoir une application permettant la gestion complè te de quatre casernes de pompiers
(personnel, matériel et missions effectuées).
Votre application devra offrir les fonctionnalités suivantes :
- Volet 1 : tableau de bord des missions en cours.
- Volet 2 : création d’une nouvelle mission puis affectation du matériel nécessaire ainsi que
des pompiers missions.
- Volet 3 : Visualisation en mode 1 à 1 des engins d’une caserne donnée.
- Volet 4 : gestion du personnel d’une caserne (données signalétiques, carrière et habilitations
des pompiers ). L’aspect « mise à jour » est réservé aux utilisateurs disposant de droits
d’administration.
- Volet 5 : Statistiques à destination du régulateur.
L’ensemble des informations utiles seront stocké es dans une base SQLite intitulé e «SDIS67.db»,
dont vous trouverez le schéma conceptuel en annexe.
Bonne pratique : La gestion de la connexion (ouverture/fermeture) sera gérée à partir d’une classe
Connexion.cs (fournie sur moodle).
Votre application devra permettre la prise en charge des diffé rents volets dé crits ci-dessous (vous
pouvez, mais ce n’est pas obligatoire, concevoir un formulaire par volet).
Vous veillerez tout particuliè rement à la qualité et la lisibilité de votre code, que vous n’hé siterez pas à
commenter autant que possible.Pour la conception des interfaces graphiques, une attention
particuliè re sera porté e à leur ergonomie et l’originalité de leur design.

---

## Formulaire de démarrage

- Tableau de bord montrant la liste des missions : permet la clôture rapide des missions et l'édition d'un pdf récapitulatif de la mission
- Des boutons permettant d'accèder aux différents formulaires de l'application

---

## Création d'une nouvelle mission

- L'utilisateur remplit les informations de la mission.
- L'application choisit ensuite une caserne dans laquelle les conditions sont remplies pour le lancement de la mission.
- L'application génère l'effectif de pompiers et de véhicules à utiliser en fonction du type de sinistre et de la disponibilité des pompiers et des véhicules.

---

## Parcours des véhicules d'une caserne

- Visualisation des différents engins de chaque caserne.
- Visualisation de l'état des engins (en panne / en mission)

---

## Gestion des pompiers

- Consultation des informations concernant les pompiers de chaque caserne
- Modification des informations des pompiers
- Ajout d'un nouveau pompier

---

## Statistiques

- Visualisation de différentes statistiques :
    - Engins les plus utilisés par caserne
    - Nombre total d'heures d'utilisation de chaque engin par caserne
    - Nombre d'interventions par sinistre
    - Habilitations les plus sollicitées
    - Liste des pompiers par habilitation

---

## Contributions

- Mathis DE AZEVEDO : Création de mission, design de l'application
- Jonathan BEVILAQUA : Formulaire de démarrage, Gestion des pompiers
- Henri ROSSMANN : Parcours des véhicules, Statistiques
