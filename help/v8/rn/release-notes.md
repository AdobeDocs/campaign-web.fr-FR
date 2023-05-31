---
audience: end-user
title: Notes de mise à jour de Campaign Web v8
description: Notes de mise à jour de Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: 0703b872bb8f452773e76f2524d47bf774c687e0
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 81%

---


# Notes de mise à jour {#release-notes}

Cette page répertorie toutes les dernières fonctionnalités et améliorations de Campaign Web v8.

## Version Alpha{#alpha-release}

Actuellement, cette nouvelle interface web de Campaign n’est disponible que pour les **utilisateurs et utilisatrices Alpha**, et dispose des fonctionnalités suivantes :

**Une expérience moderne, intuitive et unifiée**

La nouvelle IU web de Campaign offre une nouvelle expérience client, alignée sur toutes les solutions et applications Adobe Experience Cloud. Elle offre :

* Accès à la nouvelle interface et à vos autres solutions d’Adobe avec une session utilisateur unique et partagée
* Une nouvelle expérience de navigation, avec tous les menus et dossiers disponibles dans le rail de gauche
* Des sélecteurs de solution et d’organisation à partir de la barre supérieure
* Une intégration de Shell unifié, avec un accès direct à la communauté, au centre d’aide et au support

**Nouvelles fonctionnalités puissantes et processus transparents**

* Interface de canevas de workflow repensée pour concevoir et gérer vos processus
* Contenu dynamique pour offrir des expériences hautement ciblées et personnalisées à votre audience
* Intégration native aux audiences Adobe Experience Platform
* Gestion des modèles pour les workflows, les diffusions, les campagnes et le contenu

Apprenez-en davantage sur la nouvelle IU sur [cette page](../get-started/user-interface.md).

**Créer, lancer et mesurer votre campagne par**

Utilisez la nouvelle IU web de Campaign pour :

* Concevoir un contenu d’e-mail personnalisé avec le concepteur d’e-mail - [En savoir plus](../content/edit-content.md)
* Envoyez des campagnes cross-canal, y compris des SMS et des notifications push.
* Définir des audiences cibles avec le créateur de règles - [En savoir plus](../audience/about-audiences.md)
* Prévisualiser, tester et envoyer vos e-mails - [En savoir plus](../monitor/prepare-send.md)
* Surveiller l’envoi et la mesure des résultats à l’aide de rapports intégrés - [En savoir plus](../reporting/delivery-reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## Mises à jour de la terminologie{#terminology-updates}

En tant qu’utilisateur ou utilisatrice de Campaign, notez que certains concepts ont été renommés pour s’aligner sur les dernières normes terminologiques. Ces modifications s’appliquent uniquement à l’IU web de Campaign et ne sont pas répercutées dans la console cliente. Elles sont résumées ci-dessous.

* Les BAT sont maintenant des **e-mails de test** : pour envoyer un BAT, utilisez le bouton **Tester** dans l’IU de diffusion par e-mail. La cible de la cible des BAT s’appelle désormais **Profils de test**.
* Les adresses de contrôle sont désormais utilisées comme **Profils de test** : envoyez l’e-mail de test aux adresses de contrôle, qui sont des destinataires supplémentaires et fictifs dans la base de données.
* L’analyse de la diffusion s’appelle désormais **préparation de la diffusion**. Lorsque vous devez lancer l’analyse, cliquez sur le bouton **Préparer**.
* L’aperçu de l’e-mail est désormais disponible via le bouton **Simuler le contenu**.
* Les listes sont désormais des **audiences**.

## Limites{#limitations-alpha}

Les restrictions ci-dessous s’appliquent à cette version Alpha :

* Les seuls objets modifiables sont Diffusions, Campagnes, Workflows, Audiences et Modèles. Les autres sont en lecture seule. Utilisez des filtres pour tous les parcourir.
* L’interface utilisateur d’administration n’est pas disponible.
* Les mesures de rapports (telles que les ouvertures et les données de suivi) sont mises à jour toutes les heures.
* Les KPI du tableau de bord de la diffusion sont mis à jour toutes les 5 minutes. - mais la préparation de la diffusion est en temps réel.
* Les notifications d’Adobe Experience Cloud et l’aide unifiée disponibles dans la barre supérieure ne sont pas encore intégrées.

