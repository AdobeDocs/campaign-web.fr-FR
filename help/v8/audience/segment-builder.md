---
audience: end-user
title: Créer une audience à l’aide du créateur de règles de Campaign
description: Découvrez comment utiliser le créateur de règles.
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: 51f29840941974f05a930023e41adb1bb2558974
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 98%

---

# Utiliser le créateur de règles {#segment-builder}

Le créateur de règles permet de définir la population ciblée par votre diffusion en filtrant les données contenues dans la base de données. Vous pouvez l’utiliser pour créer une audience à partir d’un workflow à l’aide d’une activité **[!UICONTROL Créer une audience]** ou directement lors de la création d’une diffusion pour créer une audience unique.

* [Découvrez comment créer et enregistrer une audience](create-audience.md)
* [Découvrez comment créer une audience unique pour une diffusion.](one-time-audience.md)

## Palette

La palette, située à gauche, contient tous les éléments sur lesquels vous pouvez appliquer un filtre pour créer votre audience. Vous pouvez utiliser la barre de recherche pour rechercher rapidement des éléments. Les tuiles de la palette doivent être déplacées dans la zone de travail centrale pour être configurées et prises en compte.

![](assets/segment-builder2.png){width="70%" align="left"}

La palette est divisée en deux onglets :

* **Attributs** : cet onglet permet d’accéder à tous les champs disponibles à partir du schéma. La liste des champs dépend du schéma de ciblage défini dans le modèle d’e-mail.

* **Audiences** : cet onglet vous permet de filtrer à l’aide de l’une des audiences existantes définies dans la console Campaign Classic ou depuis Adobe Experience Platform. Découvrez comment surveiller et gérer des audiences dans [cette section](manage-audience.md).

  >[!NOTE]
  >
  >Pour tirer parti des audiences Adobe Experience Platform, vous devez configurer l’intégration avec les destinations. Consultez la [documentation sur les destinations Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=fr){target="_blank"}.

## Zone de travail

La zone de travail est la zone centrale, dans laquelle vous pouvez paramétrer et combiner les règles selon les éléments ajoutés depuis la palette. Pour ajouter une nouvelle règle, faites glisser une vignette depuis la palette et déposez-la sur la zone de travail. Des options spécifiques au contexte vous seront ensuite présentées en fonction du type de données ajouté.

![](assets/segment-builder4.png){width="70%" align="left"}

## Le volet Propriétés des règles

Sur le côté droit, le volet **Propriétés des règles** vous permet d’effectuer les actions ci-après.

![](assets/segment-builder5.png){width="70%" align="left"}

* **Afficher les résultats :** affiche la liste des personnes destinataires ciblées par l’audience.
* **Affichage du code** : affiche une version basée sur le code de l’audience dans SQL.
* **Afficher les attributs avancés** : cochez cette option si vous souhaitez afficher la liste complète des attributs dans la palette de gauche : noeuds, regroupements, liens 1-1, liens 1-N.
* **Calculer** : met à jour et affiche le nombre de profils ciblés par votre requête.
* **Sélectionner ou enregistrer un filtre** : utilisez un filtre prédéfini pour filtrer votre requête ou enregistrez votre requête en tant que nouveau filtre pour une réutilisation ultérieure. [Découvrez comment utiliser des filtres prédéfinis](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >Dans cette version du produit, certains filtres prédéfinis ne sont pas disponibles dans l’interface utilisateur. Vous pouvez toujours les utiliser. [En savoir plus](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Attributs** : affiche une description de l’audience créée.

## Exemple

Dans cet exemple, nous allons créer une audience pour cibler tous les clients et clientes habitant à Atlanta ou Seattle et nés après 1980.

1. Dans l’onglet **Attributs** de la palette, recherchez le champ **Date de naissance**. Faites glisser la vignette et déposez-la sur la zone de travail.

   ![](assets/segment-builder6.png)

1. Dans la zone de travail, choisissez l’opérateur **Après** et saisissez la date souhaitée.

   ![](assets/segment-builder7.png)

1. Dans la palette, recherchez le champ **Ville** et ajoutez-le à la zone de travail sous la première règle.

   ![](assets/segment-builder8.png)

1. Dans le champ de texte, saisissez le nom de la première ville, puis appuyez sur Entrée.

   ![](assets/segment-builder9.png)

1. Répétez cette action pour le nom de la deuxième ville.

   ![](assets/segment-builder10.png)

1. Cliquez sur **Afficher les résultats** pour afficher la liste et le nombre de destinataires correspondant à la requête. Vous pouvez également ajouter des colonnes pour visualiser et vérifier les données. Dans notre exemple, ajoutez la colonne **Ville** et vous devriez voir Atlanta et Seattle.

   ![](assets/segment-builder11.png)

1. Cliquez sur **Confirmer**.