---
title: 'Propriétaires et bénéficiaires'
---

Pour chaque réservation effectuée, **GRR** distingue le propriétaire de la réservation (celui qui a effectué la réservation) et le bénéficiaire de la réservation (celui au nom duquel la réservation a été effectuée).

La plupart du temps (fonctionnement par défaut), le propriétaire et le bénéficiaire sont une même personne.

Mais il est possible d'autoriser, ressource par ressource, des utilisateurs à réserver (ils sont alors propriétaires de la réservation) au nom d'autres utilisateurs (qui deviennent alors bénéficiaires de la réservation).

#### Délégation

L'administrateur général a toujours cette possibilité, mais il peut déléguer ce droit :
* uniquement aux administrateurs restreints du domaine,
* ou bien aux gestionnaires de la ressource (et aux administrateurs restreints du domaine),
* ou encore à tous les utilisateurs de la ressource.

Par défaut, seul l'administrateur général dispose de ce droit.

#### Bénéficiaires : des utilisateurs de GRR ou bien des personnes extérieures

Les bénéficiaires sont en général des utilisateurs enregistrés dans GRR. Mais il est également possible de réserver au nom de personnes extérieures. Dans ce cas, le créateur de la réservation dispose de deux champs supplémentaires dans l'interface de réservation :
* un champ obligatoire pour préciser les nom et prénom du bénéficiaire,
* un champ facultatif pour préciser l'adresse email du bénéficiare.

**Remarques :**
* Dans le cas où une réservation est effectuée au nom d'une personne extérieure, celle-ci ne dispose pas de la possibilité de modifier la réservation.
* Les personnes extérieures sont des personnes ne disposant pas de compte dans GRR. Par conséquent, un utilisateur qui s'authentifie par LDAP ou SSO n'est pas une personne extérieure. Mais, si un utilisateur "LDAP" ou "SSO" ne s'est jamais connecté à GRR, il n'a pas encore de compte dans GRR et par conséquent, il n'apparaît pas dans la liste déroulante des personnes au nom desquelles on peut effectuer une réservation.

#### Règles de fonctionnement

* Le propriétaire d'une réservation, même s'il n'en est pas bénéficiaire, a le droit de la modifier ou de la supprimer.
* De même le bénéficiaire d'une réservation, même s'il n'en est pas le propriétaire, a le droit de la modifier ou de la supprimer.
* Lorsque qu'un utilisateur effectue une réservation au nom d'un autre utilisateur ou bien modifie ou supprime une réservation existante faite au nom d'un autre utilisateur, un mail de notification est automatiquement envoyé au bénéficiaire de la réservation (à condition que l'envoi de mails automatiques soit activé et que le champ email du bénéficiaire soit correctement renseigné).
