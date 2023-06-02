---
audience: end-user
title: Modifier le contenu de l’e-mail
description: Découvrez comment modifier le contenu de l’e-mail dans l’interface utilisateur web de Campaign.
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: f04e8aa5ecb12fca02da640b0037441d4cd7d4d3
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 73%

---

# Modifier le contenu de l’e-mail {#configure-content}

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

Pour commencer à créer le contenu d’un e-mail, cliquez sur le bouton **[!UICONTROL Modifier le contenu]** à partir de l’écran de création d’e-mail.[](../email/create-email.md)

![](assets/email-edit-content.png)

L’écran qui s’ouvre vous permet de définir des détails de base, d’effectuer certaines actions supplémentaires, telles que l’ajout de pièces jointes ou la configuration d’offres, et d’accéder au Concepteur d’email pour créer votre contenu.

![](assets/email-edit-content-dashboard.png)

Les étapes pour éditer le contenu de votre email sont les suivantes :

1. Dans le **[!UICONTROL À partir du nom]** , utilisez un nom facilement identifiable par les destinataires, comme le nom de votre marque, pour augmenter le taux d’ouverture de vos diffusions.

1. Définissez l’**[!UICONTROL Objet]** de l’e-mail. Pour ce faire, saisissez directement l’objet dans le champ dédié ou ouvrez l’éditeur d’expression pour ajouter de la personnalisation à l’aide de divers attributs, blocs de contenu ou offres. [Découvrez comment personnaliser le contenu.](../personalization/personalize.md)
Pour améliorer davantage l’expérience des destinataires, vous pouvez ajouter le nom d’une personne, par exemple « Emma de Megastore ».

1. Dans le **[!UICONTROL Adresse électronique]** champ adresse , assurez-vous que le domaine de l’adresse est identique au sous-domaine que vous avez délégué à Adobe.

   Vous pouvez modifier la partie qui précède le signe &quot;@&quot;, mais pas l’adresse du domaine.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Définissez l’**[!UICONTROL Objet]** de l’e-mail. Saisissez l’objet directement dans le champ dédié ou ouvrez l’éditeur d’expression pour ajouter une personnalisation à l’aide de divers attributs, blocs de contenu ou offres. [Découvrez comment personnaliser le contenu.](../personalization/personalize.md)

1. Si vous souhaitez joindre un fichier à l’e-mail, cliquez sur le bouton **[!UICONTROL Ajouter une pièce jointe]** puis sélectionnez un ou plusieurs fichiers.

   >[!NOTE]
   >
   >    Pour éviter tout problème de performances, il est recommandé de ne pas inclure plusieurs pièces jointes par email.

   <!--limitation on size + number of files?-->

1. Si vous souhaitez envoyer des offres par e-mail, sélectionnez-les à l’aide du bouton **[!UICONTROL configurer les offres]**.

   Vous pouvez ensuite les insérer dans l’e-mail à l’aide de champs de personnalisation. [Découvrez comment envoyer des offres.](offers.md)

1. Cliquez sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]** pour organiser et concevoir le contenu de l’e-mail. Des informations supplémentaires sur la conception de contenu d’e-mail sont disponibles dans les sections suivantes :

   * [Découvrez comment concevoir des e-mails](create-email-content.md)
   * [Donner un style à votre contenu](get-started-email-style.md)

1. Par défaut, le tracking est activé pour la diffusion. Vous pouvez désactiver cette option dans la section **[!UICONTROL Fonctionnalités facultatives]**. [Découvrez comment ajouter des liens et gérer le tracking.](message-tracking.md)

1. Une fois le contenu de votre e-mail défini, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** pour vérifier la manière dont il s’affichera avant de l’envoyer. [Découvrez comment prévisualiser et tester votre e-mail.](../preview-test/preview-test.md)
