---
audience: end-user
title: Création d'audiences
description: Découvrez comment créer des audiences dans Adobe Campaign Web
badge: label="Beta"
source-git-commit: 44a280446f9e7f801607dd40326b56fd79ec34e9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---


# Création d&#39;audiences {#create-audiences}

Campaign Web vous permet de créer des workflows dans lesquels vous pouvez combiner des audiences existantes dans une zone de travail visuelle et exploiter diverses activités (fractionner, exclure..) pour créer de nouvelles audiences.

Une fois cette opération terminée, les audiences qui en résultent sont sauvegardées dans le Web de Campaign avec les audiences existantes et peuvent être exploitées dans des diffusions autonomes ou des campagnes pour cibler des individus.

## Créer votre première audience {#create}

Pour créer une audience, procédez comme suit :

1. Accédez au **[!UICONTROL Audiences]** et cliquez sur **[!UICONTROL Création d’une audience]** dans le coin supérieur droit.
1. Attribuez un libellé à l’audience.
1. Développez la section Options supplémentaires pour configurer les paramètres avancés de l’audience.

   >[!NOTE]
   >
   >Par défaut, les audiences sont créées dans le menu Explorateur de profils et de cibles / Listes . Vous pouvez modifier l’emplacement de stockage par défaut dans le **[!UICONTROL Dossier]** champ .

1. Une fois les paramètres de l’audience configurés, cliquez sur **[!UICONTROL Création d’une audience]** bouton .

1. Un canevas de workflow s’affiche, avec deux activités par défaut :

   * **[!UICONTROL Créer une audience]**: point de départ de votre workflow. Cette activité permet de sélectionner une ou plusieurs audiences comme base de votre workflow,
   * **[!UICONTROL Sauvegarde d’audience]**: la dernière étape de votre workflow. Cette activité permet d&#39;enregistrer le résultat de votre workflow dans une nouvelle audience.

1. Configurez votre workflow en ajoutant autant d’activités que nécessaire. Pour plus d’informations sur la configuration des différentes activités, reportez-vous à la section [documentation sur les workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Les activités de canal ne peuvent pas être utilisées dans les workflows d’audience.

   ![](assets/audience-creation-canvas.png)

1. Lorsque votre workflow est prêt, cliquez sur **[!UICONTROL Début]** pour l’exécuter.

1. Le workflow est enregistré dans la variable **[!UICONTROL Workflows]** et les audiences qui en résultent dans la **[!UICONTROL Audiences]** liste. [Découvrez comment accéder aux audiences](access-audiences.md)
