---
audience: end-user
title: Utilisation des activités de workflows
description: Découvrez comment workflows des activités
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 40ca8ca9825706be7b82a58136627911132bc14a
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 27%

---


# À propos des activités de workflows {#workflow-activities}

Les activités de workflow sont regroupées en trois catégories. Selon le contexte, les activités disponibles peuvent différer.

Toutes les activités sont présentées dans les sections ci-dessous :

* [Activités de ciblage](#targeting)
* [Activités des canaux](#channel)
* [Activités de contrôle de flux](#flow-control)

![](../assets/workflow-activities.png)

## Activités de ciblage {#targeting}

Ces activités sont spécifiques au ciblage, à la manipulation et à l&#39;enrichissement des données sur la population. Ils permettent de construire une ou plusieurs cibles en définissant une audience et en partitionnant ou en combinant ces audiences à l’aide des opérations d’intersection, d’union ou d’exclusion.

* Le [Créer une audience](build-audience.md) activité vous permet de définir votre population cible. Vous pouvez sélectionner une audience existante ou utiliser le créateur de règles pour définir votre propre requête.
* Le [Combiner](combine.md) activité permet d’effectuer une segmentation sur votre population entrante. Vous pouvez utiliser une union, une intersection ou une exclusion.
* Le [Enrichissement](enrichment.md) activité vous permet de définir des données additionnelles à traiter dans votre workflow. Avec cette activité, vous pouvez utiliser la transition entrante et configurer l&#39;activité pour compléter la transition sortante avec des données additionnelles.

## Activités des canaux {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux, tels que les emails, les SMS ou les notifications push. Vous pouvez combiner des activités de canal dans la zone de travail afin de créer des processus cross-canal pouvant déclencher des actions en fonction du comportement du client.

Les éléments suivants **Canal** les activités sont disponibles :

* E-mail
* Push
* SMS

Reportez-vous à cette [section](enrichment.md).

## Activités de contrôle de flux {#flow-control}

Les activités ci-après sont spécifiques à l&#39;organisation et à l&#39;exécution du workflow. Leur principale tâche est de coordonner les autres activités:

* Le [Et rejoindre](and-join.md) permet de synchroniser plusieurs branches d&#39;exécution d&#39;un workflow.
* Le [Fin](end.md) vous permet de marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative.
* L&#39;activité [Branchement](fork.md) permet de créer des transitions sortantes afin de lancer plusieurs activités en parallèle.
* L&#39;activité [Attente](wait.md) permet de suspendre momentanément l&#39;exécution d&#39;une partie d&#39;un workflow.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

