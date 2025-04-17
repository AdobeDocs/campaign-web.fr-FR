---
audience: end-user
title: Rapports globaux du canal de notification push
description: Comprendre les rapports globaux du canal de notification push
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 63%

---

# Rapports globaux du canal de notification push {#campaign-reports-push}

Les rapports globaux offrent aux utilisateurs une vue d’ensemble complète des mesures de trafic et d’engagement au niveau du canal.

Accédez au menu **[!UICONTROL Rapports]** dans la section **[!UICONTROL Reporting]**. Vous pouvez filtrer vos données en fonction de la date du rapport, du dossier ou des règles. [En savoir plus](global-reports.md)

## Synthèse des diffusions {#delivery-summary-push}

### Vue d’ensemble de la diffusion {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Vue d’ensemble de la diffusion des notifications push"
>abstract="Les KPI de la **Vue d’ensemble de la diffusion** des notifications push offrent un examen approfondi de vos diffusions push, en vous présentant des informations détaillées et des données ciblées. Les performances, l’efficacité et les résultats des diffusions sont scrutés à la loupe."

Le rapport **[!UICONTROL Vue d’ensemble de la diffusion]** fournit des KPI (indicateurs clés de performance) qui illustrent l’engagement de vos visiteurs et de vos visiteuses par rapport à chaque diffusion de notification push. Les mesures sont détaillées ci-dessous.

![Mesures de présentation de la diffusion, affichant les KPI liés aux performances des notifications push.](assets/global_report_push_delivery_overview.png){zoomable="yes"}

+++En savoir plus sur les mesures de présentation des diffusions.

* **[!UICONTROL Messages à diffuser]** : nombre total de messages traités lors de la préparation de la diffusion.

* **[!UICONTROL Diffusés]** : nombre de messages envoyés avec succès, par rapport au nombre total de messages envoyés.

* **[!UICONTROL Nombre total de clics]** : nombre total de destinataires distincts ayant cliqué dans une diffusion au moins une fois.

* **[!UICONTROL Erreurs]** : nombre total d’erreurs accumulées lors des diffusions et du traitement automatique des retours par rapport au nombre total de messages envoyés.

+++

### Audience ciblée {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Population ciblée des notifications push"
>abstract="Le tableau et le graphe **Population ciblée** affichent des données relatives à votre audience de messages push, notamment les messages à diffuser et les exclusions."

Le tableau et le graphe **[!UICONTROL Audience ciblée]** présentent les données relatives à vos destinataires pour chaque diffusion de notification push envoyée. Les mesures sont détaillées ci-dessous.

![Mesures d’audience ciblée, affichant les données relatives aux destinataires et aux exclusions des notifications push.](assets/global_report_push_targeted_audience.png){zoomable="yes"}

+++En savoir plus sur les mesures d’audience ciblée.

* **[!UICONTROL Audience ciblée]** : nombre total de destinataires ciblés.

* **[!UICONTROL Message à diffuser]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Exclusion]** : nombre total d’adresses ignorées pendant l’analyse lors de l’application des règles : adresse manquante, mise en quarantaine, en cas de place sur la liste bloquée et pour des raisons similaires.

+++

### Statistiques de diffusion {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Statistiques de diffusion push"
>abstract="Le rapport **Statistiques globales** fournit des informations sur les notifications push envoyées, notamment le taux de succès, les erreurs et les mises en quarantaine."

Le tableau **[!UICONTROL Statistiques de diffusion]** renseigne sur le succès des diffusions de notifications push. Les mesures sont détaillées ci-dessous.

![Mesures des statistiques de diffusion, affichant les taux de succès, les erreurs et les mises en quarantaine pour les notifications push.](assets/global_report_push_delivery_statistics.png){zoomable="yes"}

+++En savoir plus sur les mesures des statistiques de diffusion.

* **[!UICONTROL Nombre total de messages]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à diffuser.

* **[!UICONTROL Erreurs / Bounces]** : nombre total d’erreurs accumulées lors des diffusions et du traitement automatique des retours par rapport au nombre de messages à diffuser.

* **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (enregistrement non valide, rejet de message, erreur de payload et raisons similaires) par rapport au nombre de messages à diffuser.

  Les types d’erreur des notifications push sont répertoriés dans la documentation d’[Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#push-error-types){target="_blank"}.

+++

### Causes d’exclusion {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Causes d’exclusion des notifications push"
>abstract="Le graphe et le tableau **Causes d’exclusion** renseignent sur les différentes raisons pour lesquelles les profils utilisateur n’ont pas reçu les notifications push."

Le graphe et le tableau **[!UICONTROL Causes d’exclusion]** illustrent les raisons pour lesquelles les profils utilisateur exclus des profils ciblés n’ont pas reçu le message.

Les types d’erreur des notifications push sont répertoriés dans la documentation d’[Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#push-error-types){target="_blank"}.

## Débit de diffusion {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Rapport de débit de diffusion"
>abstract="Le rapport **Débit de diffusion** présente des informations détaillées sur le débit de diffusion de la notification push de l’ensemble de la plateforme dans un délai donné."

![Mesures de débit des diffusions, affichant les taux de succès et d’erreur pour les notifications push sur une période spécifiée.](assets/global_report_push_delivery_throughput.png){zoomable="yes"}

Le rapport **[!UICONTROL Débit de diffusion]** offre des informations complètes sur l’efficacité du système de diffusion des notifications push, ainsi qu’un résumé détaillé des taux de réussite et d’erreur sur une période donnée.