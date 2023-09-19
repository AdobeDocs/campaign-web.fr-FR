---
audience: end-user
title: Gérer les abonnés d'un service
description: Découvrez comment gérer et diffuser aux abonnés d’un service dans Adobe Campaign Web
badge: label="Beta"
source-git-commit: 5125de258edd4e3eda9a8507228156ee40215532
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---


# Gérer les abonnés d&#39;un service {#manage-subscribers}

Une fois que [création d’un service](manage-services.md#create-service), vous pouvez ajouter des abonnés, désabonner des destinataires et diffuser aux abonnés de ce service.

## Ajouter des abonnés à votre service {#add-subscribers}

Pour ajouter manuellement des abonnés, procédez comme suit.

1. Sélectionnez un service existant à partir de la fonction **[!UICONTROL Services d’inscriptions]** liste.

1. Sélectionnez la variable **[!UICONTROL Abonnés]** et cliquez sur **[!UICONTROL Ajout de profils]**.

   ![](assets/service-subscribers-tab.png)

1. Sélectionnez les profils à ajouter dans la liste, puis cliquez sur **[!UICONTROL Confirmer]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Cliquez sur **[!UICONTROL Envoyer]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> Les destinataires sélectionnés recevront l&#39;abonnement. [message de confirmation](manage-services.md#create-confirmation-message) que vous avez sélectionné lorsque [création du service](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

Les profils ajoutés sont affichés dans le **[!UICONTROL Abonnés]** liste. Ils sont maintenant abonnés à votre service.

## Supprimer des abonnés de votre service {#remove-subscribers}

### Désabonner manuellement les destinataires {#manual-unsubscription}

Une fois que [abonnés ajoutés](#add-subscribers) à votre service, vous pouvez vous désabonner manuellement de chacun d’eux. Suivez les étapes ci-dessous.

1. Sélectionnez un service existant à partir de la fonction **[!UICONTROL Services d’inscriptions]** liste.

1. Cliquez sur l’icône de trois points située en regard du nom du destinataire souhaité, puis sélectionnez **[!UICONTROL Supprimer]**.

   ![](assets/service-subscribers-delete.png)

1. Confirmez la suppression et cliquez sur **[!UICONTROL Envoyer]**. Le destinataire sélectionné recevra la désinscription. [message de confirmation](manage-services.md#create-confirmation-message) que vous avez sélectionné lorsque [création du service](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

Le destinataire est supprimé de la variable **[!UICONTROL Abonnés]** et n’est plus abonné à votre service.

### Désabonner automatiquement les destinataires {#automatic-unsubscription}

Un service d’abonnement peut avoir une durée limitée. Les destinataires sont automatiquement désabonnés à l&#39;expiration de la période de validité.

Cette période est spécifiée lorsque [création du service](manage-services.md#create-service). Dans la **[!UICONTROL Options supplémentaires]**, désactivez la variable **[!UICONTROL Durée de validité illimitée]** et définir une période de validité pour le service.

![](assets/service-create-validity-period.png)

Une fois la durée spécifiée expirée, tous les abonnés sont automatiquement désabonnés de ce service.

## Diffuser aux abonnés d&#39;un service

Une fois que [création d’un service d’abonnement](manage-services.md#create-service), vous pouvez cibler ses abonnés dans une diffusion. Suivez les étapes ci-dessous.

1. [Création d’une audience](../audience/create-audience.md) y compris les abonnés au service que vous avez créé :

   * Dans le **[!UICONTROL Créer une audience]** activité, afficher les attributs avancés et sélectionner **[!UICONTROL Destinataire]** > **[!UICONTROL Abonnements]** > **[!UICONTROL Service]**.

   * Dans cet exemple, sélectionnez les utilisateurs abonnés au service qui a la variable **Newsletter Luma** libellé.

   ![](assets/service-audience-subscribers.png)

1. [Créer une diffusion](../msg/gs-messages.md#create-delivery) et sélectionnez l’audience que vous avez créée ci-dessus.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Modifiez le contenu de votre message selon vos besoins et envoyez la diffusion.

   ![](assets/service-delivery-ready.png)

Votre diffusion n&#39;est envoyée qu&#39;aux abonnés de ce service.
