---
audience: end-user
title: Nouveautés de Campaign Web v8
description: Découvrez les nouvelles fonctionnalités de Campaign Web v8.
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha"
source-git-commit: 0a4d4295f8c460298dcc61fcfc78e8cb09fe963e
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 93%

---


# Nouveautés {#new}

## Version Alpha 2.0{#alpha-release}

Actuellement, cette nouvelle interface web de Campaign n’est disponible que pour les **utilisateurs et utilisatrices Alpha**, et dispose des fonctionnalités suivantes :

**Une expérience moderne, intuitive et unifiée**

La nouvelle IU web de Campaign offre une nouvelle expérience client, alignée sur toutes les solutions et applications Adobe Experience Cloud. Elle offre :

* L’accès à la nouvelle interface et aux autres solutions Adobe dans une session utilisateur unique et partagée
* Une nouvelle expérience de navigation, avec tous les menus et dossiers disponibles dans le rail de gauche
* Des sélecteurs de solution et d’organisation à partir de la barre supérieure
* Une intégration de Shell unifié, avec un accès direct à la communauté, au centre d’aide et au support

**De nouvelles fonctionnalités puissantes et des processus transparents**

* Une interface de zone de travail de workflow repensée pour concevoir et gérer vos processus
* Un contenu dynamique pour diffuser des expériences hautement ciblées et personnalisées à votre audience
* Une intégration native aux audiences Adobe Experience Platform
* Une gestion des modèles pour les workflows, les diffusions, les campagnes et le contenu

Apprenez-en davantage sur la nouvelle IU sur [cette page](../get-started/user-interface.md).

**Créer, lancer et mesurer votre campagne**

Utilisez la nouvelle IU web de Campaign pour :

* Concevoir un contenu d’e-mail personnalisé avec le concepteur d’e-mail - [En savoir plus](../content/edit-content.md)
* Envoyer des campagnes cross-canal, y compris des SMS et des notifications push
* Définir des audiences cibles avec le créateur de règles - [En savoir plus](../audience/about-audiences.md)
* Prévisualiser, tester et envoyer vos e-mails - [En savoir plus](../monitor/prepare-send.md)
* Surveiller l’envoi et la mesure des résultats à l’aide de rapports intégrés - [En savoir plus](../reporting/delivery-reports.md)


## Migrer vers l’UI de Campaign Web

En tant qu’utilisateur ou utilisatrice de Campaign, vous pouvez toujours accéder à la console cliente pour créer et gérer des ressources et des composants de Campaign. Les données et les paramètres sont synchronisés d’un environnement à un autre. En savoir plus dans [cette section](../get-started/get-started.md#about-campaign-client-consoleac-client).

De plus, l’ensemble de vos données et paramètres déjà disponibles dans la console cliente sont visibles dans l’UI de Campaign Web, à partir du volet de navigation de gauche de l’explorateur. En savoir plus sur la vue Explorateur dans [cette section](../get-started/user-interface.md#explorer-user-interface-explorer).


## Mises à jour de la terminologie {#terminology-updates}

En tant qu’utilisateur ou utilisatrice de Campaign, notez que certains concepts ont été renommés pour s’aligner sur les dernières normes terminologiques. Ces modifications concernent uniquement l’UI de Campaign Web et ne sont pas répercutées dans la console cliente. Elles sont résumées ci-dessous.

* Les BAT sont maintenant des **e-mails de test** : pour envoyer un BAT, utilisez le bouton **Tester** dans l’IU de diffusion par e-mail. La cible des BAT est désormais appelée **Profils de test**. [En savoir plus](../preview-test/test-deliveries.md).
* Les adresses de contrôle sont désormais utilisées comme **Profils de test**: envoyer l&#39;email de test aux adresses de contrôle, qui sont des destinataires supplémentaires dans la base de données ; [En savoir plus](../preview-test/test-deliveries.md).
* L’analyse de la diffusion s’appelle désormais **préparation de la diffusion**. Lorsque vous devez lancer l’analyse, cliquez sur le bouton **Préparer**.. [En savoir plus](../monitor/prepare-send.md).
* L’aperçu de l’e-mail est désormais disponible via le bouton **Simuler le contenu.** [En savoir plus](../preview-test/preview-test.md)
* Les listes s’appellent désormais **Audiences**. [En savoir plus](../audience/about-audiences.md).

## Limites{#limitations-alpha}

Les restrictions ci-dessous s’appliquent à cette version Alpha :

* Les seuls objets modifiables sont les diffusions, les campagnes, les workflows, les audiences et les modèles. Les autres sont en lecture seule. Utilisez des filtres pour tous les parcourir.
* Les audiences ne peuvent pas être enregistrées pour une utilisation ultérieure.
* L’interface utilisateur d’administration n’est pas disponible.
* Les mesures de rapports (telles que les ouvertures et les données de suivi) sont mises à jour toutes les heures.
* Les KPI du tableau de bord de la diffusion sont mis à jour toutes les 5 minutes. - mais la préparation de la diffusion est en temps réel.
* Les notifications d’Adobe Experience Cloud et l’aide unifiée disponibles dans la barre supérieure ne sont pas encore intégrées.

