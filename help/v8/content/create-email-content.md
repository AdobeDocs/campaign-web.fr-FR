---
audience: end-user
title: Concevoir des e-mails dans le concepteur d’e-mail
description: Découvrez comment concevoir le contenu des e-mails en partant de zéro.
exl-id: 23e71da3-434d-4619-a48a-334281592d85
badge: label="Alpha" type="Positive"
source-git-commit: 00396926f461b4cecfc3766ed7222337aa1aef60
workflow-type: ht
source-wordcount: '522'
ht-degree: 100%

---

# Rédiger le contenu de l’e-mail en partant de zéro {#create-email-content}

>[!CONTEXTUALHELP]
>id="ac_structure_components_email"
>title="À propos des composants de structure"
>abstract="Les composants de structure définissent la disposition de votre email."

>[!CONTEXTUALHELP]
>id="ac_structure_components_landing_page"
>title="À propos des composants de structure"
>abstract="Les composants de structure définissent la disposition de la page de destination."

>[!CONTEXTUALHELP]
>id="ac_structure_components_fragment"
>title="À propos des composants de structure"
>abstract="Les composants de structure définissent la disposition du fragment."

>[!CONTEXTUALHELP]
>id="ac_structure_components_template"
>title="À propos des composants de structure"
>abstract="Les composants de structure définissent la disposition du modèle."


>[!CONTEXTUALHELP]
>id="ac_edition_columns_email"
>title="Définition des colonnes de l’email"
>abstract="Le Concepteur d’e-mail vous permet de définir facilement la disposition de votre email en définissant la structure des colonnes."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_landing_page"
>title="Définir les colonnes de la page de destination"
>abstract="Le Concepteur d’e-mail permet de définir facilement la disposition de la page de destination en définissant la structure des colonnes."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_fragment"
>title="Définir les colonnes du fragment"
>abstract="Le Concepteur d’e-mail permet de définir facilement la disposition du fragment en définissant la structure des colonnes."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_template"
>title="Définir les colonnes du modèle"
>abstract="Le Concepteur d’e-mail permet de définir facilement la disposition de votre modèle en définissant la structure des colonnes."

Le Concepteur d’e-mail permet de définir facilement la structure de votre email. En ajoutant et en déplaçant des éléments structurels à l’aide de simples actions de glisser-déposer, vous pouvez concevoir le corps de votre e-mail en quelques secondes.

Pour commencer à créer le contenu de votre e-mail, procédez comme suit :

1. Sur la page d’accueil du Concepteur d’e-mail, cliquez sur l’option **[!UICONTROL Créer en partant de zéro]**.

   ![](assets/email_designer.png)

1. Commencez à concevoir le contenu de l’e-mail en faisant glisser et en déposant les **[!UICONTROL Composants de structure]** dans la zone de travail pour définir la disposition de l’e-mail.

   >[!NOTE]
   >
   >L’empilement des colonnes n’est pas compatible avec tous les programmes de messagerie. Lorsqu’elles ne sont pas prises en charge, les colonnes ne sont pas empilées.

   <!--Once placed in the email, you cannot move nor remove your components unless there is already a content component or a fragment placed inside. This is not true in AJO - TBC?-->

   ![](assets/email_designer_2.png)

1. Ajoutez autant de **[!UICONTROL Composants de structure]** que nécessaire et modifiez leurs paramètres dans le volet dédié de droite.

   Sélectionnez le composant **[!UICONTROL n:n colonne]** pour définir le nombre de colonnes de votre choix (entre 3 et 10). Vous pouvez aussi définir la largeur de chaque colonne en déplaçant les flèches situées au bas de celle-ci.

   >[!NOTE]
   >
   >La taille de chaque colonne ne peut pas être inférieure à 10 % de la largeur totale du composant de structure. Vous ne pouvez pas supprimer une colonne qui n’est pas vide.

1. Développez la section **[!UICONTROL Composants de contenu]** et ajoutez autant d’éléments que nécessaire dans un ou plusieurs composants de structure. [En savoir plus sur les composants de contenu](content-components.md).

1. Vous pouvez personnaliser davantage chaque composant à l’aide du volet **[!UICONTROL Paramètres des composants]** à droite. Par exemple, vous pouvez changer le style de texte, la marge intérieure ou la marge de chaque composant. [En savoir plus sur l’alignement et la marge intérieure](alignment-and-padding.md).

   ![](assets/email_designer_5.png)

1. Insérez des champs de personnalisation pour personnaliser le contenu de l’e-mail à partir des données de profil. [En savoir plus sur la personnalisation du contenu](../personalization/personalize.md).

1. Cliquez sur l’onglet **[!UICONTROL Liens]** dans le volet de gauche pour afficher toutes les URL du contenu qui doivent être trackées. Vous pouvez modifier le **[!UICONTROL Type de tracking]** ou le **[!UICONTROL Libellé]**, ainsi qu’ajouter des **[!UICONTROL Catégories]** si nécessaire. [En savoir plus sur le tracking des liens et des messages](message-tracking.md).

   ![](assets/email_designer_7.png)

1. Si nécessaire, vous pouvez personnaliser davantage votre e-mail en cliquant sur **[!UICONTROL Basculer vers l’éditeur de code]** dans le menu avancé, afin de travailler directement sur le code source de votre e-mail. [En savoir plus sur l’éditeur de code](code-content.md).

   >[!CAUTION]
   >
   >Vous ne pouvez pas revenir au concepteur visuel de cet e-mail après avoir basculé vers l’éditeur de code.

1. Une fois que votre contenu est prêt, cliquez sur **[!UICONTROL Simuler du contenu]** pour vérifier le rendu de l’e-mail. Vous pouvez choisir la vue de bureau ou mobile. [En savoir plus sur la prévisualisation des e-mails](../preview-test/preview-test.md).

   ![](assets/email_designer_28.png)

1. Lorsque votre e-mail est prêt, cliquez sur **[!UICONTROL Enregistrer]**.

