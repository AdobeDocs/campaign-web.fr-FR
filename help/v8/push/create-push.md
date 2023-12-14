---
audience: end-user
title: Créer une diffusion notification push
description: Découvrez comment créer une diffusion de notification push avec Adobe Campaign Web.
badge: label="Beta"
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 057a6b360093bc314aed6d6b0d84bfba7af3f464
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 39%

---

# Créer une diffusion notification push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Modèle de notification push"
>abstract="Sélectionnez un modèle de notification push pour démarrer votre diffusion push. Les modèles de diffusion vous permettent de réutiliser facilement du contenu et des paramètres personnalisés dans vos campagnes et diffusions."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Utilisation de modèles de diffusion"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propriétés de diffusion par notification push"
>abstract="Définissez les propriétés de la diffusion push. Saisissez le libellé de la notification push et utilisez la méthode **Options supplémentaires** pour configurer le nom interne, le dossier de diffusion et le code. Vous pouvez également saisir une description personnalisée."

Vous pouvez créer une diffusion de notification push autonome ou créer une notification push dans le cadre d’un workflow de campagne. Les étapes ci-dessous détaillent la procédure d’une diffusion de notification push autonome (ponctuelle). Si vous travaillez dans le contexte d’un workflow de campagne, les étapes de création sont détaillées dans [cette section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Création d’une diffusion push {#create-push-delivery}

Pour créer une diffusion de notification push autonome, procédez comme suit :

1. Accédez au menu **[!UICONTROL Diffusions]** dans le rail de gauche, puis cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Sous , **[!UICONTROL Canal]** , choisissez **Notification push** comme canal et sélectionnez un modèle, en fonction du système de fonctionnement de l’appareil choisi : Android ou iOS. [En savoir plus sur les modèles](../msg/delivery-template.md)

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![](assets/push_create_1.png)

## Configuration des paramètres de diffusion {#configure-push-settings}

Configurez vos paramètres de diffusion comme indiqué ci-dessous :

1. Saisissez un **[!UICONTROL Libellé]** pour la diffusion. Par défaut, le libellé est défini avec le libellé du modèle sélectionné. Il doit être mis à jour.

1. Parcourez les **[!UICONTROL Options supplémentaires]** pour personnaliser les options, le cas échéant.

   +++Configurez les paramètres suivants en fonction de vos besoins.
   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : organisez vos diffusions à l’aide de votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.
+++


## Sélection de l’audience de diffusion push {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Définition de l’audience de notification push"
>abstract="Pour définir l&#39;audience de votre message, vous devez d&#39;abord sélectionner l&#39;application associée à la diffusion push. Par défaut, votre notification push est envoyée à tous les abonnés de l&#39;application. Vous pouvez affiner une audience spécifique en cliquant sur le bouton **Sélection de l’audience** bouton . Si nécessaire, ajoutez une population témoin pour mesurer l&#39;impact de votre diffusion."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=fr" text="Configurer une population témoin"


Vous devez d&#39;abord sélectionner l&#39;application, puis affiner l&#39;audience de notification push, comme décrit ci-dessous :

1. Dans la **[!UICONTROL Audience]** , sélectionnez l&#39;application à utiliser pour cette diffusion. Par défaut, votre notification push est envoyée à tous les abonnés de l&#39;application. Vous pouvez affiner une audience spécifique en cliquant sur le bouton **[!UICONTROL Sélection de l’audience]** bouton .

   ![](assets/push_create_2.png)

1. Sélectionnez une audience existante ou créez votre propre audience pour affiner la population cible de votre diffusion push. Pour la notification push, la valeur par défaut [dimension cible](../audience/about-recipients.md#targeting-dimensions) is **Application d&#39;abonné** (nms:appSubscriptionRcp), lié à la table des destinataires.

   Découvrez comment sélectionner une audience existante dans [cette page](../audience/add-audience.md)

   Découvrez comment créer une audience dans [cette page](../audience/one-time-audience.md)

1. Activez l’option **[!UICONTROL Activer la population témoin]** pour définir une population témoin afin de mesurer l&#39;impact de votre diffusion. Les messages ne sont pas envoyés à cette population témoin, vous pouvez donc comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l&#39;ont pas fait. [En savoir plus](../audience/control-group.md)

## Définition du contenu de la notification push {#create-content-push}

Pour définir le contenu de votre notification, cliquez sur **[!UICONTROL Modifier le contenu]**. [En savoir plus](content-push.md).

![](assets/push_create_5.png)

Dans cet écran, vous pouvez également [simuler votre contenu](../preview-test/preview-test.md) et [configurer des offres](../content/offers.md).

## Planifier l’envoi de votre diffusion {#schedule-push}

Pour planifier votre diffusion à une date et une heure spécifiques, activez l’option **[!UICONTROL Activer la planification]**. Une fois la diffusion lancée, le message est automatiquement envoyé à la date et à l’heure exactes que vous avez définies pour la personne destinataire. Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#gs-schedule).

![](assets/push_create_3.png)


## Paramètres avancés de la diffusion {#adv-push}

Cliquez sur **[!UICONTROL Configurer les paramètres de diffusion]** pour accéder aux options avancées liées à votre modèle de diffusion. [En savoir plus](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png)
