---
audience: end-user
title: Créer des audiences
description: Découvrez comment créer des audiences dans Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '925'
ht-degree: 100%

---

# Créer des audiences {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="Depuis cet écran, vous pouvez accéder à la liste de toutes les audiences qui peuvent être ciblées dans des workflows ou des diffusions autonomes. Cliquez sur **Créer** pour créer une audience dans une zone de travail visuelle.<br/><br/>En plus de commencer de zéro pour créer une audience simple, vous pouvez également tirer parti des activités de workflow pour affiner votre audience. Vous pouvez par exemple combiner plusieurs audiences en une seule, enrichir votre audience avec des attributs externes ou la diviser en plusieurs audiences en fonction des règles de votre choix."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

Campaign Web vous permet de créer de nouvelles audiences dans une zone de travail visuelle de workflow. En plus de commencer de zéro pour créer une audience simple, vous pouvez également tirer parti des activités de workflow pour affiner votre audience. Vous pouvez par exemple combiner plusieurs audiences en une seule, enrichir votre audience avec des attributs externes ou la diviser en plusieurs audiences en fonction des règles de votre choix.

Une fois que vous créez votre workflow, les audiences résultantes sont automatiquement stockées dans la base de données Campaign avec les audiences existantes. Ces audiences peuvent ensuite être ciblées dans des workflows ou des diffusions autonomes.

Les colonnes **[!UICONTROL Origine]** indiquent l’origine des audiences : les audiences **[!UICONTROL Adobe Campaign]** ont été créées dans la console Adobe Campaign v8 ou l’interface d’utilisation web, tandis que les audiences **[!UICONTROL Adobe Experience Platform]** sont créées dans Adobe Experience Platform et intégrées à Campaign à l’aide de l’intégration des sources et destinations d’Adobe.

➡️ [Découvrir cette fonctionnalité en vidéo](#video)

## Créer votre première audience {#create}

Pour créer une audience, veuillez procéder comme suit :

1. Accédez au menu **[!UICONTROL Audiences]** et cliquez sur le bouton **[!UICONTROL Créer une audience]** situé dans le coin supérieur droit.

1. Un nouveau workflow est automatiquement créé, ce qui vous permet de combiner des activités pour générer votre audience. Par défaut, la zone de travail contient deux activités principales :

   * L’activité « Requête » **[!UICONTROL Créer une audience]** est le point de départ de votre workflow. Elle vous permet de créer une audience et de l’utiliser comme base pour votre workflow.

   * L’activité « Nouvelle audience » **[!UICONTROL Enregistrer l’audience]** représente la dernière étape de votre workflow. Elle vous permet d’enregistrer les résultats en tant que nouvelle audience.

   ![Zone de travail de création d’audience vierge avec deux activités par défaut : Créer une audience et Enregistrer l’audience.](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >Les workflows d’audience sont stockés dans le menu **Workflows**, avec vos autres workflows Campaign. Ils sont spécialement conçus pour créer des audiences et sont reconnaissables à leur forme de zone de travail verticale.

1. Pour une meilleure lisibilité, modifiez le nom du workflow dans le champ **Libellé** dans les paramètres du workflow. [Découvrir comment configurer les paramètres de workflow](../workflows/workflow-settings.md)

1. Ouvrez l’activité **[!UICONTROL Créer une audience]** et utilisez le concepteur de requête pour définir la population à inclure dans votre audience en filtrant les données contenues dans la base de données. [Découvrir comment configurer une activité Créer une audience](../workflows/activities/build-audience.md)

1. Si vous souhaitez effectuer des opérations supplémentaires sur la population ciblée dans le workflow, ajoutez autant d’activités que nécessaire et connectez-les l’une à l’autre. Pour plus d’informations sur la configuration des activités de workflow, reportez-vous à la [documentation sur les workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Les activités de canal ne peuvent pas être utilisées dans les workflows d’audience.

   ![Zone de travail de création d’audience avec plusieurs activités connectées pour affiner l’audience.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configurez l’activité **[!UICONTROL Enregistrer une audience]** pour indiquer comment enregistrer la population calculée en amont dans le workflow. [Découvrez comment configurer une activité Enregistrer une audience](../workflows/activities/save-audience.md).

1. Lorsque votre workflow est prêt, cliquez sur **[!UICONTROL Démarrer]** pour l’exécuter.

Le workflow est enregistré dans la liste **[!UICONTROL Workflows]** tandis que la ou les audiences obtenues sont accessibles dans la liste **[!UICONTROL Audiences]** avec le libellé défini dans l’activité **Enregistrer une audience**. Découvrez comment surveiller et gérer des audiences dans [cette section](manage-audience.md).

Vous pouvez désormais utiliser cette audience comme cible principale d’une diffusion. [En savoir plus](add-audience.md)

## Exemple de workflow d’audience {#example}

L’exemple ci-dessous montre un workflow d’audience configuré pour cibler les clientes habitant à New York et créer deux nouvelles audiences en fonction de leur dernier achat (tenue de yoga ou de running).

![Exemple de workflow d’audience ciblant les clientes de New York et les divisant en fonction de leur dernier achat.](assets/audiences-example.png){zoomable="yes"}

1. L’activité **[!UICONTROL Créer une audience]** cible tous les profils de femmes habitant à New York.
1. L’activité **[!UICONTROL Enrichissement]** enrichit l’audience avec des informations du tableau Achats pour identifier le type de produit que les clientes ont acheté.
1. L’activité **[!UICONTROL Partager]** divise le workflow en deux chemins d’accès en fonction du dernier achat des clientes.
1. L’activité **[!UICONTROL Enregistrer une audience]** à la fin de chaque chemin d’accès crée deux nouvelles audiences dans la base de données en incluant la population calculée dans chacun des chemins.

## Modifier une audience {#edit}

Vous pouvez modifier une audience générée à partir d’un workflow à n’importe quel moment en exécutant à nouveau le workflow correspondant. Cela vous permet d’actualiser les données de l’audience ou d’affiner l’audience en ajustant la requête selon vos besoins.

1. Accédez au menu **Audiences** et ouvrez l’audience que vous souhaitez modifier.
1. Dans l’onglet **Vue d’ensemble**, la section **Dernier workflow** fournit un lien vers le workflow utilisé pour générer l’audience. Cliquez sur celui-ci pour accéder au workflow.
1. Apportez les modifications souhaitées, puis cliquez sur le bouton **Démarrer** pour exécuter le workflow à nouveau. Une fois le workflow terminé, l’audience issue du workflow est automatiquement mise à jour avec les derniers résultats du workflow.

Par défaut, la réexécution d’un workflow d’audience remplace l’ensemble du contenu de l’audience par de nouvelles données, ce qui entraîne la perte des données précédentes.

Si vous préférez ne pas remplacer les résultats de l’audience existante, configurez les activités **Enregistrer une audience** pour qu’elles correspondent à vos besoins. Par exemple, vous pouvez modifier le champ **Libellé de l’audience** pour stocker les nouveaux résultats dans une nouvelle audience ou pour ajouter les nouveaux résultats au contenu de l’audience existante sans effacer les données précédentes. [Découvrez comment configurer une activité Enregistrer une audience](../workflows/activities/save-audience.md).

![Écran de configuration de l’activité Enregistrer l’audience avec des options pour ajuster le comportement d’enregistrement de l’audience.](assets/edit-audience-save.png){zoomable="yes"}

## Vidéo pratique {#video}

Découvrez comment créer et gérer des audiences, comment sélectionner des audiences pour une diffusion et définir des populations témoins.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)