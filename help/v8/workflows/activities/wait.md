---
audience: end-user
title: Utilisation de l’activité de workflow d’attente
description: Découvrez comment utiliser l’activité de workflow d’attente
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 37%

---


# Attente {#wait}

Le **Attente** est une activité **Contrôle de flux** activité. Il permet de laisser un certain temps entre l’exécution de deux activités. Par exemple, attendre plusieurs jours après une activité de diffusion email puis analyser les ouvertures et les clics générés pendant ce laps de temps avant d&#39;appliquer d&#39;autres traitements (email de rappel, création d&#39;audience, etc.).

## Configuration 

Procédez comme suit pour configurer la variable **Attente** activité :

1. Ajouter un **Attente** dans votre workflow.

1. Spécifiez la variable **Durée** de l&#39;attente entre les transitions entrante et sortante.

1. Sélectionnez l’unité de temps dans la **Points** field : secondes, minutes, heures.

## Exemple

L&#39;exemple suivant illustre l&#39;activité **Attente** dans un cas typique. Un email d&#39;invitation à un événement est envoyé. 24 heures après son envoi, une diffusion SMS est envoyée à la même population.

![](../assets/workflow-wait-example.png)
