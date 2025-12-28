---
title: Domaines
---

Un domaine est un groupe de ressource. Par défaut un domaine est accessible à tous, les ressources dans ce domaines sont réservables par les utilisateurs ayant le statut usager ou administrateur.

**Chaque domaine à des propriétés différentes.**

#### Renseignements divers :

* Un **nom**, qui permet de le désigner à l'ensemble des utilisateurs.
* Un **ordre d'affichage**. L'ordre d'affichage est l'ordre dans le menu est les affichages avec l'ensemble des ressources.
* Un **accès restreint** ou non : Si le domaine est en accès restreint, par défaut défaut les utilisateurs (hors administrateurs), n'auront pas de visibilité sur le domaine et les ressources ce trouvant à l'intérieur. Il va falloir fournir les autorisations d'accès aux utilisateurs dans _Utilisateurs et accès / Accès aux domaines restreint_.
* **Domaine par défaut pour l'adresse IP client suivante** : Imaginons que **GRR** est basé en cloud, que vous ayez les 3 domaines correspondant à 3 sites distants (Lille, Paris, Marseille). Si je configure pour chaque domaine, l'IP de mon site. A chaque fois que je suis à Lille, il m'affichera les ressources de Lille, pareil pour Paris et Marseille. L'IP peut-être public ou privé selon votre installation. Elle accepte les masque sous forme 192.168.1.0/24. L'administrateur ainsi que l'utilisateur ne doivent pas avoir défini un domaine par défaut dans la page de configuration générale.

#### Configuration de l'affichage des plannings des ressources de ce domaine

* Début de la semaine : Premier jour de la semaine. Sur les plannings hebdomadaires, les semaines commencent par cette journée.
* Sélection des jours à afficher : Choix multiple entre les 7 jours de la semaine. Si par exemple les ressources ne peuvent être réservé le dimanche, décoché "dimanche".

!!! Nouveauté GRR 4.5.0 : Fichier joint

#### Configuration de la fonctionnalité "Fichier joint"

La fonctionnalité **Fichier joint** permet aux utilisateurs autorisés de téléverser des fichiers associés à une réservation, ainsi que de consulter les fichiers joints, en fonction des droits définis.

Le téléversement et la consultation des fichiers se font directement depuis la **page de consultation d'une réservation**.

L'utilisation de la fonctionnalité repose sur deux droits distincts.

**Droit pour consulter les fichiers:**

Ce droit permet à l'utilisateur de :
- consulter les fichiers joints à une réservation ;
- télécharger les fichiers associés, si des fichiers sont présents.

Sans ce droit, les fichiers joints ne sont pas visibles par l'utilisateur.

**Droit pour téléverser les fichiers:**

Ce droit permet à l'utilisateur de :
- ajouter un ou plusieurs fichiers à une réservation ;
- remplacer ou supprimer les fichiers qu'il a téléversés, selon la configuration de GRR.

Sans ce droit, l'utilisateur ne peut pas ajouter de fichier joint à une réservation, même s'il peut la consulter.

> **Remarque :** Les droits de consultation et de téléversement sont indépendants et peuvent être attribués séparément selon les profils d'utilisateurs.


#### Configuration du type de créneaux

Deux choix :
1. Les créneaux de réservation sont basés sur le temps. _(Par défaut)_
2. Les créneaux de réservation sont basés sur des intitulés pré-définis.

!! Les deux types de configuration des créneaux sont incompatibles entre eux : un changement du type de créneaux entraîne donc, après validation, **un effacement de toutes les réservations** de ce domaine.

##### 1. Les créneaux de réservation sont basés sur le temps :

* Heure de début de journée : choisir une valeur entière entre 0 et 23
* Heure de fin de journée : choisir une valeur entière entre 0 et 23, supérieure à l'heure de début de journée.
* Nombre de minutes à ajouter à l'heure de fin de journée pour avoir la fin réelle d'une journée : voir exemples ci-dessous
* Plus petit bloc réservable, en secondes (1800 secondes = 1/2 heure) : voir exemples ci-dessous
* Durée par défaut d'une réservation

> ###### Exemple 1 :
> Pour mettre en place des réservations entre 8 h et 19 h, avec un pas de 15 minutes (900 secondes), la configuration doit être la suivante :
> 
> * Heure de début de journée : 8
> * Heure de fin de journée : 18
> * Nombre de minutes à ajouter à l'heure de fin de journée pour avoir la fin réelle d'une journée : 45
> * Plus petit bloc réservable, en secondes (1800 secondes = 1/2 heure) : 900

___

> ###### Exemple 2 :
> Pour mettre en place deux créneaux de réservations 8 h - 14 h et 14 h - 20 h, soit des bloc de réservation de 6 h (21600 secondes), la configuration doit être la suivante :
> 
> * Heure de début de journée : 8
> * Heure de fin de journée : 14
> * Nombre de minutes à ajouter à l'heure de fin de journée pour avoir la fin réelle d'une journée : 0
> * Plus petit bloc réservable, en secondes (1800 secondes = 1/2 heure) : 21600

__________________________________________________________________________________________________________________

##### 2. Les créneaux de réservation sont basés sur des intitulés pré-définis :

Il ne s'agit pas du mode normal de fonctionnement de **GRR**. N'utilisez ce mode uniquement dans le cas où le mode précédent ne correspond pas à votre cas de figure, c'est-à-dire lorsque vos créneaux de réservation sont de taille inégales et ne peuvent pas se subdiviser en blocs de tailles égales ou bien lorsque les créneaux ne couvrent pas uniformément la plage de début à la fin.

> ###### Exemple :
> * Créneau 1 : 8h10 - 9h00
> * Créneau 2 : 9h00 - 9h50
> * Créneau 3 : 10h05 - 10h55
> * Créneau 4 : 10h55 - 11h45
> * Créneau 5 : 11h45 - 12h35
> * Créneau 7 : 12h35 - 13h00
> * Créneau 8 : 13h00 - 13h50
> * Créneau 9 : 13h50 - 14h40
> * Créneau 10 : 14h40 - 15h30
> * Créneau 11 : 15h45 - 16h35
> * Créneau 12 : 16h35 - 17h25
> * Créneau 13 : 17h25 - 18h30
> * Créneau 14 : 18h30 - 19h30

#### Durée maximale d'une réservation pour une ressource donnée
Il est possible de définir une durée maximale pour une réservation donnée. Dans ce cas, une réservation ne pourra pas excéder une durée limite, suivant les propriétés suivantes :
* Durée définie en nombre de minutes dans le cas où les créneaux sont basés sur le temps,
* Durée exprimée en nombre de jours dans le cas où les créneaux sont basés sur des intitulés pré-définis. 

Cette limitation ne touche pas les administrateurs et gestionnaires des ressources du domaine.

!!! Remarque : actuellement, les journées hors réservation sont prises en compte dans le calcul de la longueur d’une réservation.

> ###### Exemple :
> Supposons que la limite soit fixée à trois jours et que le week-end soit hors réservation. Une réservation débutant le vendredi matin et se terminant le lundi soir ne sera pas acceptée car **GRR** considère à tort que la réservation dure 4 jours.

__________________________________________________________________________________________________________________