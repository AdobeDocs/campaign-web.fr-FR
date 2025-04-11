---
audience: end-user
title: Rapports de courrier
description: Découvrir comment accéder aux rapports de courrier pour les utiliser
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 41%

---

# Rapport de diffusion par courrier {#direct-mail-report}

Le **rapport de diffusion courrier** fournit des informations et des données complètes spécifiques à votre diffusion courrier. Il comprend des informations détaillées sur les performances, l’efficacité et les résultats de diffusions individuelles, offrant ainsi une vue d’ensemble complète.

## Synthèse des diffusions {#delivery-summary-direct-mail}

### Vue d’ensemble de la diffusion {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Vue d’ensemble de la diffusion"
>abstract="La **Vue d’ensemble de la diffusion** affiche des KPI, ou indicateurs clés de performance, qui offrent des informations détaillées sur la manière dont vos visiteurs et visiteuses interagissent avec les diffusions courrier. Les mesures sont décrites ci-dessous."

La **[!UICONTROL Présentation de la diffusion]** fournit des informations détaillées sur les interactions des visiteurs avec chaque diffusion de publipostage direct, en présentant les mesures de performances clés (KPI) essentielles. Les mesures sont décrites ci-dessous.

![Graphique des mesures de présentation de la diffusion présentant les indicateurs clés de performances pour la diffusion de publipostage direct.](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++En savoir plus sur les mesures de vue d’ensemble de diffusion.

* **[!UICONTROL Messages à diffuser]** : Nombre total de messages traités lors de la préparation de la diffusion.
* **[!UICONTROL Ciblés]** : nombre de profils utilisateur qui remplissent les critères des profils cibles pour les messages de publipostage direct.
* **[!UICONTROL À exclure]** : nombre de profils utilisateur exclus des profils ciblés qui ne recevront pas de messages de publipostage direct.
+++

### Population cible initiale {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Population cible initiale"
>abstract="Le graphe **Population cible initiale** affiche les données relatives à vos destinataires et messages, en fonction des résultats de la préparation de la diffusion."

Le graphique **[!UICONTROL Population cible initiale]** affiche les données relatives aux destinataires. Les mesures sont calculées lors de la préparation de la diffusion et comprennent l’audience initiale, le nombre de messages à envoyer et le nombre de destinataires exclus.

![Graphique de population cible initiale présentant la taille de l’audience, les messages à envoyer et les exclusions.](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

Placez le pointeur de la souris sur une partie du graphique pour afficher le nombre exact.

![Vue détaillée du graphique initial de la population cible avec la fonctionnalité de survol.](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++En savoir plus sur les mesures des rapports de diffusion par courrier.

* **[!UICONTROL Audience initiale]** : nombre total de personnes destinataires ciblées.
* **[!UICONTROL À délivrer]** : nombre total de messages à délivrer après la préparation de la diffusion.
* **[!UICONTROL Exclusion]** : nombre total de destinataires exclus de la population cible.
+++

### Statistiques de diffusion {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="Statistiques de diffusion"
>abstract="Le graphe **Statistiques de diffusion** détaille le succès de votre diffusion par courrier et les erreurs qui se sont produites."

Le graphique **[!UICONTROL Statistiques de diffusion]** donne un aperçu des performances des diffusions et propose des mesures détaillées pour mesurer les performances et l’efficacité.

![Graphique des statistiques de diffusion présentant les taux de succès, les erreurs et les quarantaines.](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++En savoir plus sur les mesures des rapports de campagne par courrier.

* **[!UICONTROL Message envoyé]** : nombre total de messages à délivrer après la préparation de la diffusion.
* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à diffuser.
* **[!UICONTROL Erreurs]** : nombre total d’erreurs accumulées lors des diffusions et du traitement automatique des retours par rapport au nombre de messages à diffuser.
* **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (par exemple, utilisateur ou utilisatrice inconnu(e), domaine invalide) par rapport au nombre de messages à diffuser.
+++

### Causes d’exclusion {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Causes d’exclusion des diffusions"
>abstract="Le graphe **Causes d’exclusion** illustre la distribution des messages rejetés, classés par règle, lors de la préparation de la diffusion."

Le graphique **[!UICONTROL Causes d’exclusion]** fournit une répartition des raisons du rejet du message lors de la préparation de la diffusion. Cette répartition est organisée par différentes règles, offrant une vue détaillée des facteurs contribuant à l’exclusion des messages. Les règles d’exclusion sont détaillées dans la section [Documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#email-error-types){_blank}.

![Graphique des causes d’exclusion présentant la répartition des messages rejetés par règle.](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++En savoir plus sur les mesures de causes d’exclusion.

* **[!UICONTROL Adresse en quarantaine]** : type d&#39;erreur générée lors de la mise en quarantaine d&#39;une adresse.
* **[!UICONTROL Adresse non renseignée]** : type d&#39;erreur générée lorsqu&#39;une adresse n&#39;existe pas.
* **[!UICONTROL Adresse de mauvaise qualité]** : type d’erreur générée lorsque la note de qualité de l’adresse postale est trop basse.
* **[!UICONTROL adresse Placer sur la liste bloquée placée sur la liste bloquée]** : type d&#39;erreur générée lors de l&#39;enregistrement du destinataire lors de la diffusion.
* **[!UICONTROL Double]** : type d’erreur générée lorsque le destinataire a été exclu en raison de valeurs de clé non uniques.
* **[!UICONTROL Population témoin]** : l’adresse de la personne destinataire fait partie de la population témoin.
* **[!UICONTROL Cible limitée en taille]** : la taille de diffusion maximale a été atteinte pour la personne destinataire.
+++

### Exclusions {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Exclusions"
>abstract="Le tableau **[!UICONTROL Exclusions]** affiche une répartition détaillée, par règle, des messages qui ont été rejetés pendant le processus de préparation de la diffusion."

Le tableau **[!UICONTROL Exclusions]** fournit une répartition détaillée, classée par règles spécifiques, des messages rejetés lors de la préparation de la diffusion. Cette répartition permet de bien comprendre les raisons derrière les exclusions de messages.

![Tableau des exclusions présentant la répartition détaillée des messages rejetés par règle.](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

Les mesures disponibles sont les mêmes que celles des [causes d’exclusion](#direct-mail-delivery-exclusions) décrites ci-dessus.