---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: d9d1666e0903d78560230dd81af32b53608686c5
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 100%

---


# Principes fondamentaux de la création de workflows {#gs-workflow-creation}

Un workflow est une définition de processus : le diagramme de workflow, qui est une représentation de ce qui est censé se produire. Un workflow est également une instance de ce processus : une instance de workflow, qui est une représentation de ce qui se passe réellement.

Le modèle de workflow décrit les différentes tâches à effectuer et la façon de les enchaîner. Les modèles de tâches sont appelés des activités et sont représentées par des icônes. Elles sont reliées entre elles par des transitions.

capture d’écran à déterminer

## Quels sont les éléments d’un workflow ?

Chaque workflow comprend :

* **Activities**: une activité décrit un modèle de tâche. Les différentes activités disponibles sont représentées sur le diagramme par des icônes. Chaque type possède des propriétés communes et des propriétés propres.

   Dans un diagramme de workflow, une même activité peut engendrer plusieurs tâches, notamment en cas de boucle ou d’actions récurrentes.

* **Transitions** : les transitions permettent d’associer des activités et de définir leur séquence. Une transition associe une activité source à une activité de destination.

* **Tables de travail** : la table de travail contient toutes les informations véhiculées par la transition. Chaque workflow utilise plusieurs tables de travail. Les données transmises dans ces tableaux peuvent être accélérées et utilisées tout au long du cycle de vie du workflow, tant qu’elles ne sont pas purgées. En effet, les tableaux inutiles sont purgés à chaque passivation du workflow, et potentiellement en cours d’exécution pour les workflows les plus volumineux afin de ne pas surcharger le serveur.

## Workflows autonomes et de campagne

Les workflows peuvent être créés en tant que workflows autonomes ou à partir d’une campagne.

À déterminer : les spécificités des workflows de campagne et autonomes.

## Procédure de création d’un workflow

Pour créer un workflow, procédez comme suit :

À déterminer : illustration de l’ensemble du processus, avec explication et référence aux pages du document