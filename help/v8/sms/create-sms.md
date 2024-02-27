---
audience: end-user
title: Créer une diffusion SMS
description: Découvrez comment créer et envoyer des SMS à l’aide d’Adobe Campaign Web.
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 100%

---

# Créer une diffusion SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Propriétés de la diffusion SMS"
>abstract="Les propriétés englobent les paramètres de diffusion courants qui vous aident à nommer et à classer votre diffusion. Si votre diffusion est basée sur un schéma étendu, des champs d’options personnalisées spécifiques sont disponibles."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Définir l’audience du SMS"
>abstract="Vous pouvez créer une nouvelle audience ou en sélectionner une existante en cliquant sur le bouton **Sélectionner une audience**. Si nécessaire, ajoutez une population témoin pour mesurer l’impact de votre diffusion."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=fr" text="Définir une population témoin"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Sélection du modèle de SMS"
>abstract="Sélectionnez un modèle prédéfini pour démarrer votre diffusion par SMS. Les modèles de diffusion vous permettent de réutiliser facilement du contenu et des paramètres personnalisés dans vos campagnes et diffusions."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=fr" text="Utiliser des modèles de diffusion"


Vous pouvez créer une diffusion SMS autonome ou créer un SMS dans le cadre d’un workflow de campagne. Les étapes ci-dessous détaillent la procédure d’une diffusion SMS autonome (ponctuelle). Si vous travaillez dans le contexte d’un workflow de campagne, les étapes de création sont détaillées dans [cette section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Pour créer une diffusion SMS autonome, procédez comme suit :

1. Accédez au menu **[!UICONTROL Diffusions]** dans le rail de gauche, puis cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Sous la section **[!UICONTROL Canal]**, choisissez SMS comme canal et sélectionnez un modèle. [En savoir plus sur les modèles](../msg/delivery-template.md)

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![](assets/sms_create_1.png){zoomable=&quot;yes&quot;}

1. Saisissez un **[!UICONTROL libellé]** pour la diffusion et accédez au menu déroulant **[!UICONTROL Options supplémentaires]**. Si votre diffusion est basée sur un schéma étendu, des champs d’**options personnalisées** spécifiques sont disponibles.

   +++Configurez les paramètres suivants en fonction de vos besoins.
   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : organisez vos diffusions à l’aide de votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.
+++

1. Cliquez sur le bouton **[!UICONTROL Sélectionner une audience]** pour cibler une audience existante ou créer la vôtre. [En savoir plus sur les audiences](../audience/about-recipients.md).

   ![](assets/sms_create_2.png){zoomable=&quot;yes&quot;}

   Découvrez comment sélectionner une audience existante sur [cette page](../audience/add-audience.md).

   Découvrez comment créer une audience sur [cette page](../audience/one-time-audience.md).

1. Activez l’option **[!UICONTROL Activer la population témoin]** pour définir une population témoin et mesurer l’impact de votre diffusion. Les messages ne sont pas envoyés à cette population témoin. Vous pouvez ainsi comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l’ont pas reçu. [En savoir plus](../audience/control-group.md)

1. Cliquez sur **[!UICONTROL Modifier le contenu]** pour commencer à concevoir le contenu de votre SMS. [En savoir plus](content-sms.md)

   ![](assets/sms_create_4.png){zoomable=&quot;yes&quot;}

   Dans cet écran, vous pouvez également [simuler votre contenu](../preview-test/preview-test.md) et [configurer des offres](../msg/offers.md).

1. Pour planifier votre diffusion à une date et une heure spécifiques, activez l’option **[!UICONTROL Activer la planification]**. Une fois la diffusion lancée, le message est automatiquement envoyé à la date et à l’heure exactes que vous avez définies pour la personne destinataire. Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#gs-schedule).

   >[!NOTE]
   >
   >Lorsqu’une diffusion est envoyée dans le cadre d’un workflow, vous devez utiliser l’activité **Planificateur**. En savoir plus sur [cette page](../workflows/activities/scheduler.md).

1. Cliquez sur **[!UICONTROL Paramètres]** pour accéder aux options avancées liées à votre modèle de diffusion. [En savoir plus](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png){zoomable=&quot;yes&quot;}
