---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
source-git-commit: 422f2d2cbef424a95540f359c4a5e978eace6c9f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 7%

---


# Orchestration des activités {#orchestrate}

Une fois que vous avez [création d’un workflow](create-workflow.md), que ce soit à partir du menu de workflow ou dans une campagne, vous pouvez commencer à orchestrer les différentes tâches qu’elle exécutera. Pour ce faire, un canevas visuel est fourni, vous permettant de construire un diagramme de workflow. Dans ce diagramme, vous pouvez ajouter différentes activités et les connecter dans un ordre séquentiel.

A ce stade de la configuration, le diagramme s&#39;affiche avec une icône de démarrage représentant le début de votre workflow. Pour ajouter votre première activité, cliquez sur le bouton + connecté à l&#39;icône de début.

Une liste des activités pouvant être ajoutées au diagramme s’affiche. Les activités disponibles dépendent de votre position dans le diagramme de workflow. Par exemple, lorsque vous ajoutez votre première activité, vous pouvez démarrer votre workflow en ciblant une audience, en fractionnant le chemin du workflow ou en définissant une activité Attente pour retarder l&#39;exécution du workflow. D’un autre côté, après une activité Créer une audience , vous pouvez affiner votre cible avec des activités de ciblage, envoyer une diffusion à votre audience avec des activités de canal ou organiser le processus de workflow avec des activités de contrôle de flux.

![](assets/workflow-start.png)

Une fois qu’une activité a été ajoutée au diagramme, un volet de droite s’affiche, vous permettant de configurer l’activité nouvellement ajoutée avec des paramètres spécifiques. Des informations détaillées sur la configuration de chaque activité sont disponibles dans la section [cette section](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

Répétez ce processus pour ajouter autant d&#39;activités que vous le souhaitez en fonction des tâches que votre workflow doit exécuter. Vous pouvez également insérer une nouvelle activité entre deux activités. Pour cela, cliquez sur le bouton + de la transition entre les activités, sélectionnez l&#39;activité souhaitée et paramétrez-la dans le volet de droite.

Pour supprimer une activité, sélectionnez-la dans la zone de travail, puis cliquez sur l’icône Supprimer dans les propriétés de l’activité.

>[!TIP]
>
>Vous avez la possibilité de personnaliser le nom des transitions entre chaque activité. Pour cela, sélectionnez la transition et modifiez son libellé dans le volet de droite.

Une fois le workflow terminé, ajoutez une activité Fin à la fin du diagramme. Cette activité permet de marquer visuellement la fin d&#39;un workflow et n&#39;a aucun impact fonctionnel.

Une fois le diagramme de workflow conçu, vous pouvez l’exécuter et suivre l’avancement de ses différentes tâches. [Découvrez comment démarrer un workflow et surveiller son exécution.](start-monitor-workflows.md)
