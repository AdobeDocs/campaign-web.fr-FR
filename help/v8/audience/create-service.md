---
audience: end-user
title: Utilisation des services d’abonnement
description: Découvrez comment créer des services dans Adobe Campaign Web
badge: label="Beta"
source-git-commit: dd8e8acb37cf9a68768c5da48335275c09d67cc8
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# Utilisation des services d’abonnement {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Créer et gérer vos services"
>abstract="Utilisez Adobe Campaign pour créer et surveiller vos services, tels que les newsletters, et pour vérifier les abonnements/désabonnements à ces services. Les abonnements ne s&#39;appliquent qu&#39;aux diffusions email et SMS."

Utilisez le web Adobe Campaign pour gérer et créer vos services, tels que les newsletters, et pour vérifier les abonnements/désabonnements à ces services.

>[!NOTE]
>
>Les abonnements ne s&#39;appliquent qu&#39;aux diffusions email et SMS.

Plusieurs services peuvent être définis en parallèle, par exemple : newsletters pour des catégories de produits spécifiques, des thèmes ou des zones d’un site web, abonnements à différents types de messages d’alerte et notifications en temps réel.

Pour en savoir plus sur la gestion des abonnements et des désabonnements, consultez la section [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Accès aux services d’abonnement {#access-services}

Pour accéder aux services d’abonnement disponibles pour votre plateforme, accédez au **[!UICONTROL Services d’inscriptions]** sur le rail de navigation de gauche.

![](assets/service-list.png)

La liste de tous les services d&#39;abonnement existants s&#39;affiche. Vous pouvez effectuer des recherches dans les services et filtrer par canal, par dossier ou utiliser des filtres avancés.

![](assets/service-filters.png)

Pour modifier un service existant, cliquez sur son nom.

## Créer votre premier service d’abonnement {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Propriétés du service Abonnements"
>abstract="Saisissez le libellé du service d&#39;abonnement et définissez des options supplémentaires."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Messages de confirmation du service d’inscriptions"
>abstract="Lorsqu&#39;un utilisateur s&#39;abonne à un service ou se désabonne d&#39;un service, vous pouvez envoyer un message de confirmation. Sélectionnez les modèles à utiliser pour ces messages."


Pour créer un service d&#39;abonnement, procédez comme suit :

1. Sélectionnez la variable **[!UICONTROL Créer un service d’abonnement]** bouton .

   ![](assets/service-create-button.png)

1. Sélectionnez un canal : **[!UICONTROL Email]** ou **[!UICONTROL SMS]**.

1. Dans les propriétés du service, saisissez un libellé et définissez les options supplémentaires de votre choix.

   ![](assets/service-create-properties.png)

1. Par défaut, les abonnements sont illimités. Vous pouvez désactiver la variable **[!UICONTROL Durée de validité illimitée]** pour définir une durée de validité du service. <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. Lorsqu&#39;un utilisateur s&#39;abonne à un service ou s&#39;en désabonne, vous pouvez envoyer un message de confirmation. Sélectionnez les modèles à utiliser pour ce message en fonction de votre cas d’utilisation.

   ![](assets/service-create-confirmation-msg.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**. Le nouveau service est ajouté à la variable **[!UICONTROL Services d’inscriptions]** liste.

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


