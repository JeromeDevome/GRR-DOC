---
title: 'Types de réservation'
---

!!! **Nouveauté GRR 4.5.0 :** fusion de deux types et tri automatique par identifiant ou par nom.

Dans cette section sont définis les différents types de réservation.

Les types de réservation permettent :
- de différencier les réservations par des couleurs dans le planning ;
- de simplifier l'analyse et l'affichage dans les statistiques.

**Exemples :** cours, réunion, formation.

> **Attention :** Les types de réservation ne sont pas des ressources.

### Caractéristiques des types de réservation

Il est possible de définir jusqu'à **702 types de réservation** (de `A` à `Z`, puis `AA` jusqu'à `ZZ`, etc.).

Chaque type dispose des propriétés suivantes :
- un **identifiant** ;
- un **nom** ;
- une **couleur de texte** ;
- une **couleur de fond** ;
- une **couleur pour les icônes** ;
- un **ordre d'affichage** dans les différents plannings ;
- un **disponible pour** pour savoir qui peut l'utiliser.

### Tri des types

L'ordre d'affichage peut être :
- défini **manuellement** ;
- défini **automatiquement** à l'aide des boutons :
  - *Trier l'ordre par identifiant* ;
  - *Trier l'ordre par nom*.

### Portée des types

Lorsqu'un type de réservation est créé, il est **actif pour tous les domaines**.

Ensuite, pour chaque domaine, il est possible :
- d'activer ou de désactiver un ou plusieurs types de réservation ;
- de définir un **type de réservation par défaut** lors de la création d'une nouvelle réservation.

Ces paramètres sont accessibles dans la section **Domaines et ressources**.

### Suppression d'un type

Il est **impossible de supprimer un type de réservation** s'il est déjà utilisé par une réservation existante.

Dans ce cas, il est nécessaire d'utiliser la **fusion de types** avant de procéder à la suppression.

### Fusionner des types de réservation

La fusion permet de rattacher les réservations d'un type à un autre.

#### Fonctionnement

- Sélectionner l'identifiant du type à fusionner.
- Sélectionner l'identifiant du type de destination.

Le premier type sera **supprimé**, et **toutes les réservations associées** seront rattachées au second type.

### Obligation du type de réservation

Le **type de réservation est obligatoire**
