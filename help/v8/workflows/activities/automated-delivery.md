---
audience: end-user
title: Activité de workflow Diffusion automatisée
description: Découvrez comment utiliser l’activité de workflow Diffusion automatisée.
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: ht
source-wordcount: '643'
ht-degree: 100%

---

# Diffusion automatisée {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Activité de diffusion automatisée"
>abstract="L’activité de workflow Diffusion automatisée est désormais disponible dans la palette du workflow. Vous pouvez l’utiliser pour créer ou exécuter des actions de diffusion (préparer, envoyer un BAT, préparer et démarrer, etc.) directement dans votre workflow."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="Activité de diffusion automatisée"
>abstract="L’activité **Diffusion automatisée** est utilisée à des fins d’automatisation : créez ou réutilisez une diffusion dans votre workflow, puis choisissez l’action à effectuer (préparer, préparer et démarrer, envoyer un BAT, etc.). Vous pouvez sélectionner une diffusion explicite existante créée en dehors du workflow ou créer une diffusion à partir d’un modèle à chaque exécution de l’activité."

L’activité **Diffusion automatisée** vous permet de créer, configurer et exécuter des actions de diffusion directement dans votre workflow.Vous pouvez l’utiliser pour exécuter une diffusion prédéfinie selon un planning ou dans le cadre d’un flux automatisé, ou pour générer une nouvelle diffusion à partir d’un modèle à chaque exécution de l’activité.

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. 
-->

Pour configurer cette activité, procédez comme suit :

1. Définissez les paramètres de diffusion ([en savoir plus](#delivery-settings)).
1. Sélectionnez l’action à effectuer ([en savoir plus](#action-to-execute)).
1. Configurez la transition ([en savoir plus](#transition-to-execute)).
1. Définissez un script de modification ([en savoir plus](#script)).

## Définition des paramètres de diffusion {#delivery-settings}

Lorsque vous configurez l’activité, vous choisissez d’où provient la diffusion.Deux options sont disponibles dans cette section :

![Copie d’écran montrant la diffusion automatisée](../assets/automated-delivery.png){zoomable="yes"}

* Sélectionnez **Diffusion explicite** si vous souhaitez agir sur une diffusion existante, par exemple une diffusion autonome ou une diffusion créée à partir d’une campagne.Sélectionnez la diffusion à l’aide du bouton **Sélectionner la diffusion**.Chaque fois que le workflow s’exécute et atteint cette activité, il agit sur **la même** diffusion.Aucune nouvelle diffusion n’est créée par exécution.L’activité réutilise la même diffusion.Cela s’avère utile lorsque vous souhaitez préparer ou envoyer plusieurs fois une seule diffusion, par exemple selon un planning ou après une étape d’approbation.

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* Sélectionnez **Nouvelle, créée depuis un modèle** si vous souhaitez qu’une **nouvelle** diffusion soit créée à chaque exécution de l’activité.Sélectionnez le modèle de diffusion à l’aide du bouton **Sélectionner le modèle**.Chaque exécution génère une nouvelle diffusion basée sur ce modèle.Utilisez cette option lorsque chaque exécution de workflow doit entraîner sa propre diffusion distincte (par exemple, un e-mail par exécution).

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>Les options **Spécifiée dans la transition** et **Calculée par script**, utilisées pour les cas d’utilisation avancés, ne peuvent être configurées que dans la console cliente.Consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/fr/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}.

## Sélection de l’action à effectuer {#action-to-execute}

Dans cette section, choisissez l’action que l’activité doit effectuer sur la diffusion.Les options disponibles sont les suivantes :

![Copie d’écran montrant les actions à exécuter dans la diffusion automatisée](../assets/automated-delivery2.png){zoomable="yes"}

* **Enregistrer** : crée et enregistre la diffusion sans l’analyser ni l’envoyer.
* **Estimer la cible** : calcule la cible de la diffusion afin d’évaluer son potentiel (première phase d’analyse).
* **Préparer** : exécute l’analyse complète (calcul de la cible et préparation du contenu).La diffusion n’est pas envoyée.
* **Envoyer un BAT** : envoie un BAT de la diffusion.
* **Préparer et démarrer** : lance le processus d’analyse complet (calcul de la cible et préparation du contenu) et envoie la diffusion.

## Configuration de la transition {#transition-to-execute}

Cette section vous permet de choisir si vous souhaitez générer des transitions après l’activité.Les options disponibles sont les suivantes :

![Copie d’écran montrant les transitions dans la diffusion automatisée](../assets/automated-delivery3.png){zoomable="yes"}

* **Générer une transition sortante** : génère une transition sortante lorsque l’activité termine.
* **Libellé de la transition** : permet de personnaliser le libellé affiché sur la transition dans la zone de travail.
* **Traiter les erreurs** : ajoute une transition supplémentaire pour gérer les erreurs.

## Définition d’un script de modification {#script}

Vous pouvez utiliser un script pour modifier le comportement de l’activité, par exemple les paramètres de diffusion tels que le libellé de l’activité.Utilisez cette option si vous avez besoin d’une logique personnalisée pour cette activité.

Cliquez sur **Créer un script** et écrivez votre logique de modification dans l’éditeur.

## Rubriques connexes {#related}

* [À propos des activités de workflows](about-activities.md)
* [Diffusion continue](continuous-delivery.md)
* [Activités e-mail, SMS, notification push, courrier](channels.md)
* [Modèles de diffusion](../../msg/delivery-template.md)
