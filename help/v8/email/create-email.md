---
audience: end-user
title: Envoyer votre premier e-mail
description: Découvrez comment envoyer votre premier email avec l’interface utilisateur web de Campaign
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 24%

---

# Envoyer votre premier e-mail {#first-email}

![](../assets/do-not-localize/badge.png)

Découvrez comment créer votre premier email ciblé. Dans ce cas pratique, vous planifiez l’envoi d’un email aux membres Silver et Gold à une date spécifique.

Basé sur un modèle de conception prédéfini, l’email propose également du contenu personnalisé basé sur les attributs de profil du client.

![](assets/delivery-list.png)

## Créer l’e-mail {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Sélectionnez un modèle d’e-mail."
>abstract="Un modèle d’email est une configuration de diffusion spécifique qui contient des paramètres prédéfinis, tels que des règles de typologie, des paramètres de personnalisation ou de routage. Les modèles sont définis dans la console cliente Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Propriétés de l’e-mail"
>abstract="Les propriétés sont les paramètres de diffusion courants qui vous permettent de nommer et de classer votre diffusion. Si votre diffusion est basée sur un schéma étendu défini dans la console Adobe Campaign v8, des champs spécifiques d’**Options personnalisées** sont disponibles."

1. Pour créer une diffusion, accédez au **[!UICONTROL Diffusions]** et sélectionnez **[!UICONTROL Email]** comme canal.

1. Sélectionnez le modèle à utiliser, puis cliquez sur **[!UICONTROL Créer une diffusion]**.

   >[!NOTE]
   >
   >Les modèles sont des paramètres de diffusion préconfigurés enregistrés en vue d’une utilisation ultérieure. Ils peuvent être créés par les utilisateurs administrateurs dans la console Adobe Campaign. [Découvrez comment utiliser les modèles de diffusion](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html?lang=fr){target="_blank"}.

   ![](assets/channel-template.png)

1. Indiquez un libellé pour l’e-mail et configurez les options supplémentaires en fonction de vos besoins :

   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion,
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique,
   * **[!UICONTROL Code de diffusion]** : utilisez ce champ pour organiser vos diffusions selon votre propre convention de nommage,
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion,
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Si vous avez étendu votre schéma avec des champs personnalisés spécifiques, vous pouvez y accéder dans la variable **[!UICONTROL Options personnalisées]** .

   ![](assets/email-properties.png)

   En outre, des paramètres avancés, tels que les règles de typologie et les mappings de ciblage, sont accessibles en cliquant sur le bouton situé en regard du nom de la diffusion. Ces paramètres sont préconfigurés dans le modèle sélectionné, mais peuvent être modifiés selon les besoins pour cet email spécifique.

## Créer le contenu de l’e-mail {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Découvrez comment concevoir le contenu de votre email"
>abstract="Découvrez comment utiliser le Concepteur d&#39;email."

Dans ce cas pratique, vous utilisez un modèle prédéfini pour concevoir votre email.

Des instructions détaillées sur la configuration du contenu de l’email sont disponibles dans la section [cette section](../content/edit-content.md).

1. Pour commencer à créer le contenu de l&#39;email, cliquez sur le bouton **[!UICONTROL Modifier le contenu]** bouton .

   Vous accédez ainsi à une interface dédiée dans laquelle vous pouvez configurer le contenu de l&#39;email et le concevoir à l&#39;aide du Concepteur d&#39;email.

   ![](assets/edit-content.png)

1. Saisissez l&#39;objet de votre email et personnalisez-le à l&#39;aide de l&#39;éditeur d&#39;expression. [Découvrez comment personnaliser du contenu](../personalization/personalize.md).

   ![](assets/subject-line.png)

1. Pour concevoir le corps de l&#39;email, cliquez sur le bouton **[!UICONTROL Modifier le corps de l’email]** bouton .

   Sélectionnez la méthode à utiliser pour créer le contenu de l’e-mail. Dans cet exemple, utilisez un modèle de conception prédéfini.

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Une fois le modèle sélectionné, il s&#39;affiche dans le Concepteur d&#39;email, où vous pouvez apporter les modifications nécessaires et ajouter une personnalisation.

   Par exemple, pour ajouter une personnalisation au titre de l’email, sélectionnez le bloc de composant et cliquez sur **[!UICONTROL Ajouter une personnalisation]**.

   ![](assets/add-perso.png)

1. Une fois que vous êtes satisfait du contenu, enregistrez et fermez votre conception. Cliquez sur **[!UICONTROL Enregistrer]** pour revenir à l&#39;écran de création d&#39;un email.

   ![](assets/save-content.png)

## Définir l’audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Définir l’audience"
>abstract="Sélectionnez l’audience la plus appropriée pour votre message marketing. Vous pouvez choisir une audience existante déjà définie dans une instance de Campaign v8 ou Adobe Experience Platform, ou créer une nouvelle audience à l’aide du créateur de règles."

Dans ce cas pratique, vous envoyez l’email à une audience existante. Des instructions supplémentaires sur l’utilisation des audiences sont disponibles dans [cette section](../audience/about-audiences.md).

1. Pour sélectionner l&#39;audience de l&#39;email, cliquez sur le bouton **[!UICONTROL Sélection de l’audience]** et choisissez une audience existante dans la liste.

   Dans cet exemple, nous allons utiliser une audience existante ciblant des client(e)s appartenant aux niveaux de points de fidélité argent et or.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Les audiences disponibles dans la liste proviennent soit de votre instance Campaign v8, soit de Adobe Experience Platform si l’intégration Destination/Sources a été configurée sur votre instance.
   >
   >L’intégration Destination/Sources vous permet d’envoyer des segments Experience Platform vers Adobe Campaign et d’envoyer des logs de diffusion et de tracking Campaign à Adobe Experience Platform. [Découvrez comment utiliser Campaign et Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html?lang=fr){target="_blank"}.

1. Une fois l&#39;audience sélectionnée, vous pouvez affiner davantage la cible en appliquant des règles supplémentaires.

   Vous pouvez également définir une population témoin afin d&#39;analyser le comportement des destinataires de l&#39;email par rapport à ceux qui n&#39;ont pas été ciblés. [Découvrez comment travailler avec les populations témoins.](../audience/control-group.md)

   ![](assets/audience-selected.png)

## Planifier l’envoi {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Planifier l’envoi"
>abstract="Définissez la date et l’heure exactes de votre envoi. En choisissant l’heure la plus appropriée pour votre message marketing, vous pouvez optimiser les taux d’ouverture."

Pour planifier l’envoi de l’email, cliquez sur **[!UICONTROL Activer]** et définissez la date et l’heure d’envoi.

Par défaut, la variable **[!UICONTROL Confirmer avant envoi]** est activée, ce qui nécessite de confirmer l’envoi avant que l’email ne soit envoyé à la date et à l’heure planifiées. Si vous souhaitez envoyer automatiquement l&#39;email à la date et l&#39;heure planifiées, vous pouvez désactiver cette option.

![](assets/schedule.png)

## Prévisualiser et tester l’e-mail {#preview-test}

Avant d&#39;envoyer votre email, vous pouvez le prévisualiser et le tester afin de vous assurer qu&#39;il répond à vos attentes.

Dans ce cas pratique, vous prévisualisez l’email et envoyez des versions de test à des adresses email spécifiques tout en empruntant l’identité de certains des profils ciblés.

Des informations supplémentaires sur la prévisualisation et le test des e-mails sont disponibles dans [cette section](../preview-test/preview-test.md).

1. Pour examiner et envoyer le courrier électronique, cliquez sur **[!UICONTROL Vérifier et envoyer]**. Vous affichez ainsi un aperçu de votre email, ainsi que toutes les propriétés, l’audience et le planning configurés. Vous pouvez éditer l&#39;un de ces éléments en cliquant sur le bouton de modification .

1. Pour prévisualiser l&#39;email et envoyer les versions de test, cliquez sur le bouton **[!UICONTROL Simulation du contenu]** bouton .

   ![](assets/review-email.png)

1. Sur le côté gauche, sélectionnez le ou les profils que vous souhaitez utiliser pour prévisualiser l&#39;email.

   Le volet de droite affiche un aperçu de l&#39;email en fonction du profil sélectionné. Si vous avez ajouté plusieurs profils, vous pouvez basculer entre eux pour prévisualiser l&#39;email correspondant.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Pour envoyer des versions de test de votre email, cliquez sur le bouton **[!UICONTROL Test]** puis sélectionnez le mode à utiliser.

   Dans cet exemple, utilisez la méthode **[!UICONTROL Substituer à partir de la cible principale]** , qui envoie des versions de test à des adresses email spécifiques tout en empruntant l’identité de certains des profils ciblés par l’email.

   ![](assets/proof-mode.png)

1. Cliquez sur **[!UICONTROL Ajouter une adresse]** et indiquez la ou les adresses email qui reçoivent les versions de test.

   Pour chaque adresse email, sélectionnez le profil à emprunter. Vous pouvez également laisser Adobe Campaign sélectionner un profil aléatoire à partir de la cible.

   ![](assets/proof-test-profile.png)

1. Cliquez sur **[!UICONTROL Envoyer un email de test]** et confirmez l’envoi.

   Les versions de test sont envoyées aux adresses électroniques spécifiées à l’aide du profil sélectionné avec la variable **[Bon à tirer x]** préfixe.

   ![](assets/proof-sent.png)

   Vous pouvez vérifier à tout moment l’état de l’envoi et accéder aux emails de test envoyés en cliquant sur le bouton **[!UICONTROL Afficher le journal des emails de test]** dans l’écran simuler le contenu.

## Envoyer et surveiller l’e-mail {#prepare-send}

Après avoir validé et testé votre email, vous pouvez lancer sa préparation et l&#39;envoyer.

1. Pour lancer la préparation de l’email, cliquez sur **[!UICONTROL Préparer]**. [Découvrez comment préparer un e-mail](../monitor/prepare-send.md).

   ![](assets/preparation.png)

1. Une fois que votre email est prêt à être envoyé, cliquez sur le bouton **[!UICONTROL Envoyer]** (ou **[!UICONTROL Envoyer comme prévu]** si vous avez planifié son envoi) et confirmez l’envoi.

1. Au cours du processus d&#39;envoi, vous pouvez suivre son avancement et visualiser les statistiques en temps réel directement dans cet écran.

   ![](assets/sent-mail.png)

   Vous pouvez également accéder à des informations détaillées sur l&#39;envoi en cliquant sur le lien **[!UICONTROL Journaux]** bouton . [Découvrez comment surveiller les logs de diffusion](../monitor/delivery-logs.md).

1. Une fois l&#39;email envoyé, vous pouvez accéder à des rapports dédiés pour une analyse plus approfondie en cliquant sur le lien **[!UICONTROL Reporting]** bouton .

![](assets/reports.png)
