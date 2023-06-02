---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 880f02c460d75c50347fb5716fbcdf7cd3908422
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 14%

---


# Créer le workflow {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propriétés de workflow"
>abstract="À déterminer"

La première étape pour créer votre workflow dans le Web Campaign v8 consiste à le créer soit comme un workflow autonome, soit directement dans une campagne et à définir ses propriétés générales. Pour ce faire, procédez comme suit :

1. Commencez par décider si vous souhaitez créer un workflow autonome ou l&#39;intégrer directement dans une campagne :

   * **Processus autonome**: Accédez au menu Workflows et cliquez sur le bouton Créer un workflow dans le coin supérieur droit.
   * **Workflow de campagne :** Accédez au menu Campagnes et ouvrez l&#39;opération dans laquelle vous souhaitez créer un nouveau workflow. Cliquez sur le bouton Créer un workflow dans le coin supérieur droit de l&#39;onglet Workflows .

   La boîte de dialogue Propriétés du workflow s’affiche.

   ![](assets/workflow-create.png)

1. Sélectionnez le modèle à utiliser pour créer le workflow et indiquez un libellé pour le workflow.

   Les modèles de workflow contiennent des activités préconfigurées et des configurations globales des propriétés qui peuvent être réutilisées pour créer de nouveaux workflows. Ils sont créés à partir de la console cliente. [Découvrez comment utiliser des modèles](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. Développez l’objet **[!UICONTROL Options supplémentaires]** si vous souhaitez configurer des paramètres spécifiques au workflow, tels que le dossier de stockage et le fuseau horaire. [Découvrez comment configurer les propriétés de workflow](workflow-settings.md)

1. Cliquez sur le bouton **[!UICONTROL Créer un workflow]** pour confirmer la création de votre workflow.

Une fois votre workflow créé, vous pouvez commencer à orchestrer les différentes tâches qu’il exécutera à l’aide d’une zone de travail visuelle dédiée. [Découvrez comment orchestrer des activités de workflow.](orchestrate-activities.md)
