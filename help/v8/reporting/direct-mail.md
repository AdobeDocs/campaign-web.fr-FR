---
audience: end-user
title: Rapports de courrier
description: Découvrir comment accéder aux rapports de courrier pour les utiliser
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 100%

---

# Rapport de diffusion par courrier {#direct-mail-report}

Le **rapport de diffusion par courrier** offre des informations et des données complètes spécifiques au canal Courrier. Il fournit des informations détaillées sur les performances, l’efficacité et les résultats de vos diffusions individuelles, ce qui vous permet d’obtenir une vue d’ensemble complète.

## Synthèse des diffusions {#delivery-summary-direct-mail}

### Vue d’ensemble de la diffusion {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Vue d’ensemble de la diffusion"
>abstract="La **Vue d’ensemble de la diffusion** affiche des KPI, ou indicateurs clés de performance, qui offrent des informations détaillées sur la manière dont vos visiteurs et visiteuses interagissent avec les diffusions courrier. Les mesures sont décrites ci-dessous."

La **[!UICONTROL Vue d’ensemble de la diffusion]** fournit des informations détaillées sur la manière dont vos visiteurs et visiteuses interagissent avec chaque diffusion par courrier, en exposant les KPI essentiels.  Les mesures sont décrites ci-dessous.

![](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++En savoir plus sur les mesures de vue d’ensemble de diffusion.

* **[!UICONTROL Messages à diffuser]** : nombre total de messages traités lors de la préparation de la diffusion.

* **[!UICONTROL Ciblés]** : nombre de profils de personnes qui remplissent les critères de ciblage pour vos messages courrier.

* **[!UICONTROL À exclure]** : nombre de profils de personnes exclues des profils ciblés, qui ne recevront pas vos messages courrier.
+++

### Population cible initiale {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Population cible initiale"
>abstract="Le graphe **Population cible initiale** affiche les données relatives à vos destinataires et messages, en fonction des résultats de la préparation de la diffusion."

Le graphe **[!UICONTROL Population cible initiale]** affiche les données relatives à vos destinataires. Les mesures sont calculées lors de la préparation de la diffusion. Elles affichent l’audience initiale, le nombre de messages à envoyer et le nombre de destinataires exclus.

![](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

Placez le pointeur de la souris sur une partie du graphe pour afficher le nombre exact.

![](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

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

Le graphe **[!UICONTROL Statistiques de diffusion]** offre une vue d’ensemble complète des performances de vos diffusions, avec des mesures détaillées du succès et de l’efficacité.

![](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++En savoir plus sur les mesures des rapports de campagne par courrier.

* **[!UICONTROL Message envoyé]** : nombre total de messages à délivrer après la préparation de la diffusion.

* **[!UICONTROL Succès]** : nombre de messages traités avec succès par rapport au nombre de messages à délivrer.

* **[!UICONTROL Erreurs]** : nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des retours par rapport au nombre de messages à délivrer.

* **[!UICONTROL Nouvelles quarantaines]** : nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (utilisateur ou utilisatrice inconnu(e), domaine invalide) par rapport au nombre de messages à délivrer.

+++

### Causes d’exclusion {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Causes d’exclusion des diffusions"
>abstract="Le graphe **Causes d’exclusion** illustre la distribution des messages rejetés lors de la préparation de la diffusion, classés par règle."

La graphe **[!UICONTROL Causes d’exclusion]** fournit une répartition détaillée des raisons pour lesquelles les messages sont rejetés pendant le processus de préparation de la diffusion. Cette répartition est organisée selon différentes règles, offrant une vue d’ensemble des facteurs contribuant à l’exclusion des messages. Les règles d’exclusion sont détaillées dans la section [Documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=fr#email-error-types){_blank}.

![](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++En savoir plus sur les mesures de causes d’exclusion.

* **[!UICONTROL Adresse en quarantaine]** : type d’erreur générée lorsque l’adresse est mise en quarantaine.

* **[!UICONTROL Adresse non renseignée]** : type d’erreur générée lors de l’envoi d’une diffusion indiquant que l’adresse n’existe pas.

* **[!UICONTROL Adresse de mauvaise qualité]** : type d’erreur générée lorsque la note de qualité de l’adresse postale est trop basse.

* **[!UICONTROL Adresse placée sur la liste bloquée]** : type d’erreur générée lorsque la personne destinataire a été placée sur la liste bloquée lors de l’exécution de la diffusion.

* **[!UICONTROL Double]** : type d’erreur générée lorsque la personne destinataire a été exclue, car ses valeurs de clés n’étaient pas uniques.

* **[!UICONTROL Population témoin]** : l’adresse de la personne destinataire fait partie de la population témoin.

* **[!UICONTROL Cible limitée en taille]** : la taille de diffusion maximale a été atteinte pour la personne destinataire.

+++

### Exclusions {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Exclusions"
>abstract="Le tableau **[!UICONTROL Exclusions]** affiche une répartition détaillée, par règle, des messages qui ont été rejetés pendant le processus de préparation de la diffusion."

Le tableau **[!UICONTROL Exclusions]** fournit une répartition détaillée, classée par règles spécifiques, des messages qui ont été rejetés lors de la phase de préparation de la diffusion. Cette répartition exhaustive permet de comprendre clairement les raisons de l’exclusion de ces messages du processus de diffusion.

![](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

Les mesures disponibles sont les mêmes que celles des [causes d’exclusion](#direct-mail-delivery-exclusions) décrites ci-dessus.
