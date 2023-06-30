---
audience: end-user
title: Modifier le contenu de l’e-mail
description: Découvrez comment modifier le contenu de l’e-mail dans l’interface utilisateur web de Campaign.
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '506'
ht-degree: 100%

---

# Configurer le contenu de l’e-mail {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Créer le contenu de l’e-mail"
>abstract="Dans cette section, vous pouvez créer le contenu de votre e-mail et utiliser le concepteur d’e-mail pour peaufiner son aspect."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Paramètres de l’e-mail"
>abstract="Définissez les valeurs Nom de l’expéditeur et Adresse e-mail de l’expéditeur dans le modèle d’e-mail. Vous pouvez également personnaliser l’objet de l’e-mail dans l’éditeur d’expression."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Pièce jointe d’e-mail"
>abstract="Sélectionnez un ou plusieurs fichiers à insérer dans votre message."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Options de tracking"
>abstract="Par défaut, le tracking est activé pour la diffusion. Vous pouvez désactiver cette option à partir de là."

La fenêtre **[!UICONTROL Modifier le contenu]** de l’e-mail vous permet d’effectuer les opérations suivantes :
* Définir des éléments de base de votre message, tels que l’adresse de l’expéditeur et l’objet.
* Effectuer des actions supplémentaires telles que l’ajout de pièces jointes ou la configuration d’offres.
* Accéder au [Concepteur d’e-mail](get-started-email-designer.md#start-authoring) pour commencer à créer le contenu de votre e-mail.

Pour configurer ou modifier le contenu d’un e-mail, procédez comme suit.

1. Cliquez sur le bouton **[!UICONTROL Modifier le contenu]** à partir de la fenêtre [tableau de bord de diffusion des e-mails](../email/create-email.md).

   ![](assets/email-edit-content-button.png)

1. La fenêtre de modification du contenu de l’e-mail s’ouvre.

   ![](assets/email-edit-content-dashboard.png)

   >[!NOTE]
   >
   >Si vous configurez un nouvel e-mail, les champs **[!UICONTROL Nom de l’expéditeur]** et **[!UICONTROL Adresse e-mail de l’expéditeur]** sont déjà renseignés.

1. Le champ **[!UICONTROL Nom de l’expéditeur]** est défini dans le modèle d’e-mail. Si vous voulez le modifier, utilisez un nom facilement identifiable par les destinataires, tel que le nom de votre marque, pour augmenter le taux d’ouverture de vos diffusions.

   >[!NOTE]
   >
   >Pour améliorer davantage l’expérience des destinataires, vous pouvez ajouter le nom d’une personne, par exemple « Eve de Luma ».

1. Le champ **[!UICONTROL Adresse e-mail de l’expéditeur]** est également défini dans le modèle d’e-mail. Assurez-vous que le domaine de l’adresse est identique au sous-domaine délégué à Adobe.

   >[!NOTE]
   >
   >Vous pouvez modifier la partie qui précède le signe « @ », mais pas l’adresse du domaine.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Définissez l’**[!UICONTROL Objet]** de l’e-mail. Saisissez directement l’objet dans le champ dédié ou ouvrez l’éditeur d’expression pour ajouter de la personnalisation à l’aide de divers attributs, blocs de contenu ou offres. [Découvrez comment personnaliser le contenu.](../personalization/personalize.md)

1. Si vous souhaitez joindre un fichier à l’e-mail, cliquez sur le bouton **[!UICONTROL Ajouter une pièce jointe]** puis sélectionnez un ou plusieurs fichiers.

   >[!NOTE]
   >
   >    Pour éviter tout problème de performances, il est recommandé de ne pas inclure plusieurs pièces jointes par email.

   <!--limitation on size + number of files?-->

1. Si vous souhaitez envoyer des offres par e-mail, sélectionnez-les à l’aide du bouton **[!UICONTROL configurer les offres]**.

   Vous pouvez ensuite les insérer dans l’e-mail à l’aide de champs de personnalisation. [Découvrez comment envoyer des offres.](offers.md)

1. Cliquez sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]** pour organiser et concevoir le contenu de l’e-mail en utilisant le [Concepteur d’e-mail](#start-authoring). Des informations supplémentaires sur la conception de contenu d’e-mail sont disponibles dans les sections suivantes :

   * [Rédiger des e-mails à partir de zéro](create-email-content.md)
   * [Donner un style à votre contenu](get-started-email-style.md)

   >[!NOTE]
   >
   >Vous pouvez également pointer sur l’aperçu de l’e-mail et sélectionner **[!UICONTROL Ouvrir le concepteur d&#39;e-mail]**.

1. Par défaut, le tracking est activé pour la diffusion. Vous pouvez désactiver cette option dans la section **[!UICONTROL Fonctionnalités facultatives]**. [Découvrez comment ajouter des liens et gérer le tracking.](message-tracking.md)

1. Une fois le contenu de votre e-mail défini, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** pour vérifier la manière dont il s’affichera avant de l’envoyer. [Découvrez comment prévisualiser et tester votre e-mail.](../preview-test/preview-test.md)

