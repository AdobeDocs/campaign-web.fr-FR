---
audience: end-user
title: Création d’audiences
description: Découvrez comment créer des audiences dans Adobe Campaign Web
badge: label="Beta"
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 89%

---

# Création d’audiences {#create-audiences}



>[!CONTEXTUALHELP]
>id="acw_homepage_rn1"
>title="Composition de l’audience"
>abstract="Créez de nouvelles audiences dans un canevas de workflow visuel. En plus de commencer de zéro pour créer une audience simple, vous pouvez également tirer parti des activités de workflow pour affiner votre audience. Combinez plusieurs audiences en une seule, enrichissez votre audience avec des attributs externes ou divisez-la en plusieurs audiences en fonction des règles de votre choix."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Voir les notes de mise à jour"


>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="Depuis cet écran, vous pouvez accéder à la liste de toutes les audiences qui peuvent être ciblées dans vos diffusions. Cliquez sur **Créer** pour créer de nouvelles audiences dans une zone de travail visuelle à l’aide de diverses activités de workflow, telles que **Partager** ou **Exclure**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Paramètres de l’audience"
>abstract="Saisissez le nom de l’audience et les options supplémentaires, puis cliquez sur le bouton **Créer une audience**."

Campaign Web vous permet de créer de nouvelles audiences dans une zone de travail visuelle de workflow. En plus de commencer de zéro pour créer une audience simple, vous pouvez également tirer parti des activités de workflow pour affiner votre audience. Vous pouvez par exemple combiner plusieurs audiences en une seule, enrichir votre audience avec des attributs externes ou la diviser en plusieurs audiences en fonction des règles de votre choix.

Une fois que vous avez conçu votre workflow, les audiences résultantes sont automatiquement stockées dans la base de données Campaign avec les audiences existantes. Ces audiences peuvent ensuite être ciblées dans des workflows ou des diffusions autonomes.

## Créer votre première audience {#create}

Pour créer une audience, veuillez procéder comme suit :

1. Accédez au menu **[!UICONTROL Audiences]** et cliquez sur le bouton **[!UICONTROL Créer une audience]** situé dans le coin supérieur droit.
1. Attribuez un libellé à votre audience.
1. Développez la section **[!UICONTROL Options supplémentaires]** pour configurer les paramètres d’audience avancés.

   Par défaut, les audiences sont créées dans le menu de l’explorateur **[!UICONTROL Profils et cibles]** / **[!UICONTROL Listes]**. Vous pouvez modifier l’emplacement de stockage par défaut à l’aide du champ **[!UICONTROL Dossier]**.

   ![](assets/audiences-settings.png)

1. Une fois les paramètres d’audience configurés, cliquez sur le bouton **[!UICONTROL Créer une audience]**. Une zone de travail de workflow s’affiche, avec deux activités par défaut :

   * **[!UICONTROL Créer une audience]** : il s’agit du point de départ de votre workflow, qui vous permet de créer une audience et de l’utiliser comme base de votre workflow.

   * **[!UICONTROL Enregistrer une audience]** : cela représente la dernière étape de votre workflow et vous permet d’enregistrer les résultats du workflow en tant que nouvelle audience.

1. Ouvrez le **[!UICONTROL Créer une audience]** et utilisez le modèle de requête pour définir la population à inclure dans votre audience en filtrant les données contenues dans la base de données. [Découvrez comment configurer une activité Créer une audience](../workflows/activities/build-audience.md).

1. Si vous souhaitez effectuer des opérations supplémentaires sur la population ciblée dans le workflow, ajoutez autant d’activités que nécessaire et connectez-les l’une à l’autre. Pour plus d’informations sur la configuration des activités de workflow, reportez-vous à la [documentation sur les workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Les activités de canal ne peuvent pas être utilisées dans les workflows d’audience.

   ![](assets/audience-creation-canvas.png)

1. Configurez l’activité **[!UICONTROL Enregistrer une audience]** pour indiquer comment enregistrer la population calculée en amont dans le workflow. [Découvrez comment configurer une activité Enregistrer une audience](../workflows/activities/save-audience.md).

1. Lorsque votre workflow est prêt, cliquez sur **[!UICONTROL Démarrer]** pour l’exécuter.

Le workflow est enregistré dans la liste **[!UICONTROL Workflows]** tandis que la ou les audiences obtenues sont accessibles dans la liste **[!UICONTROL Audiences]**. [Découvrez comment surveiller et gérer les audiences](manage-audience.md).

Vous pouvez désormais utiliser cette audience comme cible principale d’une diffusion. [En savoir plus](add-audience.md)

## Exemple de workflow d’audience {#example}

L’exemple ci-dessous montre un workflow d’audience configuré pour cibler les clientes habitant à New York et créer deux nouvelles audiences en fonction de leur dernier achat (tenue de yoga ou de running).

![](assets/audiences-example.png)

1. L’activité **[!UICONTROL Créer une audience]** cible tous les profils de femmes habitant à New York.
1. L’activité **[!UICONTROL Enrichissement]** enrichit l’audience avec des informations du tableau Achats pour identifier le type de produit que les clientes ont acheté.
1. L’activité **[!UICONTROL Partager]** divise le workflow en deux chemins d’accès en fonction du dernier achat des clientes.
1. L’activité **[!UICONTROL Enregistrer une audience]** à la fin de chaque chemin d’accès crée deux nouvelles audiences dans la base de données en incluant la population calculée dans chacun des chemins.
