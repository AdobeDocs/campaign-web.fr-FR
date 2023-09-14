---
audience: end-user
title: Utilisation de l’activité de workflow Sauvegarde d’audience
description: Découvrez comment utiliser l’activité de workflow Branchement.
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 17%

---


# Sauvegarde d&#39;audience {#save-audience}

<!--
>[!CONTEXTUALHELP]
>id="???"
>title="Save audience activity"
>abstract="The Save audience activity allows you to..."
-->

La variable **Sauvegarde d’audience** est une activité **Ciblage** activité. Cette activité permet de mettre à jour une audience existante ou de créer une nouvelle audience à partir de la population calculée en amont dans un workflow. Les audiences créées sont ajoutées à la liste des audiences de l&#39;application et mises à disposition via le **Audiences** .

Cette activité est essentiellement utilisée pour conserver les groupes de population calculés dans le même workflow, en les convertissant en audiences réutilisables. Connectez-la à d’autres activités de ciblage telles qu’une **Créer une audience** ou **Combiner** activité.

## Configuration

Pour configurer la variable **Sauvegarde d’audience** activité :

1. Ajouter un **Sauvegarde d’audience** à votre workflow.

   ![](../assets/workflow-save-audience.png)

1. Dans le **Mode** , sélectionnez l’action que vous souhaitez réaliser :

   * **Créer ou mettre à jour une audience existante**: définissez une **Libellé de l’audience**. Si l’audience existe déjà, elle est mise à jour, sinon une nouvelle audience est créée.

   * **Mettre à jour une audience existante**: sélectionnez la variable **Audience** vous souhaitez mettre à jour parmi la liste des audiences existantes.

1. Sélectionnez la variable **Mode de mise à jour** qui s’appliquera aux audiences existantes :

   * **Remplacer le contenu de l’audience par de nouvelles données**: tout le contenu de l’audience est remplacé. Les anciennes données sont perdues. Seules les données issues de la transition entrante de l&#39;activité de sauvegarde d&#39;audience sont conservées. Cette option supprime le type d&#39;audience et la dimension de ciblage de l&#39;audience mise à jour.

   * **Compléter l’audience avec les nouvelles données**: l&#39;ancien contenu de l&#39;audience est conservé et les données de la transition entrante de l&#39;activité de sauvegarde d&#39;audience y sont ajoutées.

1. Vérifiez les **Générer le complémentaire** si vous souhaitez exploiter la population restante. Une transition supplémentaire sera alors ajoutée à l&#39;activité.

Le contenu de l&#39;audience sauvegardée est ensuite disponible dans la vue détaillée de l&#39;audience, accessible depuis le menu **Audiences**. Les colonnes disponibles depuis cette vue correspondent aux colonnes de la transition entrante de l&#39;objet **Audience de l’Afrique du Sud** activité.


## Exemple



