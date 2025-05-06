---
title: Gérer les énumérations
description: Découvrir comment utiliser les énumérations
exl-id: d2a30fef-2cc4-49af-9f5d-d42c6396a8ab
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 62%

---

# Gérer les énumérations {#enumerations}

>[!CONTEXTUALHELP]
>id="acw_enumerations_list"
>title="Énumérations"
>abstract="Une énumération est une liste de valeurs proposées par le système pour renseigner des champs. Utilisez des énumérations pour normaliser les valeurs de ces champs, faciliter la saisie de données ou les utiliser dans des requêtes."

>[!CONTEXTUALHELP]
>id="acw_enumerations_properties"
>title="Propriétés"
>abstract="Définissez les propriétés de l’énumération telles que son nom, son nom interne et son type. Les énumérations **[!UICONTROL Fermées]** possèdent une liste fixe de valeurs qui ne peut être modifiée qu’à partir du menu **[!UICONTROL Énumérations]**. Les énumérations **[!UICONTROL Ouvertes]** permettent aux utilisateurs et aux utilisatrices d’ajouter des valeurs directement dans les champs basés sur cette énumération. Les énumérations **[!UICONTROL Système]** sont associées aux champs système. Les énumérations **[!UICONTROL Émoticône]** sont utilisées pour mettre à jour la liste des émoticônes."

>[!CONTEXTUALHELP]
>id="acw_enumerations_values"
>title="Liste de valeurs d’énumération"
>abstract="Pour ajouter une valeur à l’énumération, cliquez sur le bouton **[!UICONTROL Ajouter une valeur]**, puis configurez-la selon vos besoins."

## En quoi consiste une énumération ? {#about}

Une énumération est une liste de valeurs proposées par le système pour renseigner des champs. Utilisez des énumérations pour normaliser les valeurs de ces champs, faciliter la saisie de données ou les utiliser dans des requêtes. La liste des valeurs s’affiche sous forme d’une liste déroulante dans laquelle vous pouvez sélectionner la valeur à renseigner dans le champ. La liste déroulante permet également une entrée prédictive : saisissez les premières lettres et l’application remplit le reste.

Les valeurs de ce type de champ sont définies depuis le menu **[!UICONTROL Administration]** / **[!UICONTROL Énumérations]** du volet de navigation de gauche.

![Liste des énumérations affichées dans le menu Administration](assets/enumeration-list.png)

## Créer une énumération {#create}

Pour créer une énumération, procédez comme suit :

1. Accédez au menu **[!UICONTROL Énumérations]**, puis cliquez sur le bouton **[!UICONTROL Créer une énumération]**.

1. Saisissez un **[!UICONTROL Libellé]** et un **[!UICONTROL Nom interne]** pour l’énumération.

   ![Création d’un écran d’énumération affichant les champs de libellé et de nom interne](assets/enumeration-create.png)

1. Sélectionnez le **[!UICONTROL type]** de l’énumération :

   * Les énumérations **[!UICONTROL Fermées]** ont une liste fixe de valeurs qui ne peut être modifiée qu&#39;à partir du menu **[!UICONTROL Énumérations]**.
   * Les énumérations **[!UICONTROL Ouvertes]** permettent aux utilisateurs et aux utilisatrices d’ajouter des valeurs directement dans les champs basés sur cette énumération.
   * Les énumérations **[!UICONTROL Système]** sont associées aux champs système.
   * Les énumérations **[!UICONTROL Émoticône]** sont utilisées pour mettre à jour la liste des émoticônes.

1. Cliquez sur **[!UICONTROL Créer]**. Les détails de l’énumération s’affichent, ce qui vous permet d’ajouter des valeurs à la liste.

   ![Écran de détails de l’énumération affichant les options d’ajout de valeurs](assets/enumeration-details.png)

1. Pour ajouter une valeur, cliquez sur le bouton **[!UICONTROL Ajouter une valeur]** puis configurez-la selon vos besoins :

   * **[!UICONTROL Libellé]** : libellé à afficher dans l’énumération.
   * **[!UICONTROL Nom interne]** : nom interne de la valeur (pour les énumérations système).
   * **[!UICONTROL U+ (nom interne)]** (énumérations d’émoticônes) : code unicode de l’émoticône (pour les énumérations d’émoticônes).

   ![Écran Ajouter une valeur affichant les champs de libellé, de nom interne et de code unicode](assets/enumeration-emoticon.png)

1. Enregistrez vos modifications. L’énumération est mise à jour dans les écrans où elle est utilisée.

## Cas d’utilisation : ajouter des valeurs prédéfinies à une énumération {#uc}

Par défaut, le champ « Origine » sur l’écran des détails de profil permet aux utilisateurs et aux utilisatrices de saisir librement n’importe quelle valeur.

![Écran de détails du profil affichant le champ Origine](assets/enumeration-uc-profile.png)

Chaque fois qu’un utilisateur ou une utilisatrice saisit une valeur pour le champ, celle-ci est automatiquement ajoutée à l’énumération « Origine ». Cela peut entraîner des valeurs redondantes, incohérentes ou erronées au fil du temps dans la liste de valeurs.

![Énumération d’origine présentant des valeurs entrées par l’utilisateur incohérentes](assets/enumeration-uc-choice.png)

Pour garantir la cohérence des données et guider les utilisateurs et utilisatrices lors du remplissage du champ, définissez un ensemble de valeurs prédéfinies. Procédez comme suit :

1. Accédez au menu **[!UICONTROL Énumérations]** et ouvrez l’énumération « Origine ».

2. Passez en revue la liste des valeurs saisies par l’utilisateur ou l’utilisatrice et mettez-la en ordre. Cliquez sur le bouton représentant des points de suspension à côté d’une valeur pour la supprimer. Si la liste contient trop d’incohérences, supprimez entièrement l’énumération et recréez-la à partir de zéro.

   ![Écran affichant les options de nettoyage des valeurs saisies par l’utilisateur](assets/enumeration-uc-clean.png)

3. Ajoutez des valeurs prédéfinies. Pour ce faire, cliquez sur le bouton **[!UICONTROL Ajouter une valeur]** et saisissez les valeurs prédéfinies que les utilisateurs et les utilisatrices pourront sélectionner.

   ![Écran affichant les valeurs prédéfinies ajoutées à l’énumération](assets/enumeration-uc-create.png)

4. Pour garantir la cohérence, basculez le type d’énumération sur **[!UICONTROL Fermé]**, ce qui limite les utilisateurs à des valeurs prédéfinies. Si vous avez besoin de flexibilité, conservez le type **[!UICONTROL Ouverte]** pour autoriser de nouvelles entrées de la part des utilisateurs et utilisatrices.

5. Revenez à l’écran des détails de profil. Le champ « Origine » affiche désormais les valeurs prédéfinies pouvant être sélectionnées.

   ![Écran de détails du profil affichant les valeurs prédéfinies dans le champ Origine](assets/enumeration-uc-populated.png)