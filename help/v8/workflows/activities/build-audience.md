---
audience: end-user
title: Utiliser l’activité de workflow Créer une audience
description: Découvrez comment utiliser l’activité de workflow Créer une audience.
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 97%

---


# Créer une audience {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Créer une audience"
>abstract="L’activité **Créer une audience** est une activité de **ciblage**. Cette activité permet de définir l’audience qui va entrer dans le workflow."


L’activité **Créer une audience** est une activité de **ciblage**. Cette activité permet de définir l’audience qui va entrer dans le workflow. Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience du message n’est pas définie dans l’activité de canal, mais dans l’activité **Créer une audience**.

Pour définir la population de l’audience, vous pouvez :

* sélectionner une audience existante, créée sous forme de liste dans la console cliente ;
* sélectionner une audience Adobe Experience Platform ;
* créer une nouvelle audience avec le créateur de règles en définissant et combinant des critères de filtrage.

>[!NOTE]
>
>Dans ce contexte, vous ne pouvez pas charger d’audience à partir d’un fichier. Pour cela, vous devez créer une diffusion autonome. [En savoir plus](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuration de l’activité de création d’audience

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Sélectionner la dimension de ciblage"
>abstract="La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, la cible est sélectionnée parmi les destinataires."


Pour configurer l’activité **Créer une audience**, procédez comme suit :

1. Ajoutez une activité **Créer une audience**.
1. Définissez un libellé.
1. Définissez le type d’audience : **Créer votre audience** ou **Lecture d’audience**.

Pour créer votre propre requête, procédez comme suit :

1. Sélectionnez **Créer la vôtre (requête)**.
1. Choisissez la **dimension de ciblage**. La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, la cible est sélectionnée parmi les destinataires. Consultez la [documentation v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=fr#targeting-and-filtering-dimensions){target="_blank"}.
1. Cliquez sur **Continuer**.
1. Utilisez le créateur de règles pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un nouvel e-mail. Reportez-vous à cette [section](../../audience/segment-builder.md).

Pour sélectionner une audience existante, procédez comme suit :

1. Sélectionnez **Lecture d’audience**.
1. Cliquez sur **Continuer**.
1. Sélectionnez votre audience, de la même manière que vous utilisez une audience lors de la conception d’un e-mail. Reportez-vous à cette [section](../../audience/add-audience.md).

## Exemple

Voici un exemple de workflow avec deux activités **Créer une audience**. La première cible l’audience des joueurs et joueuses de poker, suivie d’une diffusion e-mail. La seconde cible l’audience des clientes et clients VIP, suivie d’une diffusion SMS.

![](../assets/workflow-audience-example.png)