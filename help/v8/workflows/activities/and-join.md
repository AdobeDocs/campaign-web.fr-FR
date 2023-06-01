---
audience: end-user
title: Utilisation de l’activité de workflow Rendez-vous
description: Découvrez comment utiliser l’activité de workflow Rendez-vous
badge: label="Alpha" type="Positive"
source-git-commit: 6ed2c73a5348871348ec4cbdd89fc8119fdbc718
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 21%

---


# Rendez-vous {#join}

Le **Et rejoindre** permet de synchroniser plusieurs branches d&#39;exécution d&#39;un workflow.

L&#39;activité Rendez-vous ne déclenche sa transition sortante qu&#39;une fois toutes les transitions entrantes activées, c&#39;est-à-dire quand toutes les activités précédentes sont terminées.

## Configuration

Procédez comme suit pour configurer la variable **AND-join** activité :

1. Ajoutez plusieurs activités, telles que **Combiner** pour former au moins deux branches d&#39;exécution différentes.
1. Ajoutez un **AND-join** à l’une des branches.
1. Dans le **Options de fusion** , vérifiez toutes les activités précédentes que vous souhaitez rejoindre.
1. Sélectionnez la **Principal** à conserver dans la transition sortante.

## Exemple

L&#39;exemple suivant montre deux branches d&#39;un workflow avec une diffusion email et SMS. La jointure ET se déclenche lorsque les deux transitions entrantes sont activées. Les notifications push seront alors envoyées uniquement une fois les deux diffusions terminées.

![](../assets/workflow-andjoin-example.png)