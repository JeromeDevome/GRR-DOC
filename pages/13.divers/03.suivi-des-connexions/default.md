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

Concernant le journal des connexions :
- Les dates apparaissant en rouge marquent les utilisateurs déconnectés automatiquement après un trop long délai d'inactivité.
- Les lignes apparaissant en vert marquent les utilisateurs actuellement connectés (cela peut correspondre à une connexion actuellement close mais pour laquelle l'utilisateur ne s'est pas déconnecté correctement).
- Les lignes en noir signalent une session close normalement.
Remarque : il est possible à tout moment de  désactiver les connexions _(Configuration générale => Sécurité / Connexions => Activation/désactivation des connexions)_. En désactivant les connexions, vous rendez impossible la connexion au site pour les utilisateurs, hormis les administrateurs. De plus, les utilisateurs actuellement connectés sont automatiquement déconnectés. Néanmoins, si la connexion n'est pas obligatoire pour l'accès au site en visualisation, cet accès reste possible. 


Vous pouvez à tout moment vider le journal de connexion via _Divers => Nettoyage BDD_