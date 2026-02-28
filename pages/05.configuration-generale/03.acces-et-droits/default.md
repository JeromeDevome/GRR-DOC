---
title: 'Accès et droits'
---

### Accès à GRR

Deux options : 
* Il n'est pas nécessaire de se connecter pour voir les réservations (mais la connexion est obligatoire si l'utilisateur veut réserver ou modifier une réservation) .
* Il est obligatoire de se connecter pour accéder au site _(Par défaut)_. (Pour un maximum de confidentialité, chaque utilisateur devra avoir un compte)


### Qui a accès à la fiche de description d'une ressource ?

Accès à la pop-up ou la page de la réservation _(selon configuration dans Apparence)_

Choix possibles :
* N'importe qui allant sur le site même s'il n'est pas connecté
* Il faut obligatoirement être connecté, même en simple visiteur.
* Il faut obligatoirement être connecté et avoir le statut "utilisateur"
* Il faut obligatoirement être connecté et être au moins gestionnaire d'une ressource
* Il faut obligatoirement se connecter et être au moins administrateur du domaine
* Il faut obligatoirement être connecté et être administrateur de site
* Il faut obligatoirement être connecté et être administrateur général


### Qui a accès à la fiche de réservation détaillée d'une ressource ?

La fiche de la ressource, peut contenir une description, capacité, photo _(A configurer dans "Domaine et ressources")_.

Choix possibles :
* N'importe qui allant sur le site même s'il n'est pas connecté
* Il faut obligatoirement être connecté, même en simple visiteur.
* Il faut obligatoirement être connecté et avoir le statut "utilisateur"
* Il faut obligatoirement être connecté et être au moins gestionnaire d'une ressource
* Il faut obligatoirement se connecter et être au moins administrateur du domaine
* Il faut obligatoirement être connecté et être administrateur de site
* Il faut obligatoirement être connecté et être administrateur général

### Qui peut accéder à la page d'édition d'une ressource ?
!!! Nouveauté GRR 4.5.3
Permet de modifier la ressource.

Choix possibles :
* Il faut obligatoirement être connecté et être au moins gestionnaire d'une ressource
* Il faut obligatoirement se connecter et être au moins administrateur du domaine
* Il faut obligatoirement être connecté et être administrateur de site
* Il faut obligatoirement être connecté et être administrateur général

### Accès à l'outil de recherche & stat

Permet sous forme de tableau d'exporter les réservations selon différents critères.

Choix possibles :
* N'importe qui allant sur le site peut accéder à l'outil de recherche, même s'il n'est pas connecté
* Il faut obligatoirement se connecter pour accéder à l'outil de recherche
* Il faut obligatoirement se connecter et avoir le statut "utilisateur" pour accéder à l'outil de recherche
* Il faut obligatoirement se connecter et être administrateur général pour accéder à l'outil de recherche.


### Suppression/Modification de réservations

Choix possibles pour les utilisateurs :
* Un utilisateur ne peut pas supprimer ou modifier une réservation en cours ni créer une réservation sur un créneau "entamé".
* Un utilisateur peut supprimer ou modifier dans certaines conditions une réservation en cours (et dont il est bénéficiaire) et créer une réservation sur un créneau "entamé"
* Un utilisateur peut modifier dans certaines conditions une réservation en cours (et dont il est bénéficiaire), mais ne peut pas créer ni supprimer une réservation sur un créneau "entamé"

Choix possibles pour les gestionnaire d'une ressource :
* Un gestionnaire d'une ressource ne peut pas supprimer ou modifier les réservations effectuées sur la ressource, sauf celles dont il est l'auteur.
* Un gestionnaire d'une ressource peut supprimer ou modifier n'importe quelle réservation effectuée sur la ressource


### Modification du profil utilisateur

!!! Nouveauté 4.3.0 : Gestion des paramètres affichage, domaine et ressource par défaut, thème et langue

Permet d'autoriser ou non à l'utilisateur de modifier certains éléments dans son compte.

Les éléments paramétrables sont :
* Utilisateurs autorisés à modifier leur nom et prénom
* Utilisateurs autorisés à modifier leur adresse email
* Utilisateurs autorisés à modifier leur mot de passe
* Utilisateurs autorisés à modifier leur affichage
* Utilisateurs autorisés à modifier leur domaine et ressource par défaut
* Utilisateurs autorisés à modifier leur thème
* Utilisateurs autorisés à modifier leur langue

**L'adresse mail est obligatoire dans le compte utilisateur :** Dans ce cas l'utilisateur est obliger de laisser une adresse mail dans son compte.

### Quotas

**Nombre max. de réservations par utilisateur** _(-1 si pas de restriction)_ . Cette restriction s'applique à toutes les ressources confondues. En revanche, si l'utilisateur est gestionnaire de la ressource concernée, la restriction ne s'applique pas. Vous avez également la possibilité de fixer, ressource par ressource, un nombre maximal de réservations par utilisateur. C'est la restriction la plus élevée qui sera prise en compte.