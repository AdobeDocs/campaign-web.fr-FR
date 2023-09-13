---
audience: end-user
title: Nouveautés de Campaign Web v8
description: Découvrez les nouvelles fonctionnalités de Campaign Web v8.
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Beta"
source-git-commit: 2e1f7f2a0f3e7116c57c56d9abb6866113402401
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 54%

---


# Nouveautés {#new}


Nous sommes ravis de présenter la version BÊTA de l’interface utilisateur web d’Adobe Campaign. Notre dernière version est riche en fonctionnalités intuitives conçues pour simplifier la création de campagnes cross-canal personnalisées, générer des résultats exceptionnels et vous donner un avantage concurrentiel sur tous les canaux.

## Version bêta{#beta-release}

Cette nouvelle interface web de Campaign n’est actuellement disponible que pour **Professionnels bêta** avec les fonctionnalités suivantes :

**Une expérience moderne, intuitive et unifiée**

La nouvelle UI web de Campaign offre une nouvelle expérience client, alignée sur toutes les solutions et applications Adobe Experience Cloud. Elle offre :

* L’accès à la nouvelle interface et aux autres solutions Adobe dans une session utilisateur unique et partagée
* Une nouvelle expérience de navigation, avec tous les menus et dossiers disponibles dans le rail de gauche
* Des sélecteurs de solution et d’organisation à partir de la barre supérieure
* Une intégration d’Unified Shell, avec un accès direct à la communauté, au centre d’aide et au support

**De nouvelles fonctionnalités puissantes et des processus efficaces**

* Une interface de zone de travail de workflow repensée pour concevoir et gérer vos processus
* Du contenu dynamique pour diffuser des expériences hautement ciblées et personnalisées à votre audience
* Une intégration native des audiences Adobe Experience Platform
* Une gestion des modèles pour les workflows, les diffusions, les campagnes et le contenu

Apprenez-en davantage sur la nouvelle UI sur [cette page](../get-started/user-interface.md).

**Créer, lancer et mesurer votre campagne**

Utilisez la nouvelle UI web de Campaign pour :

* Créer un contenu d’e-mail personnalisé avec le concepteur d’e-mail - [En savoir plus](../content/edit-content.md)
* Envoyer des campagnes cross-canal, y compris des SMS et des notifications push
* Définir des audiences cibles avec le créateur de règles - [En savoir plus](../audience/about-audiences.md)
* Prévisualiser, tester et envoyer vos e-mails - [En savoir plus](../monitor/prepare-send.md)
* Surveiller l’envoi et la mesure des résultats à l’aide de rapports intégrés - [En savoir plus](../reporting/delivery-reports.md)


## Dernières mises à jour

**Résumé bêta**

* Activation de la composition de données (fédérée) pour les audiences et la personnalisation
* Utiliser la technologie AI pour améliorer la génération de contenu d&#39;email
* Synchronisation transparente des ressources et des modèles de HTML complet
* Organisez et gérez efficacement vos dossiers et ressources
* Accédez à d’autres activités telles que la modification de la dimension, la déduplication et les diffusions récurrentes afin d’améliorer les workflows des opérations.

**Nouvelles fonctionnalités clés**

* Autres activités de workflow de campagne

  Surchargez vos campagnes marketing avec notre ensemble étendu d’activités de workflow. Déverrouillez de nouvelles possibilités d’automatisation et d’optimisation, ce qui vous permet de créer des parcours client plus dynamiques et personnalisés.

  De la segmentation avancée aux déclencheurs conditionnels, nos activités de workflow supplémentaires vous permettent de diffuser des messages ciblés et d’optimiser les performances de vos campagnes.

* IA dédiée aux e-mails

  Dites adieu à la création manuelle de contenu et bonjour à des campagnes efficaces et pilotées par les données avec la puissance de Gen AI.  Notre technologie Gen AI utilise des algorithmes avancés pour générer du contenu hautement attrayant et personnalisé. Augmentez les taux d’ouverture, les taux de clics publicitaires et les conversions grâce à la génération de contenu intelligent de Gen AI.

  Gardez l’avance sur le jeu et augmentez votre jeu de marketing email avec Gen AI sur le contenu des emails.


* Gestion des filtres prédéfinis

  Présentation de la gestion des filtres prédéfinis. L’interface utilisateur web de Campaign vous offre désormais une interface conviviale pour gérer et personnaliser facilement des filtres prédéfinis en fonction de vos besoins spécifiques. Créez une fois et enregistrez pour une utilisation ultérieure. [En savoir plus](predefined-filters.md)


* Public cible

  Construire une cible de diffusion n&#39;a jamais été aussi facile ! Avec notre dernier créateur de règles, vous pouvez désormais définir des critères de filtrage pour les destinataires ou toute autre dimension de ciblage de la base de données. En outre, vous pouvez tirer parti de votre audience AEP (Adobe Experience Platform) pour affiner davantage votre audience cible et optimiser l’impact de votre campagne.

* Offres avec SMS

  La nouvelle interface utilisateur web vous permet désormais d’intégrer des offres avec des SMS en plus des emails. Atteignez votre audience sur leurs appareils mobiles, en proposant des promotions et des notifications opportunes.

  Optimisez vos efforts marketing en exploitant la puissance des offres intégrées par SMS sur notre plateforme web avancée.

<!--
* Adobe Experience Manager (AEM) Integration
    
    With our AEM integration extended to web UI, you can easily manage assets and synchronize full HTML templates, empowering you to create captivating digital experiences without any hassle. 
    
    Elevate and streamline your content management capabilities on the web UI with this integration to boost productivity.
-->


## Migrer vers l’UI de Campaign Web

En tant qu’utilisateur ou utilisatrice de Campaign, vous pouvez toujours accéder à la console cliente pour créer et gérer des ressources et des composants de Campaign. Les données et les paramètres sont synchronisés d’un environnement à un autre. En savoir plus dans [cette section](../get-started/get-started.md#about-campaign-client-consoleac-client).

De plus, l’ensemble de vos données et paramètres déjà disponibles dans la console cliente sont visibles dans l’UI de Campaign Web, à partir du volet de navigation de gauche de l’explorateur. En savoir plus sur la vue Explorateur dans [cette section](../get-started/user-interface.md#explorer-user-interface-explorer).

Avec la version bêta de Campaign Web, l’interface utilisateur reflète les autorisations de l’utilisateur. En savoir plus sur les autorisations dans [cette page](../get-started/permissions.md)

## Mises à jour de la terminologie {#terminology-updates}

Comme vous utilisez déjà Campaign, vous remarquerez que certains concepts ont été renommés pour s’aligner sur les dernières normes terminologiques. Ces modifications concernent uniquement l’UI de Campaign Web et ne sont pas répercutées dans la console cliente. Elles sont résumées ci-dessous.

* Les BAT sont maintenant des **e-mails de test** : pour envoyer un BAT, utilisez le bouton **Tester** dans l’UI de diffusion par e-mail. La cible des BAT s’appelle désormais **Profils de test**. [En savoir plus](../preview-test/test-deliveries.md).
* Les adresses de contrôle sont désormais utilisées comme **Profils de test** : envoyez l’e-mail de test aux adresses de contrôle, qui sont des destinataires supplémentaires dans la base de données. [En savoir plus](../preview-test/test-deliveries.md).
* L’analyse de la diffusion s’appelle désormais **préparation de la diffusion**. Lorsque vous devez lancer l’analyse, cliquez sur le bouton **Préparer**. [En savoir plus](../monitor/prepare-send.md).
* L’aperçu de l’e-mail est désormais disponible via le bouton **Simuler le contenu.** [En savoir plus](../preview-test/preview-test.md).
* Les listes s’appellent désormais **Audiences**. [En savoir plus](../audience/about-audiences.md).

## Limites{#limitations-alpha}

Les restrictions ci-dessous s’appliquent à cette version Alpha :

* Les objets modifiables sont les suivants : diffusions, campagnes, workflows, audiences, services d’abonnement, filtres prédéfinis et modèles. Les autres sont en lecture seule. Utilisez des filtres pour tous les parcourir.
* Les audiences ne peuvent pas être enregistrées pour une utilisation ultérieure.
* L’interface utilisateur d’administration n’est pas disponible.
* Les mesures de rapports (telles que les ouvertures et les données de suivi) sont mises à jour toutes les heures.
* Les KPI du tableau de bord de la diffusion sont mis à jour toutes les 5 minutes, mais la préparation de la diffusion est en temps réel.
* Les notifications d’Adobe Experience Cloud et l’aide unifiée disponibles dans la barre supérieure ne sont pas encore intégrées.

