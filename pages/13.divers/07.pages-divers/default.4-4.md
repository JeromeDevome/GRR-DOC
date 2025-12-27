---
title: 'Pages divers'
---

!!! **Nouveauté GRR 4.4.0

**Pages divers** permet d'ajouter et de gérer des liens vers d'autres pages de GRR ou vers des sites externes.

### Emplacements disponibles
- **Menu haut droit**
- **Page de connexion**

### Tableau des liens

| Intitulé du champ | Statut | Lien | Un autre onglet | Ordre | Action |
|------------------|--------|------|----------------|-------|--------|
| Nom du lien      | Statut de l'utilisateur | URL de destination | Oui / Non | Position du lien | Modifier / Supprimer |

### Fonctionnement détaillé des champs

- **Intitulé du champ** :  
  Texte affiché pour le lien. Il doit être clair pour l'utilisateur afin qu'il comprenne la destination du lien.

- **Statut** :  
  Définit quels utilisateurs peuvent voir le lien.  
  Exemples :  
  - Administrateur → visible uniquement pour les admins  
  - Visiteur → visible pour tous les utilisateurs connectés  
  - Non connecté → visible pour les utilisateurs non connectés

Pour l'emplacement "**Page de connexion**" seul le statut "Non connecté" est disponible.

- **Lien** :  
  URL complète vers la page interne ou le site externe.  
  - Pour un lien interne : `app.php?p=XXXX`
  - Pour un site externe : `https://exemple.com`

- **Un autre onglet** :  
  Détermine si le lien s'ouvre dans un nouvel onglet du navigateur.  
  - Oui → le lien s'ouvre dans un nouvel onglet  
  - Non → le lien s'ouvre dans le même onglet

- **Ordre** :  
  Définit la position du lien dans la liste.  
  Les liens avec un ordre supérieur apparaissent avant ceux avec un ordre inférieur.
  
  


