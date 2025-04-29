---
audience: end-user
title: Création d’une diffusion de centre d’appels
description: Découvrez comment créer une diffusion de centre d’appels avec Adobe Campaign Web
source-git-commit: 0721d20ddec3271d9fac5f5645bd5865380ef9ba
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 13%

---

# Création et envoi d&#39;une diffusion de centre d&#39;appels {#create-call-center}

Vous pouvez créer une diffusion de centre d&#39;appels autonome, ou en créer une dans le cadre d&#39;un workflow de campagne. Les étapes ci-dessous décrivent la procédure à suivre pour une diffusion autonome (ponctuelle). Si vous travaillez dans le contexte d’un workflow de campagne, les étapes de création sont détaillées dans [cette section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Pour créer et envoyer une nouvelle diffusion de centre d’appel autonome, procédez comme suit :

1. Créer la diffusion, [en savoir plus](#create-delivery)
1. Sélectionnez l’audience, [en savoir plus](#select-audience)
1. Modifier le contenu, [en savoir plus](#edit-content)
1. Prévisualiser et envoyer la diffusion, [en savoir plus](#preview-send)

## Créer une diffusion{#create-delivery}

Pour créer la diffusion et configurer ses propriétés, procédez comme suit :

1. Sélectionnez le menu **[!UICONTROL Diffusions]** et cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Choisissez **[!UICONTROL Centre d’appel]** comme canal et cliquez sur **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![Capture d’écran montrant la création d’une diffusion de centre d’appels](assets/cc-create.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si vous souhaitez sélectionner un autre modèle, reportez-vous à cette [page](../msg/delivery-template.md).

1. Sous **[!UICONTROL Propriétés]**, saisissez un **[!UICONTROL Libellé]** pour la diffusion. Les autres options sont présentées dans cette [section](../email/create-email.md#create-email).

   ![Capture d’écran affichant la configuration des propriétés pour une diffusion de centre d’appels](assets/cc-properties.png){zoomable="yes"}

>[!NOTE]
>
>Vous pouvez planifier l’envoi de votre diffusion à une date spécifique. Pour plus d’informations à ce sujet, consultez cette [section](../msg/gs-deliveries.md#gs-schedule).

## Sélectionner l’audience{#select-audience}

Vous devez maintenant définir l’audience qui sera ciblée pour le fichier d’extraction.

1. Dans la section **[!UICONTROL Audience]** de la page de diffusion, cliquez sur **[!UICONTROL Sélectionner une audience]**.

   ![Capture d’écran affichant la sélection de l’audience pour une diffusion de centre d’appels](assets/cc-audience.png){zoomable="yes"}

1. Choisissez une audience existante ou créez la vôtre.

   * [Découvrir comment sélectionner une audience existante](../audience/add-audience.md)
   * [Découvrir comment créer une audience](../audience/one-time-audience.md)

   ![Capture d’écran affichant la sélection de l’audience pour une diffusion de centre d’appels](assets/cc-audience2.png){zoomable="yes"}

>[!NOTE]
>
>Les destinataires du centre d&#39;appels doivent contenir au moins leurs nom et numéro de téléphone. Tous les destinataires dont les informations sont incomplètes seront exclus des diffusions du centre d’appels.
>
>Pour savoir comment configurer des populations témoins, consultez cette [page](../audience/control-group.md)

## Modifier le contenu{#edit-content}

Maintenant, concevons le contenu du fichier d’extraction qui sera généré par la diffusion du centre d’appels.

1. Dans la page de diffusion, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

   ![Capture d’écran montrant la modification du contenu pour une diffusion de centre d’appels](assets/cc-content0.png){zoomable="yes"}

1. Renseignez le champ **[!UICONTROL Nom du fichier]**. Pour savoir comment personnaliser le nom du fichier, consultez cette [page](../personalization/personalize.md).

1. Sélectionnez un **[!UICONTROL Format de fichier]** : **Texte**, **Texte utilisant des colonnes à largeur fixe**, **CSV (Excel)** ou **XML**.

   ![Capture d’écran montrant la modification du contenu pour une diffusion de centre d’appels](assets/cc-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >Les options de format d’extraction sont présentées dans cette [page](../direct-mail/content-direct-mail.md#properties).

1. Activez l’option **[!UICONTROL Quantité demandée]** si vous souhaitez restreindre le nombre de destinataires pour votre diffusion.

1. Dans la section **[!UICONTROL Contenu]**, cliquez sur le bouton **[!UICONTROL Ajouter un attribut]** pour créer une colonne à afficher dans le fichier d’extraction.

1. Sélectionnez l’attribut à afficher dans la colonne, puis confirmez. Pour en savoir plus sur la sélection des attributs et leur ajout aux favoris, consultez cette [page](../get-started/attributes.md).

   ![Capture d’écran affichant le bouton Ajouter un attribut et les options permettant d’ajouter des attributs au fichier d’extraction.](assets/cc-add-attribute.png)

1. Répétez ces étapes pour ajouter autant de colonnes que nécessaire à votre fichier d’extraction.

   Vous pouvez ensuite modifier les attributs, trier le fichier d’extraction ou modifier la position des colonnes. Pour en savoir plus à ce sujet, consultez cette [page](../direct-mail/content-direct-mail.md#content).

   ![Capture d’écran affichant les options de configuration des attributs pour le fichier d’extraction.](assets/cc-content-attributes.png)

## Prévisualiser et envoyer la diffusion{#preview-send}

Lorsque le contenu de la diffusion est prêt, vous pouvez le prévisualiser à l’aide de profils de test et envoyer des BAT. Vous pouvez ensuite envoyer la diffusion du centre d’appel pour générer le fichier d’extraction.

Les étapes principales pour prévisualiser et envoyer le fichier d’extraction sont les suivantes. Pour plus d’informations, consultez [cette page](../direct-mail/send-direct-mail.md).

1. Sur la page de contenu de la diffusion, cliquez sur **[!UICONTROL Simuler du contenu]**.

   ![Capture d’écran affichant l’option Simuler du contenu dans la page de contenu de la diffusion](assets/cc-simulate0.png){zoomable="yes"}

1. Sélectionnez un ou plusieurs profils de test pour prévisualiser le contenu personnalisé. Vous pouvez également envoyer des BAT. [En savoir plus](../direct-mail/send-direct-mail.md#preview-dm)

   ![Capture d’écran affichant l’option Simuler du contenu dans la page de contenu de la diffusion](assets/cc-simulate.png){zoomable="yes"}

1. Dans la page de diffusion, cliquez sur **[!UICONTROL Vérifier et envoyer]**.

   ![Capture d’écran affichant l’option vérifier et envoyer dans la page de diffusion](assets/cc-review-send.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Préparer]** et suivez la progression et les statistiques fournies, puis confirmez.

   ![Capture d’écran affichant l’option de préparation et le menu Journaux](assets/cc-prepare.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final, puis confirmez.

Une fois votre diffusion envoyée, le fichier d’extraction est automatiquement généré et exporté vers l’emplacement spécifié dans le compte externe **[!UICONTROL Routage]** sélectionné dans les [paramètres avancés](../advanced-settings/delivery-settings.md) du modèle de diffusion.

Suivez les données de vos KPI (indicateurs clés de performance) à partir de votre page de diffusion et les données à partir du menu **[!UICONTROL Journaux]**.

Commencez à mesurer l’impact de votre message à l’aide de rapports intégrés. [En savoir plus](../reporting/direct-mail.md)


