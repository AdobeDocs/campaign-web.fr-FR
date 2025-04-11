---
audience: end-user
title: Utiliser l’activité de workflow Déduplication
description: Découvrez comment utiliser l’activité de workflow Déduplication.
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 38%

---

# Déduplication {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Champs pour identifier les doublons"
>abstract="Dans la section **Champs pour identifier les doublons**, cliquez sur le bouton **Ajouter un attribut** pour spécifier les champs pour lesquels des valeurs identiques permettent d&#39;identifier les doublons, tels que l&#39;adresse e-mail, le prénom et le nom. L’ordre des champs spécifie ceux à traiter en premier."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Activité Déduplication"
>abstract="L&#39;activité **Déduplication** permet de supprimer les doublons dans les résultats des activités entrantes. Elle est principalement utilisée après les activités de ciblage et avant les activités qui utilisent les données ciblées."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Générer un complément"
>abstract="Vous pouvez générer une transition sortante supplémentaire en excluant la population restante sous forme de doublons. Pour ce faire, activez l’option **Générer un complément**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Paramètres de déduplication"
>abstract="Pour supprimer des doublons dans les données entrantes, définissez la méthode de déduplication dans les champs ci-dessous. Par défaut, un seul enregistrement est conservé. Sélectionnez le mode de déduplication en fonction d’une expression ou d’un attribut. Par défaut, l’enregistrement à conserver en dehors des doublons est sélectionné de manière aléatoire."

L’activité **Déduplication** est une activité de **ciblage**. Cette activité supprime les doublons dans les résultats des activités entrantes, tels que les profils dupliqués dans la liste des destinataires. L’activité **Déduplication** est généralement utilisée après les activités de ciblage et avant les activités qui utilisent les données ciblées.

## Configurer l’activité Déduplication {#deduplication-configuration}

Pour configurer l’activité **Déduplication**, procédez comme suit :

![Processus de configuration de la déduplication des workflows](../assets/workflow-deduplication.png)

1. Ajoutez une activité **Déduplication** à votre workflow.

1. Dans la section **Champs pour identifier les doublons**, cliquez sur le bouton **Ajouter un attribut** pour spécifier les champs pour lesquels des valeurs identiques permettent d&#39;identifier les doublons, tels que l&#39;adresse e-mail, le prénom et le nom. L’ordre des champs spécifie ceux à traiter en premier. [Découvrez comment sélectionner des attributs et les ajouter aux favoris](../../get-started/attributes.md).

1. Dans la section **Paramètres de déduplication**, sélectionnez le nombre de **Doublons à conserver** uniques. La valeur par défaut de ce champs est 1. La valeur 0 conserve tous les doublons.

   Par exemple, si les enregistrements A et B sont considérés comme des doublons de l&#39;enregistrement Y, et que l&#39;enregistrement C est considéré comme un doublon de l&#39;enregistrement Z :

   * Si la valeur du champ est 1 : seuls les enregistrements Y et Z sont conservés.
   * Si la valeur du champ est 0 : tous les enregistrements sont conservés.
   * Si la valeur du champ est 2 : les enregistrements C et Z sont conservés, et deux enregistrements de A, B et Y sont conservés, soit par hasard, soit selon la méthode de déduplication sélectionnée.

1. Sélectionnez la **méthode de déduplication** à utiliser :

   * **Sélection aléatoire** : sélectionne de manière aléatoire l&#39;enregistrement à conserver en dehors des doublons.
   * **En utilisant une expression** : conserve les enregistrements dont la valeur de l’expression renseignée est la plus petite ou la plus grande.
   * **Valeurs non vides** : conserve les enregistrements pour lesquels l&#39;expression n&#39;est pas vide.
   * **En suivant une liste de valeurs** : définit une priorité de valeur pour un ou plusieurs champs. Pour définir les valeurs, cliquez sur **Attribut** pour sélectionner un champ ou créer une expression, puis ajoutez les valeurs dans le tableau approprié. Cliquez sur le bouton **Ajouter** situé au-dessus de la liste des valeurs pour définir un nouveau champ.

1. Cochez l&#39;option **Générer le complémentaire** pour exploiter la population restante. Le complémentaire est constitué de tous les doublons. Une transition supplémentaire est ensuite ajoutée à l’activité.

## Exemple {#deduplication-example}

Dans l’exemple suivant, utilisez une activité Déduplication pour exclure les doublons de la cible avant l’envoi d’une diffusion. Les profils dupliqués identifiés sont ajoutés à une audience dédiée qui peut être réutilisée si nécessaire. Choisissez l’adresse **e-mail** pour identifier les doublons. Conservez une entrée et sélectionnez la méthode de déduplication **aléatoire**.

![Exemple d&#39;activité de déduplication dans un workflow](../assets/workflow-deduplication-example.png)