---
audience: end-user
title: Création d'audiences
description: Découvrez comment créer des audiences dans Adobe Campaign Web
badge: label="Beta"
source-git-commit: f9693c08e1f0a5b5644e8026b7dfe788ee6499c4
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# Création d&#39;audiences {#create-audiences}

Campaign Web vous permet de créer des workflows dans lesquels vous pouvez combiner des audiences existantes dans une zone de travail visuelle. En intégrant diverses activités de workflow, telles que Partage ou Exclusion, vous pouvez générer de nouvelles audiences affinées.

Une fois que vous avez conçu votre workflow, les audiences résultantes sont automatiquement stockées dans Campaign Web à côté de vos audiences existantes. Ces audiences peuvent ensuite être ciblées dans des campagnes ou des diffusions autonomes.

## Créer votre première audience {#create}

Pour créer une audience, procédez comme suit :

1. Accédez au **[!UICONTROL Audiences]** et cliquez sur le bouton **[!UICONTROL Création d’une audience]** situé dans le coin supérieur droit.
1. Attribuez un libellé à votre audience.
1. Développez l’objet **[!UICONTROL Options supplémentaires]** pour configurer les paramètres d’audience avancés.

   Par défaut, les audiences sont créées dans la variable **[!UICONTROL Profils et cibles]** / **[!UICONTROL Listes]** menu de l’explorateur. Vous pouvez modifier l’emplacement de stockage par défaut à l’aide du **[!UICONTROL Dossier]** champ .

   ![](assets/audiences-settings.png)

1. Une fois les paramètres d’audience configurés, cliquez sur le bouton **[!UICONTROL Création d’une audience]** bouton .

1. Un canevas de workflow s’affiche, comprenant deux activités par défaut :

   * **[!UICONTROL Créer une audience]**: point de départ de votre workflow, vous permettant de créer une audience et de l’utiliser comme base de votre workflow.
   * **[!UICONTROL Sauvegarde d’audience]**: représente la dernière étape de votre workflow, ce qui vous permet d’enregistrer les résultats en tant que nouvelle audience.

1. Personnalisez votre workflow en ajoutant autant d’activités que nécessaire. Pour plus d’informations sur la configuration des activités de workflow, reportez-vous à la section [documentation sur les workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Les activités de canal ne peuvent pas être utilisées dans les workflows d’audience.

   ![](assets/audience-creation-canvas.png)

1. Lorsque votre workflow est prêt, cliquez sur **[!UICONTROL Début]** pour l’exécuter.

1. Le workflow est enregistré dans la variable **[!UICONTROL Workflows]** tandis que la ou les audiences obtenues sont accessibles dans la **[!UICONTROL Audiences]** liste. [Découvrez comment surveiller et gérer les audiences](access-audiences.md)
