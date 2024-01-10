---
audience: end-user
title: Utiliser une audience Adobe Experience Platform
description: Découvrez comment utiliser une audience à partir d’Adobe Experience Platform.
badge: label="Beta"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 1f2a6e0944f46c0e37ce9e2b174a08e69981d143
workflow-type: ht
source-wordcount: '283'
ht-degree: 100%

---

# Utiliser une audience Adobe Experience Platform{#aep-audience}

La destination et les connecteurs source d’Adobe Campaign Managed Cloud Services permettent une intégration transparente entre Adobe Campaign et Adobe Experience Platform.

Une fois l’audience Adobe Experience Platform créée, vous pouvez l’utiliser de la même manière qu’une audience de campagne pour personnaliser et envoyer des messages.

>[!NOTE]
>
>Pour utiliser les audiences Adobe Experience Platform dans Campaign, vous devez configurer l’intégration aux sources et destinations Adobe. Consultez la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=fr){target="_blank"}.

Pour sélectionner l’audience d’une diffusion, vous pouvez également procéder comme suit :

* Créez une audience. [En savoir plus](../query/query-modeler-overview.md)
* Chargez une audience à partir d’un fichier externe. [En savoir plus](file-audience.md)
* Utilisez une audience de campagne existante. [En savoir plus](add-audience.md).

Pour sélectionner une audience Adobe Experience Platform pour votre diffusion, procédez comme suit :

1. Dans la section **Audience** de l’assistant de création de diffusion, cliquez sur le bouton **[!UICONTROL Sélectionner une audience]**.

   ![](assets/create-audience.png)

1. Choisissez **[!UICONTROL Sélectionner une audience]** pour utiliser une audience existante. Afin de créer une nouvelle audience pour cet e-mail, choisissez **Créer la vôtre**. Reportez-vous à cette [section](../query/query-modeler-overview.md).

   Cet écran affiche toutes les audiences existantes définies dans la console cliente Adobe Campaign, pour le dossier actuel. Pour choisir une audience dans Adobe Experience Platform, accédez à `AEP Audiences folder` dans la section dédiée aux filtres de l’écran.

   ![](assets/select-audience-folder.png)

   Vous pouvez également définir une règle pour filtrer l’origine des audiences, comme indiqué ci-dessous :

   ![](assets/filter-on-aep-audience.png)

1. Choisissez une audience, puis cliquez sur **Sélectionner**.

1. Cliquez sur **Modifier les règles** si vous souhaitez affiner votre audience.

   ![](assets/refine-audience.png)

1. Le créateur de règles vous permet d’enrichir votre audience avec des filtres supplémentaires ou en combinant différentes audiences. Consultez cette [section](../query/query-modeler-overview.md).

1. Cliquez sur **Enregistrer**.
