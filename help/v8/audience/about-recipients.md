---
title: Commencer avec les profils
description: Découvrez comment surveiller et gérer les profils dans Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: 5a4bf85a1f70a0282405aededfb31038f9db17a8
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 100%

---

# Prise en main des profils {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profils"
>abstract="Un profil est un enregistrement ciblé pour recevoir les messages envoyés par Adobe Campaign. Depuis cette liste, vous pouvez visualiser les détails des profils, en fonction de vos autorisations. Utilisez les options de filtrage pour parcourir cette liste. Vous pouvez modifier et mettre à jour un petit ensemble d’attributs de vos profils."

## Qu’est-ce qu’un profil ? {#what}

Un **profil**, également appelé « personne destinataire » dans la console cliente, représente un enregistrement stocké dans la base de données de Campaign, qui sert de composant clé pour [créer des audiences](create-audience.md) pour les diffusions et [ajouter des données de personnalisation](../personalization/personalize.md) à votre contenu. Adobe Campaign vous permet de gérer facilement les profils, de la création d’entrées à l’accès à une vue complète de tous les attributs et abonnements aux services de vos profils, tout cela au moyen de l’interface utilisateur web de Campaign.

De plus, des **[!UICONTROL profils de test]**, désignés comme des « profils de contrôle » dans la console cliente, vous permettent de cibler des personnes destinataires supplémentaires qui ne correspondent pas aux critères de ciblage d’une diffusion donnée. Ces profils contiennent des coordonnées fictives ou des coordonnées contrôlées par l’expéditeur ou l’expéditrice. Les profils de test sont les profils destinataires des BAT : ils sont utilisés pour tester vos messages en envoyant des BAT. [Découvrir comment utiliser des profils test](test-profiles.md)

Les profils et les profils de test peuvent être utilisés pour tester vos diffusions avant qu’elles n’atteignent l’audience visée. Ce faisant, vous pouvez prévisualiser le contenu et la personnalisation du message, envoyer des BAT à des fins de test et de validation, évaluer le rendu des e-mails sur différents appareils et plateformes, et tester vos pages de destination. [Découvrir comment prévisualiser et tester des diffusions](../preview-test/preview-test.md)

➡️ [Découvrir cette fonctionnalité en vidéo](#video)

## Accéder à la liste des profils {#access}

Les profils sont accessibles et modifiables dans Adobe Campaign Web à partir de l’entrée **[!UICONTROL Gestion des clientes et clients]** > **Profils** dans le rail de navigation de gauche. Vous pouvez également y accéder dans la vue **[!UICONTROL Explorateur]**, dans le nœud **[!UICONTROL Profils et cibles]** > **[!UICONTROL Personnes destinataires]**. De là, vous pouvez parcourir, créer et gérer des dossiers ou des sous-dossiers, ainsi que vérifier les autorisations associées. [Découvrez comment créer des dossiers](../get-started/permissions.md#folders)

>[!NOTE]
>
>En fonction de vos autorisations, il se peut que vous n’ayez pas accès à la liste complète des profils stockés dans la base de données. [En savoir plus sur les autorisations](../get-started/permissions.md).

Vous pouvez filtrer la liste **[!UICONTROL Profils]** à l’aide du champ de recherche ou des filtres disponibles en cliquant sur le bouton **Afficher les filtres**. Vous pouvez limiter les résultats à un [dossier](../get-started/permissions.md#folders) spécifique à l’aide de la liste déroulante ou ajouter des règles à l’aide du [concepteur de requête](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable=&quot;yes&quot;}

Pour accéder aux détails d’un profil, cliquez sur son nom dans la liste. Une vue détaillée du profil s’ouvre, vous permettant d’explorer ses attributs et les services auxquels il s’est abonné. [Découvrir comment explorer les détails des profils](create-profile.md)

Pour supprimer un profil, sélectionnez l’option correspondante dans le menu **[!UICONTROL Plus d’actions]**.

## Vidéo pratique {#video}

Découvrez comment accéder aux profils, les gérer et les explorer à l’aide de l’interface utilisateur web de Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
