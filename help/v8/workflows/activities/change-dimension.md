---
audience: end-user
title: Utilisation de l’activité de workflow Changement de dimension
description: Découvrez comment utiliser l’activité de workflow Changement de dimension
badge: label="Beta"
source-git-commit: 253889459de03cf4df72be5a5fbc223588e9b86c
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 25%

---


# Changement de dimension {#change-dimension}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generate Complement"
>abstract="TBD"
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Changement de dimension activité"
>abstract="Cette activité vous permet de modifier la dimension de ciblage à mesure que vous créez une audience. Il déplace l’axe en fonction du modèle de données et de la dimension d’entrée. Par exemple, vous pouvez passer de la dimension &quot;contrats&quot; à la dimension &quot;clients&quot;."


La variable **Changement de dimension** est une activité **Ciblage** activité. Cette activité vous permet de modifier la dimension de ciblage à mesure que vous créez une audience. Cette activité déplace l’axe en fonction du modèle de données et de la dimension d’entrée. Par exemple, vous pouvez passer de la dimension &quot;contrats&quot; à la dimension &quot;clients&quot;.

Vous pouvez également utiliser cette activité pour définir les colonnes supplémentaires de la nouvelle cible et définir les critères de déduplication des données.

## Configuration

Pour configurer la variable **Changement de dimension** activité :

1. Ajouter un **Changement de dimension** à votre workflow.

   ![](../assets/workflow-change-dimension.png)

1. Définissez la variable **Nouvelle dimension cible**.

Lors du changement de dimension, tous les enregistrements sont conservés.