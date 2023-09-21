---
audience: end-user
title: Envoyer des messages aux abonnés d'un service
description: Découvrez comment envoyer des messages aux abonnés d'un service
badge: label="Beta"
source-git-commit: 6406be82c2bad9346f6743e18535fdfe132b2bd0
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 5%

---


# Envoyer des messages aux abonnés d&#39;un service

Vous pouvez créer des services d’abonnement dans Adobe Campaign et envoyer des messages à vos abonnés. Découvrez comment créer des services d’abonnements dans [cette page](../audience//manage-services.md#create-service).

Pour envoyer des messages à vos abonnés, créez une audience spécifique pour identifier les abonnés, puis créez la diffusion comme décrit ci-dessous. Pour ce faire, procédez comme suit :

1. Création d’une audience. En savoir plus sur les audiences dans [cette page](../audience/create-audience.md).

1. Dans le **[!UICONTROL Créer une audience]** activité, afficher les attributs avancés et sélectionner **[!UICONTROL Destinataire]** > **[!UICONTROL Abonnements]** > **[!UICONTROL Service]**.

   Dans cet exemple, sélectionnez les utilisateurs abonnés au service qui a la variable **Newsletter Luma** libellé.

   ![](assets/service-audience-subscribers.png)

1. Enregistrez l&#39;audience.
1. Créer une diffusion. Les étapes de création d&#39;une diffusion sont présentées dans la section [cette page](../msg/gs-messages.md#create-delivery).
1. Sélectionnez l’audience que vous avez créée ci-dessus.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Créez le contenu de votre message, testez et envoyez la diffusion, comme décrit dans la section [cette section](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

Votre diffusion n&#39;est envoyée qu&#39;aux abonnés de ce service.
