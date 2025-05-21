---
title: Commencer avec les profils
description: Découvrez comment surveiller et gérer les profils dans Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 100%

---

# Prise en main des profils {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profils"
>abstract="Un profil est un enregistrement ciblé pour recevoir les messages envoyés par Adobe Campaign. Depuis cette liste, vous pouvez visualiser les détails des profils, en fonction de vos autorisations. Utilisez les options de filtrage pour parcourir cette liste. Vous pouvez modifier et mettre à jour un petit ensemble d’attributs de vos profils."

## Qu’est-ce qu’un profil ? {#what}

Un **profil**, également appelé « destinataire » dans la console cliente, représente un enregistrement stocké dans la base de données Campaign. Il sert de composant clé pour [créer des audiences](create-audience.md) pour les diffusions et [ajouter des données de personnalisation](../personalization/personalize.md) à votre contenu. Adobe Campaign permet de gérer facilement les profils, y compris de créer des entrées et d’accéder à une vue complète des attributs et abonnements aux services de tous les profils, via l’interface d’utilisation de Campaign Web.

De plus, des **[!UICONTROL profils de test]**, désignés comme des « profils de contrôle » dans la console cliente, permettent de cibler des personnes destinataires supplémentaires qui ne correspondent pas aux critères de ciblage d’une diffusion donnée. Ces profils contiennent des coordonnées fictives ou des coordonnées contrôlées par l’expéditeur ou l’expéditrice. Les profils de test sont les profils destinataires des BAT utilisés pour tester les messages en envoyant des BAT. [Découvrir comment utiliser des profils de test](test-profiles.md)

Les profils et les profils de test sont utiles pour tester les diffusions avant qu’elles n’atteignent l’audience visée. Cela permet de prévisualiser le contenu et la personnalisation des messages, envoyer des BAT à des fins de test et de validation, évaluer le rendu des e-mails sur différentes plateformes et appareils et tester les pages de destination. [Découvrir comment prévisualiser et tester des diffusions](../preview-test/preview-test.md)

➡️ [Découvrez cette fonctionnalité en vidéo](#video)

## Accéder à la liste des profils {#access}

Les profils sont accessibles et modifiables dans Adobe Campaign Web à partir de l’entrée **[!UICONTROL Gestion des clientes et clients]** > **Profils** dans le rail de navigation de gauche. Ils sont également accessibles dans la vue **[!UICONTROL Explorateur]**, dans le nœud **[!UICONTROL Profils et cibles]** > **[!UICONTROL Personnes destinataires]**. De là, parcourez, créez et gérez des dossiers ou des sous-dossiers, et vérifiez les autorisations associées. [Découvrez comment créer des dossiers](../get-started/permissions.md#folders).

>[!NOTE]
>
>En fonction de vos autorisations, il se peut que vous n’ayez pas accès à la liste complète des profils stockés dans la base de données. [En savoir plus sur les autorisations](../get-started/permissions.md)

Filtrez la liste **[!UICONTROL Profils]** à l’aide du champ de recherche ou des filtres disponibles en cliquant sur le bouton **Afficher les filtres**. Limitez les résultats à un [dossier](../get-started/permissions.md#folders) spécifique à l’aide de la liste déroulante ou ajoutez des règles à l’aide du [concepteur de requête](../query/query-modeler-overview.md).

![Filtres disponibles dans la liste des profils](assets/profiles-list-filters.png){zoomable="yes"}

Pour accéder aux détails d’un profil, cliquez sur son nom dans la liste. Une vue détaillée du profil s’ouvre, vous permettant d’explorer ses attributs et les services auxquels il s’est abonné. [Découvrir comment explorer les détails des profils](create-profile.md)

Pour supprimer un profil, sélectionnez l’option correspondante dans le menu **[!UICONTROL Plus d’actions]**.

## Vidéo pratique {#video}

Découvrez comment accéder aux profils, les gérer et les explorer à l’aide de l’interface utilisateur web de Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)