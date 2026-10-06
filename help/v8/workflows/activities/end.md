---
audience: end-user
title: Utiliser l’activité de workflow Fin
description: Découvrir comment utiliser l’activité de workflow Fin
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 100%
---
# Fin {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Activité Fin"
>abstract="L’activité **Fin** vous permet de marquer graphiquement la fin d’un workflow. Lorsque plusieurs transitions entrantes sont disponibles, utilisez la section **Ensembles à joindre** pour sélectionner celles à connecter à l’activité."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="Ensembles à joindre"
>abstract="Sélectionnez les activités précédentes que vous souhaitez connecter en tant que transitions entrantes de l’activité **Fin**. Les activités sélectionnées sont ensuite connectées à l’activité **Fin**. Cette section s’affiche uniquement lorsque plusieurs transitions entrantes peuvent être connectées à l’activité."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="Signal externe"
>abstract="Espace réservé pour la section de signal externe dans les paramètres d’activité de fin. Disponible uniquement pour les campagnes orchestrées. NE PAS SUPPRIMER"

L’activité **Fin** est une activité de **contrôle de flux**. Elle vous permet de marquer graphiquement la fin d’un workflow. Cette activité est facultative.

L’activité prend en charge plusieurs transitions entrantes lorsque plusieurs d’entre elles sont disponibles.

Dans la section **Ensembles à joindre**, cochez les activités précédentes que vous souhaitez connecter en tant que transitions entrantes de l’activité **Fin**. Les activités sélectionnées sont ensuite liées à l’activité **Fin** dans la zone de travail du workflow.

![Processus de configuration de la déduplication des workflows](../assets/workflow-end.png)
