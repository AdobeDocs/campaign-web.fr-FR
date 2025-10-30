---
audience: end-user
title: Principes de base de la création de workflows
description: Découvrir les principes fondamentaux des workflows avec Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 100%

---

# Principes de base de la création de workflows {#gs-workflow-creation}

Avec Adobe Campaign Web, vous pouvez créer des workflows dans une zone de travail visuelle afin de concevoir des processus cross-canal tels que la segmentation, l’exécution de campagnes ou le traitement de fichiers.

## Quels sont les éléments d’un workflow ? {#gs-workflow-inside}

Le diagramme de workflow représente le processus planifié. Il décrit les différentes tâches à effectuer et la manière dont elles sont liées.

![Exemple de diagramme de workflow montrant les tâches et leurs connexions](assets/workflow-example.png){zoomable="yes"}

Chaque workflow comprend :

* des **Activités** : une activité est une tâche à effectuer. Les icônes du diagramme représentent les différentes activités. Chaque activité possède des propriétés spécifiques et des propriétés communes à toutes les activités.

  Dans un diagramme de workflow, une même activité peut engendrer plusieurs tâches, notamment en cas de boucle ou d’actions récurrentes.

* **Transitions** : les transitions relient une activité source à une activité de destination et définissent leur ordre.

* **Tables de travail** : la table de travail contient toutes les informations véhiculées par la transition. Chaque workflow utilise plusieurs tables de travail. Les données transmises dans ces tableaux peuvent être utilisées tout au long du cycle de vie du workflow.

## Étapes essentielles pour créer un workflow {#gs-workflow-steps}

Les campagnes offrent deux manières de créer un workflow :

1. Les workflows peuvent être créés en tant que workflows autonomes à partir du menu **Workflows**.

   ![Capture d’écran de l’interface de création d’un workflow autonome](assets/create-a-standalone-wf.png){zoomable="yes"}

1. Les workflows peuvent être créés directement dans une campagne, à partir de l’onglet **Workflow** de la campagne. Lorsqu’il est inclus dans une campagne, le workflow est exécuté avec tous les autres workflows de la campagne et les mesures de rapports sont toutes regroupées au niveau de la campagne.

   ![Capture d’écran de l’interface de création d’un workflow dans une campagne](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

Pour créer des workflows, procédez comme suit :

![Diagramme illustrant le processus de création de workflow](assets/workflow-creation-process.png){zoomable="yes"}

Ces étapes sont détaillées dans les sections suivantes :

1. [Créer votre workflow et définir ses propriétés](create-workflow.md)
1. [Orchestrer et configurer des activités](orchestrate-activities.md)
1. [Configurer les paramètres avancés de votre workflow](workflow-settings.md)
1. [Démarrer votre workflow et surveiller son exécution](start-monitor-workflows.md)