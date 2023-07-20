---
audience: end-user
title: Utiliser l’activité de workflow Rendez-vous
description: Découvrez comment utiliser l’activité de workflow Rendez-vous.
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '187'
ht-degree: 100%

---


# Rendez-vous {#join}

L’activité **Rendez-vous** est une activité de **contrôle de flux**. Elle vous permet de synchroniser plusieurs branches d’exécution d’un workflow.

L’activité Rendez-vous ne déclenche sa transition sortante qu’une fois toutes les transitions entrantes activées, c’est-à-dire quand toutes les activités précédentes sont terminées. Vous pouvez ainsi vous assurer que certaines activités sont terminées avant de continuer à exécuter le workflow.

## Configuration

Pour configurer l’activité **Rendez-vous**, procédez comme suit :

1. Ajoutez plusieurs activités telles que des activités de canal afin de former au moins deux branches d’exécution différentes.
1. Ajoutez une activité **Rendez-vous** à l’une des branches.
1. Dans les **Options de fusion**, cochez les activités précédentes à joindre.
1. Dans l’**Ensemble principal**, choisissez la population de transition entrante à conserver. La transition sortante ne peut contenir que l’une des populations de la transition entrante.

## Exemple

L’exemple ci-après montre deux branches d’un workflow avec une diffusion e-mail et SMS. L’activité Rendez-vous se déclenche lorsque les deux transitions entrantes sont activées. Les notifications push seront alors envoyées uniquement lorsque les deux diffusions seront terminées.

![](../assets/workflow-andjoin-example.png)