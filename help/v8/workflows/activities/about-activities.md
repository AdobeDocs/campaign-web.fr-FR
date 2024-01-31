---
audience: end-user
title: Utiliser les activités de workflows
description: Découvrez les activités de workflows.
badge: label="Disponibilité limitée"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: ht
source-wordcount: '465'
ht-degree: 100%

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

* Utilisez l’activité [Enregistrer l’audience](save-audience.md) pour mettre à jour une audience existante ou créer une nouvelle audience à partir de la population calculée en amont dans un workflow.
* Utilisez l’activité [Créer une audience](build-audience.md) pour définir votre population cible. Vous pouvez sélectionner une audience existante ou utiliser le concepteur de requête pour définir votre propre requête.
* Utilisez l’activité [Combiner](combine.md) pour effectuer une segmentation sur votre population entrante. Vous pouvez utiliser une union, une intersection ou une exclusion.
* Utilisez l’activité [Partage](split.md) pour segmenter la population entrante en plusieurs sous-ensembles.
* Utilisez l’activité [Réconciliation](reconciliation.md) pour définir le lien entre les données dans la base de données Adobe Campaign et les données dans une table de travail, par exemple les données chargées à partir d’un fichier externe.
* Utilisez l’activité [Enrichissement](enrichment.md) pour définir des données supplémentaires à traiter dans votre workflow. Avec cette activité, vous pouvez utiliser la transition entrante et configurer l’activité pour ajouter des données supplémentaires à la transition sortante.
* Utilisez l’activité [Déduplication](deduplication.md) pour supprimer les doublons dans le ou les résultats des activités entrantes.
* Utilisez l’activité [Changement de dimension](change-dimension.md) pour modifier la dimension de ciblage au fur et à mesure que vous créez votre workflow.
* Utilisez la variable [Chargement de fichier](load-file.md) pour utiliser des profils et des données stockés dans un fichier externe.


## Activités de canal {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux. Vous pouvez combiner des activités de canal dans la zone de travail afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement du client ou de la cliente. Les activités **Canal** suivantes sont disponibles : e-mail, SMS, notifications push Android et iOS. [Découvrez comment configurer une diffusion dans le contexte d’un workflow](channels.md).

## Activités de contrôle de flux {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Activité Fin"
>abstract="L’activité **Fin** vous permet de marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative."

Les activités ci-après sont spécifiques à l’organisation et à l’exécution du workflow. Leur principale tâche est de coordonner les autres activités :

* Utilisez l’activité [Planificateur](scheduler.md) pour planifier le démarrage du workflow.
* Utilisez l’activité [Rendez-vous](and-join.md) pour synchroniser plusieurs branches d’exécution d’un workflow.
* Ajoutez une activité **Fin** pour marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative.
* Utilisez l’activité [Branchement](fork.md) pour créer des transitions sortantes afin de lancer plusieurs activités en parallèle.
* Ajoutez une activité [Attente](wait.md) pour suspendre momentanément l’exécution d’une partie d’un workflow.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

