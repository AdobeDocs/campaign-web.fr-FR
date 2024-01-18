---
audience: end-user
title: Gestion des abonnés
description: Découvrez comment gérer les personnes abonnées à un service dans Adobe Campaign Web et leurs envoyer des diffusions.
badge: label="Disponibilité limitée"
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 08554d835175cd81f4df057ebfb7952500a12ba4
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 68%

---

# Gestion des abonnés {#manage-subscribers}

Après avoir [créé un service](manage-services.md#create-service), vous pouvez ajouter des personnes abonnées, désabonner des destinataires et envoyer des messages aux personnes abonnées à ce service.

La gestion des personnes abonnées est détaillée sur cette page. Pour découvrir comment envoyer des messages à vos personnes abonnées, reportez-vous à [cette section](../msg/send-to-subscribers.md).

## Ajouter des personnes abonnées à votre service {#add-subscribers}

Pour ajouter manuellement des personnes abonnées, procédez comme suit.

1. Sélectionnez un service existant dans la liste **[!UICONTROL Services d’abonnements]**.

1. Accédez au **[!UICONTROL Abonnés]** et cliquez sur **[!UICONTROL Ajouter des abonnés]**.

   ![](assets/service-subscribers-tab.png)

1. Sélectionnez les profils à ajouter dans la liste, puis cliquez sur **[!UICONTROL Confirmer]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Cliquez sur **[!UICONTROL Envoyer]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> pour que les destinataires sélectionnés reçoivent l’abonnement [message de confirmation](manage-services.md#create-confirmation-message) que vous avez défini lorsque [création du service](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

   >[!NOTE]
   >
   >Si vous sélectionnez **[!UICONTROL Annuler]**, aucun message de confirmation n&#39;est envoyé aux profils sélectionnés, mais ils sont abonnés.

Les profils ajoutés sont affichés dans le **[!UICONTROL Abonnés]** . Ils sont maintenant abonnés à votre service.

## Supprimer des personnes abonnées de votre service {#remove-subscribers}

### Désabonner manuellement des destinataires {#manual-unsubscription}

Une fois les [personnes abonnées ajoutées](#add-subscribers) à votre service, vous pouvez désabonner manuellement chacune d’elles. Suivez les étapes ci-dessous.

1. Sélectionnez un service existant à partir de la liste **[!UICONTROL Services d’abonnements]**.

1. Cliquez sur l’icône représentant trois points de suspension située en regard du nom de la personne souhaitée, puis sélectionnez **[!UICONTROL Supprimer]**.

   ![](assets/service-subscribers-delete.png)

1. Confirmez la suppression.

1. Cliquez sur **[!UICONTROL Envoyer]** pour que le destinataire sélectionné reçoive la désinscription [message de confirmation](manage-services.md#create-confirmation-message) que vous avez défini lorsque [création du service](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

Le destinataire est supprimé de la variable **[!UICONTROL Abonnés]** et n’est plus abonné à votre service.

### Désabonner automatiquement les destinataires {#automatic-unsubscription}

Un service d’abonnement peut avoir une durée limitée. Les personnes destinataires sont automatiquement désabonnées à l’expiration de la période de validité.

Cette période est spécifiée lors de la [création du service](manage-services.md#create-service). Dans les **[!UICONTROL Options supplémentaires]**, désactivez l’option **[!UICONTROL Période de validité illimitée]** et définissez une période de validité pour le service.

![](assets/service-create-validity-period.png)

Une fois la durée spécifiée expirée, toutes les personnes abonnées sont automatiquement désabonnées de ce service.
