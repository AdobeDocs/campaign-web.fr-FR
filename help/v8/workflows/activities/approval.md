---
audience: end-user
title: Activité du workflow d’approbation
description: Découvrez comment utiliser l’activité de workflow d’approbation
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 4%

---

# Validation {#approval}

>[!CONTEXTUALHELP]
>id="acw_orchestration_approval"
>title="Activité Validation"
>abstract="L&#39;activité **Validation** nécessite la participation d&#39;un opérateur. Affectez la tâche à un groupe ou à un opérateur individuel, personnalisez le titre et le message de la notification, puis définissez les réponses possibles comme des branches de sortie."

L&#39;activité de workflow **Validation** vous permet d&#39;affecter une tâche à un groupe ou à un opérateur individuel, de personnaliser le titre et le message de l&#39;e-mail de notification et de définir les réponses possibles (par exemple Oui/Non) comme des branches de sortie.

Utilisez cette activité chaque fois qu’une étape de votre workflow nécessite une décision humaine avant de continuer, par exemple pour obtenir l’approbation d’un budget, d’une audience cible ou d’un contenu avant que le workflow ne se poursuive.

## Fonctionnement du processus de validation {#process}

Elle requiert la participation d&#39;au moins un opérateur. Cette activité ne bloque pas le workflow : d’autres tâches peuvent être exécutées pendant que le workflow attend une réponse.

En attente d’une réponse, l’activité s’affiche comme étant en attente sur la zone de travail. La personne désignée répond à l’aide du lien inclus dans le message de notification.

Le processus de tâche de validation est le suivant :

1. Créez un workflow et configurez une activité **Validation**.
1. Démarrez le workflow. Lorsqu’elle atteint l’activité **Approbation**, une tâche est créée pour la personne désignée.
1. La personne désignée reçoit le message de notification, clique sur le lien et sélectionne une réponse.
1. Une fois la réponse de la personne désignée obtenue, le workflow se poursuit tout au long de la transition correspondant à sa réponse.

Pour configurer cette activité, procédez comme suit :

1. Attribuez la tâche, [en savoir plus](#assignment)
1. Définir le message de notification, [en savoir plus](#message)
1. Définissez les réponses possibles, [en savoir plus](#answers)
1. Vous pouvez éventuellement définir une expiration, [en savoir plus](#expiration)

## Affecter la tâche {#assignment}

L&#39;affectation de la tâche à un groupe ou un opérateur est obligatoire : un avertissement est affiché jusqu&#39;à ce que vous le fassiez.

![Capture d’écran affichant la section Affectation de l’activité Validation](../assets/workflow-approval1.png){zoomable="yes"}

Procédez comme suit :

1. Dans le champ **[!UICONTROL Type d’affectation]**, choisissez si la tâche est affectée à un **[!UICONTROL Groupe]** (par défaut) ou à un **[!UICONTROL Opérateur]**.

1. Sélectionnez ensuite le **[!UICONTROL Groupe]** (d’opérateurs) ou un **[!UICONTROL Opérateur]** (opérateur unique).

1. Activez l’option **[!UICONTROL Validation multiple]** si vous souhaitez que chaque personne désignée réponde avant la poursuite du workflow. Cette option est disponible quel que soit le type d’affectation. Lorsqu’il est désactivé, le workflow se poursuit dès qu’une personne désignée répond ; cette réponse est celle prise en compte.

1. Cliquez sur **[!UICONTROL Paramètres avancés]** pour sélectionner le modèle de diffusion utilisé pour la notification. Par défaut, un modèle intégré est utilisé, mais vous pouvez sélectionner n’importe quel autre modèle de diffusion.

   ![Capture d&#39;écran affichant les paramètres avancés de l&#39;activité Validation](../assets/workflow-approval1bis.png){zoomable="yes"}

## Définition du message de notification {#message}

Vous pouvez maintenant définir le message de notification envoyé à la personne désignée.

![Capture d&#39;écran affichant la section Message de l&#39;activité Validation](../assets/workflow-approval2.png){zoomable="yes"}

Procédez comme suit :

1. Définissez le **[!UICONTROL titre]** de la notification envoyée à la personne désignée.

1. Définissez le **[!UICONTROL Message]** de la notification envoyée à la personne désignée.

Les deux champs prennent en charge la personnalisation : cliquez sur l&#39;icône de personnalisation pour insérer des variables d&#39;événement, telles que le **[!UICONTROL Opérateur ayant répondu]** et le **[!UICONTROL Réponse]**, que vous pouvez réutiliser à un autre endroit de votre workflow.

![Capture d’écran affichant la personnalisation des messages](../assets/workflow-approval2bis.png){zoomable="yes"}

## Définition des réponses possibles {#answers}

L’activité s’accompagne de deux réponses par défaut : **[!UICONTROL Oui]** et **[!UICONTROL Non]**. Chaque réponse correspond à une transition sortante sur la zone de travail.

![Capture d’écran affichant la section Réponses de l’activité Validation](../assets/workflow-approval3.png){zoomable="yes"}

Cliquez sur **[!UICONTROL Ajouter une réponse]** pour définir des choix supplémentaires.

Lorsque la personne désignée répond, le workflow se poursuit tout au long de la transition correspondant à son choix.

## Définition d’une expiration {#expiration}

Enfin, vous pouvez définir une date d’expiration pour la tâche d’approbation. Comme une réponse, une expiration déclenche sa propre transition de sortie si la personne désignée n’a pas répondu dans le délai.

![Capture d’écran affichant la section Expiration de l’activité Validation](../assets/workflow-approval4.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Ajouter une expiration]**.

1. Définissez un **[!UICONTROL Libellé]** pour la transition sortante correspondante.

1. Dans le menu déroulant **[!UICONTROL Type d’expiration]**, choisissez l’une des options suivantes :

   * **[!UICONTROL Délai après le début de la tâche]** : définissez un délai à attendre après le début de la tâche d’approbation.
   * **[!UICONTROL Délai après une date]** : définissez un délai d’attente après une date spécifique.
   * **[!UICONTROL Délai avant une date]** : définissez un délai à attendre avant une date spécifique.
   * **[!UICONTROL Expiration calculée par script]** : utilisez un script pour calculer l’expiration.

1. Activez l’option **[!UICONTROL Ne pas terminer la tâche]** si vous souhaitez que la transition d’expiration soit activée sans terminer la tâche d’approbation, de sorte que la personne désignée puisse toujours répondre par la suite.

Vous pouvez définir plusieurs expirations pour la même tâche d’approbation.

Vous pouvez ensuite démarrer le workflow. Une fois la réponse de la personne désignée obtenue, le workflow se poursuit tout au long de la transition correspondant à sa réponse. [En savoir plus](#process)

## Rubriques connexes {#related}

* [À propos des activités de workflows](about-activities.md)
* [Configurer et gérer le processus de validation](../../campaigns/campaign-approvals.md)
