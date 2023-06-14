---
audience: end-user
title: Créer une diffusion de notification push
description: Découvrez comment créer une diffusion de notification push avec Adobe Campaign Web
badge: label="Alpha"
source-git-commit: 4f7cedc4197a983d4d13294744e30836a0263d3a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 65%

---

# Créer une diffusion de notification push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Définir lʼaudience de la notification push"
>abstract="Sélectionnez l’audience la plus appropriée pour votre notification push."

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Modèle de notification push"
>abstract="Sélectionnez un modèle de notification push pour démarrer votre diffusion par notification push."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propriétés de diffusion par notification push"
>abstract="Gérez les propriétés de la diffusion par notification push."

1. Dans la page d’accueil **[!UICONTROL Diffusions]**, cliquez sur **[!UICONTROL Créer une diffusion]**.

1. Sous , **[!UICONTROL Canal]** , choisissez Notification push comme canal et sélectionnez un modèle en fonction du système opérationnel sélectionné : Android ou iOS. [En savoir plus sur les modèles](../msg/delivery-template.md)

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![](assets/push_create_1.png)

1. Saisissez un **[!UICONTROL Libellé]** pour la diffusion et accédez au menu déroulant **[!UICONTROL Options supplémentaires]**.

   +++Configurez les paramètres suivants en fonction de vos besoins.
   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : organisez vos diffusions à l’aide de votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.
+++

1. Dans la **[!UICONTROL Audience]** , sélectionnez l&#39;application à utiliser pour cette diffusion.

1. Cliquez sur le bouton **[!UICONTROL Sélectionner une audience]** pour cibler une audience existante ou créer la vôtre. [En savoir plus](../audience/about-audiences.md)

   Notez que, par défaut, votre notification push sera envoyée à tous les abonnés de l&#39;application.

   ![](assets/push_create_2.png)

1. Activez l’option **[!UICONTROL Activer la population témoin]** permettant de définir une population témoin afin de mesurer l’impact de votre diffusion. Vous pouvez ainsi comparer le comportement de la population qui a reçu le message à celui des contacts qui ne l’ont pas reçu. [En savoir plus](../audience/control-group.md)

1. Cliquez sur **[!UICONTROL Modifier le contenu]** pour commencer à concevoir le contenu de votre notification push. [En savoir plus](content-push.md)

   ![](assets/push_create_5.png)

   Dans cet écran, vous pouvez également [simuler votre contenu](../preview-test/preview-test.md) et [configuration des offres](../content/offers.md).

1. Pour planifier votre diffusion à une date et une heure spécifiques, activez l’option **[!UICONTROL Activer la planification]**. Une fois la diffusion lancée, le message est automatiquement envoyé à la date et à l’heure exactes que vous avez définies pour le ou la destinataire.

   ![](assets/push_create_3.png)

1. Cliquez sur **[!UICONTROL Configuration des paramètres de diffusion]** pour accéder aux options avancées liées à votre modèle de diffusion. [En savoir plus](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_4.png)
