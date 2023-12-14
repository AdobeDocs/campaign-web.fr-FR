---
audience: end-user
title: Créer une diffusion SMS
description: Découvrez comment créer et envoyer des SMS à l’aide d’Adobe Campaign Web.
badge: label="Beta"
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 4ea25f0877fd3f0ab02f3023f041bd040e0530a3
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 64%

---

# Créer une diffusion SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Propriétés de la diffusion SMS"
>abstract="Les propriétés englobent les paramètres de diffusion courants qui vous aident à nommer et à classer votre diffusion. Si votre diffusion est basée sur un schéma étendu, des champs d’options personnalisées spécifiques sont disponibles."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Définissez l’audience du SMS."
>abstract="Vous pouvez créer une nouvelle audience ou en sélectionner une existante en cliquant sur le bouton **Sélection de l’audience** bouton . Si nécessaire, ajoutez une population témoin pour mesurer l&#39;impact de votre diffusion."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=fr" text="Configurer une population témoin"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Sélection du modèle de SMS"
>abstract="Sélectionnez un modèle prédéfini pour démarrer votre diffusion SMS. Les modèles de diffusion vous permettent de réutiliser facilement du contenu et des paramètres personnalisés dans vos campagnes et diffusions."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Utilisation de modèles de diffusion"


Vous pouvez créer une diffusion SMS autonome ou créer un SMS dans le cadre d’un workflow de campagne. Les étapes ci-dessous détaillent la procédure d’une diffusion SMS autonome (ponctuelle). Si vous travaillez dans le contexte d’un workflow de campagne, les étapes de création sont détaillées dans [cette section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Pour créer une diffusion SMS autonome, procédez comme suit :

1. Accédez au menu **[!UICONTROL Diffusions]** dans le rail de gauche, puis cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Sous , **[!UICONTROL Canal]** , choisissez SMS comme canal, puis sélectionnez un modèle. [En savoir plus sur les modèles](../msg/delivery-template.md)

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![](assets/sms_create_1.png)

1. Saisissez un **[!UICONTROL Libellé]** pour la diffusion et accéder au **[!UICONTROL Options supplémentaires]** menu déroulant. Si votre diffusion est basée sur un schéma étendu, **Options personnalisées** sont disponibles.

   +++Configurez les paramètres suivants en fonction de vos besoins.
   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : organisez vos diffusions à l’aide de votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.
+++

1. Cliquez sur le bouton **[!UICONTROL Sélectionner une audience]** pour cibler une audience existante ou créer la vôtre. [En savoir plus sur les audiences](../audience/about-recipients.md).

   ![](assets/sms_create_2.png)

   Découvrez comment sélectionner une audience existante dans [cette page](../audience/add-audience.md)

   Découvrez comment créer une audience dans [cette page](../audience/one-time-audience.md)

1. Activez l’option **[!UICONTROL Activer la population témoin]** pour définir une population témoin afin de mesurer l&#39;impact de votre diffusion. Les messages ne sont pas envoyés à cette population témoin, vous pouvez donc comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l&#39;ont pas fait. [En savoir plus](../audience/control-group.md)

1. Cliquez sur **[!UICONTROL Modifier le contenu]** pour commencer à concevoir le contenu de votre SMS. [En savoir plus](content-sms.md).

   ![](assets/sms_create_4.png)

   Dans cet écran, vous pouvez également [simuler votre contenu](../preview-test/preview-test.md) et [configurer des offres](../content/offers.md).

1. Pour planifier votre diffusion à une date et une heure spécifiques, activez l’option **[!UICONTROL Activer la planification]**. Une fois la diffusion lancée, le message est automatiquement envoyé à la date et à l’heure exactes que vous avez définies pour la personne destinataire. Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#gs-schedule).

1. Cliquez sur **[!UICONTROL Configurer les paramètres de diffusion]** pour accéder aux options avancées liées à votre modèle de diffusion. [En savoir plus](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
