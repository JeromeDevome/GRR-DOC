---
title: Interactivité
---

### Envoi de mails automatiques

**Envoi de mails automatiques :**
L'administrateur peut activer ou désactiver l'option permettant l'envoi d'emails automatiques.

 Si cette option est activée, dans un certain nombre de cas (création d'une réservation, suppression/modification, modération, ...), GRR envoie automatiquement des mails à certains utilisateurs à conditions que ces derniers ont une adresse mail renseigné dans leur compte.
Par ailleurs, dans la page de gestion des mails automatiques, toujours si cette option est activée, l'administrateur peut affecter à chaque ressource un ou plusieurs utilisateurs à prévenir par mail automatique lorsqu'une réservation est effectuée ou lorsque qu'il y a modification ou suppression de la réservation.

!!! Certains hébergeurs désactivent l'envoi automatique de mails depuis leurs serveurs. Dans ce cas, cette fonctionnalité sera inopérante. Ce n'ai pas les cas avec l'offre MyGRR.

### Configuration des liens email

* Utiliser le formulaire d'envoi de mails : dans ce cas, un clic sur un "lien email" affiche un formulaire qui permet d'envoyer un mail au(x) destinataire(s), sans divulguer leur adresse email.
* Utiliser les balises "mailto" : dans ce cas, un clic sur un "lien email" ouvre le logiciel de courrier par défaut de la machine du client et prépare un nouveau message en complétant automatiquement le champ des destinataires (à noter que bien que les adresses email apparaissent en clair dans GRR)

### Paramètres de configuration de l'envoi automatique des mails

Il existe deux méthodes pour l'envoi de mail :
1. La méthode "smtp" permettant de se connecter à un serveur de mail distant ; il faudra donc renseigner les différentes informations (serveur smtp, utilisateur mot de passe...)
2. La méthode "mail" lorsque le serveur de mail est local (aucune configuration dans GRR)

Dans les deux cas vous pouvez saisir votre adresse mail dans le champ "Email de test". Si votre configuration est bonne après avoir cliqué sur "Enregistrer" vous recevrez un mail sur l'adresse saisie. Le champ "Email de test" est réinitialisé à chaque validation.

Vous avez une option : **Mettre les destinataires en copie cachée lorsqu'un message est adressé à plusieurs personnes.**

Si L'envoi de mail est désactivée, aucun mail ne sera envoyé depuis le serveur **GRR**.


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


!!! L'option 2 n'ai pas disponible dans l'offre MyGRR
