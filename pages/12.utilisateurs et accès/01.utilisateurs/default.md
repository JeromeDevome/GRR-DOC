---
title: Utilisateurs
---

Un utilisateur, est un compte nommé, permettant de se connecter à GRR.
En bas de chaque fiche utilisateur vous pouvez y retrouver les différents privilèges (gestionnaire, administrateur...) de ce dernier.


### Création des comptes

Il existe plusieurs méthodes pour créer les comptes.

#### a) Ajout manuellement
La méthode de base où vous pouvez ajouter les utilisateurs un par un.

Avantages : Rapide et simple pour quelques utilisateurs. Configuration par utilisateur.
Inconvénient : Long en cas de grand nombre d'utilisateur.

#### b) Ajout via un fichier
Vous pouvez importer un fichier de type CSV avec l'ensemble des comptes à créer ou modifier.

Avantage : Rapide en cas de nombreux utilisateurs, surtout si vous avez déjà un fichier avec la liste des utilisateurs.
Inconvénients : Manipulation de fichier, pas de gain pour quelques utilisateurs à créer.

#### c) elycée
Vous pouvez importer un fichier de type CSV provenant d'elycée avec l'ensemble des comptes à créer ou modifier.

Avantage : Rapide.
Inconvénient : Nécessite elycée.

#### d) Connexions externe
Si vous avez un type de connexion existant qui est pris en compte par GRR, vous pouvez les inter-connecter.
_Pour plus de détail (cf. Connexions externes)_

Avantage : Les utilisateurs sont créés automatiquement.
Inconvénient : Choix unique pour le statut.

### Informations utilisateur

**Identifiant:** L'identifiant est unique, il est utilisé notamment pour la connexion. Il ne peut-être modifié ! Les espaces sont interdits.

**Nom:** Permet d'identifier l'utilisateur

**Prénom:** Permet d'identifier l'utilisateur

**E-mail:** Permet l’envoi de mail automatique _(si l'option est activé)_

**Statut:** Cf. [4. Les utilisateurs / Status & Rôles](http://devome.com/GRR/DOC/les-utilisateurs/statuts-and-roles)

**Authentification:** Locale/Externe, n'utiliser externe que si l'utilisateur se connecte via une connexion externe. Vous pouvez créer le compte en amont de sa connexion pour pouvoir lui configurer ces droits.

**Mot de passe:** Uniquement en cas d'authentification locale. Vous pouvez lui définir le mot de passe, le nombre de caractère minimum est définis dans la [configuration générale](http://devome.com/GRR/DOC/configuration-generale/securite-connexions)

**L'utilisateur doit changer son mot de passe à la prochaine connexion:** Uniquement en cas d'authentification locale. Dans ce cas l'utilisateur à la prochaine connexion aura l'obligation de changer son mot de passe.

**État (En mode édition):** Actif/Non actif permet d'autoriser ou non la connexion de l'utilisateur. Par défaut l'utilisateur est actif.

**Groupe:**  Un utilisateur peux faire partit de plusieurs groupes [(cf. Groupes)](http://devome.com/GRR/DOC/utilisateurs%20et%20acc%C3%A8s/groupes)

**Différentes option d'affichage (En mode édition):** Par défaut à la création, l'utilisateur hérite des paramétrages de la [configuration générale / Apparence](http://devome.com/GRR/DOC/configuration-generale/apparence).

