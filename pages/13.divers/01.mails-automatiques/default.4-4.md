---
title: 'Mails automatiques'
---

! Requiert l'activation et la configuration de l’envoie de mail dans [Configuration générale / Interactivité](https://devome.com/GRR/DOC/configuration-generale/interactivite)


Lorsqu'un utilisateur **réserve une ressource**, **modifie** ou bien **supprime** une réservation au nom d'un autre utilisateur, ce dernier (si le champ e-mail a été renseigné) en est averti automatiquement par un message e-mail.

La page **Mails automatiques** permet de gérer l'envoi de notifications par e-mail pour les actions liées aux réservations de ressources.

### Notifications liées aux réservations

- Lorsqu'un utilisateur **réserve une ressource**, **modifie** ou **supprime** une réservation au nom d'un autre utilisateur, ce dernier (si le champ e-mail a été renseigné) reçoit automatiquement un message e-mail.  

- Lorsqu'un utilisateur **réserve une ressource**, **modifie** ou **supprime** une réservation pour lui-même (dont il est bénéficiaire), cochez la case correspondante pour que **un e-mail de confirmation soit systématiquement envoyé**.

### Notifications supplémentaires

Certains utilisateurs peuvent également être prévenus par e-mail pour toute action sur une réservation.  
Pour chaque ressource, vous pouvez désigner un ou plusieurs utilisateurs à prévenir.

#### Ajouter un utilisateur

1. Sélectionner le domaine et la ressource.
2. Sélectionner l'utilisateur dans la liste déroulante.
3. Cliquer sur **Ajouter**.

Par défaut, l'utilisateur ajouté recevra un **mail à chaque réservation**.

#### Tableau des utilisateurs notifiés

**Explications des champs :**

- **Identifiant** : Nom d'utilisateur unique dans GRR.  
- **Nom** / **Prénom** : Informations personnelles de l'utilisateur.  
- **Mail à chaque réservation** :  
  Permet de recevoir un e-mail à chaque création, modification ou suppression d'une réservation.  
- **Mail hebdomadaire** :  
  Permet de recevoir un récapitulatif hebdomadaire des réservations.  
- **Action** :  
  Permet de supprimer l'utilisateur de la liste de notification.

!!! **Nouveauté GRR 4.4.0 :** Mail hebdomadaire

#### Mail hebdomadaire

Le mail hebdomadaire est déclenché **chaque lundi** (non paramétrable pour le moment).

Son déclenchement se fait lors de la **première visite d'un visiteur sur GRR**.  
Dans le cas où aucune visite n'aurait lieu le lundi, le déclenchement se réalisera lors de la **première visite ultérieure** sur l'application.




