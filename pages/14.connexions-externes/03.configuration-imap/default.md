---
title: 'Configuration IMAP'
---

!!! MyGRR cloud : Fonction non disponible pour le moment.

Il est possible de se connecter à GRR en s'authentifiant à l'aide d'un compte IMAP ou POP3.

L'activation de l'authentification IMAP/POP consiste à choisir le statut par défaut des utilisateurs venant de l'annuaire (« usager » ou « visiteur »).

Une fois authentification activée, il faut configurer le fichier « config_imap.inc.php », soit manuellement, soit en utilisant la procédure automatique accessible à partir de la même page.

**Remarque:** l'authentification IMAP/POP ne permet pas de récupérer les données (nom, prénom, ...) de l'utilisateur : celui-ci est donc invité lors de la première connexion à compléter son profil. 