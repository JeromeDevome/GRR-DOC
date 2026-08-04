---
title: 'Configuration LDAP'
---

!!! MyGRR Cloud : Pour la sécurité de votre réseau, la connexion LDAP n'est pas disponible.


Depuis la version GRR 1.7, il est possible de se connecter à GRR en s'authentifiant auprès d'un annuaire LDAP. LDAP (Lightweight Directory Access Protocol) est un protocole permettant d’interroger un annuaire contenant des informations d’utilisateurs (nom, login, email, ...).

Dans le panneau d'administration de GRR, une page « Configuration LDAP » permet d'activer et de configurer l'authentification LDAP. A l'ouverture de cette page, GRR détecte si PHP a été compilé avec le support LDAP. Dans le cas contraire, un message en avertit l'administrateur qui ne peut aller plus loin dans le paramétrage LDAP.

L'activation LDAP consiste à choisir le statut par défaut des utilisateurs venant de l'annuaire (« usager » ou « visiteur »).

Une fois LDAP activé, il faut configurer le fichier « config_ldap.inc.php », ce qui est relativement simple en utilisant la procédure automatique accessible à partir de cette page (attention à donner les droits d'écriture sur le fichier « config_ldap.inc.php »).
