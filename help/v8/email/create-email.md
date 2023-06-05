---
audience: end-user
title: Envoyer votre premier e-mail
description: Découvrez comment envoyer votre premier e-mail avec l’interface utilisateur web de Campaign.
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
badge: label="Alpha" type="Positive"
source-git-commit: 983541f5dea47102ae9ee3c5351a7149484a1fa5
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 85%

---


# Envoyer votre premier e-mail {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_card2"
>title="Prise en main des e-mails"
>abstract="Commencez à partir d’un modèle ou utilisez Adobe Campaign pour créer un nouveau Concepteur d’email afin de créer des emails sans avoir à écrire une seule ligne de code. Découvrez comment utiliser le Concepteur d&#39;email pour créer votre contenu, le prévisualiser et le tester, puis envoyer un email à une audience existante dans un cas pratique de bout en bout."


Découvrez comment créer votre premier e-mail ciblé. Dans ce cas d’utilisation, vous planifiez l’envoi d’un e-mail aux membres argent et or du programme de fidélité à une date spécifique.

Basé sur un modèle de conception prédéfini, l’e-mail propose également du contenu personnalisé basé sur les attributs de profil du client ou de la cliente.

![](assets/delivery-list.png)

## Créer la diffusion email {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Sélectionnez un modèle d’e-mail."
>abstract="Un modèle d’e-mail est une configuration de diffusion spécifique qui contient des paramètres prédéfinis, tels que des règles de typologie, des paramètres de personnalisation ou de routage. Les modèles sont définis dans la console cliente Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Propriétés de l’e-mail"
>abstract="Les propriétés sont les paramètres de diffusion courants qui vous permettent de nommer et de classer votre diffusion. Si votre diffusion est basée sur un schéma étendu défini dans la console Adobe Campaign v8, des champs spécifiques d’**Options personnalisées** sont disponibles."

Pour créer une diffusion, procédez comme suit :

1. Accédez au **[!UICONTROL Diffusions]** sur le rail de gauche, puis cliquez sur le  **[!UICONTROL Créer une diffusion]** bouton .

1. Sélectionner **[!UICONTROL Email]** comme canal et choisissez un modèle de diffusion email dans la liste.

   >[!NOTE]
   >
   >Les modèles sont des paramètres de diffusion préconfigurés enregistrés en vue d’une utilisation ultérieure. [En savoir plus](../msg/delivery-template.md)

   ![](assets/channel-template.png)

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.
1. Indiquez un libellé pour la diffusion et configurez les options supplémentaires en fonction de vos besoins :

   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion,
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique,
   * **[!UICONTROL Code de diffusion]** : utilisez ce champ pour organiser vos diffusions selon votre propre convention de nommage,
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion,
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Si vous avez étendu votre schéma avec des champs personnalisés spécifiques, vous pouvez y accéder dans la section **[!UICONTROL Options personnalisées]**.

   ![](assets/email-properties.png)

   En outre, vous pouvez accéder aux paramètres avancés, tels que les règles de typologie et les mappings de ciblage, en cliquant sur le bouton situé à côté du nom de la diffusion. Ces paramètres sont préconfigurés dans le modèle sélectionné, mais peuvent être modifiés selon les besoins pour cet e-mail spécifique.

## Définition du contenu de l’e-mail {#create-content}

Pour commencer à créer le contenu de votre email, procédez comme suit.

<!--Detailed instructions on how to configure the email content are available in [this section](../content/edit-content.md).-->

Dans ce cas pratique, vous utilisez un email prédéfini [modèle de diffusion](../msg/delivery-template.md) pour concevoir votre email.

1. Dans le tableau de bord des diffusions email, cliquez sur le bouton **[!UICONTROL Modifier le contenu]** bouton .

   ![](assets/email-edit-content.png)

   Vous accédez ainsi à une interface dédiée dans laquelle vous pouvez configurer le contenu de l&#39;email et accéder au Concepteur d&#39;email. [En savoir plus](../content/edit-content.md)

   ![](assets/edit-content.png)

1. Indiquez l’objet de l’e-mail et personnalisez-le à l’aide de l’éditeur d’expression. [Découvrez comment personnaliser du contenu](../personalization/personalize.md).

   ![](assets/subject-line.png)

1. Pour concevoir le contenu de l’e-mail, cliquez sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]**.

   Sélectionnez la méthode à utiliser pour créer le contenu de l’e-mail. Dans cet exemple, utilisez une [modèle de contenu prédéfini](../msg/delivery-template.md).

   ![](assets/select-template.png)

   <!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Une fois le modèle sélectionné, il s’affiche dans la [Concepteur d&#39;email](../content/create-email-content.md), où vous pouvez apporter les modifications nécessaires et ajouter une personnalisation.

   Par exemple, pour personnaliser le titre de l’e-mail, sélectionnez le bloc de composant et cliquez sur **[!UICONTROL Ajouter une personnalisation]**.

   ![](assets/add-perso.png)

1. Une fois que vous êtes satisfait du contenu, enregistrez et fermez votre conception. Cliquez sur **[!UICONTROL Enregistrer]** pour revenir à l’écran de création d’e-mail.

   ![](assets/save-content.png)

## Définir l’audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Définir l’audience"
>abstract="Sélectionnez l’audience la plus appropriée pour votre message marketing. Vous pouvez choisir une audience existante déjà définie dans une instance Campaign v8 ou dans Adobe Experience Platform ou choisir de créer une nouvelle audience à l’aide du créateur de règles. Les groupes de contrôle ne sont pas activés pour &quot;Select from file&quot; et vice versa."

Dans ce cas d’utilisation, vous envoyez l’e-mail à une audience existante. Des instructions supplémentaires sur l’utilisation des audiences sont disponibles dans [cette section](../audience/about-audiences.md).

1. Pour sélectionner l’audience de l’e-mail, cliquez sur le bouton **[!UICONTROL Sélectionner l’audience]** et choisissez une audience existante dans la liste.

   Dans cet exemple, nous allons utiliser une audience existante ciblant des client(e)s appartenant aux niveaux de points de fidélité argent et or.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Les audiences disponibles dans la liste proviennent de votre instance Campaign v8 ou d’Adobe Experience Platform si l’intégration Destination/Sources a été configurée sur votre instance.
   >
   >L’intégration Destination/Sources vous permet d’envoyer des segments Experience Platform vers Adobe Campaign et d’envoyer des logs de diffusion et de tracking Campaign à Adobe Experience Platform. [Découvrez comment utiliser Campaign et Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html?lang=fr){target="_blank"}.

1. Une fois l’audience sélectionnée, vous pouvez affiner davantage la cible en appliquant des règles supplémentaires.

   Vous pouvez également définir une population témoin afin d’analyser le comportement des destinataires de l’e-mail par rapport au comportement des profils qui n’ont pas été ciblés. [Découvrez comment travailler avec les populations témoins.](../audience/control-group.md)

   ![](assets/audience-selected.png)

## Planifier l’envoi {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Planifier l’envoi"
>abstract="Définissez la date et l’heure exactes de votre envoi. En choisissant l’heure la plus appropriée pour votre message marketing, vous pouvez maximiser les taux d’ouverture."

Pour planifier l’envoi de l’e-mail, ouvrez votre diffusion e-mail et accédez à la section **Planning**. Utilisez le bouton (bascule) **[!UICONTROL Activer le planning]** pour l’activer et définir la date et l’heure d’envoi. Une fois la diffusion envoyée, l’envoi effectif démarre à la date de contact que vous avez définie.

Par défaut, l’option **[!UICONTROL Activer la confirmation avant l’envoi]** est activée. Cette option nécessite de confirmer l’envoi avant que l’e-mail ne soit envoyé à la date et à l’heure planifiées. Si vous souhaitez envoyer automatiquement l’e-mail à la date et l’heure planifiées, vous pouvez désactiver cette option.

![](assets/schedule.png)

## Prévisualiser et tester l’e-mail {#preview-test}

Avant d’envoyer votre e-mail, vous pouvez le prévisualiser et le tester pour vous assurer qu’il répond à vos attentes.

Dans ce cas d’utilisation, vous prévisualisez l’e-mail et envoyez des versions de test à des adresses e-mail spécifiques tout en empruntant l’identité de certains des profils ciblés.

Des informations supplémentaires sur la prévisualisation et le test des e-mails sont disponibles dans [cette section](../preview-test/preview-test.md).

1. Pour vérifier votre e-mail, cliquez sur **[!UICONTROL Vérifier et envoyer]**. Un aperçu de votre e-mail s’affiche, ainsi que toutes les propriétés, l’audience et le planning configurés. Vous pouvez modifier chacun de ces éléments en cliquant sur le bouton Modifier.

1. Pour prévisualiser l’e-mail et envoyer les versions de test, cliquez sur le bouton **[!UICONTROL Simuler du contenu]**.

   ![](assets/review-email.png)

1. Dans la zone de gauche, sélectionnez le ou les profils que vous souhaitez utiliser pour prévisualiser l’e-mail.

   Le volet de droite affiche un aperçu de l’e-mail en fonction du profil sélectionné. Si vous avez ajouté plusieurs profils, vous pouvez passer d’un profil à l’autre pour prévisualiser l’e-mail correspondant.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Pour envoyer des versions de test de votre e-mail, cliquez sur le bouton **[!UICONTROL Test]**, puis sélectionnez le mode que vous souhaitez utiliser.

   Dans cet exemple, utilisez le mode **[!UICONTROL Substituer à partir de la cible principale]**, qui envoie des versions de test à des adresses e-mail spécifiques tout en empruntant l’identité de certains des profils ciblés par l’e-mail.

   ![](assets/proof-mode.png)

1. Cliquez sur **[!UICONTROL Ajouter une adresse]** et indiquez la ou les adresses e-mail qui reçoivent les versions de test.

   Pour chaque adresse e-mail, sélectionnez le profil dont vous souhaitez emprunter l’identité. Vous pouvez également laisser Adobe Campaign sélectionner un profil aléatoire à partir de la cible.

   ![](assets/proof-test-profile.png)

1. Cliquez sur **[!UICONTROL Envoyer un e-mail de test]**, puis confirmez l’envoi.

   Les versions de test sont envoyées aux adresses e-mail spécifiées à l’aide du profil sélectionné avec le préfixe **[BAT x]**.

   ![](assets/proof-sent.png)

   Vous pouvez vérifier à tout moment le statut de l’envoi et accéder aux e-mails de test envoyés en cliquant sur le bouton **[!UICONTROL Afficher le journal des e-mails de test]** dans l’écran Simuler du contenu.

## Envoyer et surveiller l’e-mail {#prepare-send}

Après avoir validé et testé votre e-mail, vous pouvez lancer sa préparation et l’envoyer.

1. Pour lancer la préparation de l’e-mail, cliquez sur **[!UICONTROL Préparer]**. [Découvrez comment préparer un e-mail](../monitor/prepare-send.md).

   ![](assets/preparation.png)

1. Une fois que votre e-mail est prêt à être envoyé, cliquez sur le bouton **[!UICONTROL Envoyer]** (ou **[!UICONTROL Envoyer comme prévu]** si vous avez planifié son envoi) et confirmez l’envoi.

1. Au cours du processus d’envoi, vous pouvez suivre son avancement et visualiser les statistiques en temps réel directement à partir de cet écran.

   ![](assets/sent-mail.png)

   Vous pouvez également accéder à des informations détaillées sur l’envoi en cliquant sur le bouton **[!UICONTROL Logs]**. [Découvrez comment surveiller les logs de diffusion](../monitor/delivery-logs.md).

1. Une fois l’e-mail envoyé, vous pouvez accéder à des rapports dédiés pour une analyse plus approfondie en cliquant sur le bouton **[!UICONTROL Créer des rapports]**.

![](assets/reports.png)
