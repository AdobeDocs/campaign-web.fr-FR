---
audience: end-user
title: Créer une diffusion par notification push
description: Découvrez comment créer une diffusion de notification push avec Adobe Campaign Web.
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 90%

---

# Créer une diffusion par notification push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Modèle de notification push"
>abstract="Sélectionnez un modèle de notification push pour démarrer votre diffusion par notification push. Les modèles de diffusion vous permettent de réutiliser facilement du contenu et des paramètres personnalisés dans vos campagnes et diffusions."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=fr" text="Utiliser des modèles de diffusion"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propriétés de diffusion par notification push"
>abstract="Définissez les propriétés de votre diffusion par notification push. Saisissez le libellé de la notification push et utilisez les **Options supplémentaires** pour configurer le nom interne, le dossier de diffusion et le code. Vous pouvez également ajouter une description personnalisée."

Vous pouvez créer une diffusion de notification push autonome ou créer une notification push dans le cadre d’un workflow de campagne. Les étapes ci-dessous détaillent la procédure d’une diffusion de notification push autonome (ponctuelle). Si vous travaillez dans le contexte d’un workflow de campagne, les étapes de création sont détaillées dans [cette section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Créer une diffusion par notification push {#create-push-delivery}

Pour créer une diffusion de notification push autonome, procédez comme suit :

1. Accédez au menu **[!UICONTROL Diffusions]** dans le rail de gauche, puis cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Dans la section **[!UICONTROL Canal]**, choisissez **Notification push** comme canal et sélectionnez un modèle en fonction du système d’exploitation sélectionné : Android ou iOS. [En savoir plus sur les modèles](../msg/delivery-template.md)

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![](assets/push_create_1.png){zoomable=&quot;yes&quot;}

## Configurer les paramètres de la diffusion {#configure-push-settings}

Configurez vos paramètres de diffusion comme indiqué ci-dessous :

1. Saisissez le **[!UICONTROL libellé]** de la diffusion. Par défaut, le libellé est défini sur celui du modèle sélectionné. Il doit être mis à jour.

1. Parcourez le menu déroulant **[!UICONTROL Options supplémentaires]** pour personnaliser les options, le cas échéant. Si votre diffusion est basée sur un schéma étendu, des champs d’**options personnalisées** spécifiques sont disponibles.

   +++Configurez les paramètres suivants en fonction de vos besoins.
   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : organisez vos diffusions à l’aide de votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.
+++


## Sélectionner l’audience de votre diffusion par notification push {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Définir le contenu de l’audience de la notification push."
>abstract="Pour définir l’audience de votre message, vous devez d’abord sélectionner l’application associée à la diffusion par notification push. Par défaut, votre notification push est envoyée à toutes les personnes abonnées de l’application. Vous pouvez affiner une audience spécifique en cliquant sur le bouton **Sélectionner une audience**. Si nécessaire, ajoutez une population témoin pour mesurer l’impact de votre diffusion."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=fr" text="Configurer une population témoin"


Vous devez d’abord sélectionner l’application, puis affiner l’audience de la notification push, comme décrit ci-dessous :

1. Dans le menu **[!UICONTROL Audience]**, sélectionnez l’application à utiliser pour cette diffusion. Par défaut, votre notification push est envoyée à toutes les personnes abonnées de l’application. Vous pouvez affiner une audience spécifique en cliquant sur le bouton **[!UICONTROL Sélectionner une audience]**.

   ![](assets/push_create_2.png){zoomable=&quot;yes&quot;}

1. Sélectionnez une audience existante ou créez votre propre audience pour affiner la population cible de votre diffusion de notification push. Pour les notifications push, la [dimension de ciblage](../audience/about-recipients.md#targeting-dimensions) par défaut est **Applications abonnée** (nms:appSubscriptionRcp), qui est liée au tableau des personnes destinataires.

   Découvrez comment sélectionner une audience existante sur [cette page](../audience/add-audience.md).

   Découvrez comment créer une audience sur [cette page](../audience/one-time-audience.md).

1. Activez l’option **[!UICONTROL Activer la population témoin]** pour définir une population témoin et mesurer l’impact de votre diffusion. Les messages ne sont pas envoyés à cette population témoin. Vous pouvez ainsi comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l’ont pas reçu. [En savoir plus](../audience/control-group.md)

## Définir le contenu de la notification push {#create-content-push}

Pour définir le contenu de votre notification, cliquez sur **[!UICONTROL Modifier le contenu]**. [En savoir plus](content-push.md)

![](assets/push_create_5.png){zoomable=&quot;yes&quot;}

Dans cet écran, vous pouvez également [simuler votre contenu](../preview-test/preview-test.md) et [configurer des offres](../msg/offers.md).

## Planifier lʼenvoi de la diffusion {#schedule-push}

Lorsqu&#39;une diffusion est envoyée dans le cadre d&#39;un workflow, vous devez utiliser la variable **Planificateur** activité. En savoir plus sur [cette page](../workflows/activities/scheduler.md). Les étapes ci-dessous s’appliquent uniquement aux diffusions autonomes.

Pour planifier une diffusion push autonome à une date et une heure spécifiques, procédez comme suit :

1. Accédez au **[!UICONTROL Planification]** de la section des propriétés de la diffusion.

1. Utilisez le bouton (bascule) **[!UICONTROL Activer la planification]** pour l’activer.

1. Définissez la date et l’heure d’envoi.

Une fois la diffusion lancée, le message est automatiquement envoyé à la date et à l&#39;heure exactes que vous avez définies pour le destinataire.

![](assets/push_create_3.png){zoomable=&quot;yes&quot;}

Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#gs-schedule).

## Paramètres avancés des diffusions {#adv-push}

Cliquez sur **[!UICONTROL Configurer les paramètres de diffusion]** pour accéder aux options avancées liées à votre modèle de diffusion. [En savoir plus](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png){zoomable=&quot;yes&quot;}
