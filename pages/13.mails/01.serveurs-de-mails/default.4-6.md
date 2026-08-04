---
title: 'Serveurs de mails'
---

!!! Avant la version 4.6, tous ces paramètres se trouvaient dans l'onglet « Interactivité » de la page « Configuration générale ».

### Envoi de mails automatiques

**Envoi de mails automatiques :**
L'administrateur peut activer ou désactiver l'option permettant l'envoi d'emails automatiques.

 Si cette option est activée, dans un certain nombre de cas (création d'une réservation, suppression/modification, modération, ...), GRR envoie automatiquement des mails à certains utilisateurs à conditions que ces derniers ont une adresse mail renseigné dans leur compte.
Par ailleurs, dans la page de gestion des mails automatiques, toujours si cette option est activée, l'administrateur peut affecter à chaque ressource un ou plusieurs utilisateurs à prévenir par mail automatique lorsqu'une réservation est effectuée ou lorsque qu'il y a modification ou suppression de la réservation.

!!! Certains hébergeurs désactivent l'envoi automatique de mails depuis leurs serveurs. Dans ce cas, cette fonctionnalité sera inopérante. Ce n'ai pas les cas avec l'offre MyGRR.


### Paramètres de configuration de l'envoi automatique des mails

Il existe deux méthodes pour l'envoi de mail :
1. La méthode "smtp" permettant de se connecter à un serveur de mail distant ; il faudra donc renseigner les différentes informations (serveur smtp, utilisateur mot de passe...)
2. La méthode "mail" lorsque le serveur de mail est local (aucune configuration dans GRR)

!!! Dans l'offre MyGRR Cloud, si vous utilisez la méthode « mail », l'adresse d'expédition sera noreply@mygrr.net

Dans les deux cas vous pouvez saisir votre adresse mail dans le champ "Email de test". Si votre configuration est bonne après avoir cliqué sur "Enregistrer" vous recevrez un mail sur l'adresse saisie. Le champ "Email de test" est réinitialisé à chaque validation.

Vous avez une option : **Mettre les destinataires en copie cachée lorsqu'un message est adressé à plusieurs personnes.**

Si L'envoi de mail est désactivée, aucun mail ne sera envoyé depuis le serveur **GRR**.
