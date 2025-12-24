---
title: 'Connexions externes'
---

Il est possible de connecter **GRR** avec une autre solution, pour permettre de gérer l'authentification.

Une fois la configuration correctement effectuée d'un connecteur, deux types d'utilisateurs peuvent cohabiter :
* les utilisateurs gérés directement par GRR dans la base locale de GRR et
* les utilisateurs importés de l'annuaire LDAP.

Dans la table "utilisateurs" un champ indique le type d'authentification (« local » ou « ext ») de l'utilisateur.
* Quand le type d'authentification d'un utilisateur est « ext », il ne peut changer son mot de passe dans GRR (celui-ci en effet n'est pas stocké dans GRR).
* L'administrateur peut modifier tous les paramètres d'un utilisateur « ext » tout comme pour un utilisateur « local », à l'exception du mot de passe qui est laissé vide dans la base locale.
* L'administrateur a la possibilité de changer un utilisateur « ext » en un utilisateur « local ».
* GRR n'inscrit aucune donnée dans les annuaires tierce. Ainsi GRR n’a besoin que d’un accès en lecture seule à l’annuaire.



Concrètement, quand un utilisateur tente de se connecter à GRR en tapant un identifiant et un mot de passe, GRR suit la procédure suivante :
* GRR regarde si un utilisateur ayant cet identifiant est présent dans la base des utilisateurs de GRR.
* Si oui : l'utilisateur est connecté à GRR.
* Dans le cas contraire : c'est la première connexion à GRR, GRR crée l'utilisateur « ext » dans la table « utilisateurs » en tentant d'importer le nom et l'adresse email. Le champ « mot de
passe » est laissé vide. Le statut « usager » ou « visiteur » est celui défini par défaut dans la configuration du connecteur. L'administrateur pourra par la suite modifier ces paramètres au cas par cas. La procédure s'arrête : l'utilisateur est alors connecté à GRR. 

!!! remarque : si un utilisateur « local » existant porte déjà le même identifiant, l'importation ne pourra avoir lieu : il y a échec de la connexion).

Une fois un utilisateur « ext » connecté, il est traité par la voie classique, c’est-à-dire simplement avec le cookie de session. Ainsi on ne se connecte au connecteur que lors de la procédure de connexion à GRR. De même, les paramètres pris en compte dans la navigation dans GRR (affichage par défaut, nom, prénom, email, ...) sont ceux de GRR.