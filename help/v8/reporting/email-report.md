---
audience: end-user
title: Rapports de diffusion par e-mail
description: Découvrez comment accéder aux rapports de diffusion par e-mail et les utiliser.
badge: label="Beta"
source-git-commit: 3c679ad284f15a46885829b68c8ebea1e99e2b98
workflow-type: tm+mt
source-wordcount: '2254'
ht-degree: 68%

---

# Rapport de diffusion par e-mail {#email-report}

Le **rapport de diffusion par e-mail** offre des informations et des données complètes spécifiques au canal e-mail. Il fournit des informations détaillées sur les performances, l’efficacité et les résultats de vos diffusions individuelles, ce qui vous permet d’obtenir une vue d’ensemble complète.

## Synthèse des diffusions {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Envoi des rapports"
>abstract="L’onglet **Envoi** de votre rapport fournit des informations détaillées sur les interactions de vos visiteurs et visiteuses avec vos diffusions, ainsi que sur les erreurs potentielles qu’ils ont pu rencontrer."

### Population cible initiale {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Population cible initiale"
>abstract="La variable **Population cible initiale** Le graphique affiche les données relatives à vos destinataires et messages, en fonction des résultats de la préparation de la diffusion."

La variable **[!UICONTROL Population cible initiale]** Le graphique affiche les données relatives à vos destinataires. Les mesures sont calculées lors de la préparation de la diffusion et affichent : l’audience initiale, le nombre de messages à envoyer, le nombre de destinataires exclus.

![](assets/reporting_email_1.png){width="50%" align="left" zoomable="yes"}

Placez le pointeur de la souris sur une partie du graphique pour afficher le nombre exact.

![](assets/reporting_email_1.1.png){width="50%" align="left" zoomable="yes"}


+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Audience initiale]** : nombre total de destinataires ciblé(e)s.

* **[!UICONTROL À diffuser]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Exclusion]**: Nombre total de destinataires exclus de la population cible.
+++

### Statistiques de diffusion {#email-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Statistiques de diffusion"
>abstract="La variable **Statistiques de diffusion** Le graphique décrit le succès de votre diffusion et les erreurs qui se sont produites."


La variable **[!UICONTROL Statistiques de diffusion]** Le graphique décrit le succès de votre diffusion. Les mesures sont détaillées ci-dessous.

![](assets/reporting_email_2.png){width="50%" align="left" zoomable="yes"}

+++En savoir plus sur les mesures des rapports de campagne par e-mail.

* **[!UICONTROL Message envoyé]** : nombre total de messages à diffuser après la préparation de la diffusion.

* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à diffuser.

* **[!UICONTROL Erreurs]** : nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre de messages à diffuser.

* **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (utilisateur ou utilisatrice inconnu(e), domaine invalide) par rapport au nombre de messages à diffuser.

+++

### Causes d&#39;exclusion  {#email-delivery-exclusions}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Statistiques de diffusion"
>abstract="La variable **Causes d&#39;exclusion** le graphique et le tableau affichent la répartition, par règle, des messages rejetés lors de la préparation de la diffusion."


La variable **[!UICONTROL Causes d&#39;exclusion]** le graphique et le tableau affichent la répartition, par règle, des messages rejetés lors de la préparation de la diffusion. Les règles d&#39;exclusion sont détaillées dans la section [Documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/reporting_email_3.png){align="center" zoomable="yes"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Utilisateur inconnu]** : type d’erreur générée lors de l’envoi d’une diffusion indiquant que l’adresse e-mail n’est pas valide.

* **[!UICONTROL Domaine invalide]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que le domaine de l&#39;adresse e-mail est erroné ou n&#39;existe plus.

* **[!UICONTROL Boîte pleine]** : type d’erreur générée, après cinq tentatives de diffusion, indiquant que la boîte de réception de la personne destinataire contient trop de messages.

* **[!UICONTROL Compte désactivé]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que l&#39;adresse n&#39;existe plus.

* **[!UICONTROL Refusé]** : type d’erreur générée lorsqu’une adresse est refusée par le FAI (Fournisseur d’accès Internet), par exemple, suite à l’application d’une règle de sécurité (logiciel anti-spams).

* **[!UICONTROL Inatteignable]** : type d&#39;erreur survenue dans la chaîne de distribution du message : incident sur le relais SMTP, domaine temporairement inatteignable, etc.

* **[!UICONTROL Non connecté]** : type d’erreur indiquant que le téléphone portable de la personne destinataire est éteint ou n’est pas connecté au réseau au moment de l’envoi du message.

+++

## Débit des diffusions (Delivery throughput) {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Débit des diffusions (Delivery throughput)"
>abstract="Le rapport **Débit de diffusion** présente des informations détaillées sur le débit de diffusion de l’ensemble de la plateforme dans un délai donné."

Ce rapport présente des informations détaillées sur le débit de diffusion de l’ensemble de la plateforme au cours d’une période donnée. La mesure principale utilisée pour mesurer la vitesse de diffusion des messages est le nombre de messages envoyés par heure.

![](assets/reporting_email_3.1.png){align="center" zoomable="yes"}


## Statistiques de diffusion {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Statistiques de diffusion"
>abstract="La variable **Statistiques de diffusion** Ce rapport contient les données disponibles relatives aux erreurs possibles rencontrées pour chaque domaine."

Le tableau **[!UICONTROL Statistiques sur les domaines]** contient les données disponibles liées aux erreurs possibles rencontrées pour chaque domaine. Les mesures sont détaillées ci-dessous.

![](assets/reporting_email_4.png){align="center" zoomable="yes"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL E-mails traités]** : nombre total de messages traités par le serveur de diffusion.

* **[!UICONTROL Diffusés]** : pourcentage du nombre de messages traités avec succès, par rapport au nombre total de messages traités.

* **[!UICONTROL Hard bounces]** : pourcentage du nombre de hard bounces, c’est-à-dire des erreurs permanentes, telles qu’une mauvaise adresse e-mail, par rapport au nombre total de messages traités.

* **[!UICONTROL Soft bounces]** : pourcentage du nombre de soft bounces, c’est-à-dire des erreurs temporaires telles qu’une boîte de réception pleine, par rapport au nombre total de messages traités.

* **[!UICONTROL Ouvertures]** : pourcentage du nombre de destinataires ciblé(e)s ayant ouvert un message au moins une fois, par rapport au nombre de messages traités avec succès.

* **[!UICONTROL Clics]** : pourcentage du nombre de personnes ayant cliqué au moins une fois dans une diffusion, par rapport au nombre de messages traités avec succès.

* **[!UICONTROL Désinscriptions]** : pourcentage du nombre de clics effectués sur un lien de désinscription, par rapport au nombre de messages traités avec succès.
+++

## Non délivrables {#non-deliverables-email}

###  Répartition des erreurs par type {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title=" Répartition des erreurs par type"
>abstract="La variable **Ventilation des erreurs par type** le tableau et le graphique contiennent les données disponibles pour chaque type d’erreur rencontré : utilisateur inconnu, boîte pleine, domaine non valide, etc."

La variable **[!UICONTROL Ventilation des erreurs par type]** le tableau et le graphique contiennent les données disponibles pour le type d’erreur. Les mesures sont détaillées ci-dessous.

Les erreurs présentées dans ce rapport déclenchent le processus de mise en quarantaine. Pour plus d’informations sur la gestion des quarantaines, consultez la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=fr){target="_blank"}.

![](assets/campaign_report_email_6.png){align="left" zoomable="yes"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Utilisateur inconnu]** : type d’erreur générée lors de l’envoi d’une diffusion indiquant que l’adresse e-mail n’est pas valide.

* **[!UICONTROL Domaine invalide]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que le domaine de l&#39;adresse e-mail est erroné ou n&#39;existe plus.

* **[!UICONTROL Boîte pleine]** : type d’erreur générée, après cinq tentatives de diffusion, indiquant que la boîte de réception de la personne destinataire contient trop de messages.

* **[!UICONTROL Compte désactivé]** : type d&#39;erreur générée lors de l&#39;envoi d&#39;une diffusion indiquant que l&#39;adresse n&#39;existe plus.

* **[!UICONTROL Refusé]** : type d’erreur générée lorsqu’une adresse est refusée par le FAI (Fournisseur d’accès Internet), par exemple, suite à l’application d’une règle de sécurité (logiciel anti-spams).

* **[!UICONTROL Inatteignable]** : type d&#39;erreur survenue dans la chaîne de distribution du message : incident sur le relais SMTP, domaine temporairement inatteignable, etc.

* **[!UICONTROL Non connecté]** : type d’erreur indiquant que le téléphone portable de la personne destinataire est éteint ou n’est pas connecté au réseau au moment de l’envoi du message.

+++


### Répartition des erreurs par domaine {#email-delivery-breakdown-domain}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Répartition des erreurs par domaine"
>abstract="La variable **Ventilation des erreurs par domaine** tableau et graphique affichent les données disponibles pour chaque type d’erreur rencontré en fonction de chaque domaine."


La variable **[!UICONTROL Ventilation des erreurs par domaine]** tableau et graphique affichent les données disponibles pour les erreurs possibles rencontrées pour chaque domaine.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Cliquez sur l’icône en regard du nom de chaque domaine pour afficher les détails.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Les mesures disponibles sont les mêmes que pour la variable [Répartition des erreurs par type](#email-delivery-breakdown-type) décrits ci-dessus.

## Indicateurs de tracking {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Tracking des rapports"
>abstract="L’onglet **Tracking** de votre rapport contient des données importantes, notamment le comportement des personnes destinataires par lien, la répartition des ouvertures et des clics, ainsi que des informations détaillées sur les URL ayant reçu le plus de clics lors d’une diffusion."


### Statistiques de diffusion  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Statistiques de diffusion"
>abstract="La variable **Statistiques de diffusion** Ce rapport fournit des indicateurs de performances clés (IPC) qui fournissent des informations détaillées sur les données disponibles pour les emails envoyés : succès, ouvertures, clics, etc."


La variable **[!UICONTROL Statistiques de diffusion]** Ce rapport fournit des indicateurs de performance clés (IPC) qui fournissent des informations détaillées sur les données disponibles pour les emails envoyés. Les mesures sont détaillées ci-dessous.

![](assets/reporting_email_5.png){align="center"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à diffuser.

* **[!UICONTROL Ouvertures distinctes]** : nombre total de destinataires ciblé(e)s ayant ouvert un message au moins une fois.

* **[!UICONTROL Ouvertures]** : nombre de destinataires ciblé(e)s distinct(e)s pour ce domaine ayant ouvert un message au moins une fois.

* **[!UICONTROL Clics sur le lien d’exclusion]** : nombre de clics effectués sur le lien d’exclusion.

* **[!UICONTROL Clics sur le lien miroir]** : nombre de clics sur le lien vers la page miroir.

* **[!UICONTROL Estimation des transferts]** : estimation du nombre d’e-mails transférés par les destinataires ciblé(e)s.
+++

### Taux d&#39;ouverture et de clic {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Taux d&#39;ouverture et de clic"
>abstract="Le tableau **Taux d’ouverture et de clic publicitaire** affiche des données relatives à l’engagement de vos personnes destinataires avec votre diffusion."



La variable **[!UICONTROL Taux d&#39;ouverture et de clic]** affiche des données relatives à vos destinataires. Les mesures sont détaillées ci-dessous.

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
>title="URL et flux de clics (URLs and click streams)"
>abstract="La variable **URL et flux de clics** Ce rapport fournit des indicateurs de performance clés (IPC) qui fournissent des informations détaillées sur les URL ayant reçu le plus grand nombre de clics lors d’une diffusion."


La variable **[!UICONTROL URL et flux de clics]** Ce rapport fournit des indicateurs de performance clés (IPC) qui fournissent des informations détaillées sur les URL ayant reçu le plus grand nombre de clics lors d’une diffusion.

![](assets/reporting_email_7.png){align="center"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Réactivité]** : ratio du nombre de destinataires ciblé(e)s ayant cliqué dans une diffusion, par rapport à l’estimation du nombre de destinataires ciblé(e)s ayant ouvert une diffusion.

* **[!UICONTROL Clics distincts]** : nombre total de destinataires distinct(e)s ayant cliqué dans une diffusion au moins une fois.

* **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

* **[!UICONTROL Moyenne plateforme]** : ce taux moyen, affiché sous chaque taux (réactivité, clics distincts et clics cumulés), est calculé pour les diffusions envoyées sur les six derniers mois. Seules les diffusions de même typologie et envoyées sur le même canal sont prises en compte. Les BAT sont exclus.

+++

### Top 10 des liens les plus visités {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="Top 10 des liens les plus visités"
>abstract="La variable **Les 10 liens les plus consultés** Le graphique et le tableau contiennent les données disponibles pour le comportement des destinataires par lien."


La variable **[!UICONTROL Les 10 liens les plus consultés]** Le graphique et le tableau contiennent les données disponibles pour le comportement des destinataires par lien.

![](assets/reporting_email_8.png){align="center"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

* **[!UICONTROL Pourcentage]** : pourcentage d’utilisateurs et utilisatrices ayant interagi avec la diffusion.

+++

### Répartition des clics dans le temps {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_click_breakdown"
>title="Répartition des clics dans le temps"
>abstract="La variable **Répartition des clics au fil du temps** Le graphique présente les données disponibles pour le comportement des destinataires par lien."


La variable **[!UICONTROL Répartition des clics au fil du temps]** Le graphique contient les données disponibles sur le comportement des destinataires par lien.

![](assets/reporting_email_9.png){align="center"}

## Activités utilisateurs {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widget Activités utilisateurs et utilisatrices"
>abstract="Le graphe **Activités utilisateurs et utilisatrices** affiche la répartition des ouvertures et des clics sous la forme d’un diagramme. Vous pouvez choisir la période pour laquelle cibler les données : dernier jour, dernière heure ou 30 dernières minutes."

La variable **[!UICONTROL Activités utilisateurs]** Le rapport présente la répartition des ouvertures et clics sous la forme d&#39;un graphique. Vous pouvez choisir la période pour laquelle cibler les données : dernier jour, dernière heure ou 30 dernières minutes.

![](assets/reporting_email_10.png){align="center"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

* **[!UICONTROL Ouvertures]** : nombre de destinataires ciblé(e)s distinct(e)s, pour ce domaine, ayant ouvert un message au moins une fois.

+++

## Statistiques de tracking {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Widget Statistiques de tracking"
>abstract="Le graphe **Statistiques de tracking** fournit des statistiques sur les ouvertures et les clics. Vous avez la possibilité de sélectionner la période spécifique pour les données de ciblage."

Le graphe **[!UICONTROL Statistiques de tracking]** fournit des statistiques sur les ouvertures et les clics. Vous avez la possibilité de sélectionner la période spécifique pour les données de ciblage.

![](assets/reporting_email_11.png){align="center"}

+++En savoir plus sur les mesures des rapports de diffusion par e-mail.

* **[!UICONTROL Clics]** : nombre total de clics sur les liens dans les diffusions.

* **[!UICONTROL Ouvertures]** : nombre de destinataires ciblé(e)s distinct(e)s, pour ce domaine, ayant ouvert un message au moins une fois.

+++

## Répartition des ouvertures {#breakdown-opens}

### Répartition des ouvertures par appareil {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Répartition par appareil"
>abstract="La variable **Ventilation par appareil** Le rapport présente la répartition des ouvertures, par appareil, sur la période. Deux graphiques sont utilisés pour chaque catégorie. Le premier affiche les statistiques d’ouverture sur un ordinateur et des appareils mobiles. La seconde affiche le nombre et le pourcentage exacts pour chaque type d’appareil."

La variable **Ventilation par appareil** Ce rapport présente la répartition des ouvertures, par appareil, sur la période : ordinateurs personnels, appareils Android, appareils Apple, etc.

Deux graphiques sont utilisés pour chaque catégorie. Le premier affiche les statistiques d’ouverture sur un ordinateur et des appareils mobiles. La seconde affiche le nombre et le pourcentage exacts pour chaque type d’appareil.

![](assets/reporting_email_13.png){align="center"}


### Répartition des ouvertures par système d&#39;exploitation {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Ventilation par système d&#39;exploitation"
>abstract="La variable **Ventilation par système d’exploitation** Le rapport présente la répartition des ouvertures, par système d&#39;exploitation, sur la période concernée. Le premier diagramme affiche les statistiques d’ouverture sur un ordinateur et des appareils mobiles. La seconde affiche le nombre et le pourcentage exacts pour chaque système d’exploitation."

La variable **Ventilation par système d’exploitation** Ce rapport présente la répartition des ouvertures, par système d’exploitation, sur la période : systèmes Windows, systèmes Android, systèmes iOS, etc.

Deux graphiques sont utilisés pour chaque catégorie. Le premier affiche les statistiques d&#39;ouverture sur un ordinateur et sur les systèmes d&#39;exploitation mobiles. La seconde affiche le nombre et le pourcentage exacts pour chaque système d’exploitation.

![](assets/reporting_email_13.1.png){align="center"}

### Répartition des ouvertures par navigateur {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Répartition par navigateur"
>abstract="La variable **Ventilation par navigateur** affiche la répartition des ouvertures, par navigateur, sur la période. Le premier diagramme affiche les statistiques d’ouverture sur un ordinateur et des appareils mobiles. La seconde affiche le nombre et le pourcentage exacts pour chaque navigateur."

La variable **Ventilation par navigateur** Ce rapport présente la ventilation des ouvertures par navigateur : Chrome, Safari, Internet Explorer, etc.

Deux graphiques sont utilisés pour chaque catégorie. Le premier affiche les statistiques d&#39;ouverture sur un ordinateur et sur les systèmes d&#39;exploitation mobiles. La seconde affiche le nombre et le pourcentage exacts pour chaque navigateur.

![](assets/reporting_email_13.2.png){align="center"}


## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Rapport Hotclicks"
>abstract="Le rapport **Hotclicks** présente le contenu de l’e-mail (HTML et/ou texte) avec, sur chaque lien, le pourcentage de clics sur ce lien. Les blocs de personnalisation, liens de désinscription, liens de page miroir et liens d’offre sont pris en compte dans le total des clics cumulés, mais ne sont pas affichés dans le rapport."

Ce rapport présente le contenu du message (HTML et/ou texte) avec, sur chaque lien, le pourcentage de clics sur ce lien. Les blocs de personnalisation, liens de désinscription, liens de page miroir et liens d’offre sont pris en compte dans le total des clics cumulés, mais ne sont pas affichés dans le rapport.

![](assets/reporting11.png)
