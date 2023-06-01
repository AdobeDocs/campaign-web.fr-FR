---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 748fef18a91a61f5ed956f65762a979e7dacabf3
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 73%

---


# Principes fondamentaux de la création de workflows {#gs-workflow-creation}

Avec Campaign v8 Web, vous pouvez créer des workflows dans une zone de travail visuelle afin de concevoir des processus cross-canal tels que la segmentation, l’exécution de campagnes ou le traitement de fichiers.

Les workflows peuvent être créés en tant que workflows autonomes, depuis le menu Workflows , ou directement au sein d&#39;une opération. Dans ce cas, le workflow sera associé à l&#39;opération et exécuté avec tous les workflows des autres opérations.

## Quels sont les éléments d’un workflow ?

Le diagramme de workflow est une représentation de ce qui est censé se produire. Il décrit les différentes tâches à effectuer et la manière dont elles sont liées.

![](assets/workflow-example.png)

Chaque workflow comprend :

* **Activities**: une activité est une tâche à effectuer. Les différentes activités disponibles sont représentées sur le diagramme par des icônes. Chaque activité possède des propriétés spécifiques et d’autres propriétés communes à toutes les activités.

   Dans un diagramme de workflow, une même activité peut engendrer plusieurs tâches, notamment en cas de boucle ou d’actions récurrentes.

* **Transitions** : les transitions relient une activité source à une activité de destination et définissent leur ordre.

* **Tables de travail** : la table de travail contient toutes les informations véhiculées par la transition. Chaque workflow utilise plusieurs tables de travail. Les données véhiculées dans ces tables peuvent être utilisées tout au long du cycle de vie du workflow.

## Procédure de création d’un workflow

Pour créer un workflow, procédez comme suit :

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="prospect" src="assets/do-not-localize/workflow-process-1 .jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>Créer le workflow</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="Peu fréquent" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>Orchestration des activités</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="Validation" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>Configuration des paramètres avancés (facultatif)</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="démarrage et surveillance des workflows" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>Démarrer et suivre l'exécution du workflow</strong></a>
</div>
<p>
</td>
</tr></table>