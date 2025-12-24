---
title: Fonctionnalités
---

!!! Nouveauté GRR 4.1.0

### Divers

**Autoriser la périodicité dans les réservations :** Permet aux utilisateurs de créer des réservations avec avec une répétition (journalière, hebdomadaire, mensuel...)

**Afficher la gestion des salles par courrier :**  Permet de générer un PDF en forme de courrier en saisissant les coordonnées du destinataire. Le PDF reprend les informations de la réservation. Ce PDF n'est pas modifiable dans l'administration.

**Échanger deux réservations :** Permet sous certaine condition, l'échange de deux réservations.


### Formulaire de contact pour réservation

Le formulaire de contact de réservation, permet à des personnes de faire une demande de réservation sous forme de mail sans pour autant l'inscrire dans le planning.

Le formulaire peut être désactivé, être disponible qu'au personnes non connecté et visiteurs, ou qu'aux visiteurs. Il faut cependant que l'accès à GRR ne nécessite pas de se connecter (Configuration générale => Accès et droits => Accès à GRR)

Saisir l'adresse du destinataire du formulaire. Vous pouvez indiquer plusieurs adresse mail en les séparant par des points virgule (sans espace).

Cocher la case **Envoyer une copie à l'utilisateur** pour que ce dernier reçoit le même mail que le destinataire.

!!! Captcha : Nouveauté 4.1.0

**Utiliser le captcha :** Permet de limiter les spam par des robots. Ce paramètre n'a pas d'utilité pour les serveurs qui ne sont pas ouvert sur internet.

!!! Texte avant le formulaire : Nouveauté 4.3.0

**Texte avant le formulaire :** Permet de définir un texte sur la page qui sera affiché juste avant le formulaire de contact.


### Demande de création de compte

!!!  Demande de création de compte : Nouveauté 4.2.0

Permettre aux personnes non connecté de demander la création d'un compte. Le formulaire est disponible sur la page de connexion via un lien sur la page de connexion.

L'utilisateur devra renseigner son nom, prénom, e-mail et mot de passe, une fois. Le gestionnaire d'utilisateur ou l'administrateur pourra valider ou non la demande en lui assignant un identifiant et un statut.

! Avertissement : Il est conseiller d'activer l’envoi de mail, dans le cas contraire l'utilisateur ne pourra recevoir son identifiant.

**Format de l'identifiant :** Forme sous la laquelle sera proposer la création de son identifiant (Nom, prénom, nom.prénom...) . Le gestionnaire peut modifier l'identifiant avant de valider la création de compte.

**Statut par défaut :** Choix entre visiteur ou usager. Le gestionnaire à le choix au moment de la validation. Il pourra dans tout les cas modifier le statut de l'utilisateur dans la gestion des utilisateurs.

**Utiliser le captcha :** Permet de limiter les spam par des robots. Ce paramètre n'a pas d'utilité pour les serveurs qui ne sont pas ouvert sur internet.
