---
audience: end-user
title: Rapports globaux pour le canal SMS
description: Présentation des rapports globaux pour le canal SMS
badge: label="Disponibilité limitée"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 19%

---

# Rapports globaux pour le canal SMS {#campaign-reports-sms}

Les rapports globaux offrent aux utilisateurs un aperçu complet des mesures de trafic et d’engagement au niveau des canaux.

Accédez au **[!UICONTROL Rapports]** dans le **[!UICONTROL Reporting]** . Vous pouvez filtrer vos données en fonction de la date, du dossier ou des règles du rapport. [En savoir plus](global-reports.md)

## Synthèse des diffusions {#delivery-summary-sms}

### Vue d’ensemble de la diffusion {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Vue d’ensemble de la diffusion SMS"
>abstract="La variable **Présentation de la diffusion SMS** Les IPC fournissent un résumé complet de votre diffusion SMS, offrant des informations détaillées et des données spécifiques. Il fournit des informations complètes sur les performances, l’efficacité et les résultats de votre diffusion."

La variable **[!UICONTROL Présentation de la diffusion]** Le rapport propose des indicateurs de performances clés (IPC) complets, qui fournissent des informations détaillées sur les schémas d’interaction de vos visiteurs avec chaque diffusion SMS. Les mesures suivantes sont décrites ci-dessous.

![](assets/global_report_sms_delivery_overview.png)

+++En savoir plus sur les mesures de présentation des diffusions.

* **[!UICONTROL Messages à diffuser]** : nombre total de messages traités lors de la préparation de la diffusion.

* **[!UICONTROL Délivrés]**: Pourcentage de messages envoyés avec succès, par rapport au nombre total de messages envoyés.

* **[!UICONTROL Taux de clics]**: pourcentage de destinataires distincts ayant cliqué au moins une fois dans une même diffusion.

* **[!UICONTROL Erreurs]**: Pourcentage des erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre total de messages envoyés.

+++

### Audience ciblée {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="Population ciblée par les SMS"
>abstract="Graphique et tableau pour le **Population ciblée** présenter les données relatives à votre audience SMS, y compris les informations sur les messages à diffuser et les exclusions ;"

La variable **[!UICONTROL Audience ciblée]** tableau et graphique présentant les données relatives à vos destinataires pour chaque diffusion SMS envoyée. Les mesures sont détaillées ci-dessous.

![](assets/global_report_sms_targeted_audience.png)

+++En savoir plus sur les mesures d’audience ciblées.

* **[!UICONTROL Audience ciblée]**: Nombre total de destinataires ciblés.

* **[!UICONTROL Message à diffuser]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Exclusion]**: Nombre total d&#39;adresses ignorées lors de l&#39;analyse lors de l&#39;application des règles : adresse manquante, en quarantaine, en liste bloquée, etc.

+++

### Statistiques de diffusion {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Statistiques de diffusion SMS"
>abstract="La variable **Statistiques de diffusion** Ce rapport fournit des informations complètes sur le SMS envoyé, en fournissant une ventilation de diverses mesures telles que les taux de succès, les occurrences d’erreur et l’audience mise en quarantaine. Cette présentation détaillée permet un examen approfondi des performances globales et des résultats du processus de diffusion des SMS."

La variable **[!UICONTROL Statistiques de diffusion]** Le tableau décrit le succès de chaque diffusion SMS. Les mesures sont détaillées ci-dessous.

![](assets/global_report_sms_delivery_statistics.png)

+++En savoir plus sur les mesures de statistiques de diffusion.

* **[!UICONTROL Messages totaux]**: Nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à délivrer.

* **[!UICONTROL Erreurs / Rebonds]**: Nombre total d&#39;erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre de messages à diffuser.

* **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (utilisateur ou utilisatrice inconnu(e), domaine invalide) par rapport au nombre de messages à délivrer.

  Les types d’erreur de SMS sont répertoriés dans la [documentation d’Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#sms-quarantines){target="_blank"}.

+++

### Causes d’exclusion {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Causes d&#39;exclusion des SMS"
>abstract="La variable **Causes d&#39;exclusion** Le graphique et le tableau illustrent les différentes raisons qui ont empêché les profils utilisateur de recevoir les SMS."

La variable **[!UICONTROL Causes d&#39;exclusion]** Le graphique et le tableau affichent les raisons qui ont empêché les profils utilisateur, qui ont été exclus des profils ciblés, de recevoir vos diffusions SMS.

Les types d’erreur sont répertoriés dans la section [Documentation d’Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Débit des diffusions {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Débit des diffusions par SMS"
>abstract="La variable **Débit de diffusion** Ce rapport fournit des informations détaillées sur l’efficacité du système de diffusion des messages SMS, ce qui présente un aperçu détaillé des taux de succès et d’erreur au cours d’une période spécifiée."

![](assets/global_report_sms_delivery_throughput.png)

La variable **[!UICONTROL Débit de diffusion]** Ce rapport offre des informations complètes sur l&#39;efficacité du système de diffusion des SMS, et offre un résumé détaillé des taux de succès et d&#39;erreur sur une période donnée.
