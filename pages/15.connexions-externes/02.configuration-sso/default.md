---
title: 'Configuration SSO'
---

Depuis la version 1.7, GRR est prévu pour fonctionner dans un environnement CAS SSO.

### a) Paramétrage

* **Serveur CAS:** Vous devez saisir l'adresse de votre serveur SSO (IP ou sous forme nom.du.serveur.fr)
* **Port:** Port du CAS SSO (souvent 8443)
* **Racine:** Racine peut-être vide ou du type chaine (souvent CAS)

Si le serveur hébergeant GRR est derrière un proxy, il peut être nécessaire de renseigner les valeurs suivantes : 
* **Adresse IP du serveur proxy**
* **Port**
* **Environnement SSO**

**Environnement SSO:** Votre type de SSO, ce champ est obligatoire et selon votre choix, différents paramétrages vous seront proposés.


Pour rendre actif votre configuration veuillez sélectionner le **statut par défaut des utilisateurs importés** (Visiteur ou Usager).


