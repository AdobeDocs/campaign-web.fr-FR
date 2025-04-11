---
audience: end-user
title: Utiliser l’activité de workflow d’attente
description: Découvrez comment utiliser l’activité de workflow d’attente.
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 39%

---

# Attente {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Activité Attente"
>abstract="L’activité **Attente** permet de retarder la transition d’une activité à une autre."

L’activité d’**attente** est une activité de **contrôle de flux**. Il laisse un certain temps s’écouler entre l’exécution de deux activités. Elle peut par exemple être utilisée pour attendre plusieurs jours après une activité de diffusion email, puis analyser les ouvertures et les clics générés pendant cette période avant d&#39;effectuer des opérations de suivi, comme l&#39;envoi d&#39;un email de rappel ou la création d&#39;une audience.

## Configuration {#wait-configuration}

Pour configurer l’activité d’**attente**, procédez comme suit :

1. Ajoutez une activité d’**attente** dans votre workflow.

1. Spécifiez la **durée** de l’attente entre les transitions entrante et sortante.

1. Sélectionnez l’unité de temps dans le champ **Périodes** : secondes, minutes, heures ou jours.

## Exemple {#wait-example}

L’exemple suivant illustre l’activité **Attente** dans un cas typique. Un e-mail d’invitation à un événement est envoyé. Au bout de 24 heures, une diffusion SMS est envoyée à la même population.

![Exemple de workflow utilisant l’activité Attente pour envoyer un SMS 24 heures après une invitation par e-mail.](../assets/workflow-wait-example.png)