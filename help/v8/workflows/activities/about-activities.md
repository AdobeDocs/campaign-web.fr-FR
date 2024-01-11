---
audience: end-user
title: Utiliser les activités de workflows
description: Découvrez les activités de workflows.
badge: label="Disponibilité limitée"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 35%

---


# À propos des activités de workflows {#workflow-activities}

Les activités de workflows sont regroupées en trois catégories. Selon le contexte, les activités disponibles peuvent différer.

Toutes les activités sont présentées dans les sections ci-dessous :

* [Activités de ciblage et de gestion des données](#targeting)
* [Activités de canal](#channel)
* [Activités de contrôle de flux](#flow-control)

![](../assets/workflow-activities.png)

## Activités de ciblage et de gestion des données {#targeting}

Ces activités sont spécifiques au ciblage, à la manipulation et à l’enrichissement des données relatives à la population. Elles permettent de construire une ou plusieurs cibles en définissant une audience, puis en partageant ou en combinant ces audiences à l’aide des opérations d’intersection, d’union ou d’exclusion.

* Utilisez la variable [Sauvegarde d’audience](save-audience.md) pour mettre à jour une audience existante ou créer une nouvelle audience à partir de la population calculée en amont dans un workflow.
* Utilisez la variable [Créer une audience](build-audience.md) activité pour définir votre population cible. Vous pouvez sélectionner une audience existante ou utiliser le modèle de requête pour définir votre propre requête.
* Utilisez la variable [Combiner](combine.md) pour effectuer une segmentation sur votre population entrante. Vous pouvez utiliser une union, une intersection ou une exclusion.
* Utilisez la variable [Partage](split.md) pour segmenter la population entrante en plusieurs sous-ensembles.
* Utilisez la variable [Réconciliation](reconciliation.md) pour définir le lien entre les données de la base Adobe Campaign et les données d&#39;une table de travail, par exemple les données chargées à partir d&#39;un fichier externe.
* Utilisez la variable [Enrichissement](enrichment.md) pour définir des données additionnelles à traiter dans votre workflow. Avec cette activité, vous pouvez utiliser la transition entrante et configurer l’activité pour ajouter des données supplémentaires à la transition sortante.
* Utilisez la variable [Déduplication](deduplication.md) activité de suppression des doublons dans le ou les résultats des activités entrantes.
* Utilisez la variable [Changement de dimension](change-dimension.md) pour modifier la dimension de ciblage au fur et à mesure de la construction de votre workflow.
* Utilisez la variable [Chargement de fichier](load-file.md) pour travailler avec des profils et des données stockés dans un fichier externe.


## Activités de canal {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux. Vous pouvez combiner des activités de canal dans la zone de travail afin de créer des processus cross-canal pouvant déclencher des actions en fonction du comportement du client. Les éléments suivants **Canal** Les activités sont disponibles : email, SMS, Android et notifications push iOS. [Découvrez comment configurer une diffusion dans le contexte d&#39;un workflow](channels.md).

## Activités de contrôle de flux {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Activité Fin"
>abstract="L’activité **Fin** vous permet de marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative."

Les activités ci-après sont spécifiques à l’organisation et à l’exécution du workflow. Leur principale tâche est de coordonner les autres activités :

* Utilisez la variable [Planificateur](scheduler.md) activité pour planifier le démarrage du workflow.
* Utilisez la variable [Et rejoindre](and-join.md) pour synchroniser plusieurs branches d&#39;exécution d&#39;un workflow.
* Ajoutez un **Fin** pour marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative.
* Utilisez la variable [Branchement](fork.md) pour créer des transitions sortantes afin de lancer simultanément plusieurs activités.
* Ajouter un [Attente](wait.md) pour suspendre momentanément l’exécution d’une partie d’un workflow.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

