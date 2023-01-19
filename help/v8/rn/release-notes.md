---
audience: end-user
title: Notes de mise à jour de Campaign Web v8
description: Notes de mise à jour de Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
source-git-commit: 54bcb9b0ba8704cde8beaf1b0400eaa01bba0b15
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 100%

---

# Notes de mise à jour {#release-notes}

![](../assets/do-not-localize/badge.png)

Cette page répertorie toutes les dernières fonctionnalités et améliorations de Campaign Web v8.

## Version Alpha{#alpha-release}

Actuellement, cette nouvelle interface web de Campaign n’est disponible que pour les **utilisateurs et utilisatrices Alpha**, et dispose des fonctionnalités suivantes :

**Une expérience moderne, intuitive et unifiée**

La nouvelle IU web de Campaign offre une nouvelle expérience client, alignée sur toutes les solutions et applications Adobe Experience Cloud. Elle offre :

* L’accès à la nouvelle interface et aux autres solutions Adobe avec une session utilisateur unique et partagée
* Une nouvelle expérience de navigation, avec tous les menus et dossiers disponibles dans le rail de gauche
* Des sélecteurs de solution et d’organisation à partir de la barre supérieure
* Une intégration de Shell unifié, avec un accès direct à la communauté, au centre d’aide et au support
<!--
No search and pulse notifications in Alpha
-->

Apprenez-en davantage sur la nouvelle IU sur [cette page](../get-started/user-interface.md).

**Créer, lancer et mesurer votre campagne par e-mail**

Utilisez la nouvelle IU web de Campaign pour :

* Concevoir un contenu d’e-mail personnalisé avec le concepteur d’e-mail - [En savoir plus](../content/edit-content.md)
* Définir des audiences cibles avec le créateur de règles - [En savoir plus](../audience/about-audiences.md)
* Prévisualiser, tester et envoyer vos e-mails - [En savoir plus](../monitor/prepare-send.md)
* Surveiller l’envoi et la mesure des résultats à l’aide de rapports intégrés - [En savoir plus](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->

>[!NOTE]
>
>Les campagnes cross-canal et les fonctionnalités de gestion des workflows seront disponibles dans la version Bêta.

## Mises à jour de la terminologie

En tant qu’utilisateur ou utilisatrice Campaign existant(e), notez que certains concepts ont été renommés pour s’aligner sur les dernières normes terminologiques. Ces modifications s’appliquent uniquement à l’IU web de Campaign et ne sont pas répercutées dans la console cliente. Elles sont résumées ci-dessous.

* Les BAT sont maintenant des **e-mails de test** : pour envoyer un BAT, utilisez le bouton **Tester** dans l’IU de diffusion par e-mail. La cible de la cible des BAT s’appelle désormais **Profils de test**.
* Les adresses de contrôle sont désormais utilisées comme **Profils de test** : envoyez l’e-mail de test aux adresses de contrôle, qui sont des destinataires supplémentaires et fictifs dans la base de données.
* L’analyse de la diffusion s’appelle désormais **préparation de la diffusion**. Lorsque vous devez lancer l’analyse, cliquez sur le bouton **Préparer**.
* L’aperçu de l’e-mail est désormais disponible via le bouton **Simuler le contenu**.
* Les listes sont désormais des **audiences**.
