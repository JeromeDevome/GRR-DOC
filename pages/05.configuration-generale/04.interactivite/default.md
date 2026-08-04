---
title: Interactivité
---

!!! Depuis la version 4.6, la configuration du serveur de messagerie se trouve dans « Mails » > « Serveurs de mails ».


### Configuration des liens email

* Utiliser le formulaire d'envoi de mails : dans ce cas, un clic sur un "lien email" affiche un formulaire qui permet d'envoyer un mail au(x) destinataire(s), sans divulguer leur adresse email.
* Utiliser les balises "mailto" : dans ce cas, un clic sur un "lien email" ouvre le logiciel de courrier par défaut de la machine du client et prépare un nouveau message en complétant automatiquement le champ des destinataires (à noter que bien que les adresses email apparaissent en clair dans GRR)


### Affichage des "pop-up" de confirmation après la création/modification/suppression d'une réservation

Choix possibles :
* Activer les messages JavaScript
* Désactiver les messages JavaScript

Affichage (oui ou non) des "pop-up" de confirmation après la création/modification/suppression d'une réservation.


### Affichage des "pop-up" de confirmation dans les menus d'administration

! Ce paramètre va prochainement disparaitre. Les pop-up sont remplacé par des toast qui sont moins intrusifs.

Choix possibles :
* Activer les messages JavaScript
* Désactiver les messages JavaScript

Affichage (oui ou non) des "pop-up" de confirmation dans les menu d'administration.


### Méthode d'exécution automatique de tâches

L'activation de certaines fonctionnalités de GRR nécessite la possibilité de mettre en place l'exécution automatiques de tâches.
Par exemple la suppression automatique de certaines réservations dans le cas des « réservations sous réserve », ou encore l'envoi d'une notification de retard en cas de non restitution d'une ressource.
Pour effectuer ces tâches automatiques de suppression, il y a deux configurations possibles, chacune ayant ses inconvénients et ses avantages. .

1. La tâche automatique est déclenchée une fois par jour lors de la connexion du premier utilisateur
*  	Avantages : Pas de configuration, natif à GRR.
*  	Inconvénient : Si pas de visite le script n'ai pas lancé.
2. La tâche automatique est déclenchée par l'exécution du script « verif_auto_grr.php ». Dans ce cas il faut configurer le champ mot de passe et chemin complet (nécessite la possibilité de programmer l'exécution automatique et périodique du script verif_auto_grr.php)
*  	Avantage : Lancé automatiquement à l'heure configuré
*  	Inconvénients : Configuration de tâche sur le serveur, maintenance supplémentaire en cas de changement

! L'option 2 n'ai pas disponible dans l'offre MyGRR
