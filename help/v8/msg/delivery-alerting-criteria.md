---
audience: end-user
title: Alertes de diffusion
description: Découvrez comment utiliser les alertes de diffusion.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 32%

---

# Critères des alertes de diffusion {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Tableau de bord des critères des alertes de diffusion"
>abstract="L’interface d’utilisation de Campaign Web fournit des critères d’alerte prédéfinis (diffusions avec faible débit, diffusions dont la préparation a échoué...) que vous pouvez ajouter à votre tableau de bord. Vous pouvez également créer vos propres critères en fonction de vos besoins."

L&#39;interface utilisateur web de Campaign fournit des critères d&#39;alerte prédéfinis (diffusions avec faible débit, diffusions dont la préparation a échoué...) que vous pouvez ajouter à votre tableau de bord. Vous pouvez également créer vos propres critères en fonction de vos besoins.

Les critères d’alerte sont accessibles à partir du **Alertes de diffusion** dans le volet de navigation de gauche, sous **Critères** .

![](assets/alerting-criteria-list.png)

## Critères d&#39;alerte prédéfinis {#ootb-criteria}

Des critères d&#39;alerte prédéfinis sont disponibles dans l&#39;interface utilisateur web de Campaign. Ces critères couvrent un éventail de scénarios, répertoriés ci-dessous :

* **Diffusions en échec** : toute diffusion planifiée sur une période définie, ayant un statut en erreur.
* **Diffusions avec préparation en échec**: toute diffusion modifiée sur une période définie, pour laquelle l’étape de préparation (calcul de la cible et génération du contenu) a échoué.
* **Diffusion avec taux d&#39;erreur soft incorrect**: toute diffusion planifiée sur une période définie, ayant au moins le statut En cours, dont le taux de soft bounces est supérieur à un pourcentage défini.
* **Diffusion avec taux d&#39;erreur incorrect pour les hard bounces**: toute diffusion planifiée sur une période définie, ayant au moins le statut En cours, dont le taux de hard bounces est supérieur à un pourcentage défini.
* **Diffusions avec un démarrage en attente long**: toute diffusion planifiée sur une période définie, ayant le statut Démarrage en attente pendant une durée supérieure à celle définie, le statut Démarrage en attente signifie que les messages n&#39;ont pas encore été pris en compte par le système.
* **Diffusions avec faible débit** : toute diffusion ayant démarré depuis plus longtemps qu&#39;une durée définie, avec un pourcentage de messages traités inférieur à un pourcentage défini et un débit inférieur à une valeur définie.
* **Diffusions en cours**: toute diffusion planifiée sur une période définie, ayant le statut En cours .

>[!NOTE]
>
>Les valeurs par défaut sont appliquées à tous les paramètres des critères ci-dessus. Ces valeurs peuvent être personnalisées dans la variable **Paramètres des critères** section des tableaux de bord des alertes de diffusion dans lesquels elles sont utilisées. [Découvrez comment utiliser les tableaux de bord](../msg/delivery-alerting-dashboards.md)

## Créer un critère d’alerte {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Créer des critères d’alerte de diffusion"
>abstract="Outre les critères d’alerte prédéfinis fournis par Adobe Campaign, vous pouvez créer vos propres critères en fonction de vos besoins."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicateurs à ajouter aux alertes"
>abstract="Sélectionnez les indicateurs à afficher en colonnes dans la section « Détails » des alertes par e-mail."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Type d’alerte"
>abstract="Spécifiez le **Type d’alerte** pour le critère, c&#39;est-à-dire le libellé et la couleur à afficher en regard du critère de diffusion dans la section « Résumé » des alertes."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Fréquence du critère"
>abstract="Contrôlez la fréquence des alertes par jour pour chaque diffusion répondant au critère."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Créer un critère d’alerte"
>abstract="Pour créer vos propres filtres de diffusion, créez un filtre prédéfini dans la console Campaign v8 à partir du nœud **Administration** > **Configuration** > **Filtres prédéfinis**."

Pour créer un nouveau critère, procédez comme suit :

1. Accédez au **Delivery Àlerting** dans le volet de navigation de gauche, puis sélectionnez **Critères** .
1. Cliquez sur le bouton **Créer des critères d&#39;alerte de diffusion** bouton .
1. Attribuez un libellé au critère. Le nom interne est automatiquement renseigné et en lecture seule.
1. La variable **Filtre de diffusion appliqué par ce critère** permet d’affiner la portée du critère en lui appliquant un filtre prédéfini.

   Dans l’exemple ci-dessous, la variable **Diffusions en cours (scriptInProgressDeliveries)** a été sélectionné, ce qui signifie que le critère ne prend en compte que les diffusions ayant le statut &quot;En cours&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Si aucun des filtres prédéfinis ne répond à vos besoins, vous pouvez contacter votre administrateur pour créer votre propre filtre.  Des informations détaillées sur la création de filtres prédéfinis dans la console Campaign sont disponibles dans la section [Documentation d’Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Cette opération ne doit être effectuée que par des utilisateurs avancés.

1. Dans le **Indicateurs à ajouter dans les alertes** , choisissez les indicateurs à afficher en colonnes dans la section &quot;Détails&quot; des alertes par email.

1. Spécifiez le **Type d’alerte** pour le critère, c&#39;est-à-dire le libellé et la couleur à afficher en regard du critère de diffusion dans la section « Résumé » des alertes.

1. La variable **Fréquence des critères** permet de contrôler la fréquence des alertes par jour pour chaque diffusion répondant au critère :

   * **Ce critère de diffusion sera répété dans chaque notification.**: affiche une diffusion répondant au critère dans chaque alerte par email du jour.
   * **Ce critère de diffusion n&#39;est envoyé que le premier événement de la journée**: affiche une diffusion répondant au critère dans le premier rapport du jour uniquement, non répétée dans les alertes par email suivantes.
