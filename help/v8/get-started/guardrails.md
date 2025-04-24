---
title: Mécanismes de sécurisation et limitations des workflows dans l’interface utilisateur web de Campaign
description: Mécanismes de sécurisation et limitations lors de l’utilisation de workflows dans l’interface utilisateur web de Campaign
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '435'
ht-degree: 100%

---

# Mécanismes de sécurisation et limitations des workflows {#guardrails-limitations}

Lorsque vous utilisez l’interface utilisateur web de Campaign avec des workflows créés ou modifiés dans la console cliente Campaign, les mécanismes de sécurisation et les limitations ci-dessous s’appliquent.

Veuillez noter que, bien que cette page identifie les points essentiels à prendre en compte lors de l’utilisation des workflows dans la console et l’interface utilisateur web, elle n’englobe pas toutes les incompatibilités potentielles entre les deux interfaces.

## Activités de workflows {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Activité non modifiable"
>abstract="Lorsqu’une activité **Requête** ou **Enrichissement** est paramétrée avec des données supplémentaires dans la console, les données d’enrichissement sont prises en compte dans Campaign Web et transmises à la transition sortante, mais elles ne peuvent pas être modifiées."

Les activités de workflow qui ne sont pas encore prises en charge dans l’interface d’utilisation web de Campaign sont en lecture seule et affichées en tant qu’activités incompatibles. Vous pouvez toujours exécuter le workflow, envoyer des messages, vérifier les journaux, etc. Les activités de workflow disponibles dans l’interface utilisateur web de Campaign et dans la console cliente Campaign sont modifiables.

| Console | Web |
| --- | --- |
| ![Capture d’écran montrant les limites des activités dans la console](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Capture d’écran montrant les limites des activités dans l’interface web](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Lorsqu’une activité **Requête** ou **Enrichissement** est paramétrée avec des données additionnelles dans la console, les données d’enrichissement sont prises en compte dans Campaign Web et transmises à la transition sortante, mais elles ne peuvent pas être éditées.

| Console | Web |
| --- | --- |
| ![Capture d’écran montrant les limites des options dans la console](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Capture d’écran montrant les limites des options dans l’interface web](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Dans la console, l’activité **Enrichissement** peut effectuer à la fois la réconciliation et l’enrichissement. Si vous avez défini des paramètres de réconciliation dans l’activité **Enrichissement** dans la console cliente, elle s’affichera en tant qu’activité **Réconciliation** dans l’interface d’utilisation de Campaign Web.

| Console | Web |
| --- | --- |
| ![Capture d’écran montrant l’activité d’enrichissement dans la console](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Capture d’écran montrant l’activité d’enrichissement dans l’interface web](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Zone de travail du workflow {#wkf-canvas}

Lors de la création d’un workflow dans l’interface utilisateur de Campaign Web, la zone de travail ne prend en charge qu’un seul point d’entrée. Toutefois, si vous avez créé un workflow dans la console avec plusieurs points d’entrée, vous pouvez l’ouvrir et le modifier dans l’interface d’utilisation de Campaign Web.

| Console | Web |
| --- | --- |
| ![Capture d’écran montrant plusieurs points d’entrée dans la console](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Capture d’écran montrant plusieurs points d’entrée dans l’interface web](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Le positionnement des nœuds est actualisé à chaque fois qu’une activité est ajoutée ou supprimée. Si vous créez un workflow dans la console, que vous le modifiez à l’aide de l’interface d’utilisation de Campaign Web et que vous le rouvrez dans la console, vous constaterez peut-être de légers problèmes de positionnement. Cela n’a aucun impact sur les processus et les tâches du workflow.

| Workflow initial | Changement de positionnement |
| --- | --- |
| ![Capture d’écran montrant le positionnement initial du workflow](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Capture d’écran montrant les changements de positionnement après modifications](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |