---
audience: end-user
title: Activité du workflow de validation
description: Découvrez comment utiliser l’activité de workflow Validation.
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 100%
---
# Validation {#approval}

>[!CONTEXTUALHELP]
>id="acw_orchestration_approval"
>title="Activité de validation"
>abstract="Une activité **Validation** requiert la participation d’un opérateur ou d’une opératrice. Attribuez la tâche à un groupe, à un opérateur individuel ou à une opératrice individuelle, personnalisez le titre et le message de la notification, puis définissez les réponses possibles comme branches de sortie."

L’activité de workflow **Validation** vous permet d’attribuer une tâche à un groupe, à un opérateur individuel ou à une opératrice individuelle, de personnaliser le titre et le message de l’e-mail de notification, puis de définir les réponses possibles (par exemple, Oui/Non) comme branches de sortie.

Utilisez cette activité chaque fois qu’une étape de votre workflow nécessite une décision humaine pour pouvoir continuer, par exemple pour obtenir l’approbation d’un budget, d’une audience cible ou d’un contenu avant que le workflow ne se poursuive.

## Fonctionnement du processus de validation {#process}

Il requiert la participation d’au moins un opérateur ou une opératrice. Cette activité ne bloque pas le workflow : d’autres tâches peuvent s’exécuter dans l’attente d’une réponse.

Dans l’attente d’une réponse, l’activité s’affiche comme étant en attente sur la zone de travail. La personne assignée répond en utilisant le lien contenu dans le message de notification.

Le processus de tâche de validation est le suivant :

1. Créez un workflow et configurez une activité **Validation**.
1. Démarrez le workflow. Lorsqu’il atteint l’activité **Validation**, une tâche est créée pour la personne assignée.
1. La personne assignée reçoit le message de notification, clique sur le lien et sélectionne une réponse.
1. Une fois que la personne assignée a répondu, le workflow se poursuit via la transition correspondant à sa réponse.

Pour configurer cette activité, procédez comme suit :

1. Attribuez la tâche, [en savoir plus](#assignment).
1. Définissez le message de notification, [en savoir plus](#message).
1. Définissez les réponses possibles, [en savoir plus](#answers).
1. Vous pouvez éventuellement définir une expiration, [en savoir plus](#expiration).

## Affecter la tâche {#assignment}

L’affectation de la tâche à un groupe, à un opérateur ou une opératrice, est obligatoire : un avertissement s’affiche jusqu’à ce que vous le fassiez.

![Capture d’écran affichant la section Affectation de l’activité Validation](../assets/workflow-approval1.png){zoomable="yes"}

Procédez comme suit :

1. Dans le champ **[!UICONTROL Type d’affectation]**, choisissez si la tâche est affectée à un **[!UICONTROL Groupe]** (par défaut) ou à un **[!UICONTROL Opérateur ou opératrice]**.

1. Sélectionnez ensuite le **[!UICONTROL Groupe]** (d’opérateurs et d’opératrices) ou un **[!UICONTROL Opérateur ou opératrice]** (opérateur ou opératrice unique).

1. Activez l’option **[!UICONTROL Validation multiple]** si vous souhaitez que chaque personne assignée réponde avant la poursuite du workflow. Cette option est disponible quel que soit le type d’affectation. Lorsqu’elle est désactivée, le workflow se poursuit dès qu’une personne assignée répond ; cette réponse est celle prise en compte.

1. Cliquez sur **[!UICONTROL Paramètres avancés]** pour sélectionner le modèle de diffusion utilisé pour la notification. Par défaut, un modèle intégré est utilisé, mais vous pouvez sélectionner n’importe quel autre modèle de diffusion.

   ![Capture d&#39;écran affichant les paramètres avancés de l’activité Validation](../assets/workflow-approval1bis.png){zoomable="yes"}

## Définir le message de notification {#message}

Vous pouvez maintenant définir le message de notification envoyé à la personne assignée.

![Capture d’écran affichant la section Message de l’activité Approbation](../assets/workflow-approval2.png){zoomable="yes"}

Procédez comme suit :

1. Définissez le **[!UICONTROL Titre]** de la notification envoyée à la personne assignée.

1. Définissez le **[!UICONTROL Message]** de la notification envoyée à la personne assignée.

Les deux champs peuvent être personnalisés : cliquez sur l’icône de personnalisation pour insérer des variables d’événement, telles que l’**[!UICONTROL Opérateur ou opératrice ayant répondu]** et la **[!UICONTROL Réponse]**, que vous pouvez réutiliser ailleurs dans votre workflow.

![Capture d’écran affichant la personnalisation du message](../assets/workflow-approval2bis.png){zoomable="yes"}

## Définir les réponses possibles {#answers}

L’activité s’accompagne de deux réponses par défaut : **[!UICONTROL Oui]** et **[!UICONTROL Non]**. Chaque réponse correspond à une transition sortante sur la zone de travail.

![Capture d’écran affichant la section Réponses de l’activité Validation](../assets/workflow-approval3.png){zoomable="yes"}

Cliquez sur **[!UICONTROL Ajouter une réponse]** pour définir des choix supplémentaires.

Lorsque la personne assignée répond, le workflow se poursuit via la transition correspondant à son choix.

## Définir une expiration {#expiration}

Enfin, vous pouvez définir une expiration pour la tâche de validation. Comme une réponse, une expiration déclenche sa propre transition sortante si la personne assignée n’a pas répondu dans le délai.

![Capture d’écran affichant la section Expiration de l’activité Validation](../assets/workflow-approval4.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Ajouter une expiration]**.

1. Définissez un **[!UICONTROL Libellé]** pour la transition sortante correspondante.

1. Dans le menu déroulant **[!UICONTROL Type d’expiration]**, choisissez l’une des options suivantes :

   * **[!UICONTROL Délai après le début de la tâche]** : définissez un délai d’attente après le début de la tâche de validation.
   * **[!UICONTROL Délai après une date]** : définissez un délai d’attente après une date spécifique.
   * **[!UICONTROL Délai avant une date]** : définissez un délai d’attente avant une date spécifique.
   * **[!UICONTROL Expiration calculée par script]** : utilisez un script pour calculer l’expiration.

1. Activez l’option **[!UICONTROL Ne pas terminer la tâche]** si vous souhaitez que la transition d’expiration soit activée sans terminer la tâche de validation, de sorte que la personne assignée puisse toujours répondre par la suite.

Vous pouvez définir plusieurs expirations pour la même tâche de validation.

Vous pouvez ensuite démarrer le workflow. Une fois que la personne assignée a répondu, le workflow se poursuit via la transition correspondant à sa réponse. [En savoir plus](#process)

## Rubriques connexes {#related}

* [À propos des activités de workflows](about-activities.md)
* [Configurer et gérer le processus de validation](../../campaigns/campaign-approvals.md)
