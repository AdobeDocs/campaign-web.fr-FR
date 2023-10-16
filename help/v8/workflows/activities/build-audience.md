---
audience: end-user
title: Utiliser l’activité de workflow Créer une audience
description: Découvrez comment utiliser l’activité de workflow Créer une audience.
badge: label="Beta"
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: ht
source-wordcount: '478'
ht-degree: 100%

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
* créer une nouvelle audience avec le créateur de règles en définissant et combinant des critères de filtrage.

>[!NOTE]
>
>Dans ce contexte, vous ne pouvez pas charger d’audience à partir d’un fichier. Pour cela, vous devez créer une diffusion d’e-mail autonome. [En savoir plus](../../audience/about-recipients.md)

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

Pour créer votre propre requête, procédez comme suit :

1. Sélectionnez **Créer la vôtre (requête)**.
1. Choisissez la **dimension de ciblage**. La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, la cible est sélectionnée parmi les destinataires. Pour en savoir plus sur les dimensions de ciblage, veuillez consulter [cette section](../../audience/about-recipients.md#targeting-dimensions).
1. Cliquez sur **Continuer**.
1. Utilisez le créateur de règles pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un nouvel e-mail. Reportez-vous à cette [section](../../audience/segment-builder.md).

Pour sélectionner une audience existante, procédez comme suit :

1. Sélectionnez **Lecture d’audience**.
1. Cliquez sur **Continuer**.
1. Sélectionnez votre audience, de la même manière que vous utilisez une audience lors de la conception d’un e-mail. Reportez-vous à cette [section](../../audience/add-audience.md).

>[!IMPORTANT]
>
>Si vous souhaitez utiliser une activité **[!UICONTROL Créer une audience]** ciblant une audience Experience Platform, vous devez ajouter une activité **[!UICONTROL Changement de dimension]** après celle-ci, pour vous assurer que la dimension de ciblage de l’audience est définie sur Personne destinataire. Un exemple de workflow est disponible au bas de cette page.

## Exemples{#build-audience-examples}

Voici un exemple de workflow avec deux activités **Créer une audience**. La première cible l’audience des joueurs et joueuses de poker, suivie d’une diffusion e-mail. La seconde cible l’audience des clientes et clients VIP, suivie d’une diffusion SMS.

![](../assets/workflow-audience-example.png)

Voici un autre exemple de workflow dans lequel une audience Adobe Experience Platform est combinée à une audience Adobe Campaign. Pour combiner ces audiences, une activité **[!UICONTROL Changement de dimension]** avec la dimension de ciblage Personne destinataire est ajoutée après l’audience Adobe Experience Platform. [Découvrez comment configurer une activité Changement de dimension](change-dimension.md).

![](../assets/workflow-audience-aep.png)
