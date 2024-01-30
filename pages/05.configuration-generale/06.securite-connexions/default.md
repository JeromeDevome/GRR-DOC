---
title: 'Sécurité / Connexions'
---

### Sauvegarde de la base GRR

!! MyGRR Cloud : Les serveurs sont sauvegardés automatiquement tout les jours

!!!! N'hésitez pas à faire des sauvegardes régulières, surtout avant de faire des mises à jours ou des modifications de configuration majeures.

Création d'un fichier de sauvegarde complet de la base SQL. Permettant le cas nécessaire la restauration de la base de GRR. 

**Remarque :** Le contenus de certaines tables non essentiel ne sont pas sauvegardés pour éviter d'alourdir le fichier (Table logs de connexion, d'envois de mail...)

! Vérifier que votre fichier de sauvegarde soit complet !

**Conseil :** Sauvegarder votre serveur complet et à intervalle régulier.


### Restauration de la base GRR

En cas de perte de donnée ou de problème sur la base GRR, cette fonction vous permet de la retrouver dans l'état antérieur lors d'une sauvegarde.


### Exécution automatique de la sauvegarde

!! MyGRR Cloud : Les serveurs sont sauvegardés automatiquement tout les jours

Une sauvegarde automatique peut être déclenchée par l'exécution du script « admin_save_mysql.php », par exemple en programmant son exécution à l'aide d'une tâche « cron ».
Pour activer cette fonctionnalité, vous devez définir ci-dessous un mot de passe.
Par exemple, si le mot de passe est jamesbond007, l'URL du type : http://mon-site.fr/grr/admin_save_mysql.php?mdp=jamesbond007 déclenchera la sauvegarde.
Il est fortement conseillé de choisir un mot de passe complexe avec lettres, chiffres et caractères spéciaux !


### Activation/désactivation des connexions

En désactivant les connexions, vous rendez impossible la connexion au site pour les utilisateurs, hormis les administrateurs. De plus, les utilisateurs actuellement connectés sont automatiquement déconnectés. Néanmoins, si la connexion n'est pas obligatoire pour l'accès au site en visualisation, cet accès reste possible.


### Divers

**Rediriger les utilisateurs en https :** Permet de rediriger le lien http vers https. Il est préférable de le faire dans la configuration d'apache.
**Activer les logs sur les mails :** Dans le où cela est activer vous pourrez voir l'ensemble des mails envoyé par GRR dans "Suivi des mails"

### Restriction des connexions via l'iP

Limite la connexion des utilisateurs via une iP _(hors administrateurs)_. Si GRR est hébergé sur un serveur externe à vos locaux, veuillez mettre une iP publique sinon les iP interne. Séparez les différentes iP par des points virgules.

### Horaire de connexion

Vous pouvez restreindre la connexion à GRR entre certains horaires. Laissez vide pour ne pas restreindre la connexion à des horaires ou saisissez la plage horaire autorisé (Format HH:MM). Les administrateurs ne sont pas impactés par cette restriction. La connexion sera impossible aux utilisateurs en dehors de cette période.

### Durée d'une session

Cette durée indique le temps maximum d'inactivité au bout duquel un utilisateur est automatiquement déconnecté _(60 minutes par défaut)_.

### Mot de passe

**Longueur minimale du mot de passe :** Par défaut 8 caractère minimum.

### Url de Déconnexion

Lorsqu'un utilisateur se déconnecte, après fermeture de la session, le navigateur est redirigé vers la page dont l'URL est spécifiée.
Si le champ est vide, selon le paramétrage de l'accès à GRR, l'utilisateur est dirigé soit vers la page d'accueil soit vers la page de déconnexion.
