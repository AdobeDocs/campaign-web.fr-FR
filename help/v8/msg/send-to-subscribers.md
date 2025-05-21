---
audience: end-user
title: Envoyer des messages aux personnes abonnées à un service
description: Découvrez comment envoyer des messages aux personnes abonnées à un service.
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 100%

---

# Envoyer des messages aux personnes abonnées à un service {#send-to-subscribers}

Vous pouvez créer des services d’abonnements dans Adobe Campaign et envoyer des messages à vos personnes abonnées. Découvrez comment créer des services d’abonnements sur [cette page](../audience//manage-services.md#create-service).

Pour envoyer des messages à vos personnes abonnées, créez une audience spécifique pour identifier les personnes abonnées, puis créez la diffusion comme décrit ci-dessous.

1. Créez une audience. Un nouveau workflow est automatiquement créé. [En savoir plus sur les audiences](../audience/create-audience.md).

1. Pour une meilleure lisibilité, modifiez le nom du workflow dans le champ **Libellé** dans les paramètres du workflow. [Découvrez comment configurer les paramètres des workflows](../workflows/workflow-settings.md).

1. Ouvrez l’activité **[!UICONTROL Créer une audience]**, puis sélectionnez **[!UICONTROL Créer une audience]**. [Découvrez comment configurer une activité Créer une audience](../workflows/activities/build-audience.md).

   ![Capture d’écran affichant la configuration de l’activité Créer une audience dans Adobe Campaign.](assets/service-create-audience.png){zoomable="yes"}

1. Dans le flux de création d’audience, sélectionnez les conditions personnalisées suivantes : les **[!UICONTROL Abonnements]** existent de manière à ce que **[!UICONTROL Service]** est égal au service que vous avez défini. Dans cet exemple, sélectionnez votre **Newsletter Luma yoga**.

   ![Capture d’écran affichant le flux de création d’audiences avec des conditions personnalisées pour les abonnements dans Adobe Campaign.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Sélectionnez **[!UICONTROL Confirmer]** et cliquez sur **[!UICONTROL Démarrer]** pour exécuter le workflow.

1. Créez une diffusion. Les étapes de création d’une diffusion sont détaillées sur [cette page](../msg/gs-messages.md#create-delivery).

1. Accédez à vos paramètres de diffusion et définissez le mapping de ciblage par défaut sur **Abonnements (nms:subscriptions)**.

   ![Capture d’écran affichant les paramètres de diffusion avec le mapping de ciblage remplacé par Abonnements dans Adobe Campaign.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. Dans la section cible principale de la diffusion, sélectionnez l’audience que vous avez créée ci-dessus.

   ![Capture d’écran affichant la section cible principale de la diffusion avec l’audience sélectionnée dans Adobe Campaign.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Créez le contenu de votre message, testez-le et envoyez la diffusion, comme décrit dans [cette section](../preview-test/preview-test.md).

   ![Capture d’écran affichant la diffusion prête à être envoyée dans Adobe Campaign.](assets/service-delivery-ready.png){zoomable="yes"}

Votre diffusion n’est envoyée qu’aux personnes abonnées à ce service.