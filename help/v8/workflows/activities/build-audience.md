---
audience: end-user
title: Utilisation de l’activité de workflow Créer l’audience
description: Découvrez comment utiliser l’activité de workflow Créer une audience
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Créer une audience {#build-audience}

Cette activité permet de définir une audience. Vous pouvez sélectionner une audience existante ou utiliser le créateur de règles pour définir votre propre requête.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuration

Procédez comme suit pour configurer la variable **Créer une audience** activité :

1. Ajoutez une activité Créer une audience .
1. Définir un libellé.
1. Définissez le type d’audience : **Créez votre propre** ou **Lecture d’audience**.

Pour créer votre propre requête, procédez comme suit :

1. Sélectionner **Créez votre propre (requête)**.
1. Choisissez la **Dimension de ciblage**. La dimension de ciblage permet de définir la population ciblée par l&#39;opération : destinataires, bénéficiaires d&#39;un contrat, opérateur, abonnés, etc. Par défaut, la cible est sélectionnée parmi les destinataires. Reportez-vous à la section [Documentation v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Cliquez sur **Continuer**.
1. Utilisez le créateur de règles pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un nouvel email. Reportez-vous à cette [section](../../audience/segment-builder.md).

Pour sélectionner une audience existante, procédez comme suit :

1. Sélectionner **Lecture d’audience**.
1. Cliquez sur **Continuer**.
1. Sélectionnez votre audience, de la même manière que vous utilisez une audience lors de la conception d&#39;un nouvel email. Reportez-vous à cette [section](../../audience/add-audience.md).

## Exemple
