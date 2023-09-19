---
audience: end-user
title: Utilisation des services d’abonnement
description: Découvrez comment créer et gérer des services dans Adobe Campaign Web
badge: label="Beta"
source-git-commit: 7a8057a0d57b28092711ca2d7f47fffefdc06df3
workflow-type: tm+mt
source-wordcount: '1099'
ht-degree: 2%

---


# Utilisation des services d’abonnement {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Créer et gérer vos services"
>abstract="Utilisez Adobe Campaign pour créer et surveiller vos services, tels que les newsletters, et pour vérifier les abonnements ou désabonnements à ces services. Les abonnements ne s&#39;appliquent qu&#39;aux diffusions email et SMS."

Utilisez le web Adobe Campaign pour gérer et créer vos services tels que les newsletters, et pour vérifier les abonnements ou désabonnements à ces services.

>[!NOTE]
>
>Les abonnements ne s&#39;appliquent qu&#39;aux diffusions email et SMS.

Plusieurs services peuvent être définis en parallèle, par exemple : newsletters pour des catégories de produits spécifiques, des thèmes ou des zones d’un site web, abonnements à différents types de messages d’alerte et notifications en temps réel.

Pour en savoir plus sur la gestion des abonnements et des désabonnements, consultez la section [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Accès aux services d’abonnement {#access-services}

Pour accéder aux services d&#39;abonnement disponibles pour votre plateforme, procédez comme suit.

1. Accédez au **[!UICONTROL Services d’inscriptions]** sur le rail de navigation de gauche.

   ![](assets/service-list.png)

1. La liste de tous les services d&#39;abonnement existants s&#39;affiche. Vous pouvez effectuer des recherches dans les services et filtrer par canal, par dossier ou utiliser des filtres avancés.

   ![](assets/service-filters.png)

1. Pour modifier un service existant, cliquez sur son nom.

1. Vous pouvez supprimer ou dupliquer n’importe quel service à l’aide de l’icône de trois points située en regard de ce nom de service.<!--so all subscribers are unsuibscribed - need to mention?-->

## Créer votre premier service d’abonnement {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Définition des propriétés du service"
>abstract="Saisissez le libellé du service d&#39;abonnement et définissez des options supplémentaires, telles qu&#39;une période de validité pour votre service."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Sélectionner un message de confirmation"
>abstract="Lorsqu&#39;un utilisateur s&#39;abonne à un service ou s&#39;en désabonne, vous pouvez envoyer un message de confirmation. Sélectionnez les modèles à utiliser pour ce message."

Pour créer un service d&#39;abonnement, procédez comme suit.

1. Sélectionnez la variable **[!UICONTROL Créer un service d’abonnement]** bouton .

   ![](assets/service-create-button.png)

1. Sélectionnez un canal : **[!UICONTROL Email]** ou **[!UICONTROL SMS]**.

1. Dans les propriétés du service, saisissez un libellé et définissez les options supplémentaires de votre choix.

   ![](assets/service-create-properties.png)

1. Par défaut, les abonnements sont illimités. Vous pouvez désactiver la variable **[!UICONTROL Durée de validité illimitée]** pour définir une durée de validité du service.

   Dans l’exemple ci-dessous, après 20 jours :
   * Aucun destinataire ne pourra plus s&#39;abonner à ce service.
   * Tous les abonnés à ce service seront automatiquement désabonnés au bout de 20 jours. [En savoir plus](#automatic-unsubscription)

   ![](assets/service-create-validity-period.png)

1. Lorsqu&#39;un utilisateur s&#39;abonne à un service ou s&#39;en désabonne, vous pouvez envoyer un message de confirmation. Sélectionnez les modèles à utiliser pour ce message en fonction de votre cas d’utilisation. Ces modèles doivent être configurés avec la variable **[!UICONTROL Abonnements]** mapping de ciblage. [En savoir plus](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. Cliquez sur **[!UICONTROL Enregistrement et révision]**. Le nouveau service est ajouté à la variable **[!UICONTROL Services d’inscriptions]** liste.

## Créer un message de confirmation {#create-confirmation-message}

Pour envoyer des messages de confirmation aux utilisateurs qui s&#39;abonnent ou se désabonnent de votre service, vous devez créer un modèle de diffusion avec la fonction **[!UICONTROL Abonnements]** mapping de ciblage, sans cible définie. Procédez comme suit :

1. Créez un modèle de diffusion pour la confirmation d&#39;inscription. [Voici comment procéder](../msg/delivery-template.md).

1. Ne sélectionnez pas d&#39;audience pour cette diffusion. À la place, accédez au **[!UICONTROL Paramètres de diffusion]**, accédez au [Audience](../advanced-settings/delivery-settings.md#audience) et sélectionnez l’option **[!UICONTROL Abonnements]** mapping de ciblage de la liste.

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >Si vous ne sélectionnez pas l’option  **[!UICONTROL Abonnements]** mapping de ciblage, vos abonnés ne recevront pas le message de confirmation. Les mappings de ciblage sont définis dans la console  Campaign v8. En savoir plus [Documentation d’Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr){target="_blank"}.

1. Editez le contenu de votre modèle de diffusion, enregistrez-le et fermez-le.

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >En savoir plus sur les canaux de diffusion et la définition d’un contenu de diffusion dans la section [Canal email](../email/create-email.md) et [Canal SMS](../sms/create-sms.md) sections.

1. Répétez les étapes ci-dessus pour créer un modèle de diffusion pour la confirmation de désinscription.

Vous pouvez maintenant sélectionner ces messages lorsque [création d’un service d’abonnement](#create-service). Les utilisateurs qui s’abonnent ou se désabonnent de ce service recevront les messages de confirmation sélectionnés.

## Ajouter des abonnés à votre service {#add-subscribers}

Une fois que vous avez créé un service, vous pouvez ajouter manuellement des abonnés. Suivez les étapes ci-dessous.

1. Sélectionnez un service existant à partir de la fonction **[!UICONTROL Services d’inscriptions]** liste.

1. Sélectionnez la variable **[!UICONTROL Abonnés]** et cliquez sur **[!UICONTROL Ajout de profils]**.

   ![](assets/service-subscribers-tab.png)

1. Sélectionnez les profils à ajouter dans la liste, puis cliquez sur **[!UICONTROL Confirmer]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Cliquez sur **[!UICONTROL Envoyer]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> Les destinataires sélectionnés recevront l&#39;abonnement. [message de confirmation](#create-confirmation-message) que vous avez sélectionné lorsque [création du service](#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

Les profils ajoutés sont affichés dans le **[!UICONTROL Abonnés]** liste. Ils sont maintenant abonnés à votre service.

## Supprimer des abonnés de votre service {#remove-subscribers}

### Désabonner manuellement les destinataires {#manual-unsubscription}

Une fois que vous avez ajouté des abonnés à votre service, vous pouvez les désabonner manuellement. Suivez les étapes ci-dessous.

1. Sélectionnez un service existant à partir de la fonction **[!UICONTROL Services d’inscriptions]** liste.

1. Cliquez sur l’icône de trois points située en regard du nom du destinataire souhaité, puis sélectionnez **[!UICONTROL Supprimer]**.

   ![](assets/service-subscribers-delete.png)

1. Confirmez la suppression et cliquez sur **[!UICONTROL Envoyer]**. Le destinataire sélectionné recevra la désinscription. [message de confirmation](#create-confirmation-message) que vous avez sélectionné lorsque [création du service](#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

Le destinataire est supprimé de la variable **[!UICONTROL Abonnés]** et n’est plus abonné à votre service.

### Désabonner automatiquement les destinataires {#automatic-unsubscription}

Un service d’abonnement peut avoir une durée limitée. Les destinataires sont automatiquement désabonnés à l&#39;expiration de la période de validité.

Cette période est spécifiée lorsque [création du service](#create-service). Dans la **[!UICONTROL Options supplémentaires]**, désactivez la variable **[!UICONTROL Durée de validité illimitée]** et définir une période de validité pour le service.

![](assets/service-create-validity-period.png)

Une fois la durée spécifiée expirée, tous les abonnés sont automatiquement désabonnés de ce service.

## Journaux et rapports du service d’abonnement {#logs-and-reports}

Pour mesurer l’efficacité de vos services d’abonnement pour les canaux SMS et email, vous pouvez accéder aux logs et aux rapports d’un service donné.

1. Sélectionnez un service existant à partir de la fonction **[!UICONTROL Services d’inscriptions]** liste. Cliquez sur **[!UICONTROL Calculer]** obtenez le nombre total d’abonnés.

   ![](assets/service-logs-reports-buttons.png)

1. Dans le tableau de bord du service, sélectionnez **[!UICONTROL Journaux]** pour visualiser la liste des abonnés à ce service. Vous pouvez vérifier le nombre total d&#39;abonnés, le nom et l&#39;adresse de chaque destinataire et le moment où il s&#39;est abonné ou s&#39;est désabonné. Vous pouvez également les filtrer.

   ![](assets/service-logs.png)

1. Dans le tableau de bord du service, sélectionnez **[!UICONTROL Rapports]**. Vérifiez les indicateurs suivants :

   * La variable **[!UICONTROL Nombre total d&#39;abonnés]** s’affiche.

   * Vous pouvez visualiser le nombre d&#39;abonnements et de désabonnements sur une période sélectionnée. Utilisez la liste déroulante pour modifier la période.

     ![](assets/service-reports.png)

   * La variable **[!UICONTROL Evolution globale des inscriptions]** Le graphique présente la répartition par période, y compris les abonnements, les désabonnements, l’évolution en nombre et le pourcentage de fidélité.<!--what is Registered?-->

1. Utilisez la variable **[!UICONTROL Recharger]** pour récupérer les dernières valeurs de l&#39;exécution et du planning du workflow de tracking.

## Diffuser aux abonnés d&#39;un service

Une fois que [création d’un service d’abonnement](#create-service), vous pouvez cibler ses abonnés dans une diffusion. Suivez les étapes ci-dessous.

1. [Création d’une audience](../audience/create-audience.md) y compris les abonnés au service que vous avez créé :

   * Dans le **[!UICONTROL Créer une audience]** activité, afficher les attributs avancés et sélectionner **[!UICONTROL Destinataire]** > **[!UICONTROL Abonnements]** > **[!UICONTROL Service]**.

   * Dans cet exemple, sélectionnez les utilisateurs abonnés au service qui a la variable **Newsletter Luma** libellé.

   ![](assets/service-audience-subscribers.png)

1. [Créer une diffusion](../msg/gs-messages.md) et sélectionnez l’audience que vous avez créée ci-dessus.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Modifiez le contenu de votre message selon vos besoins et envoyez la diffusion.

   ![](assets/service-delivery-ready.png)

Votre diffusion n&#39;est envoyée qu&#39;aux abonnés de ce service.







