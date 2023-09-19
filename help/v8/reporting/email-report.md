---
audience: end-user
title: Rapports de diffusion par e-mail
description: Découvrez comment accéder aux rapports de diffusion par e-mail et les utiliser.
badge: label="Beta"
source-git-commit: c8bce23d78960fcc5c9adbb37d376d60319d8df9
workflow-type: tm+mt
source-wordcount: '1890'
ht-degree: 68%

---

# Rapport de diffusion par e-mail {#email-report}

Le **rapport de diffusion par e-mail** offre des informations et des données complètes spécifiques au canal e-mail. Il fournit des informations détaillées sur les performances, l’efficacité et les résultats de vos diffusions individuelles, ce qui vous permet d’obtenir une vue d’ensemble complète.

## Synthèse des diffusions {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Envoi des rapports"
>abstract="he **Envoi** Cet onglet de votre rapport fournit des informations détaillées sur les interactions de vos visiteurs avec vos diffusions et sur les erreurs potentielles qu’ils ont pu rencontrer."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Widget de population cible initiale"
>abstract="La variable **Population cible initiale** Le graphique affiche les données relatives à vos destinataires et le succès de votre diffusion."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Widget de statistiques de diffusion"
>abstract="La variable **Statistiques de diffusion** Le graphique décrit le succès de votre diffusion et les erreurs qui se sont produites."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Widget de statistiques de diffusion"
>abstract="Le graphique et tableau Causes d&#39;exclusion présente la répartition, par règle, des messages rejetés lors de la préparation."

* **[!UICONTROL Population cible initiale]** Le graphique affiche les données relatives à vos destinataires :

  ![](assets/reporting_email_1.png){align="left" zoomable="yes"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Audience initiale]** : nombre total de destinataires ciblé(e)s.

   * **[!UICONTROL A envoyer]**: Nombre total de messages à diffuser après la préparation de la diffusion.

   * **[!UICONTROL Exclusion]** : nombre total de messages exclus de la cible envoyés.
+++

* **[!UICONTROL Statistiques de diffusion]** Le graphique décrit le succès de votre diffusion.

  ![](assets/reporting_email_2.png){align="left"}

  +++En savoir plus sur les mesures des rapports de campagne par e-mail.

   * **[!UICONTROL Message envoyé]**: Nombre total de messages à diffuser après la préparation de la diffusion.

   * **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à diffuser.

   * **[!UICONTROL Erreurs]** : nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre de messages à diffuser.

   * **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (utilisateur ou utilisatrice inconnu(e), domaine non valide) par rapport au nombre de messages à diffuser.

+++

* Le tableau et le graphe des **[!UICONTROL causes d’exclusion]** affichent la répartition par règle des messages rejetés lors de l’analyse.

  ![](assets/reporting_email_3.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Utilisateur inconnu]** : type d’erreur générée lors de l’envoi d’une diffusion indiquant que l’adresse e-mail n’est pas valide.

   * **[!UICONTROL Domaine invalide]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que le domaine de l&#39;adresse e-mail est erroné ou n&#39;existe plus.

   * **[!UICONTROL Boîte pleine]**: Type d&#39;erreur généré après cinq tentatives de diffusion pour indiquer que la boîte de réception du destinataire contient trop de messages.

   * **[!UICONTROL Compte désactivé]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que l&#39;adresse n&#39;existe plus.

   * **[!UICONTROL Refusé]** : type d’erreur générée lorsqu’une adresse est refusée par le FAI (Fournisseur d’accès Internet), par exemple, suite à l’application d’une règle de sécurité (logiciel anti-spams).

   * **[!UICONTROL Inatteignable]** : type d&#39;erreur survenue dans la chaîne de distribution du message : incident sur le relais SMTP, domaine temporairement inatteignable, etc.

   * **[!UICONTROL Non connecté]** : Type d&#39;erreur indiquant que le téléphone portable du destinataire est éteint ou n&#39;est pas connecté au réseau au moment de l&#39;envoi du message.

+++

## Débit des diffusions (Delivery throughput) {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Débit des diffusions (Delivery throughput) widget"
>abstract="La variable **Débit de diffusion** le rapport présente des informations détaillées sur le débit de diffusion de l’ensemble de la plateforme au cours d’une période spécifiée."

Ce rapport présente des informations détaillées sur le débit de diffusion de l’ensemble de la plateforme au cours d’une période donnée. La mesure principale utilisée pour mesurer la vitesse de diffusion des messages est le nombre de messages envoyés par heure.

## Statistiques de diffusion {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Widget de statistiques de diffusion"
>abstract="La variable **Statistiques de diffusion** contient les données disponibles pour les erreurs possibles rencontrées pour chaque domaine."

* Le tableau **[!UICONTROL Statistiques de diffusion]** contient les données disponibles liées aux erreurs possibles rencontrées pour chaque domaine.

  ![](assets/reporting_email_4.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL E-mails traités]** : nombre total de messages traités par le serveur de diffusion.

   * **[!UICONTROL Diffusés]** : pourcentage du nombre de messages traités avec succès, par rapport au nombre total de messages traités.

   * **[!UICONTROL Hard bounces]**: Pourcentage du nombre de &quot;hard&quot; bounces, d&#39;erreurs permanentes, telles qu&#39;une mauvaise adresse email, par rapport au nombre total de messages traités.

   * **[!UICONTROL Soft bounces]**: pourcentage du nombre de soft bounces, des erreurs temporaires telles qu&#39;une boîte de réception pleine, par rapport au nombre total de messages traités

   * **[!UICONTROL Ouvertures]** : pourcentage du nombre de destinataires ciblé(e)s ayant ouvert un message au moins une fois, par rapport au nombre de messages traités avec succès.

   * **[!UICONTROL Clics]** : pourcentage du nombre de personnes ayant cliqué au moins une fois dans une diffusion, par rapport au nombre de messages traités avec succès.

   * **[!UICONTROL Désinscriptions]** : pourcentage du nombre de clics effectués sur un lien de désinscription, par rapport au nombre de messages traités avec succès.
+++

## Échecs et bounces {#non-deliverables-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Ventilation des erreurs par type de widget"
>abstract="La variable **Ventilation des erreurs par type** le tableau et le graphique contiennent les données disponibles pour chaque type d’erreur rencontré."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Ventilation des erreurs par widget de domaine"
>abstract="La variable **Ventilation des erreurs par domaine** le tableau et le graphique contiennent les données disponibles pour chaque type d’erreur rencontré en fonction de chaque domaine."

* Les tableaux et graphes **[!UICONTROL Répartition des erreurs par type]** et **[!UICONTROL Répartition des erreurs par domaine]** contiennent les données disponibles pour les erreurs possibles rencontrées pour chaque domaine.

  Les erreurs présentées dans ce rapport déclenchent le processus de mise en quarantaine. Pour plus d’informations sur la gestion des quarantaines, consultez la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=fr){target="_blank"}.

  ![](assets/campaign_report_email_6.png)

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Utilisateur inconnu]** : type d’erreur générée lors de l’envoi d’une diffusion indiquant que l’adresse e-mail n’est pas valide.

   * **[!UICONTROL Domaine invalide]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que le domaine de l&#39;adresse e-mail est erroné ou n&#39;existe plus.

   * **[!UICONTROL Boîte pleine]**: Type d&#39;erreur généré après cinq tentatives de diffusion pour indiquer que la boîte de réception du destinataire contient trop de messages.

   * **[!UICONTROL Compte désactivé]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que l&#39;adresse n&#39;existe plus.

   * **[!UICONTROL Refusé]** : type d’erreur générée lorsqu’une adresse est refusée par le FAI (Fournisseur d’accès Internet), par exemple, suite à l’application d’une règle de sécurité (logiciel anti-spams).

   * **[!UICONTROL Inatteignable]** : type d&#39;erreur survenue dans la chaîne de distribution du message : incident sur le relais SMTP, domaine temporairement inatteignable, etc.

   * **[!UICONTROL Non connecté]** : Type d&#39;erreur indiquant que le téléphone portable du destinataire est éteint ou n&#39;est pas connecté au réseau au moment de l&#39;envoi du message.

+++

## Indicateurs de tracking {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Tracking des rapports"
>abstract="La variable **Tracking** dans votre rapport, cet onglet contient des données importantes, notamment le comportement des destinataires par lien, la répartition des ouvertures et des clics, ainsi que des informations détaillées sur les URL ayant reçu le plus de clics lors d&#39;une diffusion."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Widget de statistiques de diffusion"
>abstract="La variable **Statistiques de diffusion** fournit des indicateurs de performances clés (IPC) qui fournissent des informations détaillées sur les données disponibles pour les emails envoyés."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Widget de taux d’ouverture et de clic"
>abstract="La variable **Taux d&#39;ouverture et de clic** Le tableau affiche les données relatives à l’engagement de vos destinataires avec votre diffusion."

* Les **[!UICONTROL statistiques de diffusion]** fournissent des indicateurs clés de performances (KPI) qui donnent des informations détaillées sur les données disponibles pour les e-mails envoyés.

  ![](assets/reporting_email_5.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à diffuser.

   * **[!UICONTROL Ouvertures distinctes]** : nombre total de destinataires ciblé(e)s ayant ouvert un message au moins une fois.

   * **[!UICONTROL Ouvertures]** : nombre de destinataires ciblé(e)s distinct(e)s pour ce domaine ayant ouvert un message au moins une fois.

   * **[!UICONTROL Clics sur le lien d’exclusion]** : nombre de clics effectués sur le lien d’exclusion.

   * **[!UICONTROL Clics sur le lien miroir]** : nombre de clics sur le lien vers la page miroir.

   * **[!UICONTROL Estimation des transferts]** : estimation du nombre d’e-mails transférés par les destinataires ciblé(e)s.
+++

* Le tableau **[!UICONTROL Taux d’ouverture et de clic publicitaire]** affiche des données relatives à vos destinataires.

  ![](assets/reporting_email_6.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Envoyés]** : nombre total de messages envoyés.

   * **[!UICONTROL Plaintes]** : nombre de messages pour ce domaine qui ont été signalés par le ou la destinataire comme indésirables.

   * **[!UICONTROL Ouvertures]** : nombre de destinataires ciblé(e)s distinct(e)s, pour ce domaine, ayant ouvert un message au moins une fois.

   * **[!UICONTROL Clics]** : nombre de destinataires ciblé(e)s distinct(e)s ayant cliqué au moins une fois dans une même diffusion.

   * **[!UICONTROL Réactivité brute]** : pourcentage du nombre de destinataires ayant cliqué au moins une fois dans une même diffusion par rapport au nombre de destinataires ayant ouvert au moins une fois une même diffusion.
+++

## URL et flux de clics {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL et flux de clics (URLs and click streams) widget"
>abstract="La variable **URL et flux de clics** fournit des indicateurs de performances clés (IPC) qui fournissent des informations détaillées sur les URL qui ont reçu le plus grand nombre de clics lors d’une diffusion."

* Les **[!UICONTROL URL et flux de clics]** fournissent des indicateurs clés de performances (KPI) qui donnent des informations détaillées sur les URL qui ont reçu le plus grand nombre de clics lors d’une diffusion.

  ![](assets/reporting_email_7.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Réactivité]** : ratio du nombre de destinataires ciblé(e)s ayant cliqué dans une diffusion, par rapport à l’estimation du nombre de destinataires ciblé(e)s ayant ouvert une diffusion.

   * **[!UICONTROL Clics distincts]** : nombre total de destinataires distinct(e)s ayant cliqué dans une diffusion au moins une fois.

   * **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

   * **[!UICONTROL Moyenne plateforme]** : ce taux moyen, affiché sous chaque taux (réactivité, clics distincts et clics cumulés), est calculé pour les diffusions envoyées sur les six derniers mois. Seules les diffusions de même typologie et envoyées sur le même canal sont prises en compte. Les BAT sont exclus.

+++

* Le tableau et le graphe des **[!UICONTROL 10 liens les plus consultés]** contiennent les données disponibles pour le comportement des destinataires par lien.

  ![](assets/reporting_email_8.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

   * **[!UICONTROL Pourcentage]** : pourcentage d’utilisateurs et utilisatrices ayant interagi avec la diffusion.

+++

* Le graphe **[!UICONTROL Répartition des clics au fil du temps]** contient les données disponibles sur le comportement des destinataires par lien.

  ![](assets/reporting_email_9.png){align="center"}

## Activités utilisateurs {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widget Activités utilisateur"
>abstract="La variable **Activités utilisateurs** Le graphique présente la répartition des ouvertures et clics sous la forme d&#39;un graphique. Vous pouvez choisir la période pour laquelle cibler les données : dernier jour, dernière heure ou 30 dernières minutes."

* Les **[!UICONTROL Activités utilisateurs]** affiche la répartition des ouvertures et clics sous la forme d’un graphique. Vous pouvez choisir la période pour laquelle cibler les données : dernier jour, dernière heure ou 30 dernières minutes.

  ![](assets/reporting_email_10.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

   * **[!UICONTROL Ouvertures]** : nombre de destinataires ciblé(e)s distinct(e)s, pour ce domaine, ayant ouvert un message au moins une fois.

+++

## Statistiques de tracking {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Widget Statistiques de suivi"
>abstract="La variable **Statistiques de suivi** Le graphique fournit des statistiques sur les ouvertures et les clics. Vous avez la possibilité de sélectionner la période spécifique pour les données de ciblage."

* Le graphe **[!UICONTROL Statistiques de tracking]** fournit des statistiques sur les ouvertures et les clics. Vous avez la possibilité de sélectionner la période spécifique pour les données de ciblage.

  ![](assets/reporting_email_11.png){align="center"}

  +++En savoir plus sur les mesures des rapports de diffusion par e-mail.

   * **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

   * **[!UICONTROL Ouvertures]** : nombre de destinataires ciblé(e)s distinct(e)s, pour ce domaine, ayant ouvert un message au moins une fois.

+++

## Répartition des ouvertures {#breakdown-opens}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Répartition par appareil"
>abstract="La variable **Ventilation par appareil** affiche la répartition des ouvertures, par type d&#39;appareil, sur la période concernée. Le premier graphique présente les statistiques d&#39;ouverture sur un ordinateur et des appareils mobiles. Le second affiche des statistiques relatives uniquement aux ouvertures sur les appareils mobiles."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Répartition par système d’exploitation"
>abstract="La variable **Ventilation par système d’exploitation** affiche la répartition des ouvertures, par système d&#39;exploitation, sur la période concernée. Le premier graphique présente les statistiques d&#39;ouverture sur un ordinateur et des appareils mobiles. Le second affiche des statistiques relatives uniquement aux ouvertures sur les appareils mobiles."

Ce rapport affiche la répartition des ouvertures par système d&#39;exploitation, par appareil, et par navigateur, sur la période sélectionnée. Pour chaque catégorie, deux graphiques sont utilisés. Le premier affiche les statistiques d&#39;ouvertures sur ordinateur et mobile. Le second affiche uniquement les statistiques d&#39;ouvertures sur mobiles.

Vous avez la possibilité de passer de **[!UICONTROL Fixe et mobile]** à **[!UICONTROL Mobile uniquement]** pour un ciblage plus précis.

![](assets/reporting_email_13.png){align="center"}

## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Rapport HotClicks"
>abstract="La variable **Hotclicks** présente le contenu de l&#39;email (HTML et/ou texte) avec, sur chaque lien, le pourcentage de clics sur ce lien. Les blocs de personnalisation, liens de désinscription, liens de page miroir et liens d&#39;offre sont pris en compte dans le total des clics cumulés, mais ne sont pas affichés dans le rapport."

Ce rapport présente le contenu du message (HTML et/ou texte) avec, sur chaque lien, le pourcentage de clics sur ce lien. Les blocs de personnalisation, liens de désinscription, liens de page miroir et liens d&#39;offre sont pris en compte dans le total des clics cumulés, mais ne sont pas affichés dans le rapport.

![](assets/reporting11.png)
