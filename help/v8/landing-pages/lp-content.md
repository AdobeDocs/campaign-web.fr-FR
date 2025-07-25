---
title: Définir du contenu spécifique à une page de destination
description: Découvrir comment concevoir du contenu spécifique à une page de destination dans Campaign Web
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: e82c19df7faecbb75521bca54e32b1ba84ea1f81
workflow-type: ht
source-wordcount: '1161'
ht-degree: 100%

---

# Définir du contenu spécifique à une page de destination {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Utiliser les composants de contenu"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’une page de destination. Pour définir un contenu spécifique qui permet aux utilisateurs et aux utilisatrices de sélectionner et d’envoyer leurs choix, utilisez le composant de formulaire."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Définir les paramètres de la page principale"
>abstract="La page principale est la page que les utilisateurs et les utilisatrices voient en premier après avoir cliqué sur le lien de votre page de destination (à partir d’un e-mail ou d’un site web, par exemple)."

Vous pouvez modifier le contenu de n’importe quelle page de votre page de destination.

La première page, qui se présente immédiatement aux utilisateurs et utilisatrices après avoir cliqué sur le lien vers votre page de destination, est déjà préremplie avec le [composant de formulaire spécifique à une page de destination](#use-form-component) pour le modèle sélectionné<!-- to enable users to select and submit their choices-->.

Le contenu des pages **[!UICONTROL Confirmation]**, **[!UICONTROL Erreur]** et **[!UICONTROL Expiration]** est également prérempli. Modifiez-le si nécessaire.

Vous pouvez également définir des [styles pour votre page de destination](#lp-form-styles).

Pour concevoir plus précisément le contenu de votre page de destination :

* Utilisez les mêmes composants que ceux utilisés pour concevoir un e-mail. [En savoir plus](../email/content-components.md#add-content-components)

* Ajoutez du contenu conditionnel à vos pages de destination, comme vous le feriez pour un e-mail. [En savoir plus](../personalization/conditions.md#condition-condition-builder)

## Utiliser le composant de formulaire {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Définir les champs de composant de formulaire"
>abstract="Définissez la manière dont vos personnes destinataires verront et soumettront leurs choix depuis votre page de destination."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Résultat du clic sur le bouton"
>abstract="Définissez ce qui se passe lorsque les utilisateurs et les utilisatrices envoient le formulaire de la page de destination."

Pour définir un contenu spécifique qui permet aux utilisateurs et aux utilisatrices de sélectionner et d’envoyer leurs choix depuis votre page de destination, modifiez le composant **[!UICONTROL Formulaire]**. Suivez les étapes ci-dessous.

1. Le composant **[!UICONTROL Formulaire]** spécifique à la page de destination est déjà affiché dans la zone de travail du modèle sélectionné.

   >[!NOTE]
   >
   >Le composant **[!UICONTROL Formulaire]** ne peut être utilisé qu’une seule fois sur la même page.

1. Sélectionnez-le. Lʼonglet **[!UICONTROL Contenu du formulaire]** s’affiche dans le panneau de droite et vous permet de modifier les différents champs du formulaire.

   ![Composant de formulaire affiché dans la zone de travail](assets/lp-form-component.png){zoomable="yes"}

   >[!NOTE]
   >
   >Basculez vers l’onglet **[!UICONTROL Styles]** à tout moment pour modifier les styles du contenu de votre composant de formulaire. [En savoir plus](#lp-form-styles)

1. Développez le premier champ de texte, le cas échéant, ou ajoutez-en un à l’aide du bouton **[!UICONTROL Ajouter]**. Dans la section **[!UICONTROL Champ de texte 1]**, modifiez le type de champ, le champ de la base de données à mettre à jour, le libellé et le texte qui s’affichent dans le champ avant que l’utilisateur ou l’utilisatrice ne saisisse une valeur.

   ![Paramètres de champ de texte dans le composant de formulaire](assets/lp-form-text-field.png){zoomable="yes"}

1. Activez l’option **[!UICONTROL Rendre le champ du formulaire obligatoire]** si nécessaire. Dans ce cas, la page de destination ne peut être envoyée que si l&#39;utilisateur a renseigné ce champ.

   >[!NOTE]
   >
   >Si un champ obligatoire n’est pas renseigné, un message d’erreur s’affiche lorsque l’utilisateur ou l’utilisatrice envoie la page.

1. Développez la case à cocher, le cas échéant, ou ajoutez-en une à l’aide du bouton **[!UICONTROL Ajouter]**. Cochez cette case pour mettre à jour un service ou un champ de la base de données.

   ![Paramètres des cases à cocher dans le composant de formulaire](assets/lp-form-checkbox.png){zoomable="yes"}

   Si vous sélectionnez **[!UICONTROL Abonnement et services]**, sélectionnez un [service](../audience/manage-services.md) dans la liste, puis choisissez l’une des deux options ci-dessous :

   * **[!UICONTROL S’abonner si cette case est cochée]** : les utilisateurs et les utilisatrices doivent cocher la case pour accepter (abonnement).
   * **[!UICONTROL Se désabonner si cette case est cochée]** : les utilisateurs et les utilisatrices doivent cocher la case pour retirer leur consentement (désabonnement).

   Si vous sélectionnez **[!UICONTROL Champ]**, sélectionnez un champ dans la [liste des attributs](../get-started/attributes.md), puis choisissez l’une des deux options ci-dessous :

   * **[!UICONTROL Oui si coché]**.
   * **[!UICONTROL Non si coché]**.

1. Supprimez et ajoutez autant de champs que vous le souhaitez (champs de texte, boutons radio, cases à cocher, listes déroulantes, etc.).

1. Une fois tous les champs ajoutés ou mis à jour, cliquez sur **[!UICONTROL Appel à l’action]** pour développer la section correspondante. Cela permet de définir le comportement du bouton dans le composant **[!UICONTROL Formulaire]**. [Voici comment procéder](#define-actions-on-form-submission)

   ![Paramètres d’appel à l’action dans le composant de formulaire](assets/lp-call-to-action.png){zoomable="yes"}

1. Enregistrez votre contenu pour revenir aux [propriétés de page de destination](create-lp.md#create-landing-page).

### Définir des actions lors de l’envoi du formulaire {#define-actions-on-form-submission}

1. Définissez ce qui se passe lors du clic sur le bouton :

   * **[!UICONTROL Page de confirmation]** : par défaut, la personne est redirigée vers la page de **[!UICONTROL confirmation]** définie pour la page de destination active.

   * **[!UICONTROL URL de redirection]** : saisissez l’URL de la page vers laquelle les personnes sont redirigées.

   * **[!UICONTROL Page de destination]** : sélectionnez une autre page de destination vers laquelle les personnes seront redirigées. Veillez à configurer la page de destination sélectionnée en conséquence.

1. Pour apporter des mises à jour supplémentaires lors de l’envoi du formulaire, sélectionnez **[!UICONTROL Mises à jour supplémentaires]**, puis sélectionnez l’élément à mettre à jour :
   * [Service d’abonnement](../audience/manage-services.md) : définissez si vous souhaitez abonner ou désabonner des utilisateurs et des utilisatrices lors de l’envoi du formulaire. Lors de la conception d’un email, si vous définissez un lien de type **[!UICONTROL page de destination]** vers cette page de destination, le service sélectionné est automatiquement utilisé. [En savoir plus sur l’insertion de liens](../email/message-tracking.md)

     >[!NOTE]
     >
     >Si vous souhaitez utiliser plusieurs services avec cette page de destination, utilisez l’option **[!UICONTROL Service à partir de l’URL]** décrite ci-dessous.

   * Canal : adresse e-mail utilisée lors du renseignement du formulaire.
   * Tous les canaux : lors de l’envoi du formulaire, les personnes sont abonnées ou désabonnées (selon le modèle sélectionné) de toutes les communications de votre marque sur tous les canaux.
   * Un champ de la base de données : sélectionnez un champ dans la liste des attributs et définissez s’il doit être défini sur True ou False lors de l’envoi du formulaire.

   ![Paramètres de mises à jour supplémentaires dans le composant de formulaire](assets/lp-form-additionnal-updates.png){zoomable="yes"}

1. Sélectionnez l’option **[!UICONTROL Service à partir d’une URL]** pour permettre l’utilisation de la page de destination pour plusieurs services, ce qui la rend dynamique. Définissez si vous souhaitez abonner ou désabonner des utilisateurs et des utilisatrices lors de l’envoi du formulaire.

   ![Paramètres du service à partir de l’URL dans le composant de formulaire](assets/lp-form-service-from-url.png){zoomable="yes"}

   Lors de la conception d’un e-mail, si vous définissez un lien de type **[!UICONTROL page de destination]** vers cette page de destination, vous pouvez sélectionner n’importe quel service dans la liste. Vous pouvez ensuite sélectionner d’autres services lors de la définition d’autres liens vers cette page de destination. [En savoir plus sur l’insertion de liens](../email/message-tracking.md)

   ![Paramètres du lien d’e-mail vers la page de destination](assets/email-link-to-landing-page.png){zoomable="yes"}

1. Envoyez un message lors de la soumission de votre page de destination. [En savoir plus ici](#lp-message)

### Envoyer un message après la soumission {#lp-message}

Pour envoyer automatiquement un message de confirmation après la soumission d’une page de destination, procédez comme suit :

1. Dans la section **[!UICONTROL APPEL À L’ACTION]**, cochez l’option **[!UICONTROL Envoyer un e-mail de confirmation]**.

1. Dans la liste déroulante associée, choisissez le modèle de message transactionnel qui doit être envoyé.

![Paramètres d’e-mail de confirmation dans le composant de formulaire](assets/lp-confirmation.png){zoomable="yes"}

## Définir les styles de formulaire de page de destination {#lp-form-styles}

1. Pour modifier les styles du contenu de votre composant de formulaire, accédez à tout moment à l’onglet **[!UICONTROL Styles]**.

1. La section **[!UICONTROL Champ de texte]** est développée par défaut. Elle vous permet de modifier l’aspect des champs de texte, comme le libellé et la police, la position du libellé, la couleur d’arrière-plan du champ ou la bordure du champ.

   ![Paramètres de style de champ de texte](assets/lp-text-styles.png){zoomable="yes"}

1. Développez la section **[!UICONTROL Case à cocher]** pour définir l’aspect des cases à cocher et du texte correspondant. Par exemple, réglez la famille et la taille de police ou la couleur de la bordure de la case à cocher.

   ![Paramètres du style des cases à cocher](assets/lp-checkbox-style.png){zoomable="yes"}

1. Développez et modifiez toute autre section correspondant aux autres champs que vous avez ajoutés à votre formulaire (bouton radio, liste déroulante, date et heure, etc.).

1. Développez la section **[!UICONTROL Appel à l’action]** pour modifier l’aspect du bouton dans le formulaire du composant. Par exemple, changez de police, ajoutez une bordure, modifiez la couleur du libellé en le survolant avec votre souris ou ajustez lʼalignement du bouton.

   ![Paramètres de style d’appel à l’action](assets/lp-call-to-action-style.png){zoomable="yes"}

   Prévisualisez certains de vos paramètres, comme la couleur du libellé du bouton lorsque vous survolez en utilisant le bouton **[!UICONTROL Simuler du contenu]**. [En savoir plus](create-lp.md#test-landing-page)

1. Enregistrez vos modifications.