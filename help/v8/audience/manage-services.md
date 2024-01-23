---
audience: end-user
title: Utiliser des services d’inscription
description: Découvrez comment accéder aux services d’abonnements, comment les créer et comment les gérer dans Adobe Campaign Web.
badge: label="Disponibilité limitée"
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: 08554d835175cd81f4df057ebfb7952500a12ba4
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 74%

---

# Créer et gérer des services d’abonnement {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Création et gestion des services"
>abstract="Utilisez Adobe Campaign pour créer et surveiller vos services, tels que les newsletters, et pour vérifier les inscriptions ou désinscriptions à ces services. Les abonnements ne s’appliquent qu’aux diffusions e-mail et SMS."

Utilisez Adobe Campaign Web pour créer et surveiller vos services tels que les newsletters, ainsi que pour vérifier les abonnements et désabonnements relatifs à ces services.

>[!NOTE]
>
>Les abonnements ne s’appliquent qu’aux diffusions e-mail et SMS.

Plusieurs services peuvent être définis en parallèle, comme les newsletters spécialisées dans certaines catégories de produits, certains thèmes ou certaines rubriques d’un site Web, les abonnements à divers types de messages d’alerte et les notifications en temps réel.

Pour en savoir plus sur la gestion des abonnements et des désabonnements, consultez la section [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html?lang=fr){target="_blank"}.

## Accès aux services d’abonnements {#access-services}

Pour accéder aux services d’abonnements disponibles pour votre plateforme, procédez comme suit.

1. Accédez au menu **[!UICONTROL Services d’abonnements]** sur le rail de navigation de gauche.

   ![](assets/service-list.png)

1. La liste de tous les services d’abonnements existants s’affiche. Vous pouvez rechercher les services et les filtrer selon le canal, le dossier ou ajouter des règles à l’aide de la variable [query modeler](../query/query-modeler-overview.md).

   ![](assets/service-filters.png)

1. Pour modifier un service existant, cliquez sur son nom.

1. Vous pouvez supprimer ou dupliquer n’importe quel service à l’aide de l’icône de trois points située en regard du nom du service.<!--so all subscribers are unsubscribed - need to mention?-->

## Créer votre premier service d’abonnement {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Définition des propriétés du service"
>abstract="Saisissez le libellé du service d’abonnement et définissez des options supplémentaires, telles qu’une période de validité pour votre service."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Sélectionner un message de confirmation"
>abstract="Lorsqu’une personne s’abonne à un service ou s’en désabonne, vous pouvez envoyer un message de confirmation. Sélectionnez les modèles à utiliser pour ce message."

Pour créer un service d’abonnement, procédez comme suit :

1. Sélectionnez le bouton **[!UICONTROL Créer un service d’abonnement]**.

   ![](assets/service-create-button.png)

1. Sélectionnez un canal : **[!UICONTROL E-mail]** ou **[!UICONTROL SMS]**.

1. Dans les propriétés du service, saisissez un libellé et définissez **[!UICONTROL Options supplémentaires]** comme voulu.

   ![](assets/service-create-properties.png)

1. Par défaut, les services sont stockés dans la variable **[!UICONTROL Services et abonnements]** dossier. Vous pouvez le modifier en accédant à l’emplacement souhaité. [Découvrez comment utiliser les dossiers](../get-started/permissions.md#folders)

1. Par défaut, les abonnements sont illimités. Vous pouvez désactiver l’option **[!UICONTROL Période de validité illimitée]** pour définir une durée de validité du service.

   Dans l’exemple ci-dessous, après 20 jours :
   * Aucun destinataire ne pourra plus s’abonner à ce service.
   * Toutes les personnes abonnées à ce service seront automatiquement désabonnées au bout de 20 jours. [En savoir plus](#automatic-unsubscription)

   ![](assets/service-create-validity-period.png)

1. Lorsqu’une personne s’abonne à un service ou s’en désabonne, vous pouvez envoyer un message de confirmation. Sélectionnez les modèles à utiliser pour ce message en fonction de votre cas d’utilisation. Ces modèles doivent être configurés avec le mapping de ciblage **[!UICONTROL Abonnements]**. [En savoir plus](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. Cliquez sur **[!UICONTROL Enregistrer et réviser]**. Le nouveau service est ajouté à la liste **[!UICONTROL Services d’abonnements]**.

Vous pouvez maintenant :

* Ajoutez des abonnés à ce service et désabonnez-vous des destinataires. [En savoir plus](../msg/send-to-subscribers.md)

* Envoyez des messages aux abonnés de ce service. [Voici comment procéder](../msg/send-to-subscribers.md).

## Créer un message de confirmation {#create-confirmation-message}

Pour envoyer des messages de confirmation aux personnes qui s’abonnent à ou se désabonnent de votre service, vous devez créer un modèle de diffusion avec le mapping de ciblage **[!UICONTROL Abonnements]**, sans cible définie. Procédez comme suit :

1. Créez un modèle de diffusion pour la confirmation d’abonnement. [Découvrez comment créer un modèle](../msg/delivery-template.md)

1. Ne sélectionnez pas d’audience pour cette diffusion. Au lieu de cela, accédez à la diffusion **[!UICONTROL Paramètres]**, accédez au [Audience](../advanced-settings/delivery-settings.md#audience) et sélectionnez l’option **[!UICONTROL Abonnements]** mapping de ciblage de la liste.

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >Si vous ne sélectionnez pas le mapping de ciblage **[!UICONTROL Abonnements]**, vos personnes abonnées ne recevront pas le message de confirmation. Les mappings de ciblage sont définis dans la console Campaign v8. En savoir plus dans la section [Documentation d’Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr){target="_blank"}.

1. Modifiez le contenu de votre modèle de diffusion, enregistrez-le et fermez-le.

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >En savoir plus sur les canaux de diffusion et la définition d’un contenu de diffusion dans les sections [Canal e-mail](../email/create-email.md) et [Canal SMS](../sms/create-sms.md).

1. Répétez les étapes ci-dessus pour créer un modèle de diffusion pour la confirmation de désinscription.

Vous pouvez maintenant sélectionner ces messages lors de la [création d’un service d’abonnement](#create-service). Les utilisateurs et utilisatrices qui se sont abonnés ou désabonnés à ce service recevront les messages de confirmation sélectionnés.

## Surveiller vos services d’abonnement {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Nombre total de personnes abonnées"
>abstract="Cliquez sur **Calculer** obtenez le nombre total d’abonnés pour ce service."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Nombre d&#39;abonnements sur la période"
>abstract="Utilisez la liste déroulante pour modifier la période et visualiser le nombre d&#39;abonnements et de désabonnements sur la période sélectionnée."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Évolution globale des abonnements"
>abstract="Ce graphique présente la répartition par période, y compris les abonnements, les désabonnements, l’évolution en nombre et le pourcentage de fidélité."

Pour mesurer l’efficacité de vos services d’abonnement pour les canaux SMS et e-mail, vous pouvez accéder aux journaux et aux rapports d’un service donné.

1. Sélectionnez un service existant dans la liste **[!UICONTROL Services d’abonnements]**. Cliquez sur **[!UICONTROL Calculer]** obtenez le nombre total d’abonnés.

   ![](assets/service-logs-subscribers-count.png)

1. Dans le tableau de bord du service, sélectionnez **[!UICONTROL Journaux]** pour visualiser la liste des abonnés à ce service.

   Vous pouvez vérifier le nombre total d&#39;abonnés, le nom et l&#39;adresse de chaque destinataire, ainsi que le moment où il s&#39;est abonné ou s&#39;est désabonné. Vous pouvez également les filtrer.

   ![](assets/service-logs.png)

1. Dans le tableau de bord du service, sélectionnez **[!UICONTROL Rapports]**. Vérifiez les indicateurs suivants :

   * Le **[!UICONTROL nombre total de personnes abonnées]** s’affiche.

   * Vous pouvez visualiser le nombre d’abonnements et de désabonnements sur une période sélectionnée. Utilisez la liste déroulante pour modifier la période.

     ![](assets/service-reports.png)

   * Le graphe **[!UICONTROL Évolution globale des abonnements]** affiche la répartition par période, y compris les abonnements, les désabonnements, l’évolution en nombre et le pourcentage de fidélité.<!--what is Registered?-->

1. Utilisez le bouton **[!UICONTROL Recharger]** pour récupérer les dernières valeurs de l’exécution et du planning du workflow de tracking.
