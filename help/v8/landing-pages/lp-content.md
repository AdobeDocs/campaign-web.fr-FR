---
title: Définir du contenu spécifique à une page de destination
description: Découvrir comment concevoir du contenu spécifique à une page de destination dans Campaign Web
feature: Landing Pages
source-git-commit: 2afb8c03305262c5695121fb03936c6d738833b5
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 96%

---

# Définir du contenu spécifique à une page de destination {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Utiliser les composants de contenu"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’une page de destination. Pour définir un contenu spécifique qui permettra aux utilisateurs et aux utilisatrices de sélectionner et d’envoyer leurs choix, utilisez le composant de formulaire."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Définir les paramètres de la page principale"
>abstract="La page principale s’affiche immédiatement pour les utilisateurs et les utilisatrices qui cliquent sur le lien vers votre page de destination (provenant, par exemple, d’un e-mail ou d’un site web)."

Vous pouvez modifier le contenu de n’importe quelle page de votre page de destination.

La première page, qui se présente immédiatement aux utilisateurs et utilisatrices lorsqu’ils cliquent sur le lien vers votre page de destination, est déjà préremplie avec le [composant de formulaire spécifique à une page de destination](#use-form-component) pour le modèle sélectionné<!-- to enable users to select and submit their choices-->.

Le contenu des pages **[!UICONTROL Confirmation]**, **[!UICONTROL Erreur]** et **[!UICONTROL Expiration]** est également prérempli. Modifiez-le si nécessaire.

Vous pouvez également définir des [styles pour votre page de destination](#lp-form-styles).

Pour concevoir plus précisément le contenu de votre page de destination, vous pouvez utiliser les mêmes composants que pour un e-mail. [En savoir plus](../email/content-components.md#add-content-components)

## Utiliser le composant de formulaire {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Définir les champs de composant de formulaire"
>abstract="Définissez la manière dont vos personnes destinataires verront et soumettront leurs choix depuis votre page de destination."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Résultat du clic sur le bouton"
>abstract="Définissez ce qui se passe lorsque les utilisateurs et les utilisatrices envoient le formulaire de la page de destination."

Pour définir un contenu spécifique qui permettra aux utilisateurs et aux utilisatrices de sélectionner et d’envoyer leurs choix depuis votre page de destination, modifiez le composant **[!UICONTROL Formulaire]**. Procédez comme suit :

1. Le composant **[!UICONTROL Formulaire]** spécifique à la page de destination est déjà affiché dans la zone de travail du modèle sélectionné.

   >[!NOTE]
   >
   >Le composant **[!UICONTROL Formulaire]** ne peut être utilisé qu’une seule fois sur la même page.

1. Sélectionnez-le. Lʼonglet **[!UICONTROL Contenu du formulaire]** s’affiche dans le panneau de droite et vous permet de modifier les différents champs du formulaire.

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >Basculez vers l’onglet **[!UICONTROL Styles]** à tout moment pour modifier les styles du contenu de votre composant de formulaire. [En savoir plus](#lp-form-styles)

1. Développez le premier champ de texte, le cas échéant, ou ajoutez-en un à l’aide du bouton **[!UICONTROL Ajouter]**. Dans la section **[!UICONTROL Champ de texte 1]**, vous pouvez modifier le type de champ, le champ de la base de données à mettre à jour, le libellé et le texte qui s’afficheront dans le champ avant que l’utilisateur ou l’utilisatrice ne saisisse une valeur.

   ![](assets/lp-form-text-field.png)

1. Activez l’option **[!UICONTROL Rendre le champ du formulaire obligatoire]** si nécessaire. Dans ce cas, la landing page ne peut être envoyée que si l&#39;utilisateur a renseigné ce champ.

   >[!NOTE]
   >
   >Si un champ obligatoire n&#39;est pas renseigné, un message d&#39;erreur s&#39;affiche lorsque l&#39;utilisateur envoie la page.

1. Développez la case à cocher, le cas échéant, ou ajoutez-en une à l’aide du bouton **[!UICONTROL Ajouter]**. Cochez cette case pour mettre à jour un service ou un champ de la base de données.

   ![](assets/lp-form-checkbox.png)

   Si vous sélectionnez **[!UICONTROL Abonnements et services]**, sélectionnez un service dans la liste, puis choisissez l’une des deux options ci-dessous :

   * **[!UICONTROL S’abonner si cette case est cochée]** : les utilisateurs et les utilisatrices doivent cocher la case pour accepter (abonnement).
   * **[!UICONTROL Se désabonner si cette case est cochée]** : les utilisateurs et les utilisatrices doivent cocher la case pour retirer leur consentement (désabonnement).

   Si vous sélectionnez **[!UICONTROL Champ]**, sélectionnez un champ dans la liste des attributs, puis choisissez l’une des deux options ci-dessous :

   * **[!UICONTROL Oui si coché]**.<!--TBC-->

   * **[!UICONTROL Non coché]**.<!--TBC-->

1. Vous pouvez supprimer et ajouter autant de champs que vous le souhaitez (champs de texte, boutons radio, cases à cocher, liste déroulante, etc.) selon les besoins.

1. Une fois tous les champs ajoutés ou mis à jour, cliquez sur **[!UICONTROL Appel à l’action]** pour développer la section correspondante. Cela permet de définir le comportement du bouton dans le composant **[!UICONTROL Formulaire]**.

   ![](assets/lp-call-to-action.png)

1. Définissez ce qui se passe lors du clic sur le bouton :

   * **[!UICONTROL Page de confirmation]** : la personne sera redirigée vers la page de **[!UICONTROL confirmation]**  pour la page de destination active.

   * **[!UICONTROL URL de redirection]** : saisissez l’URL de la page vers laquelle les utilisateurs et les utilisatrices seront redirigés.

1. Si vous souhaitez apporter des mises à jour supplémentaires lors de l’envoi du formulaire, sélectionnez **[!UICONTROL Mises à jour supplémentaires]**, puis sélectionnez l’élément à mettre à jour :
   * Un service d’abonnement : dans ce cas, définissez si vous souhaitez abonner ou désabonner des utilisateurs et des utilisatrices lors de l’envoi du formulaire.
   * Adresse e-mail utilisée lors du renseignement du formulaire.
   * Tous les canaux : lors de l’envoi du formulaire, les utilisateurs seront invités à participer ou à refuser (selon le modèle sélectionné) à toutes les communications de votre marque sur tous les canaux.
   * Un champ de la base de données : sélectionnez un champ dans la liste des attributs et définissez s’il doit être défini sur True ou False lors de l’envoi du formulaire.

   ![](assets/lp-form-additionnal-updates.png)

1. Enregistrez votre contenu pour revenir aux [propriétés de page de destination](create-lp.md#create-landing-page).

## Définir les styles de formulaire de page de destination {#lp-form-styles}

1. Pour modifier les styles du contenu de votre composant de formulaire, accédez à tout moment à l’onglet **[!UICONTROL Styles]**.

1. La section **[!UICONTROL Champ de texte]** est développée par défaut. Elle vous permet de modifier l’aspect des champs de texte, comme le libellé et la police, la position du libellé, la couleur d’arrière-plan du champ ou la bordure du champ.

   ![](assets/lp-text-styles.png)

1. Développez la section **[!UICONTROL Case à cocher]** pour définir l’aspect des cases à cocher et du texte correspondant. Par exemple, vous pouvez régler la famille et la taille de police ou la couleur de la bordure de la case à cocher.

   ![](assets/lp-checkbox-style.png)

1. Développez et modifiez toute autre section correspondant aux autres champs que vous avez ajoutés (bouton radio, liste déroulante, date et heure, etc.) à votre formulaire.

1. Développez la section **[!UICONTROL Appel à l’action]** pour modifier l’aspect du bouton dans le formulaire du composant. Par exemple, vous pouvez changer de police, ajouter une bordure, modifier la couleur du libellé en le survolant avec votre souris ou ajuster lʼalignement du bouton.

   ![](assets/lp-call-to-action-style.png)

   Vous pouvez prévisualiser certains de vos paramètres, comme la couleur du libellé du bouton lorsque vous survolez en utilisant le bouton **[!UICONTROL Simuler du contenu]**. [En savoir plus](create-lp.md#test-landing-page)

1. Enregistrez vos modifications.
