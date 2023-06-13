---
audience: end-user
title: Modifier le contenu de l’e-mail
description: Découvrez comment modifier le contenu de l’e-mail dans l’interface utilisateur web de Campaign.
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 42%

---

# Configuration du contenu de l&#39;email {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Créer le contenu de l’e-mail"
>abstract="Dans cette section, vous pouvez créer le contenu de votre e-mail et utiliser le concepteur d’e-mail pour peaufiner son aspect."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Paramètres de l’e-mail"
>abstract="Les valeurs De nom et De courrier électronique sont définies dans le modèle de courrier électronique. La ligne Objet peut être personnalisée à l&#39;aide de l&#39;éditeur d&#39;expression."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Pièce jointe d’e-mail"
>abstract="Sélectionnez un ou plusieurs fichiers à insérer dans votre message."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Options de tracking"
>abstract="Par défaut, le tracking est activé pour la diffusion. Vous pouvez désactiver cette option à partir de là."

L&#39;email **[!UICONTROL Modifier le contenu]** vous permet d’effectuer les opérations suivantes :
* Définissez des éléments de base de votre message, tels que l’adresse de l’expéditeur et l’objet.
* Effectuer des actions supplémentaires telles que l’ajout de pièces jointes ou la configuration d’offres
* Accédez au [Concepteur d&#39;email](get-started-email-designer.md#start-authoring) pour commencer à créer le contenu approprié de votre email

Pour configurer ou éditer le contenu d&#39;un email, procédez comme suit.

1. Cliquez sur le bouton **[!UICONTROL Modifier le contenu]** à partir du bouton [tableau de bord des diffusions email](../email/create-email.md) écran.

   ![](assets/email-edit-content-button.png)

1. L’écran d’édition du contenu d’email s’affiche.

   ![](assets/email-edit-content-dashboard.png)

   >[!NOTE]
   >
   >Si vous configurez un nouvel email, la variable **[!UICONTROL À partir du nom]** et **[!UICONTROL Adresse électronique]** sont déjà renseignés.

1. Le **[!UICONTROL À partir du nom]** est défini dans le modèle d’email. Si vous souhaitez le modifier, utilisez un nom facilement identifiable par les destinataires, tel que le nom de votre marque, afin d&#39;augmenter le taux d&#39;ouverture de vos diffusions.

   >[!NOTE]
   >
   >Pour améliorer davantage l’expérience du destinataire, vous pouvez ajouter le nom d’une personne, par exemple &quot;Eve de Luma&quot;.

1. Le **[!UICONTROL Adresse électronique]** Le champ address est également défini dans le modèle email. Assurez-vous que le domaine d’adresse est identique au sous-domaine que vous avez délégué à Adobe.

   >[!NOTE]
   >
   >Vous pouvez modifier la partie qui précède le signe &quot;@&quot;, mais pas l’adresse du domaine.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Définissez l’**[!UICONTROL Objet]** de l’e-mail. Saisissez l’objet directement dans le champ dédié ou ouvrez l’éditeur d’expression pour ajouter une personnalisation à l’aide de divers attributs, blocs de contenu ou offres. [Découvrez comment personnaliser le contenu.](../personalization/personalize.md)

1. Si vous souhaitez joindre un fichier à l’e-mail, cliquez sur le bouton **[!UICONTROL Ajouter une pièce jointe]** puis sélectionnez un ou plusieurs fichiers.

   >[!NOTE]
   >
   >    Pour éviter tout problème de performances, il est recommandé de ne pas inclure plusieurs pièces jointes par email.

   <!--limitation on size + number of files?-->

1. Si vous souhaitez envoyer des offres par e-mail, sélectionnez-les à l’aide du bouton **[!UICONTROL configurer les offres]**.

   Vous pouvez ensuite les insérer dans l’e-mail à l’aide de champs de personnalisation. [Découvrez comment envoyer des offres.](offers.md)

1. Cliquez sur le bouton **[!UICONTROL Modifier le corps de l’email]** pour structurer et concevoir le contenu de l&#39;email à l&#39;aide du bouton [Concepteur d&#39;email](#start-authoring). Des informations supplémentaires sur la conception de contenu d’e-mail sont disponibles dans les sections suivantes :

   * [Création d’emails à partir de zéro](create-email-content.md)
   * [Donner un style à votre contenu](get-started-email-style.md)

   >[!NOTE]
   >
   >Vous pouvez également passer la souris sur l’aperçu de l’email et sélectionner **[!UICONTROL Ouvrir le Concepteur d&#39;email]**.

1. Par défaut, le tracking est activé pour la diffusion. Vous pouvez désactiver cette option dans la section **[!UICONTROL Fonctionnalités facultatives]**. [Découvrez comment ajouter des liens et gérer le tracking.](message-tracking.md)

1. Une fois le contenu de votre e-mail défini, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** pour vérifier la manière dont il s’affichera avant de l’envoyer. [Découvrez comment prévisualiser et tester votre e-mail.](../preview-test/preview-test.md)

