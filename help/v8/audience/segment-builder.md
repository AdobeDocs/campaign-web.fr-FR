---
audience: end-user
title: Créer une audience à l’aide du créateur de règles de Campaign
description: Découvrez comment utiliser le créateur de règles.
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 30%

---

# Utiliser le créateur de règles {#segment-builder}

Le créateur de règles permet de définir la population ciblée par votre diffusion en filtrant les données contenues dans la base de données. Utilisez-la pour créer une audience à partir d’un workflow à l’aide d’une activité **[!UICONTROL Créer une audience]** ou directement lors de la création d’une diffusion afin de créer une audience unique.

* [Découvrir comment créer et enregistrer une audience](create-audience.md)
* [Découvrez comment créer une audience unique pour une diffusion.](one-time-audience.md)

## Palette

La palette, située à gauche, contient tous les éléments sur lesquels vous pouvez appliquer un filtre pour créer votre audience. Utilisez la barre de recherche pour rechercher rapidement des éléments. Déplacez les vignettes contenues dans la palette vers la zone de travail centrale pour les configurer et en tenir compte.

![Interface de palette affichant les options de filtrage et les onglets](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

La palette est divisée en deux onglets :

* **Attributs** : cet onglet permet d’accéder à tous les champs disponibles à partir du schéma. La liste des champs dépend du schéma de ciblage défini dans le modèle d’e-mail.

* **Audiences** : cet onglet vous permet de filtrer à partir de l’une des audiences existantes définies dans la console Campaign Classic ou depuis Adobe Experience Platform. Découvrez comment surveiller et gérer les audiences dans [cette section](manage-audience.md).

  >[!NOTE]
  >
  >Pour utiliser les audiences Adobe Experience Platform, configurez l’intégration avec les destinations. Consultez la [documentation sur les destinations Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=fr){target="_blank"}.

## Zone de travail

La zone de travail est la zone centrale où vous pouvez configurer et combiner des règles en fonction des éléments ajoutés à partir de la palette. Pour ajouter une nouvelle règle, faites glisser une vignette depuis la palette et déposez-la sur la zone de travail. Des options spécifiques au contexte sont présentées en fonction du type de données ajouté.

![Interface de la zone de travail affichant les options de configuration des règles](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## Le volet Propriétés des règles

Sur le côté droit, le volet **Propriétés des règles** vous permet d’effectuer les actions répertoriées ci-dessous.

![Volet Propriétés des règles affichant les actions disponibles](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **Afficher les résultats :** affiche la liste des profils ciblés par l’audience.
* **Affichage du code** : affiche une version basée sur le code de l’audience dans SQL.
* **Afficher les attributs avancés** : cochez cette option pour afficher la liste complète des attributs dans la palette de gauche, y compris les nœuds, les regroupements, les liens 1-1 et les liens 1-N.
* **Calculer** : met à jour et affiche le nombre de profils ciblés par votre requête.
* **Sélectionner ou enregistrer le filtre** : utilisez un filtre prédéfini pour filtrer votre requête ou enregistrez votre requête en tant que nouveau filtre pour une réutilisation ultérieure. [Découvrez comment utiliser des filtres prédéfinis](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >Dans cette version du produit, certains filtres prédéfinis ne sont pas disponibles dans l’interface utilisateur. Vous pouvez toujours les utiliser. [En savoir plus](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations).

* **Attributs** : affiche une description de l’audience créée.

## Exemple

Dans cet exemple, une audience est créée pour cibler tous les clients qui vivent à Atlanta ou Seattle et qui sont nés après 1980.

1. Dans l’onglet **Attributs** de la palette, recherchez le champ **Date de naissance**. Faites glisser la vignette et déposez-la sur la zone de travail.

   ![Ajout du champ Date de naissance à la zone de travail](assets/segment-builder6.png){zoomable="yes"}

1. Dans la zone de travail, choisissez l’opérateur **Après** et saisissez la date souhaitée.

   ![Configuration de l’opérateur Après pour le champ Date de naissance](assets/segment-builder7.png){zoomable="yes"}

1. Dans la palette, recherchez le champ **Ville** et ajoutez-le à la zone de travail sous la première règle.

   ![Ajout du champ Ville à la zone de travail](assets/segment-builder8.png){zoomable="yes"}

1. Dans le champ de texte, saisissez le nom de la première ville, puis appuyez sur Entrée.

   ![Saisie du nom de la première ville dans le champ Ville](assets/segment-builder9.png){zoomable="yes"}

1. Répétez cette action pour le nom de la deuxième ville.

   ![Saisie du nom de la deuxième ville dans le champ Ville](assets/segment-builder10.png){zoomable="yes"}

1. Cliquez sur **Afficher les résultats** pour afficher la liste et le nombre de destinataires correspondant à la requête. Ajoutez des colonnes pour visualiser et vérifier les données. Dans cet exemple, ajoutez la colonne **City** pour voir Atlanta et Seattle.

   ![Affichage des résultats avec la colonne Ville ajoutée](assets/segment-builder11.png){zoomable="yes"}

1. Cliquez sur **Confirmer**.