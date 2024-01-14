---
title: 'Mise à jour - Depuis version >= 4'
---

!!! La mise à jour ne s'applique pas à l'offre MyGRR, l'ensemble de la prestation est comprise dans l'offre


# 1 - Préambule

Cette page vous explique comment procédé à une mise à jour à partir d'une version 4.X.X de GRR vers la dernière version de GRR.
Si vous êtes dans une version plus ancienne, veuillez suivre la procédure  [Mise à jour - Depuis version < 4](http://devome.com/GRR/DOC/installation-et-mise-a-jour/mise-a-jour-depuis-version-less-than-4)

Il est fortement conseillé de vérifier et de mettre à jour son GRR régulièrement. Les mises à jour peuvent comporter des nouveautés, des corrections, des patchs de sécurité, et malheureusement des bogues.

Vous pouvez faire des sauts de versions, il n'est pas nécessaire de mettre à jour votre GRR vers les versions que vous avez manqué. Une fois la base de données à jour, il est déconseillé de rétrograder de version.

Dans tout les cas ni les développeurs, ni DEVOME n'est responsable des dysfonctionnement et des dommages que cela peut occasionner.



!! Avant de commencer procéder par une sauvegarde complète de vos fichiers et de la base SQL


# 2 - Prérequis

Pour obtenir la dernière version de GRR, veuillez télécharger l'archive sur GitHub  [https://github.com/JeromeDevome/GRR/releases](https://github.com/JeromeDevome/GRR/releases)

! Il est déconseillé d'utiliser les version en "Pre-release" pour un serveur en production


Veuillez aussi vérifier que votre serveur est compatible avec la dernière version de GRR [2.1 Prérequis](http://devome.com/GRR/DOC/installation-et-mise-a-jour/installation#2-1-serveur)

# 3 - Mise à jour des fichiers


## 3.1 - Mise à jour des fichiers

Supprimer du serveur, l'ensemble des fichiers de GRR **à l’exception du dossier "personnalisation"**. _(Supprimer et n'écraser pas pour ne pas laisser des fichiers inutile pouvant comporter des failles)_
Transférer sur votre serveur les fichiers précédemment téléchargé à l'étape 2.


## 3.2 - Mise à jour de la base de données

En accédant via un navigateur à votre GRR, on vous proposera l'installation ou la mise à jour. Sélectionner `mise à jour`, et vérifier le résultat de la mise à jour. Les erreurs non critiques peuvent être ignoré.

Si vous n'avez pas la proposition ci-dessous : veuillez accéder à http://www.monsite/grr/installation/maj.php _(à adapter !)_

La mise à jour est terminé


## 3.3 - Sécurité

Pour des raisons de sécurité, veuillez supprimer le dossier `installation` de votre serveur.
