---
audience: end-user
title: Utilisation de l’activité de workflow Changement de dimension
description: Découvrez comment utiliser l’activité de workflow Changement de dimension
badge: label="Beta"
source-git-commit: 9bb80d10f20bb36162b74982d51ed67c1600f831
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 9%

---


# Changement de dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Générer un complémentaire"
>abstract="Vous pouvez générer une transition sortante supplémentaire avec la population restante, qui a été exclue en tant que doublon. Pour ce faire, activez l’option **Générer le complémentaire**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Activité Changement de dimension"
>abstract="Cette activité vous permet de modifier la dimension de ciblage à mesure que vous créez une audience. Il déplace l’axe en fonction du modèle de données et de la dimension d’entrée. Par exemple, vous pouvez passer de la dimension &quot;contrats&quot; à la dimension &quot;clients&quot;."

La variable **Changement de dimension** est une activité **Ciblage** activité. Cette activité permet de modifier la dimension de ciblage au fur et à mesure de la construction de votre workflow.
Cette activité déplace l’axe en fonction du modèle de données et de la dimension d’entrée.

Par exemple, vous pouvez passer la dimension de ciblage d&#39;un workflow de &quot;Destinataires&quot; à &quot;Application d&#39;abonnés&quot; afin d&#39;envoyer des notifications push aux destinataires ciblés.

## Configuration de l’activité Changement de dimension {#configure}

Pour configurer la variable **Changement de dimension** activité :

1. Ajouter un **Changement de dimension** à votre workflow.

   ![](../assets/workflow-change-dimension.png)

1. Définissez la variable **Nouvelle dimension cible**. Lors du changement de dimension, tous les enregistrements sont conservés. D’autres options ne sont pas encore disponibles.

1. Exécutez le workflow pour visualiser le résultat. Comparez les données des tables avant et après l&#39;activité de changement de dimension et comparez la structure des tables du workflow.

## Exemple {#example}

Dans cet exemple, nous souhaitons envoyer une diffusion SMS à tous les profils ayant effectué un achat. Pour ce faire, nous utilisons d’abord un **[!UICONTROL Créer une audience]** activité liée à une dimension de ciblage &quot;Achat&quot; personnalisée pour cibler tous les achats qui se sont produits.

Nous utilisons ensuite une **[!UICONTROL Changement de dimension]** pour changer la dimension de ciblage du workflow en &quot;Destinataires&quot;. Cela nous permet de cibler les destinataires qui correspondent à la requête.

![](../assets/workflow-change-dimension-example.png)

