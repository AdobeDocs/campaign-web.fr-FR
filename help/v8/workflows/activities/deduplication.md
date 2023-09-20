---
audience: end-user
title: Utilisation de l’activité de workflow Déduplication
description: Découvrez comment utiliser l’activité de workflow Déduplication
badge: label="Beta"
source-git-commit: 690e2a2d17f8201c8dbb070ba936c3db513b8329
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 29%

---


# Déduplication {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Champs pour identifier les doublons"
>abstract="Dans le **Champs permettant d’identifier des doublons** , cliquez sur le bouton **Ajouter un attribut** pour indiquer les champs pour lesquels des valeurs identiques permettent d&#39;identifier les doublons, par exemple : adresse email, prénom, nom, etc. L’ordre des champs vous permet de spécifier ceux à traiter en premier."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Activité Déduplication"
>abstract="La variable **Déduplication** permet de supprimer des doublons dans les résultats des activités entrantes. Il est principalement utilisé à la suite des activités de ciblage et avant les activités permettant l’utilisation des données ciblées."


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Générer un complémentaire"
>abstract="Vous pouvez générer une transition sortante supplémentaire avec la population restante, qui a été exclue en tant que doublon. Pour ce faire, activez l’option **Générer le complémentaire**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Paramètres de déduplication"
>abstract="Pour supprimer des doublons dans les données entrantes, définissez la méthode de déduplication dans les champs ci-dessous. Par défaut, un seul enregistrement est conservé. Vous devez également sélectionner le mode de déduplication en fonction d&#39;une expression ou d&#39;un attribut. Par défaut, l’enregistrement à conserver en dehors des doublons est sélectionné de manière aléatoire."

La variable **Déduplication** est une activité **Ciblage** activité. Cette activité permet de supprimer les doublons dans le ou les résultats des activités entrantes, par exemple les profils dupliqués dans la liste des destinataires. La variable **Déduplication** est généralement utilisée à la suite des activités de ciblage, et avant les activités permettant l&#39;utilisation des données ciblées.

## Configuration de l&#39;activité Déduplication{#deduplication-configuration}

Pour configurer la variable **Déduplication** activité :

![](../assets/workflow-deduplication.png)

1. Ajouter un **Déduplication** à votre workflow.

1. Dans le **Champs permettant d’identifier des doublons** , cliquez sur le bouton **Ajouter un attribut** pour indiquer les champs pour lesquels des valeurs identiques permettent d&#39;identifier les doublons, par exemple : adresse email, prénom, nom, etc. L’ordre des champs vous permet de spécifier ceux à traiter en premier.

1. Sélectionnez le nombre d’attributs uniques **Doublons à conserver**. La valeur par défaut de ce champs est 1. La valeur 0 permet de conserver tous les doublons.

   Par exemple, si des enregistrements A et B sont considérés comme des doublons d&#39;un enregistrement Y, et un enregistrement C est considéré comme un doublon d&#39;un enregistrement Z :

   * Si la valeur du champ est 1 : seuls les enregistrements Y et Z sont conservés.
   * Si la valeur du champ est 0 : tous les enregistrements sont conservés.
   * Si la valeur du champ est 2 : les enregistrements C et Z sont conservés et deux enregistrements parmi A, B et Y sont conservés, au hasard ou en fonction de la méthode de déduplication choisie par la suite.

1. Sélectionnez la variable **Méthode de déduplication** pour utiliser :

   * **Sélection aléatoire**: sélectionne au hasard parmi les doublons l&#39;enregistrement à conserver.
   * **A partir d&#39;une expression** : permet de conserver les enregistrements dont la valeur de l&#39;expression renseignée est la plus petite ou la plus grande.
   * **Par ordonnancement de valeurs** : permet de définir un ordre de priorité des valeurs pour un ou plusieurs champs. Pour définir les valeurs, cliquez sur **Attribut** pour sélectionner un champ ou créer une expression, ajoutez la ou les valeurs dans le tableau correspondant. Cliquez sur le bouton Ajouter situé au-dessus de la liste des valeurs pour définir un nouveau champ.

1. Vérifiez les **Générer le complémentaire** si vous souhaitez exploiter la population restante. Le complémentaire est constitué de tous les doublons. Une transition supplémentaire sera alors ajoutée à l&#39;activité.

## Exemple{#deduplication-example}

Dans l&#39;exemple suivant, utilisez une activité de déduplication pour exclure les doublons de la cible avant l&#39;envoi d&#39;une diffusion. Les destinataires dupliqués identifiés sont ajoutés à une audience dédiée qui peut être réutilisée si nécessaire. Choisissez la **Email** pour identifier les doublons. Conserver une entrée et sélectionnez **Random** méthode de déduplication.

![](../assets/workflow-deduplication-example.png)
