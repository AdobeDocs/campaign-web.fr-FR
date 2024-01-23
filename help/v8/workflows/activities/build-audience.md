---
audience: end-user
title: Utiliser l’activité de workflow Créer une audience
description: Découvrez comment utiliser l’activité de workflow Créer une audience.
badge: label="Disponibilité limitée"
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: 1435a8c2bc62e5064eaacf5e0cabf11d5642f152
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 92%

---

# Créer une audience {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Activité Créer une audience"
>abstract="L’activité **Créer une audience** permet de définir l’audience qui va entrer dans le workflow. Lors de l’envoi de messages dans le cadre d’un workflow, l’audience du message n’est pas définie dans l’activité de canal, mais dans l’activité **Créer une audience**."

L’activité **Créer une audience** est une activité de **ciblage**. Cette activité permet de définir l’audience qui va entrer dans le workflow. Lors de l’envoi de messages dans le cadre d’un workflow, l’audience du message n’est pas définie dans l’activité de canal, mais dans l’activité **Créer une audience**.

Pour définir la population de l’audience, vous pouvez :

* sélectionner une audience existante, créée sous forme de liste dans la console cliente ;
* sélectionner une audience Adobe Experience Platform ;
* Créez une audience à l’aide du concepteur de requêtes en définissant et combinant des critères de filtrage.

>[!NOTE]
>
>Les audiences chargées à partir d’un fichier ne peuvent pas être ciblées à l’aide d’une activité Créer une audience . Pour ce faire, vous devez utiliser une **Chargement de fichier** activité suivie d’une **Réconciliation** activité. [En savoir plus](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurer l’activité Créer une audience{#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Sélectionner la dimension de ciblage"
>abstract="La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, la cible est sélectionnée parmi les destinataires."

Pour configurer l’activité **Créer une audience**, procédez comme suit :

![](../assets/workflow-audience.png)

1. Ajoutez une activité **Créer une audience**.
1. Définissez un libellé.
1. Définissez le type d’audience : **Créer votre audience** ou **Lecture d’audience**.
1. Configurez votre audience en suivant les étapes présentées dans les onglets ci-dessous.

>[!BEGINTABS]

>[!TAB Créer votre propre (requête)]

Pour créer votre propre requête, procédez comme suit :

1. Sélectionnez **Créer la vôtre (requête)**.
1. Choisissez la **dimension de ciblage**. La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, la cible est sélectionnée parmi les destinataires. [En savoir plus sur les dimensions de ciblage](../../audience/about-recipients.md#targeting-dimensions)
1. Cliquez sur **Continuer**.
1. Utilisez le concepteur de requêtes pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un nouvel e-mail. [Découvrez comment utiliser le concepteur de requêtes](../../audience/../query/query-modeler-overview.md).

>[!TAB Lecture d’audience]

Pour sélectionner une audience existante, procédez comme suit :

1. Sélectionnez **Lecture d’audience**.
1. Cliquez sur **Continuer**.
1. Sélectionnez votre audience, de la même manière que vous utilisez une audience lors de la conception d’une nouvelle diffusion. Reportez-vous à cette [section](../../audience/add-audience.md).

>[!ENDTABS]

## Exemples{#build-audience-examples}

Voici un exemple de workflow avec deux activités **Créer une audience**. La première cible l’audience des joueurs et joueuses de poker, suivie d’une diffusion e-mail. La seconde cible l’audience des clientes et clients VIP, suivie d’une diffusion SMS.

![](../assets/workflow-audience-example.png)
