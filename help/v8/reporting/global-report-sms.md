---
audience: end-user
title: Rapports globaux pour le canal SMS
description: Présentation des rapports globaux pour le canal SMS
badge: label="Disponibilité limitée"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 26%

---

# Rapports globaux pour le canal SMS {#campaign-reports-sms}

Les rapports globaux offrent aux utilisateurs un aperçu complet des mesures de trafic et d’engagement au niveau des canaux.

Accédez au **[!UICONTROL Rapports]** dans le **[!UICONTROL Reporting]** . Vous pouvez filtrer vos données en fonction de la date, du dossier ou des règles du rapport. [En savoir plus](global-reports.md)

## Synthèse des diffusions {#delivery-summary-sms}

### Vue d’ensemble de la diffusion {#delivery-overview-sms}

La variable **[!UICONTROL Présentation de la diffusion]** Le rapport propose des indicateurs de performances clés (IPC) complets, qui fournissent des informations détaillées sur les schémas d’interaction de vos visiteurs avec chaque diffusion SMS. Les mesures suivantes sont décrites ci-dessous.

![](assets/global_report_sms_delivery_overview.png)

+++En savoir plus sur les mesures de présentation des diffusions.

* **[!UICONTROL Messages à diffuser]** : nombre total de messages traités lors de la préparation de la diffusion.

* **[!UICONTROL Délivrés]**: Pourcentage de messages envoyés avec succès, par rapport au nombre total de messages envoyés.

* **[!UICONTROL Taux de clics]**: pourcentage de destinataires distincts ayant cliqué au moins une fois dans une même diffusion.

* **[!UICONTROL Erreurs]**: Pourcentage des erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre total de messages envoyés.

+++

### Audience ciblée {#delivery-summary-sms-initial-target}

La variable **[!UICONTROL Audience ciblée]** tableau et graphique présentant les données relatives à vos destinataires pour chaque diffusion SMS envoyée. Les mesures sont détaillées ci-dessous.

![](assets/global_report_sms_targeted_audience.png)

+++En savoir plus sur les mesures d’audience ciblées.

* **[!UICONTROL Audience ciblée]**: Nombre total de destinataires ciblés.

* **[!UICONTROL Message à diffuser]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Exclusion]**: Nombre total d&#39;adresses ignorées lors de l&#39;analyse lors de l&#39;application des règles : adresse manquante, en quarantaine, en liste bloquée, etc.

+++

### Statistiques de diffusion {#delivery-summary-sms-exec-stats}

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

La variable **[!UICONTROL Causes d&#39;exclusion]** Le graphique et le tableau affichent les raisons qui ont empêché les profils utilisateur, qui ont été exclus des profils ciblés, de recevoir vos diffusions SMS.

Les types d’erreur sont répertoriés dans la section [Documentation d’Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Débit des diffusions (Delivery throughput)  {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

Ce rapport fournit des détails complets sur le débit de diffusion au cours d’une période spécifiée.
