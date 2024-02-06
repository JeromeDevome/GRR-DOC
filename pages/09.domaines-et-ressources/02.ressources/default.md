---
title: Ressources
---

Une ressource est un élément réservable (Une salle, une voiture, un vidéoprojecteur, une personne...). Chaque ressource appartient à un unique domaine.

Chaque ressource peut posséder une configuration différente des unes des autres, qui vient s'ajouter aux paramètre du domaine au qu'elle elle est rattachée.

#### Renseignements divers
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
* **Déclarer cette ressource temporairement non disponible.** Les réservations sont alors impossibles. La restriction ne s'applique pas aux gestionnaires de la ressource et aux administrateurs.
* **Rendre visible la fiche de présentation de la ressource dans l'interface publique.** Dans cas il y ara une loupe sur la vue planning, lors d'un clic sur celle-ci la fiche de la ressource s'ouvre. Elle comprend nom, description, capacité, image.
* **Choisir une image de la ressource pour la fiche de présentation.** Une seule image est possible par ressource.
* **Supprimer l'image actuelle de la ressource.** Dans ce cas après validation, l'image sera simplement supprimé du serveur.
* **Afficher la description complète dans le titre des plannings.** Si la case est coché elle s'affichera en dessous du nom et de la description.
* Une **Description complète** qui permet d'écrire un texte avec mise en forme (liste, gras, surligner, tableau, lien).

#### Configuration des fonctionnalités

!! En cours  de rédaction

* on peut définir un nombre maximum de réservations par utilisateur, pour une ressource donnée. Par défaut (valeur -1) il n'y a pas de restriction.
* Attention : ces restrictions ne s'appliquent pas aux administrateurs généraux ainsi qu'aux administrateurs restreints du domaine ou aux gestionnaires chargés d'administrer la ressource.
* Vous pouvez également définir, dans la configuration générale de GRR, un nombre maximal de réservations qui s'applique toutes ressources confondues.
* Possibilité de définir un nombre maximal de jours au-delà duquel l'utilisateur ne peut pas réserver ou modifier une réservation.
* Exemple : une valeur égale à 30 signifie qu'un utilisateur ne peut réserver une ressource que 30 jours à l'avance au maximum. Cette limitation ne touche pas les gestionnaires de la ressources ainsi que les administrateurs du domaine.
* Possibilité de définir un temps en minutes en-deçà duquel l'utilisateur ne peut pas réserver ou modifier une réservation (0 si pas de restriction).
* Exemple : une valeur égale à 60 signifie qu'un utilisateur ne peut pas réserver une ressource ou modifier une réservation moins de 60 minutes avant le début de la réservation.
* Cette limitation ne touche pas les gestionnaires de la ressources ainsi que les administrateurs du domaine.
* Possibilité (case à cocher) de permettre ou non les réservation dans le passé ainsi que les modifications et suppressions de réservations passées.
* Si la case n'est pas cochée, un usager (ni même un gestionnaire ou un administrateur restreint de domaines) ne peut effectuer une réservation dans le passé, ni modifier ou supprimer une réservation passée. Seul l'administrateur général a cette possibilité.
* L'administrateur et le(s) gestionnaire(s) désigné(s) ont la possibilité de déclarer la ressource « temporairement indisponible ». Ceci est alors clairement signalé sur les plannings de réservation (« jour » et « semaine ») et a pour effet de rendre impossible toute nouvelle réservation et toute modification de réservations existantes (sauf pour l'administrateur et les gestionnaires de la ressource).
* L'administrateur et le(s) gestionnaire(s) désigné(s) peuvent choisir de rendre visible ou non la fiche de présentation d'une ressource. Pour cette fiche, ils disposent d'un champ permettant une description complète de la ressource. Ce champ dispose d'une barre d'outils de mise en forme utilisant l'application ckEditor. (Il est possible de désactiver cette fonctionnalité dans la page de configuration générale de GRR. Le répertoire "ckeditor" et tout ce qu'il contient n'est alors pas nécessaire au bon fonctionnement de GRR.)
* On peut également choisir une image pour la ressource qui sera alors visible dans la fiche de présentation.
* Dans la page de modification des paramètres d'une ressource, l'administrateur a la possibilité d'activer la fonction « Poser des réservations sous réserve ». Dans ce cas, la personne effectuant une réservation a la possibilité de remplir un champ supplémentaire : « Réservation à confirmer au plus tard le ... ». Si l'utilisateur ne confirme pas sa réservation avant la date indiquée, la réservation est automatiquement supprimée et un mail automatique est envoyé aux personnes concernées.
* Possibilité, sous certaines conditions, de changer l'affectation d'une ressource à un domaine.
* Possibilité d'activer la fonctionnalité "gestion des clés".

