---
audience: end-user
title: Sélectionner une audience
description: Découvrez comment sélectionner une audience.
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Positif"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 98%

---


# Sélectionner une audience {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Sélectionner une audience existante"
>abstract="Les audiences sont définies dans la console Adobe Campaign v8. Si une intégration Adobe Experience Platform est disponible, vous devriez également voir les audiences définies par Platform."

Cette section explique comment sélectionner une audience existante lors de la définition de la population cible de la diffusion d’un e-mail. Si vous souhaitez créer une nouvelle audience, reportez-vous à cette [section](segment-builder.md).

1. Dans la section **Audience** de l’assistant de création de diffusion, cliquez sur le bouton **[!UICONTROL Sélectionner une audience]**.

   ![](assets/create-audience.png)

1. Choisissez **[!UICONTROL Sélectionner une audience]** pour utiliser une audience existante. Afin de créer une nouvelle audience pour cet e-mail, choisissez **Créer la vôtre**. Reportez-vous à cette [section](segment-builder.md).

   Cet écran affiche toutes les audiences existantes définies dans la console Adobe Campaign ou à partir d’Adobe Experience Platform.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Pour tirer parti des audiences Adobe Experience Platform, vous devez configurer l’intégration avec les destinations. Consultez la [documentation sur les destinations](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=fr){target="_blank"}.

1. Choisissez une audience, puis cliquez sur **Sélectionner**.

1. Cliquez sur **Modifier les règles** si vous souhaitez affiner votre audience.

   ![](assets/create-audience3.png)

1. Le créateur de règles vous permet d’enrichir votre audience avec des filtres supplémentaires ou en combinant différentes audiences. Consultez cette [section](segment-builder.md).

   ![](assets/create-audience4.png)

1. Cliquez sur **Enregistrer**.

Vous pouvez également définir une population témoin afin de mesurer l’impact de vos campagnes. La population témoin ne reçoit pas le message. Vous pouvez ainsi comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l’ont pas reçu. Reportez-vous à la [section](control-group.md).