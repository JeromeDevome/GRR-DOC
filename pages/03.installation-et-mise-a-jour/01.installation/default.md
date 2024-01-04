---
title: Installation
---

!!! L'installation ne s'applique pas à l'offre MyGRR, l'ensemble de l'installation est comprise dans l'offre


# 1 - Téléchargement de GRR

Pour obtenir la dernière version de GRR, veuillez télécharger l'archive sur GitHub  [https://github.com/JeromeDevome/GRR/releases](https://github.com/JeromeDevome/GRR/releases)

! Il est déconseillé d'utiliser les version en "Pre-release" pour un serveur en production


# 2 - Prérequis

## 2.1 - Serveur

GRR, fonction sur un serveur web avec PHP et MySQL. Nous de détaillerons pas l'installation de ces derniers dans la procédure, ce ceux peuvent varier selon le type serveur que vous avez. L'espace disque minimum requis est conseillé à 200Mo pour le code de GRR. Le processeur et la RAM dépendent du type de serveur.


### Table

| Version de GRR       | Service                       | Mini & Max       |
| :-------------------------- | :---------------------------: | -------------------: |
| 4.0 							 | PHP							  | 7.2.5 à 8.1.X    |
| 								   | SQL               			    | 5.4 à 5.7       	  |


**Les modules PHP suivant sont obligatoire pour le bon fonctionnement de GRR :**
* php-gd
* php-mbstring
* php-mysqli
* php-mysqlnd
* php-xml
* php-intl `(Obligatoire depuis la version GRR 4.1.0)`

## 2.2 - Poste client

Un navigateur web autorisant les cookies.

# 3 - Installation

## 3.1 - Transfert des fichiers

La première étape de l'installation consiste à transférer tous les fichiers de
l'archive que vous avez téléchargée vers le serveur web/php.

Pour cela, munissez-vous des codes des paramètres de connexion au serveur et
utilisez un logiciel de transfert de fichiers (FTP). Vous aurez besoin de l'adresse du serveur ftp, de votre login, et de votre  mot de passe (fournis par l'hébergeur si vous utilisez un service extérieur, par l'administrateur système si vous utilisez un serveur au sein de l'établissement).

On pourra par exemple créer un répertoire "grr" dans le répertoire
web du serveur ("htdocs" dans le cas d'Apache).

Modification des droits : les droits d'écriture doivent être attribués
* au répertoire "/personnalisation" 
* au répertoire "/temp"

## 3.2 - Création des bases


Vous avez le choix entre deux types d'installation de la base de données Mysql:
*  une installation automatisée , `Recommandé`
*  une installation manuelle, réservée aux experts.


### 3.2.1 - Installation automatisée


Une fois que les fichiers php sont en place sur le serveur web/php (étape 2),
lancez un navigateur et connectez-vous au site en tapant l'adresse complète du
genre : http://www.monsite.fr/grr
Vous n'avez plus qu'à cliquer sur le lien vous proposant d'installer la base
et à suivre la procédure en complétant les différents éléments demandés.


### 3.2.1 - Installation manuelle

Si vous optez pour cette installation, il est nécessaire d'avoir renseigné le
fichier "connect.inc.php" ce trouvant dans le dossier "personnalisation" (voir plus haut)

Dans l'archive figure le fichier tables.my.sql (dans le dossier "installation") à exécuter sur le serveur mysql et qui
contient l'ensemble des tables mysql ainsi que les données minimales pour
que ça fonctionne.

-  Sur le serveur mysql :
* créez une base mysql (avec phpMyAdmin par exemple) en lui donnant un nom (par
exemple "grr")
* créez un utilisateur de cette base,

-  Connectez-vous à cette base.
* Exécuter le  fichier tables.my.sql dans cette base
(toujours avec phpMyAdmin par exemple)


# 4 - L'après

Une fois le système installé, vous pouvez vous connecter à GRR :
-  nom de connexion : `administrateur` et le mot de passe créé lors de l'installation


! Il est conseillé de supprimer le dossier installation

! Il est fortement conseillé de vérifier régulièrement si des mises à jour GRR sont disponibles et de les appliquer pour des raisons de sécurités.