---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 696fa6192c16f8fd1d2dd77ad533203277f8a2dd
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 8%

---


# Créer un workflow {#create}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propriétés de workflow"
>abstract="À déterminer"

## Créer le workflow {#create-workflow}

La première étape pour créer votre workflow dans le Web Campaign v8 consiste à le créer soit comme un workflow autonome, soit directement dans une campagne et à définir ses propriétés générales. Pour ce faire, procédez comme suit :

1. Commencez par décider si vous souhaitez créer un workflow autonome ou l&#39;intégrer directement dans une campagne :

   * **Processus autonome**: Accédez au menu Workflows et cliquez sur le bouton Créer un workflow dans le coin supérieur droit.
   * **Workflow de campagne :** Accédez au menu Campagnes et ouvrez l&#39;opération dans laquelle vous souhaitez créer un nouveau workflow. Cliquez sur le bouton Créer un workflow dans le coin supérieur droit de l&#39;onglet Workflows .

1. La boîte de dialogue Propriétés du workflow s’affiche. Sélectionnez le modèle à utiliser pour créer le workflow et attribuez-lui un nom.

   Les modèles de workflow contiennent des activités préconfigurées et des configurations globales des propriétés qui peuvent être réutilisées pour créer de nouveaux workflows. Ils sont créés à partir de la console cliente. [Découvrez comment utiliser des modèles](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

   ![](assets/workflow-create.png)

1. Dans la section Options supplémentaires , configurez des paramètres spécifiques au workflow, tels que le dossier de stockage et le fuseau horaire. [Découvrez comment configurer les propriétés de workflow](workflow-settings.md)

1. Cliquez sur le bouton Créer un workflow pour valider la création de votre workflow.

Une fois votre workflow créé, vous pouvez commencer à orchestrer les différentes tâches qu’il exécutera à l’aide d’une zone de travail visuelle dédiée. [Découvrez comment orchestrer des activités de workflow.](#build)

## Orchestrer les activités de workflow {#build}

Une fois que vous avez [création d’un workflow](create-workflow.md), que ce soit à partir du menu de workflow ou dans une campagne, vous pouvez commencer à orchestrer les différentes tâches qu’elle exécutera. Pour ce faire, un canevas visuel est fourni, vous permettant de construire un diagramme de workflow. Dans ce diagramme, vous pouvez ajouter différentes activités et les connecter dans un ordre séquentiel.

A ce stade de la configuration, le diagramme s&#39;affiche avec une icône de démarrage représentant le début de votre workflow. Pour ajouter votre première activité, cliquez sur le bouton + connecté à l&#39;icône de début.

Une liste des activités pouvant être ajoutées au diagramme s’affiche. Les activités disponibles dépendent de votre position dans le diagramme de workflow. Par exemple, lorsque vous ajoutez votre première activité, vous pouvez démarrer votre workflow en ciblant une audience, en fractionnant le chemin du workflow ou en définissant une activité Attente pour retarder l&#39;exécution du workflow. D’un autre côté, après une activité Créer une audience , vous pouvez affiner votre cible avec des activités de ciblage, envoyer une diffusion à votre audience avec des activités de canal ou organiser le processus de workflow avec des activités de contrôle de flux.

![](assets/workflow-start.png)

Une fois qu’une activité a été ajoutée au diagramme, un volet de droite s’affiche, vous permettant de configurer l’activité nouvellement ajoutée avec des paramètres spécifiques. Des informations détaillées sur la configuration de chaque activité sont disponibles dans la section [cette section](workflow-activities.md).

![](assets/workflow-configure-activities.png)

Répétez ce processus pour ajouter autant d&#39;activités que vous le souhaitez en fonction des tâches que votre workflow doit exécuter. Vous pouvez également insérer une nouvelle activité entre deux activités. Pour cela, cliquez sur le bouton + de la transition entre les activités, sélectionnez l&#39;activité souhaitée et paramétrez-la dans le volet de droite.

Pour supprimer une activité, sélectionnez-la dans la zone de travail, puis cliquez sur l’icône Supprimer dans les propriétés de l’activité.

>[!TIP]
>
>Vous avez la possibilité de personnaliser le nom des transitions entre chaque activité. Pour cela, sélectionnez la transition et modifiez son libellé dans le volet de droite.

Une fois le workflow terminé, ajoutez une activité Fin à la fin du diagramme. Cette activité permet de marquer visuellement la fin d&#39;un workflow et n&#39;a aucun impact fonctionnel.

Une fois le diagramme de workflow conçu, vous pouvez l’exécuter et suivre l’avancement de ses différentes tâches. [Découvrez comment démarrer un workflow et surveiller son exécution.](start-monitor-workflows.md)
