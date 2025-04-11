---
audience: end-user
title: Utiliser les activités de workflows
description: Découvrez les activités de workflows.
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 54%

---

# À propos des activités de workflows {#workflow-activities}

Les activités de workflows sont regroupées en trois catégories. Selon le contexte, les activités disponibles peuvent différer.

Toutes les activités sont présentées dans les sections ci-dessous :

* [Activités de ciblage et de gestion des données](#targeting)
* [Activités de canal](#channel)
* [Activités de contrôle de flux](#flow-control)

![Présentation des activités de workflow](../assets/workflow-activities.png)

## Activités de ciblage {#targeting}

Ces activités sont spécifiques au ciblage. Elles vous permettent de créer une ou plusieurs audiences cibles en définissant une audience, puis en divisant ou en combinant ces audiences à l’aide des opérations d’intersection, d’union ou d’exclusion.

* [Créer une audience](build-audience.md) : définissez votre population cible. Sélectionnez une audience existante ou utilisez le modéliseur de requête pour définir votre propre requête.
* [Modifier la source de données](change-data-source.md) : modifiez la source de données de la table de travail de votre workflow.
* [Modifier la dimension](change-dimension.md) : modifiez la dimension de ciblage lors de la création de votre workflow.
* [Combiner](combine.md) : effectuez une segmentation sur votre population entrante. Utilisez une union, une intersection ou une exclusion.
* [Déduplication](deduplication.md) : permet de supprimer les doublons dans les résultats des activités entrantes.
* [Enrichissement](enrichment.md) : définissez des données supplémentaires à traiter dans votre workflow. Configurez l’activité pour terminer la transition sortante avec des données supplémentaires.
* [Requête incrémentale](incremental-query.md) : interrogez la base de données à des moments planifiés. Chaque fois que cette activité s’exécute, elle exclut les résultats des exécutions précédentes, et ne cible que les nouveaux éléments.
* [Réconciliation](reconciliation.md) : permet de définir le lien entre les données de la base Adobe Campaign et les données d&#39;une table de travail, telles que les données chargées à partir d&#39;un fichier externe.
* [Enregistrer l’audience](save-audience.md) : mettez à jour une audience existante ou créez une nouvelle audience à partir de la population calculée en amont dans un workflow.
* [Partage](split.md) : segmenter la population entrante en plusieurs sous-ensembles.

## Activités de gestion des données {#data}

Ces activités sont spécifiques à la manipulation et à l’enrichissement des données de population.

* [Extraction de fichier](extract-file.md) : exportez des données à partir d’Adobe Campaign vers un autre système sous la forme d’un fichier externe.
* [Chargement de fichier](load-file.md) : utilisez des profils et des données stockés dans un fichier externe.
* [Transfert de fichier](transfer-file.md) : recevez ou envoyez des fichiers, testez la présence de fichiers ou répertoriez les fichiers sur un serveur. Le protocole utilisé peut être soit un protocole serveur à serveur, soit un protocole HTTP.
* [Code JavaScript ](javascript-code.md) : exécutez un fragment de code JavaScript dans le cadre d’un workflow.
* [Services d’abonnement](subscription-services.md) : abonnez ou désabonnez plusieurs profils à un service en une seule action.
* [Mise à jour des données](update-data.md) : effectuez des mises à jour en masse des champs de la base de données. Plusieurs options vous permettent de personnaliser la mise à jour des données.

## Activités de canal {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux. Combinez les activités de canal dans la zone de travail pour créer des workflows cross-canal qui déclenchent des actions en fonction du comportement du client ou de la cliente. Les activités **Canal** suivantes sont disponibles : e-mail, SMS, Android et notifications push iOS. [Découvrez comment configurer une diffusion dans le contexte d’un workflow](channels.md).

## Activités de contrôle de flux {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Activité Fin"
>abstract="L’activité **Fin** vous permet de marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative."

Les activités ci-après sont spécifiques à l’organisation et à l’exécution du workflow. Leur principale tâche est de coordonner les autres activités :

* [Rendez-vous](and-join.md) : synchronisez plusieurs branches d’exécution d’un workflow.
* **Fin** : marque visuellement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative.
* [Signal externe](external-signal.md) : déclenchez l&#39;exécution d&#39;un workflow à partir d&#39;un autre workflow ou d&#39;un appel API.
* [Branchement](fork.md) : créez des transitions sortantes pour démarrer plusieurs activités simultanément.
* [Planificateur](scheduler.md) : planifiez le démarrage du workflow.
* [Test](test.md) : activez des transitions en fonction de conditions spécifiées.
* [Attente](wait.md) : suspendre temporairement l’exécution d’une partie d’un workflow.