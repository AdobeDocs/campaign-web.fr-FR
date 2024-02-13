---
audience: end-user
title: Principes fondamentaux de la création de workflows
description: Découvrir les principes fondamentaux des workflows avec Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 98%

---


# Principes fondamentaux de la création de workflows {#gs-workflow-creation}

Avec Adobe Campaign Web, vous pouvez créer des workflows dans une zone de travail visuelle afin de concevoir des processus cross-canal tels que la segmentation, l’exécution de campagnes ou le traitement de fichiers.


## Quels sont les éléments d’un workflow ? {#gs-workflow-inside}

Le diagramme de workflow est une représentation de ce qui est censé se produire. Il décrit les différentes tâches à effectuer et la manière dont elles sont liées.

![](assets/workflow-example.png){zoomable=&quot;yes&quot;} {zoomable=&quot;yes&quot;}

Chaque workflow comprend :

* des **Activités** : une activité est une tâche à effectuer. Les différentes activités disponibles sont représentées sur le diagramme par des icônes. Chaque activité possède des propriétés spécifiques et d’autres propriétés communes à toutes les activités.

  Dans un diagramme de workflow, une même activité peut engendrer plusieurs tâches, notamment en cas de boucle ou d’actions récurrentes.

* **Transitions** : les transitions relient une activité source à une activité de destination et définissent leur ordre.

* **Tables de travail** : la table de travail contient toutes les informations véhiculées par la transition. Chaque workflow utilise plusieurs tables de travail. Les données transmises dans ces tableaux peuvent être utilisées tout au long du cycle de vie du workflow.

## Étapes essentielles pour créer un workflow {#gs-workflow-steps}


Les campagnes offrent deux manières de créer un workflow :

1. Les workflows peuvent être créés en tant que workflows autonomes à partir du menu **Workflows**.

   ![](assets/create-a-standalone-wf.png){zoomable=&quot;yes&quot;}

1. Les workflows peuvent être créés directement au sein d’une campagne, à partir de l’onglet **Workflow** de la campagne. Lorsqu’il est inclus dans une campagne, le workflow est exécuté avec tous les autres workflows de la campagne et les mesures de rapports sont toutes regroupées au niveau de la campagne.

   ![](assets/create-a-wf-from-a-campaign.png){zoomable=&quot;yes&quot;}


Pour créer des workflows, procédez comme suit :

![](assets/workflow-creation-process.png){zoomable=&quot;yes&quot;}

Ces étapes sont détaillées dans la section suivante :

1. [Créer votre workflow et définir ses propriétés](create-workflow.md)
1. [Orchestrer et configurer des activités](orchestrate-activities.md)
1. [Configurer les paramètres avancés de votre workflow](workflow-settings.md)
1. [Démarrer votre workflow et surveiller son exécution](start-monitor-workflows.md)
