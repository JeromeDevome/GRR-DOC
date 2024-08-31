---
title: 'Suivi des connexions'
---

Vous pouvez voir les utilisateurs actuellement connecté, si besoin vous pouvez les déconnecter à partir d'ici (par exemple dans le cadre d'une maintenance).

Vous pouvez aussi voir le journal de toute les connexions _(exportable sous différents formats)_ Par défaut GRR conserve 365 jours de logs des connexions pour être conforme avec la RGPD. Cette valeur peut être modifié via le fichier _"configperso.inc.php"_ .

Les logs de connexions contiennent :
* Nom de l'utilisateur
* Date de début de la session
* Fin de la session (Maximum)
* Adresse IP
* Navigateur web utilisé
* URL de provenance

Vous pouvez à tout moment vider le journal de connexion via _Divers => Nettoyage BDD_