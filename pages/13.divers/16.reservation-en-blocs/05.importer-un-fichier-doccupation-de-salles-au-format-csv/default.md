---
title: 'Importer un fichier d''occupation de salles au format CSV'
---

Télécharger un fichier CSV au format suivant:
> date du jour; heure de début; heure de fin; ressource; description; type

! Attention si vous avez des ressources ayant le même nom dans différents domaines. Il sera préférable de les renommer avant.

Si le fichier comporte des caractères accentués, il convient que le fichier CSV soit encodé en UTF-8 sans BOM.

Le temps d'importation est en général limité par le serveur à quelques minutes par fichier. Pour éviter des erreurs de type "timeout" qui conduiraient à une importation incomplète, scindez votre fichier en fichiers plus petits que vous importerez successivement.