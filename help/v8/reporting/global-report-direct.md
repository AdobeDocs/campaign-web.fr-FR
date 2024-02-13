---
audience: end-user
title: Rapports globaux pour le canal courrier
description: En savoir plus sur les rapports globaux pour le canal courrier
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 98%

---

# Rapports globaux pour le canal courrier {#global-report-direct}

Les rapports globaux offrent aux utilisateurs et utilisatrices une vue d’ensemble complète des mesures de trafic et d’engagement au niveau d’un canal.

Accédez au menu **[!UICONTROL Rapports]** dans la section **[!UICONTROL Reporting]**. Vous pouvez filtrer vos données en fonction de la date, du dossier ou des règles du rapport. [En savoir plus](global-reports.md)

## Synthèse des diffusions {#delivery-summary-direct}

### Vue d’ensemble de la diffusion {#delivery-overview-direct}

La **[!UICONTROL Vue d’ensemble de la diffusion]** présente des indicateurs clés de performance (KPI) qui donnent des informations détaillées sur l’interaction de vos visiteurs et visiteuses avec chaque diffusion d’e-mail. Les mesures sont décrites ci-dessous.

![](assets/global_report_email_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++En savoir plus sur les mesures de vue d’ensemble de diffusion.

* **[!UICONTROL Messages à diffuser]** : nombre total de messages traités lors de la préparation de la diffusion.

* **[!UICONTROL Diffusés]** : nombre de messages envoyés avec succès, par rapport au nombre total de messages envoyés.

* **[!UICONTROL Erreurs]** : nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre total de messages envoyés.

* **[!UICONTROL Désabonnements]** : nombre de destinataires ayant cliqué afin de se désabonner.
+++

### Audience ciblée {#delivery-summary-direct-initial-target}

Le tableau et le graphe pour **[!UICONTROL Audience ciblée]** présentent des données relatives à vos destinataires, avec les mesures détaillées fournies ci-dessous.

![](assets/global_report_email_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++En savoir plus sur les mesures d’audience ciblée.

* **[!UICONTROL Audience ciblée]** : nombre total de destinataires ciblés.

* **[!UICONTROL Message à diffuser]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Exclusion]** : nombre d’adresses ignorées pendant l’analyse lors de l’application des règles : adresse manquante, mise en quarantaine, placée sur la liste bloquée, etc.

+++

### Statistiques de diffusion {#delivery-summary-direct-exec-stats}

Le tableau **[!UICONTROL Statistiques de diffusion]** fournit une répartition du succès de chaque diffusion courrier, avec les mesures détaillées décrites ci-dessous.

![](assets/global_report_email_delivery_statistics.png){zoomable=&quot;yes&quot;}{align="center"}

+++En savoir plus sur les mesures des statistiques de diffusion.

* **[!UICONTROL Message à diffuser]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à délivrer.

* **[!UICONTROL Erreurs/Rebonds]** : nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des rebonds par rapport au nombre de messages à diffuser.

* **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (utilisateurs et utilisatrices inconnus, domaine non valide) par rapport au nombre de messages à diffuser.

+++

### Causes d’exclusion {#causes-exclusion}

![](assets/global_report_email_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

Le graphe et le tableau Exclusions illustrent les raisons qui ont empêché des profils utilisateur et utilisatrice exclus des profils ciblés de recevoir le message.

## Débit des diffusions {#delivery-throughput}

Ce rapport fournit des détails complets sur le débit de diffusion dans un délai donné. La mesure clé utilisée pour mesurer la vitesse de diffusion des messages est le nombre de messages envoyés par heure.

## Non diffusables {#non-deliverables-direct}

### Répartition des erreurs par type {#delivery-summary-direct-breakdown-per-type}

Le tableau et le graphe **[!UICONTROL Répartition des erreurs par type]** présentent les données liées aux erreurs potentielles rencontrées dans différents domaines, avec des mesures spécifiques fournies ci-dessous.

Les erreurs présentées dans ce rapport déclenchent le processus de mise en quarantaine. Pour plus d’informations sur la gestion des quarantaines, consultez la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=fr){target="_blank"}.

+++En savoir plus sur les mesures de répartition des erreurs par type.

* **[!UICONTROL Utilisateur inconnu]** : type d’erreur générée lors de l’envoi d’une diffusion indiquant que l’adresse e-mail est non valide.

* **[!UICONTROL Domaine non valide]** : type d’erreur générée lors de l’envoi d’une diffusion indiquant que le domaine de l’adresse est erroné ou n’existe plus.

* **[!UICONTROL Boîte pleine]** : type d’erreur générée, après cinq tentatives de diffusion, indiquant que la boîte de réception de la personne destinataire contient trop de messages.

* **[!UICONTROL Compte désactivé]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que l&#39;adresse n&#39;existe plus.

* **[!UICONTROL Refusé]** : type d’erreur générée lorsqu’une adresse est refusée par le FAI (Fournisseur d’accès Internet), par exemple, suite à l’application d’une règle de sécurité (logiciel anti-spams).

* **[!UICONTROL Inatteignable]** : type d&#39;erreur survenue dans la chaîne de distribution du message : incident sur le relais SMTP, domaine temporairement inatteignable, etc.

* **[!UICONTROL Non connecté]** : type d’erreur indiquant que le téléphone portable de la personne destinataire est éteint ou n’est pas connecté au réseau au moment de l’envoi du message.

+++

### Répartition des erreurs par domaine {#delivery-summary-email-breakdown-per-domain}

Le tableau et le graphe **[!UICONTROL Répartition des erreurs par domaine]** illustrent les données liées aux erreurs potentielles dans chaque domaine. Les mesures sont communes au tableau et au graphe **[!UICONTROL Répartition des erreurs par type]** présentés ci-dessus.

