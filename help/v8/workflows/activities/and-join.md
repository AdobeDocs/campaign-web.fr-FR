---
audience: end-user
title: Utiliser l’activité de workflow Rendez-vous
description: Découvrez comment utiliser l’activité de workflow Rendez-vous.
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 100%

---

# Rendez-vous {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Activité Rendez-vous"
>abstract="L’activité **Rendez-vous** vous permet de synchroniser plusieurs branches d’exécution d’un workflow. Elle est déclenchée une fois toutes les activités précédentes terminées. Vous pouvez ainsi vous assurer que certaines activités sont terminées avant de continuer à exécuter le workflow."

L’activité **Rendez-vous** est une activité de **contrôle de flux**. Elle vous permet de synchroniser plusieurs branches d’exécution d’un workflow.

L’activité Rendez-vous ne déclenche sa transition sortante qu’une fois toutes les transitions entrantes activées, c’est-à-dire quand toutes les activités précédentes sont terminées. Vous pouvez ainsi vous assurer que certaines activités sont terminées avant de continuer à exécuter le workflow.

## Configurer l’activité Rendez-vous{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Options de fusion"
>abstract="Sélectionnez les activités auxquelles vous souhaitez adhérer. Dans l’**Ensemble principal**, choisissez la population de transition entrante à conserver."

Pour configurer l’activité **Rendez-vous**, procédez comme suit :

![](../assets/workflow-andjoin.png)

1. Ajoutez plusieurs activités telles que des activités de canal afin de former au moins deux branches d’exécution différentes.
1. Ajoutez une activité **Rendez-vous** à l’une des branches.
1. Dans les **Options de fusion**, cochez les activités précédentes à joindre.
1. Dans l’**Ensemble principal**, choisissez la population de transition entrante à conserver. La transition sortante ne peut contenir que l’une des populations de la transition entrante.

## Exemple{#and-join-example}

L’exemple ci-après montre deux branches d’un workflow avec une diffusion e-mail et SMS. L’activité Rendez-vous se déclenche lorsque les deux transitions entrantes sont activées. Les notifications push seront alors envoyées uniquement lorsque les deux diffusions seront terminées.

![](../assets/workflow-andjoin-example.png){zoomable="yes"}
