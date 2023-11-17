---
title: Mécanismes de sécurisation et limites de l’interface utilisateur web de Campaign
description: Mécanismes de sécurisation et limites de l’interface utilisateur web de Campaign
badge: label="Beta"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 441add3d624ab730c3dce39a4305107998c5cc62
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 100%

---

# Mécanismes de sécurisation et limitations {#guardrails-limitations}

Lorsque vous utilisez l’interface utilisateur web de Campaign avec des composants créés ou modifiés dans la console cliente Campaign, les mécanismes de sécurisation et les limites répertoriés ci-dessous s’appliquent.

## Workflows {#wf-guardrails-limitations}

### Activités

Les activités de workflow qui ne sont pas encore prises en charge dans l’interface utilisateur web sont en lecture seule et affichées en tant qu’activités incompatibles. Vous pouvez toujours exécuter le workflow, envoyer des messages, vérifier les journaux, etc. Les activités de workflow disponibles dans l’interface utilisateur web et dans la console cliente sont modifiables.

| Console | Interface utilisateur web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

Les paramètres d’activité de workflow qui ne sont pas encore pris en charge dans l’interface utilisateur web ne s’affichent pas. Toutefois, lorsque le workflow est exécuté, ces paramètres s’appliquent.

| Console | Interface utilisateur web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

Dans la console, l’activité **Enrichissement** peut effectuer à la fois la réconciliation et l’enrichissement. Dans l’interface utilisateur web, les fonctionnalités de réconciliation ne sont pas encore disponibles. Si vous avez défini des paramètres de réconciliation dans la console, dans l’activité **Enrichissement**, celle-ci s’affiche en tant qu’activité en lecture seule non compatible dans l’interface utilisateur web.

| Console | Interface utilisateur web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

### Zone de travail

Lors de la création d’un workflow dans l’interface utilisateur web, la zone de travail ne prend en charge qu’un seul point d’entrée. Cependant, si vous avez créé un workflow dans la console avec plusieurs points d’entrée, vous pouvez l’ouvrir et le modifier dans l’interface utilisateur web.

| Console | Interface utilisateur web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

Les boucles ne sont pas encore disponibles dans l’interface utilisateur web. Si vous avez créé un workflow comprenant une boucle à l’aide de la console, vous ne pouvez pas y accéder à partir de l’interface utilisateur web. Un message d’erreur s’affiche.

| Console | Interface utilisateur web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="800px" align="left" zoomable="yes"} |

Le positionnement des nœuds est actualisé à chaque fois qu’une activité est ajoutée ou supprimée. Si vous créez un workflow dans la console, que vous le modifiez à l’aide de l’interface utilisateur web et que vous le rouvrez dans la console, vous constaterez peut-être des imperfections mineures du positionnement. Cela n’a aucun impact sur les processus et les tâches du workflow.

| Workflow initial | Changement de positionnement |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |

## Filtres prédéfinis {#filters-guardrails-limitations}

>[!CONTEXTUALHELP]
>id="acw_predefined_filter_read_only"
>title="Ce filtre est en lecture seule."
>abstract="Certains filtres prédéfinis ne sont pas disponibles dans l’interface utilisateur de cette version du produit. Ces filtres sont marqués comme étant en lecture seule. Même si vous ne pouvez pas afficher la représentation graphique de la requête dans le créateur de règles et que vous ne pouvez pas modifier le filtre, vous pouvez toujours l’utiliser et afficher les conditions de filtrage dans la section **Attributs** de l’écran."

Lors de la sélection de l’audience d’une diffusion ou lors de la création d’une audience dans un workflow, certains filtres prédéfinis ne sont pas disponibles dans l’interface utilisateur, dans cette version du produit. Ces filtres sont marqués comme étant en lecture seule.

Un message d’erreur spécifique s’affiche.

![](assets/filter-unavailable.png){width="70%" align="left"}

Même si vous ne pouvez pas afficher la représentation graphique de la requête dans le créateur de règles et que vous ne pouvez pas modifier le filtre, vous pouvez toujours l’utiliser et afficher les conditions de filtrage dans la section **Attributs** de l’écran.

![](assets/rule-edit.png){width="70%" align="left"}

Vous pouvez également accéder à la requête SQL pour vérifier les paramètres exacts. Pour ce faire, cliquez sur le bouton **Affichage du code**.

![](assets/rule-code-view.png){width="70%" align="left"}

Cliquez sur le bouton **Calculer** pour vérifier le nombre d’éléments qui correspondent aux critères du filtre.

![](assets/rule-calculate.png){width="70%" align="left"}

Utilisez le bouton **Afficher les résultats** pour afficher ces éléments.

![](assets/rule-view-results.png){width="70%" align="left"}

Notez que si vous créez un filtre dans l’interface web et que vous le modifiez dans la console avec des attributs non pris en charge, la représentation graphique ne sera plus disponible dans l’interface web. Dans tous les cas, vous pouvez toujours utiliser le filtre.

Les attributs non pris en charge sont répertoriés ci-dessous.

### Types de données non pris en charge {#unsupported-data-type}

Les types de données suivants, disponibles dans la console cliente, ne sont pas pris en charge lors de l’affichage d’un filtre ou d’une règle dans l’interface web :

* datetime
* time
* timespan
* double
* float

### Fonctionnalités de filtrage non prises en charge {#unsupported-filtering-capabilities}

Lorsqu’un filtre est créé avec des expressions et fonctions complexes dans la console cliente, il ne peut pas être édité dans l’interface web.

En outre, les opérateurs suivants ne sont pas pris en charge :

* Type numérique
   * est compris dans
   * pas dans

* Type de chaîne
   * supérieur à
   * inférieur à
   * supérieur ou égal à
   * inférieur ou égal à
   * comme
   * pas comme

* Type de date
   * après ou égal à
   * avant ou égal à
   * n’est pas égal à
   * est vide
   * n’est pas vide
   * est compris dans
   * pas dans
   * ces derniers

* 1-N liens
   * COUNT, SUM, AVG, MIN, MAX
