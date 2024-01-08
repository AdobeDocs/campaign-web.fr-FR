---
audience: end-user
title: Utiliser le concepteur de requête
description: Découvrez comment travailler avec le concepteur de requête d’Adobe Campaign Web.
badge: label="Disponibilité limitée"
source-git-commit: 26d4b548a7019a79826af435a90deb72e956bcde
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 58%

---

# Utiliser le concepteur de requête {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Nouveau modèle de requête"
>abstract="Adobe Campaign Web comporte un concepteur de requête qui simplifie le processus de filtrage des bases de données afin de sélectionner des cibles spécifiques selon différents critères. Cela inclut l’utilisation d’expressions et d’opérateurs avancés. Le concepteur de requête est disponible dans tout contexte où vous devez définir des règles pour filtrer les données."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Concepteur de requête"
>abstract="Définissez des critères de filtrage pour les personnes destinataires ou toute autre dimension de ciblage issue de la base de données. Tirez parti de votre audience Adobe Experience Platform pour affiner davantage votre audience cible et maximiser l’impact de votre campagne."

Adobe Campaign Web comporte un concepteur de requête qui simplifie le processus de filtrage des bases de données afin de sélectionner des cibles spécifiques selon différents critères. Cela inclut l’utilisation d’expressions et d’opérateurs avancés.

## Accéder au concepteur de requête

Le concepteur de requête est disponible dans tout contexte où vous devez définir des règles pour filtrer les données.

| Usage | Exemple |
|  ---  |  ---  |
| **Définir les audiences** : indiquez la population à cibler dans vos messages ou workflows et créez facilement de nouvelles audiences adaptées à vos besoins. | ![](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **Personnaliser les activités de workflow** : appliquez des règles aux activités de workflow, telles que Partage et Réconciliation, afin de respecter vos besoins spécifiques. | ![](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **Filtres prédéfinis** : créez des filtres prédéfinis qui servent de raccourcis lors de diverses opérations de filtrage, que vous utilisiez des listes de données ou que vous créiez l’audience pour une diffusion. | ![](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **Filtrer les données de rapports** : ajoutez une règle pour filtrer les données affichées dans les rapports. | ![](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **Personnaliser les listes** : créez des règles personnalisées pour filtrer les données affichées dans les listes, telles que les personnes destinataires, les listes de diffusions, etc. | ![](assets/access-lists.png){width="200" align="center" zoomable="yes"} |

<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png)

 +++
-->

## Interface du concepteur de requête {#interface}

Le créateur de modèles de requêtes fournit un canevas central dans lequel vous créez votre requête, ainsi qu’un volet de droite fournissant des informations sur votre requête.

![](assets/query-interface.png)

### Zone de travail centrale {#canvas}

Le canevas central du modeleur de requête est l’endroit où vous ajoutez et combinez les différents composants qui construisent votre requête. [Découvrez comment créer une requête](build-query.md)

La barre d’outils située dans le coin supérieur droit du canevas fournit des options pour manipuler facilement les composants de requête et naviguer dans la zone de travail :

* **Mode de sélection multiple**: sélectionnez plusieurs composants de filtrage à copier et coller à l’emplacement de votre choix.
* **Rotation**: basculez le canevas verticalement.
* **Ajuster à l’écran**: adaptez le niveau de zoom de la zone de travail à votre écran.
* **Zoom arrière** / **Zoom avant**: permet de zoomer ou dans la zone de travail.
* **Afficher la carte**: ouvre un instantané de la zone de travail indiquant que vous vous trouvez.

### Volet Propriétés de la règle {#rule-properties}

Sur le côté droit, le **[!UICONTROL Propriétés des règles]** Le volet fournit des informations sur votre requête. Il vous permet d’effectuer diverses opérations pour vérifier la requête et vous assurer qu’elle correspond à vos besoins. [Découvrez comment vérifier et valider votre requête](build-query.md#check-and-validate-your-query)
