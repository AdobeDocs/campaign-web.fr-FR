---
audience: end-user
title: Notes de mise à jour de Campaign Web v8
description: Notes de mise à jour de Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
source-git-commit: 54bcb9b0ba8704cde8beaf1b0400eaa01bba0b15
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 12%

---

# Notes de mise à jour {#release-notes}

![](../assets/do-not-localize/badge.png)

Cette page répertorie toutes les dernières fonctionnalités et améliorations de Campaign Web v8.

## Version Alpha{#alpha-release}

Cette nouvelle interface web de Campaign n’est actuellement disponible que pour **Utilisateurs Alpha** avec les fonctionnalités suivantes :

**Une expérience moderne, intuitive et unifiée.**

La nouvelle interface utilisateur web de Campaign offre une nouvelle expérience utilisateur, alignée sur toutes les solutions et applications Adobe Experience Cloud. Il offre :

* Accédez à la nouvelle interface et aux autres solutions Adobe avec une session utilisateur unique et partagée.
* Nouvelle expérience de navigation, avec tous les menus et dossiers disponibles dans le rail de gauche
* Sélecteur de solution et d’organisation à partir de la barre supérieure
* Intégration de Shell unifiée, avec un accès direct à la communauté, au centre d’aide et au support
<!--
No search and pulse notifications in Alpha
-->

En savoir plus sur la nouvelle interface utilisateur dans [cette page](../get-started/user-interface.md).

**Créer, lancer et mesurer votre campagne par e-mail**

Utilisez la nouvelle interface utilisateur web de Campaign pour :

* Concevoir un contenu d&#39;email personnalisé avec le Concepteur d&#39;email - [En savoir plus](../content/edit-content.md)
* Définition des audiences cibles avec le créateur de règles - [En savoir plus](../audience/about-audiences.md)
* Prévisualiser, tester et envoyer vos emails - [En savoir plus](../monitor/prepare-send.md)
* Surveillez les envois et mesurez les résultats à l’aide de rapports natifs - [En savoir plus](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->

>[!NOTE]
>
>Les campagnes cross-canal et les fonctionnalités de gestion des workflows seront disponibles avec la version bêta.

## Mises à jour de terminologie

En tant qu’utilisateur Campaign existant, notez que certains concepts ont été renommés pour s’aligner sur les dernières normes terminologiques. Ces modifications s’appliquent uniquement à l’interface utilisateur web de Campaign et ne sont pas répercutées dans la console cliente. Elles sont résumées ci-dessous.

* Les bons à tirer sont maintenant **Tester les emails**: pour envoyer un bon à tirer, utilisez la méthode **Test** dans l’interface utilisateur de diffusion par courrier électronique. La cible de la cible des BAT est désormais appelée **Profils de test**
* Les adresses de contrôle sont désormais utilisées comme **Profils de test**: envoyer l&#39;email de test aux adresses de contrôle, qui sont des destinataires supplémentaires et fictifs dans la base de données ;
* L’analyse des diffusions est désormais **préparation de la diffusion**. Lorsque vous devez lancer l’analyse, cliquez sur le bouton **Préparer** button
* L’ aperçu de l’email est maintenant disponible dans la **Simulation du contenu** button
* Les listes sont maintenant **Audiences**
