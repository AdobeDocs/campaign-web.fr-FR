---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 59%

---


# Principes fondamentaux de la création de workflows {#gs-workflow-creation}

Avec le Web de Campaign v8, vous pouvez créer des workflows dans un canevas visuel afin de concevoir des processus cross-canal tels que la segmentation, l’exécution de campagnes, le traitement de fichiers.

Les workflows peuvent être créés en tant que workflows autonomes, depuis le menu Workflows ou depuis une campagne, à partir du menu Campagnes .

À déterminer : les spécificités des workflows de campagne et autonomes.

## Quels sont les éléments d’un workflow ?

Le diagramme de workflow est une représentation de ce qui est censé se produire. Il décrit les différentes tâches à effectuer et la manière dont elles sont liées.

Chaque workflow comprend :

* **Activities**: Une activité est une tâche à effectuer. Les différentes activités sont représentées sur le diagramme par des icônes. Chaque activité possède des propriétés spécifiques et d’autres propriétés communes à toutes les activités.

   Dans un diagramme de workflow, une même activité peut engendrer plusieurs tâches, notamment en cas de boucle ou d’actions récurrentes.

* **Transitions**: Les transitions relient une activité source à une activité de destination et définissent leur séquence.

* **Tables de travail** : la table de travail contient toutes les informations véhiculées par la transition. Chaque workflow utilise plusieurs tables de travail. Les données transmises dans ces tableaux peuvent être accélérées et utilisées tout au long du cycle de vie du workflow, tant qu’elles ne sont pas purgées. En effet, les tableaux inutiles sont purgés à chaque passivation du workflow, et potentiellement en cours d’exécution pour les workflows les plus volumineux afin de ne pas surcharger le serveur.

## Procédure de création d’un workflow

Pour créer un workflow, procédez comme suit :

À déterminer : illustration de l’ensemble du processus, avec explication et référence aux pages du document

Créer et définir les propriétés > orchestrer les activités dans la zone de travail > configurer les paramètres si nécessaire > démarrer l’exécution et surveiller