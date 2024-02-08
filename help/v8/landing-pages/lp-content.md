---
title: Définir du contenu spécifique à une page de destination
description: Découvrir comment concevoir du contenu spécifique à une page de destination dans Campaign Web
feature: Landing Pages
badge: label="Disponibilité limitée"
source-git-commit: 5e5c731fa76684407080d9a1aa6f8a81de7ebc92
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 48%

---

# Définir du contenu spécifique à une page de destination {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Utiliser les composants de contenu"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’une page de destination. Pour définir un contenu spécifique qui permettra aux utilisateurs et aux utilisatrices de sélectionner et d’envoyer leurs choix, utilisez le composant de formulaire."

Lors de la modification du contenu d’une page de votre page de destination, celle-ci est déjà préremplie.

La première page, immédiatement affichée par les utilisateurs lorsqu’ils cliquent sur le lien vers votre landing page, est déjà prérenseignée avec le champ [composant de formulaire spécifique à une page d’entrée](#use-form-component) pour le modèle sélectionné<!-- to enable users to select and submit their choices-->. Vous pouvez également définir [styles de votre landing page](#lp-form-styles).

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

1. Développez le premier champ de texte, le cas échéant, ou ajoutez-en un à l’aide de la propriété **[!UICONTROL Ajouter]** bouton . Dans la **[!UICONTROL Champ de texte 1]** , vous pouvez éditer le type de champ, le champ de la base de données à mettre à jour, le libellé et le texte qui s&#39;afficheront dans le champ avant que les utilisateurs ne saisissent une valeur.

   ![](assets/lp-form-text-field.png)

1. Activez l’option **[!UICONTROL Rendre le champ du formulaire obligatoire]** si nécessaire. Dans ce cas, la landing page ne peut être envoyée que si l&#39;utilisateur a renseigné ce champ.

   >[!NOTE]
   >
   >Si un champ obligatoire n&#39;est pas renseigné, un message d&#39;erreur s&#39;affiche lorsque l&#39;utilisateur envoie la page.

1. Développez la case à cocher, le cas échéant, ou ajoutez-en une à l’aide de la fonction **[!UICONTROL Ajouter]** bouton . Cochez cette case pour mettre à jour un service ou un champ de la base de données.

   ![](assets/lp-form-checkbox.png)

   Si vous sélectionnez **[!UICONTROL Abonnements et services]**, sélectionnez un service dans la liste, puis choisissez l’une des deux options ci-dessous :

   * **[!UICONTROL S’abonner à si cette option est cochée]**: les utilisateurs doivent cocher la case pour accepter (opt-in).
   * **[!UICONTROL Se désabonner si cette case est cochée]** : les utilisateurs et les utilisatrices doivent cocher la case pour retirer leur consentement (désabonnement).

   Si vous sélectionnez **[!UICONTROL Champ]**, sélectionnez un champ dans la liste des attributs, puis effectuez une sélection parmi les deux options ci-dessous :

   * **[!UICONTROL Oui si coché]**<!--TBC-->

   * **[!UICONTROL Non coché]**<!--TBC-->

1. Vous pouvez supprimer et ajouter autant de champs que vous le souhaitez (champs de texte, boutons radio, cases à cocher, liste déroulante, etc.) selon les besoins.

1. Une fois tous les champs ajoutés ou mis à jour, cliquez sur **[!UICONTROL Appel à l’action]** pour développer la section correspondante. Cela permet de définir le comportement du bouton dans le composant **[!UICONTROL Formulaire]**.

   ![](assets/lp-call-to-action.png)

1. Définissez ce qui se passe lors du clic sur le bouton :

   * **[!UICONTROL Page de confirmation]** : la personne sera redirigée vers la page de **[!UICONTROL confirmation]**  pour la page de destination active.

   * **[!UICONTROL URL de redirection]** : saisissez l’URL de la page vers laquelle les utilisateurs et les utilisatrices seront redirigés.

1. Si vous souhaitez apporter des mises à jour supplémentaires lors de l’envoi du formulaire, sélectionnez **[!UICONTROL Mises à jour supplémentaires]**, puis sélectionnez l’élément à mettre à jour :
   * Un service d’abonnement : dans ce cas, définissez si vous souhaitez inscrire ou exclure des utilisateurs lors de l’envoi du formulaire.
   * Adresse électronique utilisée lors du remplissage du formulaire.
   * Tous les canaux : lors de l’envoi du formulaire, les utilisateurs seront inscrits ou désinscrits (selon le modèle sélectionné) pour toutes les communications de votre marque sur tous les canaux.
   * Un champ de la base de données : sélectionnez un champ dans la liste des attributs et définissez s’il doit être défini sur True ou False lors de l’envoi du formulaire.

   ![](assets/lp-form-additionnal-updates.png)

1. Enregistrez votre contenu pour revenir aux [propriétés de page de destination](create-lp.md#create-landing-page).

## Définir les styles de formulaire de page de destination {#lp-form-styles}

1. Pour modifier les styles du contenu de votre composant de formulaire, basculez à tout moment vers la fonction **[!UICONTROL Styles]** .

1. La variable **[!UICONTROL Champ de texte]** est développée par défaut. Il permet de modifier l’aspect des champs de texte, tels que la police du libellé, la position du libellé, la couleur d’arrière-plan du champ ou la bordure du champ.

   ![](assets/lp-text-styles.png)

1. Développez l’objet **[!UICONTROL Case à cocher]** pour définir l’aspect des cases à cocher et du texte correspondant. Par exemple, vous pouvez ajuster la famille et la taille de police ou la couleur de la bordure de la case à cocher.

   ![](assets/lp-checkbox-style.png)

1. Développez et modifiez toute autre section correspondant aux autres champs que vous avez ajoutés (bouton radio, liste déroulante, date et heure, etc.) à votre formulaire.

1. Développez l’objet **[!UICONTROL Appel à l’action]** pour modifier l’aspect du bouton dans le formulaire du composant. Par exemple, vous pouvez changer de police, ajouter une bordure, modifier la couleur du libellé en le survolant avec votre souris ou ajuster lʼalignement du bouton.

   ![](assets/lp-call-to-action-style.png)

   Vous pouvez prévisualiser certains de vos paramètres, comme la couleur du libellé du bouton lorsque vous survolez en utilisant le bouton **[!UICONTROL Simuler du contenu]**. [En savoir plus](create-lp.md#test-landing-page)

1. Enregistrez vos modifications.
