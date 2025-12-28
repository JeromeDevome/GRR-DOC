---
title: Ressources
---

Une ressource est un élément réservable (Une salle, une voiture, un vidéoprojecteur, une personne...). Chaque ressource appartient à un unique domaine.

Chaque ressource peut posséder une configuration différente des unes des autres, qui vient s'ajouter aux paramètre du domaine au qu'elle elle est rattachée.

#### Renseignements divers

!!! **Nouveauté GRR 4.5.0:** Réservation confidentielle

* Un **nom** qui sera afficher dans le planning et les statistiques.
* Une **description**, elle serra affichée juste en dessous du nom de la ressource dans les vues plannings.
* Un **domaine** au qu'elle elle est rattachée.
* Un **ordre d'affichage**, qui sera utile dans l'affichage du menu ou dans les vues comportant toute les ressources d'un domaine.
* Un droit de visibilité sur la ressource (**Qui peut voir cette ressource ?**). Si le domaine est en restreint, ce droit ne substitut pas à l'accès au domaine en question.
 * N'importe qui allant sur le site même s'il n'est pas connecté
 * Il faut obligatoirement être connecté, même en simple visiteur.
 * Il faut obligatoirement être connecté et avoir le statut "utilisateur"
 * Il faut obligatoirement être connecté et être au moins gestionnaire d'une ressource
 * Il faut obligatoirement se connecter et être au moins administrateur du domaine
 * Il faut obligatoirement être connecté et être administrateur de site
 * Il faut obligatoirement être connecté et être administrateur général
* **Déclarer cette ressource temporairement non disponible.** Ceci est alors clairement signalé sur les plannings de réservation (« jour » et « semaine ») et a pour effet de rendre impossible toute nouvelle réservation et toute modification de réservations existantes (sauf pour l'administrateur et les gestionnaires de la ressource).
* **Réservation confidentielle**, permet de limiter les informations disponible aux usager et à l'accès de la fiche du détail de la réservation en dehors de l'utilisateur et du gestionnaire de ressource.
* **Accès restreint**,  si la case est cochée, seuls les utilisateurs autorisés peuvent réserver cette ressource.
* **Rendre visible la fiche de présentation de la ressource dans l'interface publique.** Dans cas il y ara une loupe sur la vue planning, lors d'un clic sur celle-ci la fiche de la ressource s'ouvre. Elle comprend nom, description, capacité, image.
* **Choisir une image de la ressource pour la fiche de présentation.** Une seule image est possible par ressource. Extensions autorisées : jpg, png, gif.
* **Supprimer l'image actuelle de la ressource.** Dans ce cas après validation, l'image sera simplement supprimé du serveur.
* **Afficher la description complète dans le titre des plannings.** Si la case est cochée, elle s'affichera en dessous du nom et de la description.
* Une **Description complète** qui permet d'écrire un texte avec mise en forme (liste, gras, surligner, tableau, lien).

#### Configuration des fonctionnalités

**Pour une nouvelle réservation ou modification d'une réservation, l'utilisateur spécifie la date/heure de début de réservation et** :
- la durée de la réservation
- la date/heure de fin de réservation

**Nombre de personnes maximum autorisé dans la salle (0 s'il ne s'agit pas d'une salle)** : Il ne s'agit que d'un élément à titre indicatif.

**Le nombre maximum de réservations de cette ressource par utilisateur a été fixé à** :  "-1" par défaut,  il n'y a pas de restriction. La valeur 0 empêchera tout utilisateur de réserver. Une valeur supérieur limitera le nombre de réservation possible à la date heure du jour.

_Exemple : Le paramètre est à 2.  Nous sommes le 1er février,  l'utilisateur à une réservation le 7 et 14 février, il ne pourra pas poser de troisième réservation sur cette ressource. Le 8 février il pourra poser une nouvelle réservation. Cette limitation ne touche pas les gestionnaires de la ressource ainsi que les administrateurs du domaine._

**Nombre maximal de jours au-delà duquel l'utilisateur ne peut pas réserver ou modifier une réservation (-1 si pas de restriction).**
_Exemple : une valeur égale à 30 signifie qu'un utilisateur ne peut réserver une ressource que 30 jours à l'avance au maximum. Cette limitation ne touche pas les gestionnaires de la ressource ainsi que les administrateurs du domaine._

**Temps en minutes en-deçà duquel l'utilisateur ne peut pas réserver ou modifier une réservation (0 si pas de restriction).**
_Exemple : une valeur égale à 60 signifie qu'un utilisateur ne peut pas réserver une ressource ou modifier une réservation moins de 60 minutes avant le début de la réservation. Cette limitation ne touche pas les gestionnaires de la ressource ainsi que les administrateurs du domaine._

**Poser des réservations "sous réserve" : indiquer une valeur différente de 0 pour activer cette fonctionnalité. La valeur ci-contre désigne le nombre maximal de jours dont dispose le réservant pour confirmer une réservation.**

**Modérer les réservations de cette ressource : Une réservation n'est effective qu'après validation par un administrateur du domaine ou un gestionnaire de la ressource.**
Si les conditions sont réunis, le bénéficiaire recevra un mail de confirmation.

**Permettre les réservations dans le passé ainsi que les modifications/suppressions de réservations passées. Si la case n'est pas cochée, un usager (ni même un gestionnaire ou un administrateur restreint) ne peut effectuer une réservation dans le passé, ni modifier ou supprimer une réservation passée. Seul l'administrateur général a cette possibilité.**

**Ne pas permettre aux utilisateurs (hormis les gestionnaires et les administrateurs) de modifier ou de supprimer leurs propres réservations.**

**Hormis les administrateurs, précisez ci-contre quels types d'utilisateurs ont le droit de faire des réservations au nom d'autres utilisateurs.** Une liste avec l'ensemble des utilisateurs de GRR et un champ pour les personnes extérieur sera affiché dans le formulaire de réservation si l'utilisateur à les droits.
Choix :
- personne
- uniquement les administrateurs restreints
- les gestionnaire de la ressource
- tout les utilisateurs

**Activer la fonctionnalité "ressource empruntée/restituée"** : Dans la fiche de réservation vous aurez accès à un formulaire avec les options suivantes :
- La ressource a été restituée. (Sélectionner également cette option si vous n'utilisez pas cette fonctionnalité)
- Signaler que la ressource est empruntée dans le cadre de cette réservation.
- Signaler que la ressource est empruntée dans le cadre de cette réservation et envoyer quotidiennement un mail notifiant le retard.
ET
 - Envoyer immédiatement un mail de notification de retard (non restitution dans les délais) 


**Activer la fonctionnalité "gestion des clés"** : Dans la fiche de réservation vous aurez accès à une case clé emprunté oui/non.

!!! **Nouveauté GRR 4.4.0:** Ajout des droits sur l'utilisation de la fonctionnalité "participant" lors de la création d'une réservation*

**Qui peut utiliser la fonctionnalité "participant" lors de la création d'une réservation**
Choix :
- personne
- Il faut obligatoirement être connecté et avoir le statut "utilisateur" 
- Il faut obligatoirement être connecté et être au moins gestionnaire d'une ressource
- Il faut obligatoirement se connecter et être au moins administrateur du domaine
- Il faut obligatoirement être connecté et être administrateur de site
- Il faut obligatoirement être connecté et être administrateur général


!!! **Nouveauté GRR 4.4.0:** Les droits à "Qui peut utiliser la fonctionnalité" sont plus précis

**Qui peut utiliser la fonctionnalité "participant"**
Choix :
- personne
- Il faut obligatoirement être connecté, même en simple visiteur.
- Il faut obligatoirement être connecté et avoir le statut "utilisateur" 
- Il faut obligatoirement être connecté et être au moins gestionnaire d'une ressource
- Il faut obligatoirement se connecter et être au moins administrateur du domaine
- Il faut obligatoirement être connecté et être administrateur de site
- Il faut obligatoirement être connecté et être administrateur général

La fonctionnalité permet à la personne qui pose une réservation de mettre un nombre maximum de participant. Les utilisateurs pourrons s'inscrire à l'évènement.
_Exemple : Un utilisateur créé une réservation d'une salle pour un cours, il indique 10 participants, les 10 premiers utilisateur cliquant sur "Je participe dans la réservation" sont inscrits_

La fonctionnalité, peut-être utilisé pour des formations, du covoiturage, des concours...

!!! **Nouveauté GRR 4.4.0:** Nombre de participant par défaut 

**Nombre de participant par défaut ":** Permet de définir un nombre de participant maximum par défaut lors de la création d'une réservation. 


