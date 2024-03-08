---
audience: end-user
title: Envoyer votre premier e-mail
description: Découvrez comment envoyer votre premier e-mail avec l’interface utilisateur web de Campaign.
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: efb5d5d9ea3b3559c57d6a0b2a250f075dabf831
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 88%

---


# Créer votre premier e-mail {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Commencer avec les e-mails"
>abstract="Vous pouvez créer une diffusion par e-mail autonome ou créer un e-mail dans le cadre d’un workflow de campagne. Découvrez comment créer la diffusion, sélectionner l’audience et concevoir le contenu de l’e-mail."

Découvrez comment créer votre premier e-mail ciblé. Dans ce cas d’utilisation, vous planifiez l’envoi d’un e-mail aux membres argent et or du programme de fidélité à une date spécifique.

Basé sur un [modèle de conception](../email/create-email-templates.md) prédéfini, l’e-mail propose également du contenu personnalisé en fonction des attributs de profil du client ou de la cliente.

## Créer la diffusion e-mail {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Sélectionner le modèle d’e-mail"
>abstract="Un modèle d’e-mail est une configuration de diffusion spécifique qui contient des paramètres prédéfinis, tels que des règles de typologie, des paramètres de personnalisation ou de routage. Les modèles sont définis dans la console cliente Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Définir les propriétés de vos e-mails"
>abstract="Les propriétés sont les paramètres de diffusion courants qui vous permettent de nommer et de classer votre diffusion. Les paramètres supplémentaires sont facultatifs. Si votre diffusion est basée sur un schéma étendu défini dans la console Adobe Campaign v8, des champs spécifiques d’**Options personnalisées** sont disponibles."

Vous pouvez créer une diffusion par e-mail autonome ou créer un e-mail dans le cadre d’un workflow de campagne. Les étapes ci-dessous détaillent la procédure d’une diffusion d’e-mail autonome (ponctuelle). En savoir plus sur les étapes de création de diffusions dans Adobe Campaign sur [cette page](../msg/gs-deliveries.md).

Pour créer une diffusion d’e-mail autonome, procédez comme suit :

1. Accédez au menu **[!UICONTROL Diffusions]** dans le rail de gauche, puis cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

   ![](../msg/assets/create-a-delivery.png)

1. Sélectionnez le canal **[!UICONTROL E-mail]** et choisissez un modèle de diffusion e-mail dans la liste.

   >[!NOTE]
   >
   >Les modèles sont des paramètres de diffusion préconfigurés enregistrés en vue d’une utilisation ultérieure. [En savoir plus](../msg/delivery-template.md)

   ![](assets/channel-template.png){zoomable=&quot;yes&quot;}

1. Cliquez sur le bouton **[!UICONTROL Créer une diffusion]** pour confirmer.
1. Indiquez un libellé pour la diffusion et configurez les options supplémentaires en fonction de vos besoins :

   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : utilisez ce champ pour organiser vos diffusions selon votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Si vous avez étendu votre schéma avec des champs personnalisés spécifiques, vous pouvez y accéder dans la section **[!UICONTROL Options personnalisées]**.

   ![](assets/email-properties.png){zoomable=&quot;yes&quot;}

1. De plus, des paramètres avancés, tels que les règles de typologie et les mappings de ciblage, sont accessibles via le bouton **[!UICONTROL Paramètres]** situé en haut à droite de l’écran. Ces paramètres sont préconfigurés dans le modèle sélectionné, mais peuvent être modifiés selon les besoins pour cet e-mail spécifique. [En savoir plus](../advanced-settings/delivery-settings.md)

## Définir l’audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Sélectionner une audience pour votre diffusion"
>abstract="Sélectionnez l’audience la plus appropriée pour votre message marketing. Vous pouvez choisir une audience existante (déjà définie dans une instance de Campaign v8 ou à partir d’Adobe Experience Platform), créer une audience à l’aide du concepteur de requête ou charger un fichier contenant votre audience. Les populations témoins ne sont pas activées pour l’option **Sélectionner à partir du fichier** et vice versa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html?lang=fr" text="Sélectionner les audiences principales"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=fr" text="Définir une population témoin"

Dans ce cas d’utilisation, vous envoyez l’e-mail à une audience existante.

Des instructions supplémentaires sur l’utilisation des audiences sont disponibles dans [cette section](../audience/about-recipients.md).

1. Pour sélectionner l’audience de l’e-mail, cliquez sur le bouton **[!UICONTROL Sélectionner l’audience]** et choisissez une audience existante dans la liste.

   Dans cet exemple, nous allons utiliser une audience existante ciblant des client(e)s appartenant aux niveaux de points de fidélité argent et or.

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Les audiences disponibles dans la liste proviennent de votre instance Campaign v8 ou d’Adobe Experience Platform si l’intégration Destination/Source a été configurée sur votre instance. L’intégration vous permet d’envoyer des segments Experience Platform vers Adobe Campaign et d’envoyer des logs de diffusion et de tracking Campaign à Adobe Experience Platform. Découvrez comment utiliser Campaign et Adobe Experience Platform dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=fr){target="_blank"}.

1. Une fois l’audience sélectionnée, vous pouvez affiner davantage la cible en appliquant des règles supplémentaires.

   ![](assets/audience-selected.png){zoomable=&quot;yes&quot;}

1. Vous pouvez également définir une population témoin afin d’analyser le comportement des destinataires de l’e-mail par rapport au comportement des profils qui n’ont pas été ciblés. [Découvrez comment travailler avec les populations témoins.](../audience/control-group.md)

## Définir le contenu de l’e-mail {#create-content}

Pour commencer à créer le contenu de votre e-mail, procédez comme suit. Dans ce cas d’utilisation, vous allez utiliser un [modèle de diffusion](../msg/delivery-template.md) prédéfini pour concevoir votre e-mail.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. Dans le tableau de bord de la diffusion e-mail, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

   ![](assets/email-edit-content.png){zoomable=&quot;yes&quot;}

   Une interface dédiée s’affiche, dans laquelle vous pouvez configurer le contenu de l’e-mail et accéder au concepteur d’e-mail. [En savoir plus](edit-content.md)

   ![](assets/edit-content.png){zoomable=&quot;yes&quot;}

1. Indiquez l’objet de l’e-mail et personnalisez-le à l’aide de l’éditeur d’expression. [Découvrez comment personnaliser du contenu](../personalization/personalize.md).

   ![](assets/subject-line.png){zoomable=&quot;yes&quot;}

1. Pour concevoir le contenu de l’e-mail, cliquez sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]**.

   Sélectionnez la méthode à utiliser pour créer le contenu de l’e-mail. Dans cet exemple, utilisez un [modèle de contenu prédéfini](create-email-templates.md).

   ![](assets/select-template.png){zoomable=&quot;yes&quot;}

1. Une fois le modèle sélectionné, il s’affiche dans le [concepteur d’e-mail](create-email-content.md). Vous pouvez ainsi apporter les modifications nécessaires et le personnaliser à souhait.

   Par exemple, pour personnaliser le titre de l’e-mail, sélectionnez le bloc de composant et cliquez sur **[!UICONTROL Ajouter une personnalisation]**.

   ![](assets/add-perso.png){zoomable=&quot;yes&quot;}

1. Une fois que vous êtes satisfait du contenu, enregistrez et fermez votre conception. Cliquez sur **[!UICONTROL Enregistrer]** pour revenir à l’écran de création d’e-mail.

   ![](assets/save-content.png){zoomable=&quot;yes&quot;}

## Planifier l’envoi {#schedule}

Lorsqu’une diffusion est envoyée dans le cadre d’un workflow, vous devez utiliser l’activité **Planificateur**. En savoir plus sur [cette page](../workflows/activities/scheduler.md). Les étapes ci-dessous s’appliquent uniquement aux diffusions autonomes.

1. Accédez à la section **[!UICONTROL Planifier]** des propriétés de la diffusion.

1. Utilisez le bouton (bascule) **[!UICONTROL Activer la planification]** pour l’activer.

1. Définissez la date et l’heure d’envoi.

   ![](assets/schedule.png){zoomable=&quot;yes&quot;}

Une fois la diffusion envoyée, l’envoi effectif démarre à la date de contact que vous avez définie.

Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Prévisualiser un email et envoyer des BAT {#preview-test}

Avant d’envoyer votre e-mail, vous pouvez le prévisualiser et le tester pour vous assurer qu’il répond à vos attentes.

Dans ce cas pratique, vous prévisualisez l&#39;email et envoyez des BAT à des adresses email spécifiques tout en empruntant l&#39;identité de certains des profils ciblés.

Des informations supplémentaires sur la prévisualisation d&#39;un email et l&#39;envoi de BAT sont disponibles dans la section [cette section](../preview-test/preview-test.md).

1. Pour vérifier votre e-mail, cliquez sur **[!UICONTROL Vérifier et envoyer]**. Un aperçu de votre e-mail s’affiche, ainsi que toutes les propriétés, l’audience et le planning configurés. Vous pouvez modifier chacun de ces éléments en cliquant sur le bouton Modifier.

1. Pour prévisualiser l&#39;email et envoyer les BAT, cliquez sur le bouton **[!UICONTROL Simulation du contenu]** bouton .

   ![](assets/review-email.png){zoomable=&quot;yes&quot;}

1. Dans la zone de gauche, sélectionnez le ou les profils que vous souhaitez utiliser pour prévisualiser l’e-mail.

   Le volet de droite affiche un aperçu de l’e-mail en fonction du profil sélectionné. Si vous avez ajouté plusieurs profils, vous pouvez passer d’un profil à l’autre pour prévisualiser l’e-mail correspondant.

   ![](assets/preview.png){zoomable=&quot;yes&quot;}

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Pour envoyer des bons à tirer, cliquez sur le bouton **[!UICONTROL Envoyer un bon à tirer]** puis sélectionnez le mode à utiliser.

   Dans cet exemple, utilisez la méthode **[!UICONTROL Substituer à partir de la cible principale]** le mode , qui envoie des BAT à des adresses email spécifiques tout en empruntant l&#39;identité de certains des profils ciblés par l&#39;email.

   ![](assets/proof-mode.png){zoomable=&quot;yes&quot;}

1. Cliquez sur **[!UICONTROL Ajouter une adresse]** et indiquez la ou les adresses email qui reçoivent les bons à tirer.

   Pour chaque adresse e-mail, sélectionnez le profil dont vous souhaitez emprunter l’identité. Vous pouvez également laisser Adobe Campaign sélectionner un profil aléatoire à partir de la cible.

   ![](assets/proof-test-profile.png){zoomable=&quot;yes&quot;}

1. Cliquez sur **[!UICONTROL Envoyer un bon à tirer]** et confirmez l’envoi.

   Les bons à tirer sont envoyés aux adresses email spécifiées à l’aide du profil sélectionné avec la variable **[Bon à tirer x]** préfixe.

   ![](assets/proof-sent.png){zoomable=&quot;yes&quot;}

   Vous pouvez vérifier à tout moment l&#39;état de l&#39;envoi et accéder aux BAT envoyés en cliquant sur le bouton **[!UICONTROL Affichage des bons à tirer]** dans l’écran simuler le contenu.

## Envoyer et surveiller l’e-mail {#prepare-send}

Après avoir validé et testé votre e-mail, vous pouvez lancer sa préparation et l’envoyer.

1. Pour lancer la préparation de l’e-mail, cliquez sur **[!UICONTROL Préparer]**. [Découvrez comment préparer un e-mail](../monitor/prepare-send.md).

   ![](assets/preparation.png){zoomable=&quot;yes&quot;}

1. Une fois que votre e-mail est prêt à être envoyé, cliquez sur le bouton **[!UICONTROL Envoyer]** (ou **[!UICONTROL Envoyer comme prévu]** si vous avez planifié son envoi) et confirmez l’envoi.

1. Au cours du processus d’envoi, vous pouvez suivre son avancement et visualiser les statistiques en temps réel directement à partir de cet écran.

   ![](assets/sending-email.png){zoomable=&quot;yes&quot;}

   <!--
    ![](assets/sent-email.png){zoomable="yes"}-->

   Vous pouvez également accéder à des informations détaillées sur l’envoi en cliquant sur le bouton **[!UICONTROL Logs]**. [Découvrez comment surveiller les logs de diffusion](../monitor/delivery-logs.md).

1. Une fois l’e-mail envoyé, vous pouvez accéder à des rapports dédiés pour une analyse plus approfondie en cliquant sur le bouton **[!UICONTROL Créer des rapports]**.

![](assets/reports.png){zoomable=&quot;yes&quot;}
