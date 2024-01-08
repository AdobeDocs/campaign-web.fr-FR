---
audience: end-user
title: Rapports globaux pour le canal push
description: Présentation des rapports globaux pour le canal push
badge: label="Disponibilité limitée"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 34%

---

# Rapports globaux pour le canal push {#campaign-reports-push}

Les rapports globaux offrent aux utilisateurs un aperçu complet des mesures de trafic et d’engagement au niveau des canaux.

Accédez au **[!UICONTROL Rapports]** dans le **[!UICONTROL Reporting]** . Vous pouvez filtrer vos données en fonction de la date, du dossier ou des règles du rapport. [En savoir plus](global-reports.md)

## Synthèse des diffusions {#delivery-summary-push}

### Vue d’ensemble de la diffusion {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Vue d’ensemble de la diffusion des notifications push"
>abstract="Push **présentation des diffusions** Les indicateurs de performance clés offrent un examen approfondi de vos diffusions push, fournissant des informations détaillées et des données spécifiques. Il fournit des détails complets sur les performances, l’efficacité et les résultats des diffusions."

La variable **[!UICONTROL Présentation de la diffusion]** Ce rapport fournit des indicateurs de performances clés (IPC) qui fournissent des informations détaillées sur la manière dont vos visiteurs interagissent avec chaque diffusion de notification push. Les mesures sont détaillées ci-dessous.

![](assets/global_report_push_delivery_overview.png)

+++En savoir plus sur les mesures de présentation des diffusions.

* **[!UICONTROL Messages à diffuser]** : nombre total de messages traités lors de la préparation de la diffusion.

* **[!UICONTROL Délivrés]** : nombre de messages envoyés avec succès, par rapport au nombre total de messages envoyés.

* **[!UICONTROL Nombre total de clics]** : nombre total de personnes destinataires distinctes ayant cliqué dans une diffusion au moins une fois.

* **[!UICONTROL Erreurs]** : nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre total de messages envoyés.

+++

### Audience ciblée {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Population ciblée des notifications push"
>abstract="La variable **Population ciblée** le graphique et le tableau présentent les données relatives à votre audience de messagerie push, avec des informations sur les messages à diffuser et les exclusions."

La variable **[!UICONTROL Audience ciblée]** tableau et graphique présentant les données relatives à vos destinataires pour chaque diffusion de notification push envoyée. Les mesures sont détaillées ci-dessous.

![](assets/global_report_push_targeted_audience.png)

+++En savoir plus sur les mesures d’audience ciblées.

* **[!UICONTROL Audience ciblée]**: Nombre total de destinataires ciblés.

* **[!UICONTROL Message à diffuser]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Exclusion]**: Nombre total d&#39;adresses ignorées lors de l&#39;analyse lors de l&#39;application des règles : adresse manquante, en quarantaine, en liste bloquée, etc.

+++

### Statistiques de diffusion {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Statistiques de diffusion push"
>abstract="La variable **Statistiques globales** Ce rapport fournit des informations sur les notifications push envoyées, notamment les taux de succès, les erreurs et les mises en quarantaine."

La variable **[!UICONTROL Statistiques de diffusion]** Le tableau décrit le succès de chaque diffusion de notification push. Les mesures sont détaillées ci-dessous.

![](assets/global_report_push_delivery_statistics.png)

+++En savoir plus sur les mesures de statistiques de diffusion.

* **[!UICONTROL Messages totaux]**: Nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à délivrer.

* **[!UICONTROL Erreurs / Rebonds]**: Nombre total d&#39;erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre de messages à diffuser.

* **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (enregistrement non valide, rejet du message, erreur de payload, par exemple), par rapport au nombre de messages à diffuser.

  Les types d’erreur de notifications push sont répertoriés dans la [documentation d’Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#push-error-types){target="_blank"}.

+++

### Causes d’exclusion {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Causes d’exclusion des notifications push"
>abstract="La variable **Causes d’exclusion** Le graphique et le tableau illustrent les différentes raisons qui ont empêché les profils utilisateur de recevoir les notifications push."

La variable **[!UICONTROL Causes d&#39;exclusion]** le graphique et le tableau affichent les raisons qui ont empêché les profils utilisateur, qui ont été exclus des profils ciblés, de recevoir le message.

Les types d’erreur de notifications push sont répertoriés dans la [documentation d’Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#push-error-types){target="_blank"}.

## Débit des diffusions (Delivery throughput)  {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Rapport de débit de diffusion"
>abstract="La variable **Débit de diffusion** le rapport présente des informations détaillées sur le débit de diffusion des notifications push de l’ensemble de la plateforme au cours d’une période spécifiée."

![](assets/global_report_push_delivery_throughput.png)

La variable **[!UICONTROL Débit de diffusion]** Ce rapport offre des informations complètes sur l’efficacité du système de diffusion des notifications push, et offre un résumé détaillé des taux de succès et d’erreur sur une période donnée.

