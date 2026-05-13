---
audience: end-user
title: Utiliser l’activité de workflow d’attente
description: Découvrez comment utiliser l’activité de workflow d’attente.
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
TQID: https://experienceleague.adobe.com/pe-T3-3w5HaS0pNOZITNC1YS5hiJpj3H3P1eM0GmXb8
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 185
ht-degree: 100%

---

# Attente {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Activité Attente"
>abstract="L’activité **Attente** est utilisée pour retarder la transition d’une activité à une autre."

L’activité d’**attente** est une activité de **contrôle de flux**. Elle est utilisée pour permettre qu’un certain temps s’écoule entre l’exécution de deux activités. Elle peut par exemple être utilisée pour attendre plusieurs jours après une activité de diffusion e-mail, puis analyser les ouvertures et les clics générés pendant cette période avant d’effectuer les opérations à suivre, comme l’envoi d’un e-mail de rappel ou la création d’une audience.

## Configuration {#wait-configuration}

Pour configurer l’activité d’**attente**, procédez comme suit :

1. Ajoutez une activité d’**attente** dans votre workflow.

1. Spécifiez la **durée** de l’attente entre les transitions entrante et sortante.

1. Sélectionnez l’unité de temps dans le champ **Périodes** : secondes, minutes, heures, jours.

## Exemple {#wait-example}

L’exemple suivant illustre l’activité **Attente** dans un cas typique. Un e-mail d’invitation à un événement est envoyé. Au bout de 24 heures, une diffusion SMS est envoyée à la même population.

![Exemple de workflow utilisant l’activité Attente pour envoyer un SMS 24 heures après une invitation par e-mail.](../assets/workflow-wait-example.png)