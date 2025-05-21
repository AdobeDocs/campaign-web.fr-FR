---
audience: end-user
title: Utiliser les activités de workflows
description: Découvrez les activités de workflows.
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 100%

---

# À propos des activités de workflows {#workflow-activities}

Les activités de workflows sont regroupées en trois catégories. Selon le contexte, les activités disponibles peuvent différer.

Toutes les activités sont présentées dans les sections ci-dessous :

* [Activités de ciblage et de gestion des données](#targeting)
* [Activités de canal](#channel)
* [Activités de contrôle de flux](#flow-control)

![Vue d’ensemble des activités de workflows](../assets/workflow-activities.png)

## Activités de ciblage {#targeting}

Ces activités sont spécifiques au ciblage. Elles permettent de créer une ou plusieurs audiences cibles en définissant une audience, puis en divisant ou en combinant ces audiences à l’aide des opérations d’intersection, d’union ou d’exclusion.

* [Créer une audience](build-audience.md) : définissez votre population cible. Sélectionnez une audience existante ou utilisez le concepteur de requête pour définir votre propre requête.
* [Modifier la source de données](change-data-source.md) : modifiez la source de données de la table de travail de votre workflow.
* [Changement de dimension](change-dimension.md) : modifiez la dimension de ciblage lors de la création de votre workflow.
* [Combiner](combine.md) : effectuez une segmentation sur votre population entrante. Utilisez une union, une intersection ou une exclusion.
* [Déduplication](deduplication.md) : supprimez les doublons dans les résultats des activités entrantes.
* [Enrichissement](enrichment.md) : définissez des données supplémentaires à traiter dans votre workflow. Configurez l’activité pour terminer la transition sortante avec des données supplémentaires.
* [Requête incrémentale](incremental-query.md) : interrogez la base de données à des moments planifiés. Chaque fois que cette activité s’exécute, elle exclut les résultats des exécutions précédentes, et ne cible que les nouveaux éléments.
* [Réconciliation](reconciliation.md) : définissez le lien entre les données de la base de données d’Adobe Campaign et les données d’une table de travail, par exemple les données chargées à partir d’un fichier externe.
* [Enregistrer l’audience](save-audience.md) : mettez à jour une audience existante ou créez une nouvelle audience à partir de la population calculée en amont dans un workflow.
* [Partage](split.md) : segmentez la population entrante en plusieurs sous-ensembles.

## Activités de gestion des données {#data}

Ces activités sont spécifiques à la manipulation et à l’enrichissement des données de population.

* [Extraction de fichier](extract-file.md) : exportez des données à partir d’Adobe Campaign vers un autre système sous la forme d’un fichier externe.
* [Chargement de fichier](load-file.md) : utilisez des profils et des données stockés dans un fichier externe.
* [Transfert de fichier](transfer-file.md) : recevez ou envoyez des fichiers, testez la présence de fichiers ou répertoriez les fichiers sur un serveur. Le protocole utilisé peut être soit un protocole serveur à serveur, soit un protocole HTTP.
* [Code JavaScript](javascript-code.md) : exécutez un fragment de code JavaScript dans le contexte d’un workflow.
* [Services d’abonnement](subscription-services.md) : abonnez plusieurs profils à un service ou désabonnez-les de ce service en une seule action.
* [Mise à jour des données](update-data.md) : effectuez des mises à jour en masse des champs de la base de données. Plusieurs options vous permettent de personnaliser la mise à jour des données.

## Activités de canal {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux. Combinez des activités de canal dans la zone de travail afin de créer des workflows cross-canal qui déclenchent des actions en fonction du comportement du client ou de la cliente. Les activités **Canal** suivantes sont disponibles : e-mail, SMS, notifications push Android et iOS. [Découvrez comment configurer une diffusion dans le contexte d’un workflow](channels.md).

## Activités de contrôle de flux {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Activité Fin"
>abstract="L’activité **Fin** vous permet de marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative."

Les activités ci-après sont spécifiques à l’organisation et à l’exécution du workflow. Leur principale tâche est de coordonner les autres activités :

* [Rendez-vous](and-join.md) : synchronisez plusieurs branches d’exécution d’un workflow.
* **Fin** : marque visuellement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative.
* [Signal externe](external-signal.md) : déclenchez l’exécution d’un workflow à partir d’un autre workflow ou d’un appel API.
* [Branchement](fork.md) : créez des transitions sortantes afin de lancer plusieurs activités simultanément.
* [Planificateur](scheduler.md) : planifiez le moment de démarrage du workflow.
* [Test](test.md) : activez des transitions en fonction de conditions spécifiées.
* [Attente](wait.md) : suspendez temporairement l’exécution d’une partie d’un workflow.