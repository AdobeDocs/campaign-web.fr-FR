---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Beta"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 100%

---


# Créer le workflow {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propriétés de workflow "
>abstract="Dans cet écran, choisissez le modèle à utiliser pour créer le workflow et indiquez un libellé. Développez la section Options supplémentaires pour configurer des paramètres spécifiques tels que le dossier de stockage du workflow ou le fuseau horaire."

La première étape pour créer votre workflow dans Campaign v8 Web consiste à le créer soit en tant que workflow autonome, soit directement dans une campagne, puis à définir ses propriétés. Pour ce faire, procédez comme suit :

1. Commencez par décider si vous souhaitez créer un workflow autonome ou l’intégrer directement dans une campagne :

   * **Workflow autonome** : accédez au menu Workflows et cliquez sur le bouton Créer un workflow dans le coin supérieur droit.
   * **Workflow de campagne :** accédez au menu Campagnes et ouvrez la campagne dans laquelle vous souhaitez créer un nouveau workflow. Cliquez sur le bouton Créer un workflow dans le coin supérieur droit de l’onglet Workflows.

   La boîte de dialogue Propriétés du workflow s’affiche.

   ![](assets/workflow-create.png)

1. Sélectionnez le modèle à utiliser pour créer le workflow et indiquez un libellé pour le workflow.

   Les modèles de workflow contiennent des activités préconfigurées et des configurations globales des propriétés qui peuvent être réutilisées pour créer de nouveaux workflows. Ils sont créés à partir de la console cliente. [Découvrez comment utiliser les modèles](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html?lang=fr#workflow-templates).

1. Développez la section **[!UICONTROL Options supplémentaires]** si vous souhaitez configurer des paramètres spécifiques au workflow, tels que le dossier de stockage et le fuseau horaire. [Découvrez comment configurer les propriétés de workflow](workflow-settings.md).

1. Cliquez sur le bouton **[!UICONTROL Créer un workflow]** pour confirmer la création de votre workflow.

Une fois votre workflow créé, vous pouvez commencer à orchestrer les différentes tâches qu’il exécutera à l’aide d’une zone de travail visuelle dédiée. [Découvrez comment orchestrer des activités de workflow.](orchestrate-activities.md)
