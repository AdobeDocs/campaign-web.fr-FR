---
audience: end-user
title: Utilisation de l’activité de workflow Changement de dimension
description: Découvrez comment utiliser l’activité de workflow Changement de dimension
badge: label="Beta"
source-git-commit: 9b945dcd4151e536e8a8be904100730c86e483b7
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 13%

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

La variable **Changement de dimension** est une activité **Ciblage** activité. Cette activité vous permet de modifier la dimension de ciblage à mesure que vous créez une audience. Cette activité déplace l’axe en fonction du modèle de données et de la dimension d’entrée. Par exemple, vous pouvez passer de la dimension &quot;contrats&quot; à la dimension &quot;clients&quot;.

## Configuration

Pour configurer la variable **Changement de dimension** activité :

1. Ajouter un **Changement de dimension** à votre workflow.

   ![](../assets/workflow-change-dimension.png)

1. Définissez la variable **Nouvelle dimension cible**. Lors du changement de dimension, tous les enregistrements sont conservés. D’autres options ne sont pas encore disponibles.

1. Exécutez le workflow pour visualiser le résultat. Comparez les données des tables avant et après l&#39;activité de changement de dimension et comparez la structure des tables du workflow.



