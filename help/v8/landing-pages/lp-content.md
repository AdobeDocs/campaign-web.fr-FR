---
title: Définition du contenu spécifique à une landing page
description: Découvrez comment concevoir du contenu spécifique à une landing page dans Campaign Web
badge: label="Disponibilité limitée"
source-git-commit: 2a02015d9d7a7de67f0bcffd328d37080c0f50c4
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 7%

---

# Définition du contenu spécifique à une landing page {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Utiliser les composants de contenu"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la mise en page d’une landing page. Pour définir un contenu spécifique qui permettra aux utilisateurs de sélectionner et d’envoyer leurs choix, utilisez le composant de formulaire."

Lors de l&#39;édition du contenu d&#39;une page de votre landing page, celle-ci est déjà préremplie.

La page principale est la page qui s’affiche immédiatement pour les utilisateurs lorsqu’ils cliquent sur le lien vers votre page d’entrée (provenant d’un courrier électronique ou d’un site web, par exemple). La page principale est déjà prérenseignée avec la variable [composant de formulaire spécifique à une page d’entrée](#use-form-component) pour permettre aux utilisateurs de sélectionner et d’envoyer leurs choix. Vous pouvez également définir [styles spécifiques aux landing pages](#lp-form-styles).

Pour concevoir plus précisément le contenu de votre landing page, vous pouvez utiliser les mêmes composants que pour un email. [En savoir plus](../email/content-components.md#add-content-components)

<!--
The content of the **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages is also pre-filled. Edit them as needed.

Set the subscription form to the appropriate fields from the database to make sure it will work correctly.

The landing page default fields are already there for the selected template.

>[!NOTE]
>
>You can also create a click-through landing page without a **[!UICONTROL Form]** component. In that case, the landing page will be displayed to users, but they will not be required to submit any form. This can be useful if you only want to showcase a landing page without requiring any action from your recipients such as opt-in or opt out, or want to provide information that doesn't require user input.

Using the landing page content designer, you can also leverage contextual data coming from the primary page in a subpage. [Learn more](#use-primary-page-context)-->

## Utilisation du composant de formulaire {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Définition des champs de composant de formulaire"
>abstract="Définissez la manière dont vos destinataires verront et soumettront leurs choix depuis votre landing page."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Que se passe-t-il lorsque vous cliquez sur le bouton ?"
>abstract="Définissez ce qui se passera lorsque les utilisateurs envoient le formulaire de landing page."

Pour définir un contenu spécifique qui permettra aux utilisateurs de sélectionner et d’envoyer leurs choix depuis votre landing page, utilisez la méthode **[!UICONTROL Formulaire]** composant. Procédez comme suit :

1. Spécifique à la landing page **[!UICONTROL Formulaire]** est déjà affiché dans la zone de travail du modèle sélectionné.

   >[!NOTE]
   >
   >La variable **[!UICONTROL Formulaire]** ne peut être utilisé qu’une seule fois sur la même page.

1. Sélectionnez-le. La variable **[!UICONTROL Contenu du formulaire]** s’affiche dans la palette de droite pour vous permettre de modifier les différents champs du formulaire.

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >Basculez vers le **[!UICONTROL Styles]** à tout moment pour modifier les styles du contenu de votre composant de formulaire. [En savoir plus](#lp-form-styles)

1. Développez le premier champ de texte. Dans la **[!UICONTROL Champ de texte 1]** , vous pouvez modifier le type de champ, le champ de la base de données, le libellé et le texte qui s’afficheront dans le champ avant que l’utilisateur ne le renseigne.

   ![](assets/lp-form-text-field.png)

1. Vérifiez les **[!UICONTROL Rendre le champ de formulaire obligatoire]** si nécessaire. Dans ce cas, la landing page ne peut être envoyée que si l&#39;utilisateur a renseigné ce champ.

   >[!NOTE]
   >
   >Si un champ obligatoire n&#39;est pas renseigné, un message d&#39;erreur s&#39;affiche lorsque l&#39;utilisateur envoie la page.

1. Ajoutez une case à cocher. Cochez cette case pour mettre à jour un service ou un champ de la base de données.

   ![](assets/lp-form-checkbox.png)

   Définissez si cette case doit être activée ou désactivée pour les utilisateurs. Sélectionnez l’une des deux options ci-dessous :

   * **[!UICONTROL S’abonner si coché]**: les utilisateurs doivent cocher la case pour accepter (opt-in).
   * **[!UICONTROL Se désabonner si cette case est cochée]**: les utilisateurs doivent cocher la case pour retirer leur consentement (opt-out).

1. Vous pouvez supprimer et ajouter autant de champs de texte et/ou de cases à cocher que nécessaire.

1. Une fois que vous avez ajouté toutes les cases à cocher et/ou tous les champs de texte, cliquez sur **[!UICONTROL Appel à l’action]** pour développer la section correspondante. Il permet de définir le comportement du bouton dans la variable **[!UICONTROL Formulaire]** composant.

   ![](assets/lp-call-to-action.png)

1. Définissez ce qui se passe lorsque vous cliquez sur le bouton :

   * **[!UICONTROL Page de confirmation]**: l’utilisateur sera redirigé vers la fonction **[!UICONTROL Confirmation]** jeu de pages pour la page d’entrée active.

   * **[!UICONTROL URL de redirection]**: saisissez l’URL de la page vers laquelle les utilisateurs seront redirigés.

1. Si vous souhaitez apporter des mises à jour supplémentaires lors de l’envoi du formulaire, sélectionnez **[!UICONTROL Mises à jour supplémentaires]**, choisissez **[!UICONTROL Inclusion]** ou **[!UICONTROL Exclusion]** et définissez si vous souhaitez mettre à jour une liste d’abonnements, le canal ou uniquement l’adresse électronique utilisée.

   ![](assets/lp-form-additionnal-updates.png)

1. Enregistrez votre contenu pour revenir au [propriétés de page d’entrée](create-lp.md).

## Définition des styles de formulaire de landing page {#lp-form-styles}

1. Pour modifier les styles du contenu de votre composant de formulaire, basculez à tout moment vers la fonction **[!UICONTROL Style]** .

   ![](assets/lp_designer-form-style.png)

1. La variable **[!UICONTROL Champs]** La section est développée par défaut et permet de modifier l’aspect du champ de texte, comme le libellé et la police de l’espace réservé, la position du libellé, la couleur d’arrière-plan du champ ou la bordure du champ.

   ![](assets/lp_designer-form-style-fields.png)

1. Développez l’objet **[!UICONTROL Cases à cocher]** pour définir l’aspect des cases à cocher et du texte correspondant. Par exemple, vous pouvez régler la famille ou la taille de police ou la couleur de la bordure de la case à cocher.

   ![](assets/lp_designer-form-style-checkboxes.png)

1. Développez l’objet **[!UICONTROL Boutons]** pour modifier l’aspect du bouton dans le formulaire du composant. Par exemple, vous pouvez modifier la police, ajouter une bordure, modifier la couleur du libellé au survol ou ajuster l’alignement du bouton.

   ![](assets/lp_designer-form-style-buttons.png)

   Vous pouvez prévisualiser certains de vos paramètres, comme la couleur de l’étiquette du bouton lorsque vous survolez en utilisant la fonction **[!UICONTROL Simulation du contenu]** bouton . En savoir plus sur le test des landing pages [here](create-lp.md#test-landing-page).

1. Développez l’objet **[!UICONTROL Mettre en page le formulaire]** pour modifier les paramètres de mise en page, tels que la couleur d’arrière-plan, la marge intérieure ou la marge.

   ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

