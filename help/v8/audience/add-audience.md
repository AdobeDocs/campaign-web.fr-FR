---
audience: end-user
title: Sélectionner une audience existante
description: Découvrez comment sélectionner une audience.
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 1d639f16c470297d115443b5579547419413a3d3
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 100%

---


# Sélectionner une audience existante {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Sélectionner une audience existante"
>abstract="Parcourez la liste pour sélectionner une audience existante. Utilisez l&#39;icône Afficher les filtres pour filtrer la liste ou sélectionnez un dossier spécifique."

Cette section explique comment sélectionner une audience existante lors de la définition de la population cible d’une diffusion. Lors de la définition de la cible principale d’une diffusion, vous pouvez également :

* [Créer une audience unique](one-time-audience.md) à l’aide du concepteur de requête.
* [Charger une audience depuis un fichier externe](file-audience.md) (pour les e-mails uniquement).

Les audiences qui peuvent être ciblées dans les diffusions sont accessibles à partir du menu **Audience** sur la gauche. Elles proviennent de plusieurs sources telles que la console cliente, ou encore les workflows d’audience Web Campaign ou Adobe Experience Platform. [Découvrez comment surveiller et gérer les audiences](manage-audience.md)

Pour sélectionner une audience existante pour votre message, procédez comme suit :

1. Dans la section **Audience** de l’assistant de création de diffusion, cliquez sur le bouton **[!UICONTROL Sélectionner une audience]** puis choisissez **[!UICONTROL Sélectionner une audience]** pour utiliser une audience existante.

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

1. Cet écran affiche toutes les audiences existantes pour le dossier actuel.

   ![](assets/create-audience2.png){zoomable=&quot;yes&quot;}

   Pour choisir une audience dans Adobe Experience Platform, accédez à `AEP Audiences folder` dans la section de l’écran dédiée aux filtres. [En savoir plus sur les audiences Adobe Experience Platform](manage-audience.md#monitor)

   ![](assets/select-audience-folder.png){zoomable=&quot;yes&quot;}

1. La section Filtre permet d’accéder aux options de filtrage afin d’affiner la liste des audiences. Pour ce faire, cliquez sur **Ajouter des règles** pour accéder au concepteur de requête, qui vous permet de créer des filtres avancés pour la liste des audiences. [Découvrir comment utiliser le concepteur de requête](../query/query-modeler-overview.md)

   Par exemple, vous pouvez également définir une règle pour filtrer l’origine des audiences, comme indiqué ci-dessous :

   ![](assets/filter-on-aep-audience.png){zoomable=&quot;yes&quot;}

1. Cliquez sur **Confirmer** pour ajouter votre audience comme cible principale de la diffusion. Une fois l’opération terminée, vous pouvez toujours affiner l’audience à l’aide du concepteur de requête en cliquant sur le bouton **Modifier des règles**.

   ![](assets/refine-audience.png){zoomable=&quot;yes&quot;}

   Vous pouvez également définir une population témoin afin de mesurer l’impact de vos campagnes. La population témoin ne reçoit pas le message. Vous pouvez ainsi comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l’ont pas reçu. [En savoir plus](control-group.md)
