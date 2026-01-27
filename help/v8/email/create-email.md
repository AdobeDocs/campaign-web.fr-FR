---
audience: end-user
title: Envoyer votre premier e-mail
description: Découvrez comment envoyer votre premier e-mail avec l’interface utilisateur web de Campaign.
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '1648'
ht-degree: 98%

---

# Créer votre premier e-mail {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Commencer avec les e-mails"
>abstract="Vous pouvez créer une diffusion par e-mail autonome ou créer un e-mail dans le cadre d’un workflow de campagne. Découvrez comment créer la diffusion, sélectionner l’audience et concevoir le contenu de l’e-mail."

Découvrez comment créer votre premier e-mail ciblé. Dans ce cas d’utilisation, vous planifiez l’envoi d’un e-mail aux membres argent et or du programme de fidélité à une date spécifique.

Basé sur un [modèle de conception](../content/create-email-templates.md) prédéfini, l’e-mail propose également du contenu personnalisé en fonction des attributs de profil du client ou de la cliente.

➡️ [Découvrez cette fonctionnalité en vidéo](#video)

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

   ![Capture d’écran montrant le bouton Créer une diffusion dans le menu Diffusions](../msg/assets/create-a-delivery.png)

1. Sélectionnez le canal **[!UICONTROL E-mail]** et choisissez un modèle de diffusion e-mail dans la liste.

   >[!NOTE]
   >
   >Les modèles sont des paramètres de diffusion préconfigurés enregistrés en vue d’une utilisation ultérieure. [En savoir plus](../msg/delivery-template.md)

   ![Capture d’écran affichant la sélection du canal e-mail et du modèle](assets/channel-template.png){zoomable="yes"}

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

   ![Capture d’écran affichant la configuration des propriétés de l’e-mail](assets/email-properties.png){zoomable="yes"}

1. De plus, des paramètres avancés, tels que les règles de typologie et les mappings de ciblage, sont accessibles via le bouton **[!UICONTROL Paramètres]** situé en haut à droite de l’écran. Ces paramètres sont préconfigurés dans le modèle sélectionné, mais peuvent être modifiés selon les besoins pour cet e-mail spécifique. [En savoir plus](../advanced-settings/delivery-settings.md)

## Définition de l’audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Sélectionner une audience pour votre diffusion"
>abstract="Sélectionnez l’audience la plus appropriée pour votre message marketing. Vous pouvez choisir une audience existante (déjà définie dans une instance de Campaign v8 ou à partir d’Adobe Experience Platform), créer une audience à l’aide du concepteur de requête ou charger un fichier contenant votre audience. Les populations témoins ne sont pas activées pour l’option **Sélectionner à partir du fichier** et vice versa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html?lang=fr" text="Sélectionner les audiences principales"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=fr" text="Définir une population témoin"

Dans ce cas d’utilisation, vous envoyez l’e-mail à une audience existante.

Des instructions supplémentaires sur l’utilisation des audiences sont disponibles dans [cette section](../audience/about-recipients.md).

1. Pour sélectionner l’audience de l’e-mail, cliquez sur le bouton **[!UICONTROL Sélectionner l’audience]** et choisissez une audience existante dans la liste.

   Dans cet exemple, nous allons utiliser une audience existante ciblant les clientes et clients appartenant aux niveaux de points de fidélité argent et or.

   ![Capture d’écran montrant le processus de sélection de l’audience](assets/create-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >Les audiences disponibles dans la liste proviennent de votre instance Campaign v8 ou d’Adobe Experience Platform si l’intégration Destination/Source a été configurée sur votre instance. L’intégration vous permet d’envoyer des segments Experience Platform vers Adobe Campaign et d’envoyer des logs de diffusion et de tracking Campaign à Adobe Experience Platform. Découvrez comment utiliser Campaign et Adobe Experience Platform dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=fr){target="_blank"}.

1. Une fois l’audience sélectionnée, vous pouvez affiner davantage la cible en appliquant des règles supplémentaires.

   ![Capture d’écran montrant le processus d’affinement de l’audience](assets/audience-selected.png){zoomable="yes"}

1. Vous pouvez également définir une population témoin afin d’analyser le comportement des destinataires de l’e-mail par rapport au comportement des profils qui n’ont pas été ciblés. [Découvrez comment travailler avec les populations témoins.](../audience/control-group.md)

## Définition du contenu de l’e-mail {#create-content}

Pour commencer à créer le contenu de votre e-mail, procédez comme suit. Dans ce cas d’utilisation, vous allez utiliser un [modèle de diffusion](../msg/delivery-template.md) prédéfini pour concevoir votre e-mail.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. Dans le tableau de bord de la diffusion e-mail, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

   ![Capture d’écran affichant le bouton Modifier le contenu](assets/email-edit-content.png){zoomable="yes"}

   Une interface dédiée s’affiche, dans laquelle vous pouvez configurer le contenu de l’e-mail et accéder au concepteur d’e-mail. [En savoir plus](edit-content.md)

   ![Capture d’écran montrant l’interface du concepteur d’e-mail](assets/edit-content.png){zoomable="yes"}

1. Indiquez l’objet de l’e-mail et personnalisez-le à l’aide de l’éditeur d’expression. [Découvrir comment personnaliser du contenu](../personalization/personalize.md)

   ![Capture d’écran affichant la configuration de l’objet](assets/subject-line.png){zoomable="yes"}

1. Pour concevoir le contenu de l’e-mail, cliquez sur le bouton **[!UICONTROL Modifier le corps de l’e-mail]**.

   Sélectionnez la méthode à utiliser pour créer le contenu de l’e-mail. Dans cet exemple, utilisez un [modèle de contenu prédéfini](../content/create-email-templates.md).

   ![Capture d’écran montrant la sélection d’un modèle de contenu prédéfini](assets/select-template.png){zoomable="yes"}

1. Une fois le modèle sélectionné, il s’affiche dans le [concepteur d’e-mail](create-email-content.md). Vous pouvez ainsi apporter les modifications nécessaires et le personnaliser à souhait.

   Par exemple, pour personnaliser le titre de l’e-mail, sélectionnez le bloc de composant et cliquez sur **[!UICONTROL Ajouter une personnalisation]**.

   ![Capture d’écran montrant le processus de personnalisation](assets/add-perso.png){zoomable="yes"}

1. Une fois que vous êtes satisfait du contenu, enregistrez et fermez votre conception. Cliquez sur **[!UICONTROL Enregistrer]** pour revenir à l’écran de création d’e-mail.

   ![Capture d’écran affichant le bouton Enregistrer](assets/save-content.png){zoomable="yes"}

## Planifier l’envoi {#schedule}

Lorsqu’une diffusion est envoyée dans le cadre d’un workflow, vous devez utiliser l’activité **Planificateur**. En savoir plus sur [cette page](../workflows/activities/scheduler.md). Les étapes ci-dessous s’appliquent uniquement aux diffusions autonomes.

1. Accédez à la section **[!UICONTROL Planifier]** des propriétés de la diffusion.

1. Utilisez le bouton (bascule) **[!UICONTROL Activer la planification]** pour l’activer.

1. Définissez la date et l’heure d’envoi.

   ![Capture d’écran affichant la configuration de planification](assets/schedule.png){zoomable="yes"}

Une fois la diffusion envoyée, l’envoi effectif démarre à la date de contact que vous avez définie.

Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Prévisualiser un e-mail et envoyer des BAT {#preview-test}

Avant d’envoyer votre e-mail, vous pouvez le prévisualiser et le tester pour vous assurer qu’il répond à vos attentes.

Dans ce cas d’utilisation, vous prévisualisez l’e-mail et envoyez des BAT à des adresses e-mail spécifiques tout en empruntant l’identité de certains des profils ciblés.

Vous pouvez également valider la qualité de votre contenu pour vérifier la lisibilité, l’efficacité de CTA, la qualité de l’objet, etc. [En savoir plus sur la validation de la qualité du contenu](../content/brands-score.md#validate-quality)

Des informations supplémentaires sur la prévisualisation des e-mails et l’envoi de BAT sont disponibles dans [cette section](../preview-test/preview-test.md).

1. Pour vérifier votre e-mail, cliquez sur **[!UICONTROL Vérifier et envoyer]**. Un aperçu de votre e-mail s’affiche, ainsi que toutes les propriétés, l’audience et le planning configurés. Vous pouvez modifier chacun de ces éléments en cliquant sur le bouton Modifier.

1. Pour prévisualiser l’e-mail et envoyer des BAT, cliquez sur le bouton **[!UICONTROL Simuler du contenu]**.

   ![Capture d’écran montrant le bouton Simuler du contenu](assets/review-email.png){zoomable="yes"}

   >[!NOTE]
   >
   >Le bouton **[!UICONTROL Simuler le contenu]** est désactivé dans des contextes spécifiques. Les limitations sont présentées [dans cette section](#content-simulation-limitations).

1. Dans la zone de gauche, sélectionnez le ou les profils que vous souhaitez utiliser pour prévisualiser l’e-mail.

   Le volet de droite affiche un aperçu de l’e-mail en fonction du profil sélectionné. Si vous avez ajouté plusieurs profils, vous pouvez passer d’un profil à l’autre pour prévisualiser l’e-mail correspondant.

   ![Capture d’écran montrant l’aperçu de l’e-mail en fonction des profils sélectionnés](assets/preview.png){zoomable="yes"}

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using multiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Pour envoyer des BAT, cliquez sur le bouton **[!UICONTROL Envoyer des BAT]**, puis sélectionnez le mode à utiliser.

   Dans cet exemple, utilisez le mode **[!UICONTROL Substituer à partir de la cible principale]**, qui envoie des BAT à des adresses e-mail spécifiques tout en empruntant l’identité de certains des profils ciblés par l’e-mail.

   ![Capture d’écran montrant la sélection du mode d’envoi du BAT](assets/proof-mode.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Ajouter une adresse]** et indiquez la ou les adresses e-mail qui reçoivent les BAT.

   Pour chaque adresse e-mail, sélectionnez le profil dont vous souhaitez emprunter l’identité. Vous pouvez également laisser Adobe Campaign sélectionner un profil aléatoire à partir de la cible.

   ![Capture d’écran montrant l’ajout d’adresses e-mail pour les BAT](assets/proof-test-profile.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Envoyer un BAT]**, puis confirmez l’envoi.

   Les BAT sont envoyés aux adresses e-mail spécifiées à l’aide du profil sélectionné avec le préfixe **[BAT x]**.

   ![Capture d’écran montrant la confirmation de l’envoi du BAT](assets/proof-sent.png){zoomable="yes"}

   Vous pouvez vérifier à tout moment le statut de l’envoi et accéder aux BAT envoyés en cliquant sur le bouton **[!UICONTROL Afficher les BAT]** dans l’écran Simuler du contenu.

### Limitations de la simulation de contenu {#content-simulation-limitations}

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_multilingual"
>title="La simulation de contenu n’est pas prise en charge."
>abstract="Le bouton **Simuler le contenu** est désactivé, car la diffusion multilingue ne contient qu’un seul ensemble de paramètres régionaux."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_reconcilied_deliveries"
>title="La simulation de contenu n’est pas prise en charge."
>abstract="Le bouton **Simuler le contenu** est inactif, car il n’est pas compatible avec les diffusions réconciliées de cette phase."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_ffda"
>title="La simulation de contenu n’est pas prise en charge."
>abstract="Le bouton **Simuler le contenu** est désactivé, car il n’est pas pris en charge en mode Campaign Enterprise Full Federated Access (FFDA)."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_no_file"
>title="La simulation de contenu n’est pas prise en charge."
>abstract="Le bouton **Simuler le contenu** est désactivé, car aucun contenu n’a été chargé."

Dans certains cas, vous ne pouvez pas effectuer de simulation de contenu et le bouton **[!UICONTROL Simuler le contenu]** est désactivé.

La simulation de contenu n’est pas prise en charge dans les cas suivants :

<!--* When a multilingual delivery contains only one locale,-->
* Avec des diffusions réconciliées
* Lorsque votre modèle de déploiement Campaign est [Adobe Campaign Enterprise Full Federated Access (FFDA)](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/config/architecture/ffda/enterprise-deployment){target="_blank"}.
* Lorsqu’aucun fichier de données n’a été chargé.

## Envoyer et surveiller l’e-mail {#prepare-send}

Après avoir validé et testé votre e-mail, vous pouvez lancer sa préparation et l’envoyer.

1. Pour lancer la préparation de l’e-mail, cliquez sur **[!UICONTROL Préparer]**. [Découvrez comment préparer un e-mail](../monitor/prepare-send.md).

   ![Capture d’écran montrant le bouton Préparer](assets/preparation.png){zoomable="yes"}

1. Une fois que votre e-mail est prêt à être envoyé, cliquez sur le bouton **[!UICONTROL Envoyer]** (ou **[!UICONTROL Envoyer comme prévu]** si vous avez planifié son envoi) et confirmez l’envoi.

1. Au cours du processus d’envoi, vous pouvez suivre son avancement et visualiser les statistiques en temps réel directement à partir de cet écran.

   ![Capture d’écran montrant la progression de l’envoi des e-mails](assets/sending-email.png){zoomable="yes"}

   <!--
    ![Screenshot showing the email sent confirmation](assets/sent-email.png){zoomable="yes"}-->

   Vous pouvez également accéder à des informations détaillées sur l’envoi en cliquant sur le bouton **[!UICONTROL Logs]**. [Découvrez comment surveiller les logs de diffusion](../monitor/delivery-logs.md).

1. Une fois l’e-mail envoyé, vous pouvez accéder à des rapports dédiés pour une analyse plus approfondie en cliquant sur le bouton **[!UICONTROL Créer des rapports]**.

![Capture d’écran affichant le bouton Rapports](assets/reports.png){zoomable="yes"}

## Vidéo pratique {#video}

Découvrez comment créer entièrement une diffusion par e-mail, définir l’audience, concevoir le contenu, simuler l’aperçu et envoyer un BAT.

>[!VIDEO](https://video.tv.adobe.com/v/3454007/?captions=fre_fr&quality=12)