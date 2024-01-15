---
title: Apparence
---

### Choix des paramètres d'affichage par défaut

Le choix des paramètres d'affichage par défaut s'applique au nouveaux utilisateurs. Si l'utilisateur est créé avant ou si il change les paramètres dans son comptes, s'est ces derniers qui seront pris en compte.

**Type d'affichage des listes des domaines et des ressources :** Type d'affichage des domaines et ressources dans le menu de gauche ou du haut _(selon configuration)_ . Choix possible boutons, arborescence ou liste. Certains sont à privilégier selon le nombre de domaines et ressources.

**Domaine par défaut & Ressource(s) affichée(s) :** Vous pouvez définir un domaine par domaine, attention que les utilisateurs ont bien accès à celui-ci.

**Choix du style/thème :** Un choix entre différente couleurs. Le choix personnalisé via l'admin est à configurer _(Administration => Divers => Gestion des couleurs)_.

**Choix de la langue par défaut :** Choix entre les différentes langues de GRR.

!!! **Nouveauté GRR 4 :** Les paramètres ci dessus peuvent être synchroniser pour les appliquer aux utilisateurs déjà créé.

### Affichage du menu

Affichage du menu mini calendrier et des ressources. Choix entre gauche et haut ou de ne pas l'afficher _(déconseillé si vous avez plusieurs ressources)_.

### Affichage des informations sur les réservations dans les vues journées, semaine et mois

!!! **Nouveauté GRR 4.3.0 :** L'affichage peut-être définit par statut de l'utilisateur.


|                       | Non connecté | Visiteur | Usager | Gestionnaire de ressource | Administrateur |
|:--------------------|
|Bénéficiaire| Ne pas afficher / Afficher /Info-Bulle</option>| | | | |
|Horaires|<select class="form-control" name="display_horaires_nc">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_horaires_vi">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_horaires_us">| | | | | | | | | | | |<!--<option value="0" >Ne pas afficher</option>-->| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_horaires_gr">| | | | | | | | | | | |<!--<option value="0" >Ne pas afficher</option>-->| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_horaires_ad">| | | | | | | | | | | |<!--<option value="0" >Ne pas afficher</option>-->| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|
|Brève description|<select class="form-control" name="display_short_description_nc">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_short_description_vi">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_short_description_us">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_short_description_gr">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_short_description_ad">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|
|Description complète|<select class="form-control" name="display_full_description_nc">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_full_description_vi">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_full_description_us">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_full_description_gr">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_full_description_ad">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|
|Type|<select class="form-control" name="display_type_nc">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_type_vi">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_type_us">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_type_gr">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|<select class="form-control" name="display_type_ad">| | | | | | | | | | | |<option value="0">Ne pas afficher</option>| | | | | | | | | | | |<option value="1">Afficher</option>| | | | | | | | | | | |<option value="2">Info-Bulle</option>| | | | | | | | | | |</select>|



### Affichage des liens email dans les fiches détaillées de réservation


### Affichage des informations des réservations sous forme de page ou de popup


### Remplissage de la rubrique "brève description" dans le formulaire réservation


### Remplissage de la rubrique "description complète" dans le formulaire réservation



### Ouverture des pages au format imprimable


### Affichage plannings divers


### Paramétrage de l'outil "Recherche & Stats"


### Formulaire de réservation
