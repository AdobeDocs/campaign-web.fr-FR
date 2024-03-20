---
audience: end-user
title: Création d’une diffusion courrier
description: Découvrez comment créer une diffusion courrier avec Adobe Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 48%

---


# Création d’une diffusion courrier {#create-direct-mail}

Vous pouvez créer une diffusion courrier autonome ou créer une diffusion courrier dans le cadre d&#39;un workflow de campagne. Les étapes ci-dessous décrivent la procédure pour une diffusion courrier autonome (ponctuelle). Si vous travaillez dans le cadre d&#39;un workflow de campagne, les étapes de création sont présentées dans la section [cette section](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Pour créer une diffusion courrier autonome, procédez comme suit :

1. Accédez au menu **[!UICONTROL Diffusions]** dans le rail de gauche, puis cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Sous , **[!UICONTROL Canal]** , choisissez **[!UICONTROL Canal Courrier]** comme canal, puis sélectionnez un modèle. [En savoir plus sur les modèles](../msg/delivery-template.md)

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![](assets/dm-create.png){zoomable=&quot;yes&quot;}

1. Saisissez un **[!UICONTROL libellé]** pour la diffusion et accédez au menu déroulant **[!UICONTROL Options supplémentaires]**. Si votre diffusion est basée sur un schéma étendu, des champs d’**options personnalisées** spécifiques sont disponibles.

   ![](assets/dm-properties.png){zoomable=&quot;yes&quot;}

   +++Configurez les paramètres suivants en fonction de vos besoins.
   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : organisez vos diffusions à l’aide de votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]**: spécifiez la nature de la diffusion à des fins de classification.
+++

1. Cliquez sur le bouton **[!UICONTROL Sélection de l’audience]** pour cibler une audience existante ou créer la vôtre.

   * [Découvrez comment sélectionner une audience existante](../audience/add-audience.md)
   * [Découvrez comment créer une audience](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Les destinataires du courrier doivent contenir au moins leurs noms et adresses postales. Une adresse est considérée comme complète si les champs relatifs au nom, au code postal et à la ville ne sont pas vides. Les personnes destinataires dont les adresses sont incomplètes seront exclues des diffusions par courrier.

1. Activez l’option **[!UICONTROL Activer la population témoin]** pour définir une population témoin et mesurer l’impact de votre diffusion. Les messages ne sont pas envoyés à cette population témoin, de sorte que vous puissiez comparer le comportement de la population qui a reçu le message au comportement des contacts qui ne l’ont pas fait. [Découvrez comment travailler avec les populations témoins.](../audience/control-group.md)

1. Cliquez sur **[!UICONTROL Modifier le contenu]** pour définir les informations (colonnes) à exporter dans le fichier d&#39;extraction. [En savoir plus](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable=&quot;yes&quot;}

1. Pour planifier votre diffusion à une date et une heure spécifiques, activez l’option **[!UICONTROL Activer la planification]**. Une fois la diffusion lancée, le fichier d&#39;extraction sera généré automatiquement à la date et à l&#39;heure exactes que vous avez définies. [Découvrez comment planifier des livraisons](../msg/gs-messages.md#gs-schedule).

   >[!NOTE]
   >
   >Lorsqu’une diffusion est envoyée dans le cadre d’un workflow, vous devez utiliser l’activité **Planificateur**. En savoir plus sur [cette page](../workflows/activities/scheduler.md).

1. Cliquez sur **[!UICONTROL Paramètres]** pour accéder aux options avancées liées à votre modèle de diffusion. [En savoir plus](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable=&quot;yes&quot;}

1. Une fois votre diffusion courrier prête, cliquez sur le bouton **[!UICONTROL Vérifier et envoyer]** pour valider et envoyer votre diffusion et générer le fichier d&#39;extraction. [Découvrez comment prévisualiser et envoyer une diffusion courrier](send-direct-mail.md)

