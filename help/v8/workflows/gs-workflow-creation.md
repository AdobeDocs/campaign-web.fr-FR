---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 53148300ecb5d52d89875519c44ae979d29a4d76
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 57%

---


# Principes fondamentaux de la création de workflows {#gs-workflow-creation}

Avec Campaign v8 Web, vous pouvez créer des workflows dans une zone de travail visuelle afin de concevoir des processus cross-canal tels que la segmentation, l’exécution de campagnes ou le traitement de fichiers.


## Quels sont les éléments d’un workflow ? {#gs-workflow-inside}

Le diagramme de workflow est une représentation de ce qui est censé se produire. Il décrit les différentes tâches à effectuer et la manière dont elles sont liées.

![](assets/workflow-example.png)

Chaque workflow comprend :

* **Activities**: une activité est une tâche à effectuer. Les différentes activités disponibles sont représentées sur le diagramme par des icônes. Chaque activité possède des propriétés spécifiques et d’autres propriétés communes à toutes les activités.

  Dans un diagramme de workflow, une même activité peut engendrer plusieurs tâches, notamment en cas de boucle ou d’actions récurrentes.

* **Transitions** : les transitions relient une activité source à une activité de destination et définissent leur ordre.

* **Tables de travail** : la table de travail contient toutes les informations véhiculées par la transition. Chaque workflow utilise plusieurs tables de travail. Les données véhiculées dans ces tables peuvent être utilisées tout au long du cycle de vie du workflow.

## Étapes clés de création d’un workflow {#gs-workflow-steps}


Les campagnes offrent deux manières de créer un workflow :

1. Les workflows peuvent être créés en tant que workflows autonomes à partir de la **Workflows** .

   ![](assets/create-a-standalone-wf.png)

1. Les workflows peuvent être créés directement au sein d&#39;une opération, à partir de la fonction **Workflow** de l&#39;opération. Lorsqu’il est inclus dans une campagne, le workflow est exécuté avec tous les autres workflows de la campagne et les mesures de création de rapports sont toutes regroupées au niveau de la campagne.

   ![](assets/create-a-wf-from-a-campaign.png)


Les étapes clés pour créer des workflows sont les suivantes :

![](assets/workflow-creation-process.png)

Ces étapes sont présentées dans la section suivante :

1. [Créer votre workflow et définir ses propriétés](create-workflow.md)
1. [Orchestration et configuration des activités](orchestrate-activities.md)
1. [Configuration des paramètres avancés de votre workflow](workflow-settings.md)
1. [Démarrer votre workflow et suivre son exécution](start-monitor-workflows.md)

