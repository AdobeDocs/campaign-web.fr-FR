---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer un workflow avec Adobe Campaign Web
badge: label="Beta"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 2afec0260566c2393c96063037adbf1902497289
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 8%

---


# Créer le workflow {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propriétés de workflow "
>abstract="Dans cet écran, choisissez le modèle à utiliser pour créer le workflow et indiquez un libellé. Développez la section OPTIONS SUPPLÉMENTAIRES pour configurer d’autres paramètres tels que le nom interne du workflow, son dossier, son fuseau horaire et le groupe de superviseurs. Il est vivement recommandé de sélectionner un groupe de superviseurs afin d&#39;alerter les opérateurs en cas d&#39;erreur."


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Liste des workflows de l&#39;opération"
>abstract="La variable **Diffusions** répertorie tous les workflows liés à l&#39;opération en cours. Cliquez sur le nom d&#39;un workflow pour l&#39;éditer. Utilisez le bouton Créer un workflow pour ajouter un nouveau workflow pour cette campagne."


Vous pouvez créer des workflows autonomes ou des workflows au sein d’une campagne. La première étape consiste à sélectionner un modèle et à définir ses propriétés générales. Vous pouvez ensuite configurer d’autres paramètres si nécessaire.

Pour ce faire, procédez comme suit :

1. Pour créer une **Processus autonome**, accédez à la **Workflows** .

   Pour créer une **Workflow de campagne**, accédez à la **Campagnes** puis ouvrez la campagne pour laquelle vous souhaitez créer un nouveau workflow.

1. Cliquez sur le bouton **[!UICONTROL Créer un workflow]** dans le coin supérieur droit de l’écran.

   ![](assets/workflow-create.png)

1. Dans le workflow **Propriétés** , sélectionnez le modèle à utiliser pour créer le workflow (vous pouvez également utiliser le modèle intégré par défaut). En savoir plus sur les modèles dans [la section ci-dessous](#work-with-workflow-templates-workflow-templates).

1. Saisissez le libellé du workflow. En outre, il est vivement recommandé d&#39;ajouter une description à votre workflow, dans le champ dédié du **[!UICONTROL Options supplémentaires]** de l’écran.

1. Développez l’objet **[!UICONTROL Options supplémentaires]** pour configurer d’autres paramètres pour le workflow. Découvrez comment configurer les propriétés de workflow dans [cette page](workflow-settings.md#properties)

   ![](assets/workflow-additional-options.png)

1. Cliquez sur le bouton **[!UICONTROL Créer un workflow]** pour confirmer la création de votre workflow.

Votre workflow est maintenant créé et disponible dans la liste des workflows. Vous pouvez maintenant accéder à sa zone de travail visuelle et commencer à ajouter, configurer et orchestrer les tâches qu’elle exécutera. Découvrez comment orchestrer des activités de workflow dans [cette page](orchestrate-activities.md).

## Utilisation de modèles de workflow {#workflow-templates}

Les modèles de workflow contiennent des paramètres et des activités préconfigurés qui peuvent être réutilisés pour créer de nouveaux workflows. Vous pouvez sélectionner le modèle de votre workflow dans les propriétés du workflow lors de la création d’un workflow. Un modèle vide est fourni par défaut.

Vous pouvez créer un modèle à partir d’un workflow existant ou créer un nouveau modèle à partir de zéro. Les deux méthodes sont présentées ci-dessous.


>[!BEGINTABS]

>[!TAB Créer un modèle à partir d’un workflow existant]

Pour créer un modèle de workflow à partir d&#39;un workflow existant, procédez comme suit :

1. Ouvrez le **Workflows** et accédez au workflow à enregistrer en tant que modèle.
1. Cliquez sur les trois points à droite du nom du workflow, puis choisissez **Copier en tant que modèle**.

   ![](assets/wf-copy-as-template.png)

1. Dans la fenêtre contextuelle, validez la création du modèle.
1. Dans le canevas du modèle de workflow, vérifiez, ajoutez et configurez les activités selon vos besoins.
1. Accédez aux paramètres, depuis le **Paramètres** pour modifier le nom du modèle de workflow, puis saisissez une description.
1. Sélectionnez la variable **folder** et **dossier d’exécution** du modèle. Le dossier correspond à l’emplacement où le modèle de workflow est enregistré. Le dossier d’exécution est le dossier dans lequel les workflows créés à partir de ce modèle sont enregistrés.

   ![](assets/wf-settings-template.png)

   Les autres propriétés sont communes aux workflows. Apprenez-en davantage en consultant [cette page](workflow-settings.md#properties).

1. Enregistrez vos modifications.

Le modèle de workflow est désormais disponible dans la liste des modèles. Vous pouvez créer un workflow à partir de ce modèle. Ce workflow sera préconfiguré avec les paramètres et activités définis dans le modèle.


>[!TAB Créer entièrement un modèle]


Pour créer entièrement un modèle de workflow, procédez comme suit :

1. Ouvrez le **Workflows** et accédez au **Modèles** . Vous pouvez voir la liste des modèles de workflow disponibles.
1. Cliquez sur le bouton **[!UICONTROL Créer un modèle]** dans le coin supérieur droit de l’écran.
1. Saisissez le libellé et ouvrez les options supplémentaires afin de saisir une description de votre modèle de workflow.
1. Sélectionnez le dossier et le dossier d’exécution du modèle. Le dossier correspond à l’emplacement où le modèle de workflow est enregistré. Le dossier d’exécution est le dossier dans lequel les workflows créés à partir de ce modèle sont enregistrés.

   ![](assets/new-wf-template.png)

   Les autres propriétés sont communes aux workflows. Apprenez-en davantage en consultant [cette page](workflow-settings.md#properties).

1. Cliquez sur le bouton **Créer** pour confirmer vos paramètres.
1. Dans le canevas du modèle de workflow, ajoutez et configurez les activités selon vos besoins.

   ![](assets/wf-template-activities.png)

1. Enregistrez vos modifications.

Le modèle de workflow est désormais disponible dans la liste des modèles. Vous pouvez créer un workflow à partir de ce modèle. Ce workflow sera préconfiguré avec les paramètres et activités définis dans le modèle.

>[!ENDTABS]
