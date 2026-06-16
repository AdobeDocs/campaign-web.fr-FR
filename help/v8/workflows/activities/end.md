---
audience: end-user
title: Utiliser l’activité de workflow Fin
description: Découvrez comment utiliser l’activité de workflow Fin.
source-git-commit: a9c701b9c3ac2d16d8a2dda8e851f09ac801a13e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 22%

---

# Fin {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Activité Fin"
>abstract="L’activité **Fin** vous permet de marquer graphiquement la fin d’un workflow. Lorsque plusieurs transitions entrantes sont disponibles, utilisez la section **Ensembles à joindre** pour sélectionner les transitions à connecter à l’activité."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="Ensembles à joindre"
>abstract="Cochez les activités précédentes que vous souhaitez connecter en tant que transitions entrantes de l&#39;activité **Fin**. Les activités sélectionnées sont ensuite connectées à la **Fin**. Cette section s&#39;affiche uniquement lorsque plusieurs transitions entrantes sont disponibles pour être connectées à l&#39;activité."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="Signal externe"
>abstract="Espace réservé pour la section de signal externe dans les paramètres d’activité de fin. Disponible uniquement pour les campagnes orchestrées. NE PAS SUPPRIMER"

L’activité **Fin** est une activité de contrôle de **Flux**. Il permet de marquer graphiquement la fin d’un workflow. Cette activité est facultative.

L’activité prend en charge plusieurs transitions entrantes lorsque plusieurs transitions entrantes sont disponibles.

Dans la section **Ensembles à joindre**, cochez les activités précédentes que vous souhaitez connecter en tant que transitions entrantes de l&#39;activité **Fin**. Les activités sélectionnées sont ensuite liées à la **Fin** dans la zone de travail du workflow.

![Processus de configuration de la déduplication des workflows](../assets/workflow-end.png)
