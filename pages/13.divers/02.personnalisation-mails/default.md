---
title: 'Personnalisation mails'
media_order: Variables-Mails-GRR.xlsx
---

!!! Ceci est une nouveauté GRR 4.2.0

Vous pouvez ici personnaliser les mails (titre et sujet) envoyés aux utilisateurs pour chaque évènement et chaque langue de GRR. 
Vous pouvez y modifier le texte tout en utilisant des variables (cf. ci dessous) ainsi qu'ajouter des styles à vos textes.

! **Attention:** A ce jour il n'existe pas de bouton pour réinitialiser les paramètres par défaut. Modifier les donc avec prudence.


### Les variables

Les variables sont définit entre des "%" , exemple : 
> %ceciestunevariable%

Les variables, permette d'y mettre des éléments dynamique, tel que des paramètres configuré dans l'administration ou des informations de la réservation.

Les variables disponible dépende de la version de GRR mais aussi du type de mail. Elles sont utilisables dans les titres et le texte du mail.

#### a) Variables et définitions

**decisionmoderation**: Texte indiquant si la réservation est accepté ou refusé.

**decisionmotif**: Réponse du modérateur de la réservation.

**domaine**: Domaine de la réservation.

**enattentemoderation**: Affiche un "(En attente de modération)" si c'est le cas, sinon rien.

**formcommentaire**: Commentaire dans le formulaire (uniquement pour les demandes de création de compte).

**formemail**: E-mail dans le formulaire (uniquement pour les demandes de création de compte).

**formnom**: Nom dans le formulaire (uniquement pour les demandes de création de compte).

**formprenom**: Prénom dans le formulaire (uniquement pour les demandes de création de compte).

**formtelephone**: Téléphone dans le formulaire (uniquement pour les demandes de création de compte).

**identifiant**: Identifiant créer dans le cas où la demande de création de compte est accepté.

**logincompletbeneficiaire**: Nom Prénom et E-Mail du bénéficiaire de la réservation.

**logincompletuser**: Nom Prénom et E-Mail de la personne connectée.

**maildestinataire**: Indique l'adresse mail à qui le retard est envoyé.

**nomdusite**: Paramètre dans "Configuration générale" : "Gros titre de la page de connexion".

**nometablissement**: Paramètre dans "Configuration générale" : "Nom de l'établissement ".

**raisonmail**: Affiche la raison de l’envoi du mail à cet adresse mail.

**resachampsadditionnels**: Affiche les champs additionnels de la réservations.

**resaconfirmation**: Message et date de réservation de confirmation au plus tard dans le cas contraire rien.

**resadatedebut**: Date et heure du début de la réservation.

**resadatefin**: Date et heure de fin de la réservation.

**resadescription**: Description complète de la réservation.

**resaduree**: Durée de la réservation.

**resanom**: Brève description de la réservation.

**resaperiodique**: Affiche les informations de la périodicité, dans le cas contraire rien.

**resatype**: Type de la réservation.

**ressource**: Ressource concernant la ressource.

**urldetail**: Lien vers la réservation. Attention utilise le paramètre dans "Configuration générale" => "Adresse (URL) exacte de GRR".

**urlgrr**:Paramètre dans "Configuration générale" : "Adresse (URL) exacte de GRR".

**webmasteremail**: Paramètre dans "Configuration générale" : "Adresse email du gestionnaire du site".


#### b) Variables et disponibilités

Vous pouvez voir dans la disponibilité de chaque variable pour les différents cas de mail, et la version minimum de GRR requis dans ce tableur [Variables-Mails-GRR.xlsx](Variables-Mails-GRR.xlsx).
