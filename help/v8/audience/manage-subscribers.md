---
audience: end-user
title: Gérer les personnes abonnées
description: Découvrez comment gérer les personnes abonnées à un service dans Adobe Campaign Web et leurs envoyer des diffusions.
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '359'
ht-degree: 100%

---

# Gérer les personnes abonnées {#manage-subscribers}

Après avoir [créé un service](manage-services.md#create-service), vous pouvez ajouter des personnes abonnées, désabonner des destinataires et envoyer des messages aux personnes abonnées à ce service.

La gestion des personnes abonnées est détaillée sur cette page. Pour découvrir comment envoyer des messages à vos personnes abonnées, reportez-vous à [cette section](../msg/send-to-subscribers.md).

## Ajouter des personnes abonnées à votre service {#add-subscribers}

Pour ajouter manuellement des personnes abonnées, procédez comme suit.

1. Sélectionnez un service existant dans la liste **[!UICONTROL Services d’abonnements]**.

1. Accédez à l’onglet **[!UICONTROL Personnes abonnées]** et cliquez sur **[!UICONTROL Ajouter des personnes abonnées]**.

   ![Capture d’écran affichant l’onglet Personnes abonnées dans l’interface des services d’abonnement.](assets/service-subscribers-tab.png){zoomable="yes"}

1. Sélectionnez les profils à ajouter dans la liste, puis cliquez sur **[!UICONTROL Confirmer]**.

   ![Capture d’écran affichant l’interface de sélection de profil pour ajouter des personnes abonnées.](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Envoyer]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> pour que les personnes destinataires sélectionnées reçoivent le [message de confirmation](manage-services.md#create-confirmation-message) d’abonnement que vous avez défini lors de la [création du service](manage-services.md#create-service).

   ![Capture d’écran affichant l’interface du message de confirmation pour l’ajout des personnes abonnées.](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si vous sélectionnez **[!UICONTROL Annuler]**, aucun message de confirmation n’est envoyé aux profils sélectionnés, mais ceux-ci sont quand même abonnés.

Les profils ajoutés sont affichés dans l’onglet **[!UICONTROL Personnes abonnées]**. Ils sont maintenant abonnés à votre service.

## Supprimer des personnes abonnées de votre service {#remove-subscribers}

### Désabonner manuellement des profils {#manual-unsubscription}

Une fois les [personnes abonnées ajoutées](#add-subscribers) à votre service, vous pouvez désabonner manuellement chacune d’elles. Suivez les étapes ci-dessous.

1. Sélectionnez un service existant à partir de la liste **[!UICONTROL Services d’abonnements]**.

1. Cliquez sur l’icône représentant trois points de suspension située en regard du nom de la personne destinataire, puis sélectionnez **[!UICONTROL Supprimer]**.

   ![Capture d’écran affichant l’option de suppression pour le désabonnement des profils.](assets/service-subscribers-delete.png){zoomable="yes"}

1. Confirmez la suppression.

1. Cliquez sur **[!UICONTROL Envoyer]** pour que la personne destinataire sélectionnée reçoive le [message de confirmation](manage-services.md#create-confirmation-message) de désabonnement que vous avez défini lors de la [création du service](manage-services.md#create-service).

   ![Capture d’écran affichant l’interface du message de confirmation pour le désabonnement des profils.](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

La personne destinataire est supprimée de l’onglet **[!UICONTROL Personnes abonnées]** et n’est plus abonnée à votre service.

### Désabonner automatiquement les destinataires {#automatic-unsubscription}

Un service d’abonnement peut avoir une durée limitée. Les profils sont automatiquement désabonnés à l’expiration de la période de validité.

Cette période est spécifiée lors de la [création du service](manage-services.md#create-service). Dans les **[!UICONTROL Options supplémentaires]**, désactivez l’option **[!UICONTROL Période de validité illimitée]** et définissez une période de validité pour le service.

![Capture d’écran affichant la configuration de la période de validité d’un service d’abonnement.](assets/service-create-validity-period.png){zoomable="yes"}

Une fois la durée spécifiée expirée, toutes les personnes abonnées sont automatiquement désabonnées de ce service.