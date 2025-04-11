---
audience: end-user
title: Variables d’événement de workflow
description: Découvrez comment exploiter les variables d’événement dans vos workflows.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 43%

---

# Variables d’événement de workflow {#event-variables}

Certaines activités de workflow vous permettent de modifier des scripts dans l’éditeur d’expression afin d’effectuer des actions spécifiques, comme récupérer des données d’activités précédentes, créer des conditions ou calculer des noms de fichier en fonction de variables d’événement.

## Que sont les variables d’événement ? {#scripting}

Les scripts exécutés dans le cadre d’un workflow accèdent à une série d’**objets** globaux supplémentaires, tels que le workflow en cours d’exécution (`instance`), ses différentes tâches (`task`) ou les événements qui ont activé une tâche donnée (`event`).

Chaque type d’**objet** est associé à une catégorie de **variables** qui peut être utilisée dans l’éditeur d’expression lors de l’édition de scripts dans des activités, telles que le code **[!UICONTROL JavaScript]** ou le **[!UICONTROL Test]**.

* Les **variables d’instance** (`instance.vars.xxx`) sont comparables à des variables globales. Elles sont partagées par toutes les activités.
* Les **variables de tâche** (`task.vars.xxx`) sont comparables à des variables locales. Elles ne sont utilisées que par la tâche en cours. Ces variables sont utilisées par les activités persistantes pour conserver les données et sont parfois utilisées pour échanger des données entre les différents scripts d’une même activité.
* Les **variables d’événement** (`vars.xxx`) activent l’échange des données entre les tâches élémentaires d’un processus de workflow. Ces variables sont transmises par la tâche qui a activé la tâche en cours. Elles sont ensuite transmises aux activités suivantes. Les **variables d’événement** sont les variables les plus couramment utilisées. Elles doivent être utilisées de préférence aux variables d’instance.

>[!NOTE]
>
>Des informations supplémentaires sur les scripts et les objets et variables exposés dans Adobe Campaign sont disponibles dans la documentation de Campaign v8 (console cliente) dans [cette section](https://experienceleague.adobe.com/fr/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Bien que cette ressource offre de précieuses informations, des incohérences peuvent exister dans la mesure où elle s’applique spécifiquement à la console cliente plutôt qu’à l’interface utilisateur web de Campaign.

## Utiliser des variables d’événement dans l’éditeur d’expression {#expression-editor}

Les variables d’événement prédéfinies peuvent être utilisées dans le volet gauche de l’éditeur d’expression. Vous pouvez également en créer de nouvelles en initialisant une nouvelle variable dans votre code.

![Capture d’écran affichant les variables d’événement prédéfinies dans le volet de gauche de l’éditeur d’expression](assets/event-variables.png)

Outre ces variables d’événement, vous pouvez également utiliser le menu **[!UICONTROL Conditions]** dans le volet de gauche pour créer des conditions et le menu **[!UICONTROL Ajouter la date actuelle]** pour appliquer des fonctions liées au formatage des dates.