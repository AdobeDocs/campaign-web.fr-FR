---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 9a4ca68d475cfbbcccb7a5b0d84f841589824288
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 34%

---


# Principes clés de la création de workflows {#gs-workflow-creation}

Un workflow est une définition de processus : le diagramme de workflow, qui est une représentation de ce qui est censé se produire. Un workflow est également une instance de ce processus : une instance de workflow, qui est une représentation de ce qui se passe réellement.

Le modèle de workflow décrit les différentes tâches à effectuer et la façon de les enchaîner. Les modèles de tâches sont appelés des activités et sont représentées par des icônes. Elles sont reliées entre elles par des transitions.

capture d’écran à déterminer

## Qu’y a-t-il dans un workflow ?

Chaque workflow comprend :

* **Activities**: Une activité décrit un modèle de tâche. Les différentes activités disponibles sont représentées sur le diagramme par des icônes. Chaque type possède des propriétés communes et des propriétés spécifiques.

   Dans un diagramme de workflow, une activité donnée peut produire plusieurs tâches, notamment en cas de boucle ou d&#39;actions récurrentes.

* **Transitions**: Les transitions permettent de lier des activités et de définir leur ordre. Une transition relie une activité source à une activité de destination.

* **Tables de travail**: La table de travail contient toutes les informations véhiculées par la transition. Chaque workflow utilise plusieurs tables de travail. Les données véhiculées dans ces tables peuvent être accélérées et utilisées tout au long du cycle de vie du workflow, à condition qu’elles ne soient pas purgées. En effet, les tables inutiles sont purgées chaque fois que le workflow est passivé, et éventuellement pendant l&#39;exécution des workflows les plus volumineux afin d&#39;éviter de surcharger le serveur.

## Workflows autonomes et de campagne

Les workflows peuvent être créés en tant que workflows autonomes ou au sein d’une campagne.

À déterminer : les spécificités des workflows de campagne et autonomes.

## Etapes principales pour créer un workflow

Les principales étapes pour créer des workflows sont les suivantes :

À déterminer : graphique montrant l’ensemble du processus avec explication et référence aux pages de document