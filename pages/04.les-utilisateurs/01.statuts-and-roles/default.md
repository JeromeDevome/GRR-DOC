---
title: 'Statuts & Rôles'
login:
    visibility_requires_access: false
---

Chaque utilisateur possède un statut ( visiteur, usager, gestionnaire d'utilisateur ou Administrateur). En plus de son statut l'utilisateur peut avoir des privilèges supplémentaire (Gestionnaire de ressource, administrateur de domaine...) .

### a) Les administrateurs

L'administrateur a accès à l’ensemble des fonctionnalités de l’application : il gère les ressources, la base de données et les autres utilisateurs. Il peut tout voir, réserver et modifier ou effacer toutes les réservations. Il a accès à l'ensemble des paramètres de configuration de GRR.

### b) Les administrateurs restreints de sites (versions 1.9.6+)

Lorsque la fonctionnalité "multi-sites" est activée, il est possible de définir des "sites", qui sont des unités qui regroupent des domaines. Il est alors possible de définir des administrateurs de sites.
En plus de ses droits normaux, l'administrateur d'un site a la possibilité de gérer entièrement un site : création, suppression, modification d'un domaine ou d'une ressource, ajout et suppression de gestionnaires des réservations, d'administrateur de domaines, gestion des mails automatiques.

c) Les administrateurs restreints de domaines

Un administrateur de domaines est à la base un « usager » (voir plus bas) à qui l'administrateur a donné des droits supplémentaires pour administrer tel ou tel domaine.

Concernant les domaines dont ils ont la charge, les administrateurs restreints peuvent, pour le(s) domaine(s) qu'ils administrent :

    créer, modifier ou supprimer des ressources,
    dans le cas d'un domaine à accès restreint, ajouter ou supprimer des utilisateurs autorisés à avoir accès au domaine,
    gérer la liste des utilisateurs à avertir automatiquement par mail lors des réservations d'une ressources donnée,
    gérer la liste des gestionnaires pour chaque ressource du domaine (voir plus bas),
    activer ou désactiver un ou plusieurs types de réservation pour le domaine.

### d) Les gestionnaires

Un gestionnaire est à la base un « usager » (voir plus bas) à qui l'administrateur a donné des droits supplémentaires pour gérer telle ou telle ressource.

Concernant les ressources dont ils ont la charge, les gestionnaires peuvent :

    supprimer ou modifier n'importe quelle réservation,
    être prévenus par mail de la réservation d'une ressource ou de la modification/suppression de la réservation (voir rubrique plus bas),
    signaler qu'une réservation est en cours d'utilisation (sur les plannings, un symbole spécifique apparaît alors dans la case de la réservation),
    rendre temporairement indisponible à la réservation une ressource (pour maintenance par exemple).

### e) Les usagers

Un usager :

* peut voir les réservations dans les domaines publics, réserver et modifier ou effacer ses propres réservations,
* peut être prévenu par mail de la réservation d'une ressource ou de la modification/suppression de la réservation (voir rubrique plus bas),
* a accès à la consultation de la disponibilité ou indisponibilité des ressources des domaines publics,
* a accès au détail des réservations,
* a accès à l'outil "Recherche - Rapports - Statistiques" (selon le paramétrage dans la configuration générale) ,
* a accès à la gestion de son compte pour modifier ses paramètres personnels (mot de passe, email, affichage par défaut, ...)

Pour les domaines à accès restreint, seuls les usagers spécifiés par l'administrateur y ont accès. Les usagers autorisés y ont alors les mêmes possibilités que dans les domaines publics.
Par défaut, un usager (ni même un gestionnaire ou un administrateur restreint de domaines) ne peut effectuer une réservation dans le passé, ni modifier ou supprimer une réservation passée. Seul l'administrateur a cette possibilité. Il est néanmoins possible de permettre, pour une ressource donnée, la réservation dans le passé ainsi que les modifications/suppressions de réservations passées.

### f) Les usagers "gestionnaires d'utilisateurs"

Le gestionnaire d'utilisateurs, en plus des possibilités d'un usager normal peut :

* ajouter des utilisateurs ayant pour statut "usager" ou "visiteur",
* modifier un utilisateur ayant pour statut "usager" ou "visiteur", (nom, prénom, mot de passe, email, statut, etat),
* supprimer un utilisateur ayant pour statut "usager" ou "visiteur",
* importer dans GRR un fichier d'utilisateurs (format CSV)

### g) Les visiteurs

Un « visiteur » peut voir les réservations dans les domaines publics (et dans les domaines à accès restreints selon la configuration) ainsi que le détail des réservations mais ne peut ni réserver, ni effacer, ni modifier une réservation. Le visiteur n'a pas accès à son compte et ne peut donc pas modifier son mot de passe. Selon le paramétrage dans la configuration générale, le visiteur a ou non accès à l'outil "Recherche - Rapports - Statistiques". 