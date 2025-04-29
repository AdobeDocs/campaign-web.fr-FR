---
audience: end-user
title: Modifier le contenu de l’e-mail
description: Découvrez comment modifier le contenu de l’e-mail dans l’interface utilisateur web de Campaign.
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: 498162045a2a58a5326a3cf311a153cf9dfef5c3
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 48%

---

# Configurer le contenu de l’e-mail {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Définir le contenu de l’e-mail"
>abstract="L’écran **Modifier le contenu** vous permet de définir des éléments de base de votre message, tels que l’adresse de l’expéditeur et l’objet, d’effectuer des actions supplémentaires telles que l’ajout de pièces jointes ou d’offres, et d’accéder au Designer d’e-mail pour donner un aspect soigné à votre message."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Définir les propriétés de l’e-mail"
>abstract="La section **Détails de base** vous permet de mettre à jour l’adresse de la personne expéditrice et l’adresse de réponse, puis de définir l’objet à l’aide de l’éditeur d’expression."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Joindre des fichiers à un e-mail"
>abstract="Sélectionnez un ou plusieurs fichiers à insérer dans votre message. Pour éviter tout problème de performances, il est recommandé de ne pas inclure plusieurs pièces jointes par email."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Modifier le tracking"
>abstract="Par défaut, le tracking est activé pour la diffusion, ce qui signifie que tous les liens inclus dans le contenu du message sont suivis. Vous pouvez désactiver cette option à partir d’ici."
>additional-url="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="Ajouter des liens et suivre les messages"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Ajouter des langues"
>abstract="Dans cet onglet, vous trouverez une liste des langues dans lesquelles la diffusion doit être envoyée. Vous pouvez ajouter d’autres langues en cliquant sur le bouton Ajouter une langue , ou en dupliquant une autre langue via cet onglet."

La fenêtre **[!UICONTROL Modifier le contenu]** de l’e-mail vous permet d’effectuer les opérations suivantes :

* Définissez des éléments de base de votre message, tels que l’adresse de l’expéditeur et l’objet.
* Exécuter des actions supplémentaires, telles que l’ajout de pièces jointes ou la configuration d’offres.
* Accédez au [Designer d’e-mail](get-started-email-designer.md#start-authoring) pour commencer à créer le contenu de votre e-mail.

>[!NOTE]
>
>Tous les champs de texte modifiables de cet écran peuvent être remplis à l’aide de champs de personnalisation. [Découvrez comment personnaliser le contenu.](../personalization/personalize.md)

Pour configurer ou modifier le contenu d’un e-mail, procédez comme suit.

1. Cliquez sur le bouton **[!UICONTROL Modifier le contenu]** à partir de la fenêtre [tableau de bord de diffusion des e-mails](../email/create-email.md).

   ![Capture d’écran affichant le bouton Modifier le contenu dans le tableau de bord de la diffusion e-mail.](assets/email-edit-content-button.png){zoomable="yes"}

1. La fenêtre de modification du contenu de l’e-mail s’ouvre.

   ![Capture d’écran affichant le tableau de bord d’édition du contenu de l’e-mail.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si vous configurez un nouvel e-mail, les champs **[!UICONTROL Nom de l’expéditeur]** et **[!UICONTROL Adresse e-mail de l’expéditeur]** sont déjà renseignés.

1. Le champ **[!UICONTROL Nom de l’expéditeur]** est défini dans le modèle d’e-mail. Si vous voulez le modifier, utilisez un nom facilement identifiable par les destinataires, tel que le nom de votre marque, pour augmenter le taux d’ouverture de vos diffusions.

   >[!NOTE]
   >
   >Pour améliorer davantage l’expérience des destinataires, vous pouvez ajouter le nom d’une personne, par exemple « Eve de Luma ».

1. Le champ **[!UICONTROL Adresse e-mail de l’expéditeur]** est également défini dans le modèle d’e-mail. Assurez-vous que le domaine de l’adresse correspond au sous-domaine que vous avez délégué à Adobe.

   >[!NOTE]
   >
   >Vous pouvez modifier la partie qui précède le signe « @ », mais pas l’adresse du domaine.

1. Développez la section **[!UICONTROL Champs de réponse]**. Le nom et l’adresse de la personne expéditrice sont utilisés par défaut pour les réponses. Cependant, Adobe recommande d’utiliser une adresse réelle existante, telle que l’assistance clientèle de votre marque. Dans ce cas, si un destinataire envoie une réponse, l’équipe de l’assistance clientèle sera en mesure de la gérer.

   ![Capture d’écran affichant la section Champs de réponse dans l’éditeur de contenu d’e-mail.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Définissez l’**[!UICONTROL Objet]** de l’e-mail. Saisissez directement l’objet dans le champ dédié ou ouvrez l’éditeur d’expression pour ajouter [personnalisation](../personalization/personalize.md) à l’aide de divers attributs, fragments d’expression ou offres.

1. Si vous souhaitez joindre un fichier à l’e-mail, cliquez sur le bouton **[!UICONTROL Ajouter une pièce jointe]**, puis sélectionnez un ou plusieurs fichiers.

   >[!NOTE]
   >
   >Pour éviter tout problème de performances, il est recommandé de ne pas inclure plusieurs pièces jointes par email.

   <!--limitation on size + number of files?-->

1. Si vous souhaitez envoyer des offres par e-mail, sélectionnez-les à l’aide du bouton **[!UICONTROL configurer les offres]**.

   Vous pouvez ensuite les insérer dans l’e-mail à l’aide de champs de personnalisation. [Découvrez comment envoyer des offres.](../msg/offers.md)

1. Cliquez sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]** pour organiser et concevoir le contenu de l’e-mail en utilisant le [concepteur d’e-mail](get-started-email-designer.md#start-authoring). Pour plus d’informations sur la conception de contenu d’e-mail, consultez les sections suivantes :

   * [Rédiger des e-mails à partir de zéro](create-email-content.md)
   * [Donner un style à votre contenu](get-started-email-style.md)

   >[!NOTE]
   >
   >Vous pouvez également pointer sur l’aperçu de l’e-mail et sélectionner **[!UICONTROL Ouvrir le concepteur d&#39;e-mail]**.

1. Par défaut, le tracking est activé pour la diffusion. Vous pouvez désactiver cette option dans la section **[!UICONTROL Fonctionnalités facultatives]**. [Découvrez comment ajouter des liens et gérer le tracking](message-tracking.md).

1. Une fois le contenu de votre e-mail défini, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** pour vérifier la manière dont il s’affichera avant de l’envoyer. [Découvrez comment prévisualiser et tester votre e-mail](../preview-test/preview-test.md).