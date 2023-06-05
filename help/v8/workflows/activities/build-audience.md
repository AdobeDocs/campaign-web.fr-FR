---
audience: end-user
title: Utilisation de l’activité de workflow Créer l’audience
description: Découvrez comment utiliser l’activité de workflow Créer une audience
badge: label="Alpha" type="Positive"
source-git-commit: bdf569913dfcf9bee549c6ae3252f5a92a5f34e8
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 7%

---


# Créer une audience {#build-audience}

Le **Créer une audience** est une activité **Ciblage** activité. Cette activité permet de définir l&#39;audience qui va entrer dans le workflow. Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience du message n’est pas définie dans l’activité de canal, mais dans la variable **Créer une audience** activité.

Pour définir la population de l&#39;audience, vous pouvez :

* Sélectionnez une audience existante, créée sous forme de liste dans la console cliente.
* Sélectionnez une audience Adobe Experience Platform.
* Créez une nouvelle audience avec le créateur de règles en définissant et combinant des critères de filtrage.

>[!NOTE]
>
>Dans ce contexte, vous ne pouvez pas charger une audience à partir d’un fichier. Pour cela, vous devez créer une diffusion autonome. [En savoir plus](../../audience/about-audience.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuration

Procédez comme suit pour configurer la variable **Créer une audience** activité :

1. Ajouter un **Créer une audience** activité.
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

Voici un exemple de workflow avec deux **Créer une audience** activités. Le premier cible l&#39;audience des joueurs de poker, suivi d&#39;une diffusion email. La seconde cible l&#39;audience des clients VIP, suivie d&#39;une diffusion SMS.

![](../assets/workflow-audience-example.png)