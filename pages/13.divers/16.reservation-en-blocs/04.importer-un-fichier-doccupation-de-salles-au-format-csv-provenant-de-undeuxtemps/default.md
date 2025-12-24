---
title: 'Importer un fichier d''occupation de salles au format CSV provenant de UnDeuxTemps'
---

Cette procédure vous permet d'importer les données d'un emploi du temps réalisé avec le logiciel UnDeuxTemps.

Pour cela, commencer par faire l'extraction depuis UnDeuxTemps :

Lancer UnDeuxTemps, module "emploi du temps des salles" et demander une recherche.

Ne rentrer aucun critère dans la recherche si bien qu'UDT recherche tout; cliquer alors sur le bouton "Excel" et UDT exporte tout le fichier d'occupation hebdomadaire des salles au format CSV.

Supprimer la première ligne (les en-têtes de colonnes) par exemple avec Notepad++ et enregistrer en CSV.

Dans GRR  télécharger le fichier CSV qui doit être du format suivant:

> jour de la semaine; heure au format: 12h00 (pour un créneau d'une heure) ou 12h00-13h30 (pour un créneau différent); classe ou division; discipline; enseignant; salle; groupe; regroupement; effectif; mode; fréquence; aire

(ces 6 derniers champs ne sont pas exploités pour le moment mais doivent figurer: c'est le format d'exportation UnDeuxTemps) Le temps d'importation est en général limité par le serveur à quelques minutes par fichier. Pour éviter des erreurs de type "timeout" qui conduirait à une importation incomplète, scindez votre fichier en fichiers plus petits (par exemple suivant les jours de la semaine) que vous importerez successivement.

! Remarque : lors d'une réimportation, les créneaux inchangés sont maintenus, les créneaux modifiés sont écrasés, les créneaux libérés ne le sont pas. 