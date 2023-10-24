---
audience: end-user
title: Utiliser l’activité de workflow d’attente
description: Découvrez comment utiliser l’activité de workflow d’attente.
badge: label="Beta"
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 100%

---

# Attente {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Activité Attente"
>abstract="L’activité **Attente** est utilisée pour retarder la transition d’une activité à une autre."

L’activité d’**attente** est une activité de **contrôle de flux**. Elle est utilisée pour permettre qu’un certain temps s’écoule entre l’exécution de deux activités. Par exemple, elle permet d’attendre plusieurs jours après une activité de diffusion e-mail puis d’analyser les ouvertures et les clics générés pendant ce laps de temps avant d’appliquer d’autres traitements (e-mail de rappel, création d’audience, etc.).

## Configuration{#wait-configuration}

Pour configurer l’activité d’**attente**, procédez comme suit :

1. Ajoutez une activité d’**attente** dans votre workflow.

1. Spécifiez la **durée** de l’attente entre les transitions entrante et sortante.

1. Sélectionnez l’unité de temps dans le champ **Périodes** : secondes, minutes, heures.

## Exemple{#wait-example}

L’exemple suivant illustre l’activité **Attente** dans un cas typique. Un e-mail d’invitation à un événement est envoyé. 24 heures après son envoi, une diffusion SMS est envoyée à la même population.

![](../assets/workflow-wait-example.png)
