---
title: Barrières de sécurité et limitations des workflows de l'interface utilisateur Web de Campaign
description: Barrières de sécurité et limitations lors de l'utilisation de workflows dans l'interface utilisateur Web de Campaign
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 19864179f02d39583cc90d42bf6ab677f4841600
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 93%

---

# Barrières de sécurité et limites des workflows {#guardrails-limitations}

Lorsque vous utilisez l’interface utilisateur web de Campaign avec des workflows créés ou modifiés dans la console cliente Campaign, les mécanismes de sécurisation et les limitations ci-dessous s’appliquent.

Veuillez noter que, bien que cette page identifie les points essentiels à prendre en compte lors de l’utilisation des workflows dans la console et l’interface utilisateur web, elle n’englobe pas toutes les incompatibilités potentielles entre les deux interfaces.

## Activités de workflows {#wkf-activities}

Les activités de workflow qui ne sont pas encore prises en charge dans Campaign Web sont en lecture seule et s’affichent en tant qu’activités incompatibles. Vous pouvez toujours exécuter le workflow, envoyer des messages, vérifier les journaux, etc. Les activités de workflow disponibles dans Campaign Web et dans la console cliente sont modifiables.

Les activités de workflow qui ne sont pas encore prises en charge dans l’interface utilisateur web de Campaign sont en lecture seule et affichées en tant qu’activités incompatibles. Vous pouvez toujours exécuter le workflow, envoyer des messages, vérifier les journaux, etc. Les activités de workflow disponibles dans l’interface utilisateur web de Campaign et dans la console cliente Campaign sont modifiables.

| Console | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

Lorsqu’une activité **Requête** ou **Enrichissement** est paramétrée avec des données additionnelles dans la console, les données d’enrichissement sont prises en compte dans Campaign Web et transmises à la transition sortante, mais elles ne peuvent pas être éditées.

| Console | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

Dans la console, l’activité **Enrichissement** peut effectuer à la fois la réconciliation et l’enrichissement. Dans la console, si vous avez défini des paramètres de réconciliation dans l’activité **Enrichissement**, celle-ci s’affiche en tant qu’activité **Réconciliation** dans l’interface utilisateur web de Campaign.

| Console | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

## Zone de travail du workflow {#wkf-canvas}

Lors de la création d’un workflow dans l’interface utilisateur de Campaign Web, la zone de travail ne prend en charge qu’un seul point d’entrée. Cependant, si vous avez créé un workflow dans la console avec plusieurs points d’entrée, vous pouvez l’ouvrir et le modifier dans l’interface utilisateur web de Campaign.

| Console | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

Le positionnement des nœuds est actualisé à chaque fois qu’une activité est ajoutée ou supprimée. Si vous créez un workflow dans la console, que vous le modifiez à l’aide de l’interface utilisateur web de Campaign et que vous le rouvrez dans la console, vous constaterez peut-être des imperfections mineures du positionnement. Cela n’a aucun impact sur les processus et les tâches du workflow.

| Workflow initial | Changement de positionnement |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |
