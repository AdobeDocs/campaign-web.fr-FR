---
title: Définir du contenu spécifique à une page de destination
description: Découvrir comment concevoir du contenu spécifique à une page de destination dans Campaign Web
feature: Landing Pages
badge: label="Disponibilité limitée"
source-git-commit: e8b59db0608e1e307c4603b32d1dde3b176fc036
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 85%

---

# Définir du contenu spécifique à une page de destination {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Utiliser les composants de contenu"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’une page de destination. Pour définir un contenu spécifique qui permettra aux utilisateurs et aux utilisatrices de sélectionner et d’envoyer leurs choix, utilisez le composant de formulaire."

Lors de la modification du contenu d’une page de votre page de destination, celle-ci est déjà préremplie.

La première page, immédiatement affichée par les utilisateurs lorsqu’ils cliquent sur le lien vers votre landing page, est déjà prérenseignée avec le champ [composant de formulaire spécifique à une page d’entrée](#use-form-component) pour le modèle sélectionné afin de permettre aux utilisateurs de sélectionner et d’envoyer leurs choix. Vous pouvez également définir des [styles spécifiques aux pages de destination](#lp-form-styles).

Pour concevoir plus précisément le contenu de votre page de destination, vous pouvez utiliser les mêmes composants que pour un e-mail. [En savoir plus](../email/content-components.md#add-content-components)

Le contenu de la **[!UICONTROL Confirmation]**, **[!UICONTROL Erreur]** et **[!UICONTROL Expiration]** Les pages sont également préremplies. Modifiez-les si nécessaire.

## Utiliser le composant de formulaire {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Définir les champs de composant de formulaire"
>abstract="Définissez la manière dont vos personnes destinataires verront et soumettront leurs choix depuis votre page de destination."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Résultat du clic sur le bouton"
>abstract="Définissez ce qui se passe lorsque les utilisateurs et les utilisatrices envoient le formulaire de la page de destination."

Pour définir un contenu spécifique qui permettra aux utilisateurs et aux utilisatrices de sélectionner et d’envoyer leurs choix depuis votre page de destination, utilisez le composant **[!UICONTROL Formulaire]**. Procédez comme suit :

1. Le composant **[!UICONTROL Formulaire]** spécifique à la page de destination est déjà affiché dans la zone de travail du modèle sélectionné.

   >[!NOTE]
   >
   >Le composant **[!UICONTROL Formulaire]** ne peut être utilisé qu’une seule fois sur la même page.

1. Sélectionnez-le. Lʼonglet **[!UICONTROL Contenu du formulaire]** s’affiche dans le panneau de droite et vous permet de modifier les différents champs du formulaire.

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >Basculez vers l’onglet **[!UICONTROL Styles]** à tout moment pour modifier les styles du contenu de votre composant de formulaire. [En savoir plus](#lp-form-styles)

1. Développez le premier champ de texte. Dans la section **[!UICONTROL Champ de texte 1]**, vous pouvez modifier le type de champ, le champ de la base de données, le libellé et le texte qui s’afficheront dans le champ avant que l’utilisateur ou l’utilisatrice ne le renseigne.

   ![](assets/lp-form-text-field.png)

1. Activez l’option **[!UICONTROL Rendre le champ du formulaire obligatoire]** si nécessaire. Dans ce cas, la landing page ne peut être envoyée que si l&#39;utilisateur a renseigné ce champ.

   >[!NOTE]
   >
   >Si un champ obligatoire n&#39;est pas renseigné, un message d&#39;erreur s&#39;affiche lorsque l&#39;utilisateur envoie la page.

1. Ajoutez une case à cocher. Cochez cette case pour mettre à jour un service ou un champ de la base de données.

   ![](assets/lp-form-checkbox.png)

   Définissez si cette case doit être activée ou désactivée pour les utilisateurs et les utilisatrices. Sélectionnez l’une des deux options ci-dessous :

   * **[!UICONTROL S’abonner à si cette option est cochée]**: les utilisateurs doivent cocher la case pour accepter (opt-in).
   * **[!UICONTROL Se désabonner si cette case est cochée]** : les utilisateurs et les utilisatrices doivent cocher la case pour retirer leur consentement (désabonnement).

1. Vous pouvez supprimer et ajouter autant de champs de texte et/ou de cases à cocher que nécessaire.

1. Une fois que vous avez ajouté toutes les cases à cocher et/ou tous les champs de texte, cliquez sur **[!UICONTROL Appel à l’action]** pour développer la section correspondante. Cela permet de définir le comportement du bouton dans le composant **[!UICONTROL Formulaire]**.

   ![](assets/lp-call-to-action.png)

1. Définissez ce qui se passe lors du clic sur le bouton :

   * **[!UICONTROL Page de confirmation]** : la personne sera redirigée vers la page de **[!UICONTROL confirmation]**  pour la page de destination active.

   * **[!UICONTROL URL de redirection]** : saisissez l’URL de la page vers laquelle les utilisateurs et les utilisatrices seront redirigés.

1. Si vous souhaitez apporter des mises à jour supplémentaires lors de l’envoi du formulaire, sélectionnez **[!UICONTROL Mises à jour supplémentaires]**, choisissez **[!UICONTROL Inclusion]** ou **[!UICONTROL Exclusion]** et définissez si vous souhaitez mettre à jour une liste d’abonnements, le canal ou uniquement l’adresse électronique utilisée.

   ![](assets/lp-form-additionnal-updates.png)

1. Enregistrez votre contenu pour revenir aux [propriétés de page de destination](create-lp.md).

## Définir les styles de formulaire de page de destination {#lp-form-styles}

1. Pour modifier les styles du contenu de votre composant de formulaire, accédez à tout moment à l’onglet **[!UICONTROL Style]**.

   ![](assets/lp_designer-form-style.png)

1. La section **[!UICONTROL Champs]** est développée par défaut et permet de modifier l’aspect du champ de texte, comme le libellé et la police de l’espace réservé, la position du libellé, la couleur d’arrière-plan du champ ou la bordure du champ.

   ![](assets/lp_designer-form-style-fields.png)

1. Développez la section **[!UICONTROL Cases à cocher]** pour définir l’aspect des cases à cocher et du texte correspondant. Par exemple, vous pouvez régler la famille ou la taille de police ou la couleur de la bordure de la case à cocher.

   ![](assets/lp_designer-form-style-checkboxes.png)

1. Développez la section **[!UICONTROL Boutons]** pour modifier l’aspect du bouton dans le formulaire du composant. Par exemple, vous pouvez changer de police, ajouter une bordure, modifier la couleur du libellé en le survolant avec votre souris ou ajuster lʼalignement du bouton.

   ![](assets/lp_designer-form-style-buttons.png)

   Vous pouvez prévisualiser certains de vos paramètres, comme la couleur du libellé du bouton lorsque vous survolez en utilisant le bouton **[!UICONTROL Simuler du contenu]**. En savoir plus sur le test des pages de destination [ici](create-lp.md#test-landing-page).

1. Développez la section **[!UICONTROL Disposition du formulaire]** pour modifier les paramètres de disposition, tels que la couleur d’arrière-plan, la dilatation ou la marge.

   ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

