---
audience: end-user
title: Utiliser l’activité de workflow Changement de dimension
description: Découvrez comment utiliser l’activité de workflow Changement de dimension.
badge: label="Beta"
source-git-commit: 2894766336d5ac52625175981c6969a0ac5882d8
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 100%

---


# Changement de dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Générer un complémentaire"
>abstract="Vous pouvez générer une transition sortante supplémentaire avec la population restante, qui a été exclue en tant que doublon. Pour ce faire, activez l’option **Générer le complémentaire**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Activité Changement de dimension"
>abstract="Cette activité vous permet de modifier la dimension de ciblage à mesure que vous créez une audience. Elle déplace l’axe en fonction du modèle de données et de la dimension d’entrée. Par exemple, vous pouvez passer de la dimension « contrats » à la dimension « clientèle »."

L’activité **Changement de dimension** est une activité de **ciblage**. Cette activité permet de modifier la dimension de ciblage au fur et à mesure de la construction de votre workflow. Elle déplace l’axe en fonction du modèle de données et de la dimension d’entrée. [En savoir plus sur les dimensions de ciblage](../../audience/about-recipients.md#targeting-dimensions)

Par exemple, vous pouvez passer de la dimension de ciblage d’un workflow « Personnes destinataires » à « Application des abonnées et abonnés » afin d’envoyer des notifications push aux personnes destinataires ciblées.

## Configurer l’activité Changement de dimension {#configure}

Pour configurer l’activité **Changement de dimension**, procédez comme suit :

1. Ajoutez une activité **Changement de dimension** à votre workflow.

   ![](../assets/workflow-change-dimension.png)

1. Définissez la **Nouvelle dimension cible**. Lors du changement de dimension, tous les enregistrements sont conservés. D’autres options ne sont pas encore disponibles.

1. Exécutez le workflow pour visualiser le résultat. Comparez les données contenues dans les tables avant et après l’activité Changement de dimension, puis comparez la structure des tables du workflow.

## Exemple {#example}

Dans cet exemple, nous souhaitons envoyer une diffusion SMS à tous les profils ayant effectué un achat. Pour ce faire, nous utilisons d’abord une activité **[!UICONTROL Créer une audience]** liée à une dimension de ciblage « Achat » personnalisée pour cibler tous les achats qui se sont produits.

Nous utilisons ensuite une activité **[!UICONTROL Changement de dimension]** pour changer la dimension de ciblage du workflow sur « Personnes destinataires ». Cela nous permet de cibler les personnes destinataires qui correspondent à la requête.

![](../assets/workflow-change-dimension-example.png)
