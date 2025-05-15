---
audience: end-user
title: Modifier le contenu de l’e-mail
description: Découvrez comment modifier le contenu de l’e-mail dans l’interface utilisateur web de Campaign.
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: df5883f8178bc5287145c587b06dd5664400ed90
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 57%

---

# Configurer le contenu de l’e-mail {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Définir le contenu de l’e-mail"
>abstract="L’écran **Modifier le contenu** vous permet de définir les éléments de base de votre message, tels que l’adresse de la personne expéditrice et l’objet, d’effectuer des actions supplémentaires, telles que l’ajout de pièces jointes ou d’offres, et d’accéder au concepteur d’e-mail pour peaufiner l’aspect de votre message."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Définir les propriétés de l’e-mail"
>abstract="La section **Détails de base** vous permet de mettre à jour l’adresse de la personne expéditrice et l’adresse de réponse, puis de définir l’objet à l’aide de l’éditeur d’expression."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Joindre des fichiers à un e-mail"
>abstract="Sélectionnez un ou plusieurs fichiers à insérer dans votre message. Pour éviter tout problème de performances, il est recommandé de ne pas inclure plusieurs pièces jointes par e-mail."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Modifier le tracking"
>abstract="Par défaut, le tracking est activé pour la diffusion, ce qui signifie que tous les liens inclus dans le contenu du message sont suivis. Vous pouvez désactiver cette option à partir d’ici."
>additional-url="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="Ajouter des liens et suivre les messages"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Ajouter des langues"
>abstract="Dans cet onglet, vous trouverez une liste des langues dans lesquelles la diffusion doit être envoyée. Vous pouvez ajouter d’autres langues en cliquant sur le bouton Ajouter une langue, ou en dupliquant une autre langue via cet onglet."

La fenêtre **[!UICONTROL Modifier le contenu]** de l’e-mail vous permet d’effectuer les opérations suivantes :

* Définir des éléments de base de votre message, tels que l’adresse de l’expéditeur et l’objet.
* Effectuer des actions supplémentaires telles que l’ajout de pièces jointes ou la configuration d’offres.
* Accéder au [concepteur d’e-mail](get-started-email-designer.md#start-authoring) pour commencer à créer le contenu de votre e-mail.
* Ajoutez des variantes linguistiques à vos diffusions.

>[!NOTE]
>
>Tous les champs de texte modifiables de cet écran peuvent être remplis à l’aide de champs de personnalisation. [Découvrez comment personnaliser le contenu.](../personalization/personalize.md)

## Configuration de la diffusion

Pour configurer ou modifier le contenu d’un e-mail, procédez comme suit.

1. Cliquez sur le bouton **[!UICONTROL Modifier le contenu]** à partir de la fenêtre [tableau de bord de diffusion des e-mails](../email/create-email.md).

   ![Capture d’écran montrant le bouton Modifier le contenu dans le tableau de bord de la diffusion e-mail.](assets/email-edit-content-button.png){zoomable="yes"}

1. La fenêtre de modification du contenu de l’e-mail s’ouvre.

   ![Capture d’écran montrant le tableau de bord de modification du contenu de l’e-mail.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si vous configurez un nouvel e-mail, les champs **[!UICONTROL Nom de la personne expéditrice]** et **[!UICONTROL Adresse e-mail de la personne expéditrice]** sont déjà renseignés.

1. Le champ **[!UICONTROL Nom de l’expéditeur]** est défini dans le modèle d’e-mail. Si vous voulez le modifier, utilisez un nom facilement identifiable par les destinataires, tel que le nom de votre marque, pour augmenter le taux d’ouverture de vos diffusions.

   >[!NOTE]
   >
   >Pour améliorer davantage l’expérience des destinataires, vous pouvez ajouter le nom d’une personne, par exemple « Eve de Luma ».

1. Le champ **[!UICONTROL Adresse e-mail de l’expéditeur]** est également défini dans le modèle d’e-mail. Assurez-vous que le domaine de l’adresse est identique au sous-domaine délégué à Adobe.

   >[!NOTE]
   >
   >Vous pouvez modifier la partie qui précède le signe « @ », mais pas l’adresse du domaine.

1. Développez la section **[!UICONTROL Champs de réponse]**. Le nom et l’adresse de la personne expéditrice sont utilisés par défaut pour les réponses. Adobe recommande toutefois d’utiliser une adresse réelle existante, telle que l’assistance clientèle de votre marque. Ainsi, si une personne destinataire envoie une réponse, l’assistance clientèle sera en mesure de la traiter.

   ![Capture d’écran montrant la section Champs de réponse dans l’éditeur de contenu d’e-mail.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Définissez l’**[!UICONTROL Objet]** de l’e-mail. Saisissez directement l’objet dans le champ dédié ou ouvrez l’éditeur d’expression pour ajouter des éléments de [personnalisation](../personalization/personalize.md) à l’aide de divers attributs, fragments d’expression ou offres.

1. Si vous souhaitez joindre un fichier à l’e-mail, cliquez sur le bouton **[!UICONTROL Ajouter une pièce jointe]** puis sélectionnez un ou plusieurs fichiers.

   >[!NOTE]
   >
   >Pour éviter tout problème de performances, il est recommandé de ne pas inclure plusieurs pièces jointes par e-mail.

   <!--limitation on size + number of files?-->

1. Si vous souhaitez envoyer des offres par e-mail, sélectionnez-les à l’aide du bouton **[!UICONTROL configurer les offres]**.

   Vous pouvez ensuite les insérer dans l’e-mail à l’aide des champs de personnalisation. [Découvrez comment envoyer des offres.](../msg/offers.md)

## Modifier le corps de l’e-mail

1. Cliquez sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]** pour structurer et concevoir le contenu de l’e-mail à l’aide du [Designer d’e-mail](get-started-email-designer.md#start-authoring).

   >[!NOTE]
   >
   >Vous pouvez également pointer sur l’aperçu de l’e-mail et sélectionner **[!UICONTROL Ouvrir le concepteur d&#39;e-mail]**.


   Des informations supplémentaires sur la conception de contenu d’e-mail sont disponibles dans les sections suivantes :

   * [Rédiger des e-mails à partir de zéro](create-email-content.md)
   * [Donner un style à votre contenu](get-started-email-style.md)

1. Par défaut, le tracking est activé pour la diffusion. Vous pouvez désactiver cette option dans la section **[!UICONTROL Fonctionnalités facultatives]**. [Découvrez comment ajouter des liens et gérer le tracking.](message-tracking.md)

1. Une fois le contenu de votre e-mail défini, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** pour vérifier la manière dont il s’affichera avant de l’envoyer. [Découvrez comment prévisualiser et tester votre e-mail.](../preview-test/preview-test.md)

## Configurer une diffusion multilingue

Dans l’interface utilisateur web de Campaign, vous pouvez configurer vos diffusions e-mail en tant que multilingues, ce qui vous permet d’envoyer des messages en fonction de la langue préférée d’un profil. Lorsqu’aucune préférence n’est définie, le message est envoyé dans la langue par défaut.

Dans une diffusion multilingue, la gestion des langues repose sur des variantes. Chaque variante représente une langue.

Lors de la création de la diffusion, vous pouvez ajouter le nombre de variantes correspondant au nombre de langues nécessaires dans le message. Vous pouvez également définir la langue par défaut lors de l’ajout de nouvelles langues.

### Ajouter une variante de langue

Pour créer des variantes de langue, procédez comme suit :

1. Cliquez sur le bouton **[!UICONTROL Ajouter une langue]** dans la section supérieure de l’écran de configuration de l’e-mail.

   >[!IMPORTANT]
   >
   >Le bouton **[!UICONTROL Ajouter une langue]** n’est disponible que si la dimension cible contient le schéma Langue . Pour en savoir plus sur les schémas et les dimensions de la cible, consultez la [documentation détaillée](https://experienceleague.adobe.com/en/docs/campaign-web/v8/audiences/targeting-dimensions){target=_blank}.

   ![](assets/edit-content_2.png){zoomable="yes"}


1. Sélectionnez la langue à ajouter dans la liste déroulante **[!UICONTROL Langue]**. Lors de l’ajout de la première langue, elle est définie par défaut et le contenu actuel est celui par défaut. Lorsque vous ajoutez de nouvelles langues, le contenu est basé sur le contenu par défaut.

   >[!NOTE]
   >
   >Les langues disponibles dans cette liste dépendent des valeurs définies par l’attribut Langue (valeurs telles que : système, utilisateur, dbenum, etc.) En savoir plus sur la gestion des énumérations dans cette [section](https://experienceleague.adobe.com/en/docs/campaign-web/v8/conf/enumerations){target=_blank}.


   ![](assets/edit-content_3.png){zoomable="yes"}

   Par exemple ici, pour l’anglais (US) :

   ![](assets/edit-content_8.png){zoomable="yes"}


1. Répétez ce processus pour ajouter d’autres langues. Le panneau **[!UICONTROL Langue]** affiche la liste des langues sélectionnées, le nombre de langues différentes ainsi que la langue par défaut.

   Par exemple, si vous avez choisi l’anglais, le français et le suédois, vous pouvez voir ces 3 langues comme illustré ci-dessous :

   ![](assets/edit-content_9.png){zoomable="yes"}

   Vous pouvez cliquer sur le bouton Développer dans le coin supérieur droit pour supprimer toutes les langues.

### Définir le contenu de l’e-mail pour chaque variante

Une fois les langues définies, définissez le contenu de l’e-mail qui sera envoyé aux profils avec cette langue préférée.

Pour définir le contenu d’un e-mail, procédez comme suit :

1. Ouvrez le [Designer d’e-mail](get-started-email-designer.md#start-authoring) en cliquant sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]**.

   >[!NOTE]
   >
   >Vous pouvez également pointer sur l’aperçu de l’e-mail et sélectionner **[!UICONTROL Ouvrir le concepteur d&#39;e-mail]**.

   ![](assets/edit-content_11.png){zoomable="yes"}


1. Vous pouvez prévisualiser la diffusion en cliquant sur le bouton **[!UICONTROL Simuler du contenu]**, puis choisir le profil et la langue d’affichage de l’e-mail.

1. Dans la fenêtre Simuler du contenu , vous pouvez changer de profil pour prévisualiser le contenu de l’e-mail correspondant à la langue configurée pour ce profil.

   ![](assets/edit-content_5.png){zoomable="yes"}

### Dupliquer ou supprimer des variantes de langue

Vous pouvez cliquer sur le bouton de développement dans le coin supérieur droit, puis cliquer sur le bouton **[!UICONTROL Supprimer toutes les variantes]** pour supprimer toutes les langues.

![](assets/edit-content_13.png){zoomable="yes"}

Pour supprimer une variante de langue, cliquez sur les trois points du côté droit de l’onglet et sélectionnez Supprimer.

Pour dupliquer une variante de langue, cliquez sur les trois points du côté droit de l’onglet et sélectionnez Dupliquer. Si vous choisissez de dupliquer une langue autre que la langue par défaut, le contenu dupliqué sera basé sur la langue que vous avez choisi de dupliquer.


1. Une fois le contenu de votre e-mail défini, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** pour vérifier la manière dont il s’affichera avant de l’envoyer. [Découvrez comment prévisualiser et tester votre e-mail.](../preview-test/preview-test.md)