---
audience: end-user
title: Créer votre premier email
description: Documentation web de Campaign v8
source-git-commit: cdddef89cda4fa39cee38e9d0171a6ea395537c7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 2%

---

# Envoyer votre premier email {#first-email}

>[!NOTE]
>
>Cette documentation est en cours de construction et fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

Ce cas pratique montre comment créer votre premier email

Dans cet exemple, nous allons planifier l’envoi d’un email à une date spécifique aux clients fidèles à l’or et à l’argent. Cet email sera conçu à l’aide d’un modèle de HTML prédéfini à partir d’un fichier ZIP et inclura la personnalisation à l’aide des attributs de profil.

![](assets/delivery-list.png)

## Créer l&#39;email {#create-email}

1. Créez une nouvelle diffusion à partir de la fonction **[!UICONTROL Diffusions]** .
1. Sélectionnez la **[!UICONTROL Email]** canal et modèle à utiliser, puis cliquez sur **[!UICONTROL Créer]**.

   >[!NOTE]
   >
   >informations sur les modèles. Vérification des informations dans V7 doc

   ![](assets/channel-template.png)

1. Indiquez un libellé pour la diffusion et paramétrez des options supplémentaires en fonction de vos besoins :

   * Nom interne:
   * Dossier:
   * Code diffusion:
   * Description:
   * Nature:

   vérifier quels paramètres sont définis dans le modèle et les mentionner (description ? dossier ?, nature ?)

   ![](assets/email-properties.png)

   >[!NOTE]
   >
   >info sur le bouton des paramètres de diffusion + lien vers le document

## Créer le contenu de l&#39;email {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Créez votre premier contenu d&#39;email à l&#39;aide du Concepteur d&#39;email."
>abstract="Créer votre premier contenu d&#39;email"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Créer le contenu de l&#39;email"
>abstract="TBC"

1. Cliquez sur le bouton **[!UICONTROL Modifier le contenu]** pour commencer à créer le contenu de votre email.

   Cet écran vous permet de paramétrer le contenu de l&#39;email et de le concevoir à l&#39;aide du Concepteur d&#39;email.

   ![](assets/edit-content.png)

   >[!NOTE]
   >
   >Les informations De et De l&#39;email sont prédéfinies dans le modèle d&#39;email sélectionné.
   >
   >Par défaut, le tracking des emails est activé pour les ouvertures et les clics. Pour désactiver ces options, désélectionnez-les dans la section Fonctionnalités facultatives .

1. Indiquez l&#39;objet de votre email à l&#39;aide de l&#39;éditeur d&#39;expression. [Découvrez comment personnaliser votre contenu](../personalization/personalize.md)

   Dans cet exemple, nous souhaitons personnaliser l’objet à l’aide du prénom des profils.

   ![](assets/subject-line.png)

1. Ajoutez un fichier joint à votre email si nécessaire. Découvrez comment modifier le contenu d&#39;un email

1. Cliquez sur le bouton **[!UICONTROL Modifier le corps de l’email]** pour créer et concevoir le contenu de votre email.

   Choisissez la méthode à utiliser pour créer le contenu de votre email. Dans cet exemple, nous voulons importer un contenu de HTML existant.

   ![](assets/import-html.png)

1. Sélectionnez le fichier de HTML ou ZIP à importer, puis cliquez sur **[!UICONTROL Suivant]**.

   Si votre dossier contient des ressources, choisissez l’instance et le dossier dans lesquels elles doivent être stockées, puis cliquez sur **[!UICONTROL Importer]**. (+ lien vers un document sur les ressources ?)

   ![](assets/import-folder.png)

1. Une fois votre contenu importé, il s&#39;affiche dans le Concepteur d&#39;email, ce qui vous permet de l&#39;éditer si nécessaire et d&#39;ajouter une personnalisation.

   Dans cet exemple, nous allons ajouter une personnalisation dans le titre de l&#39;email. Pour ce faire, sélectionnez le bloc de composant, puis cliquez sur **[!UICONTROL Ajouter une personnalisation]**.

   ![](assets/add-perso.png)

1. Une fois votre contenu prêt, enregistrez-le, puis cliquez sur la flèche pour revenir à l&#39;écran de création d&#39;email.

   ![](assets/save-content.png)

## Définition de l’audience {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Définition de l’audience"
>abstract="TBC"

1. Cliquez sur le bouton **[!UICONTROL Sélection de l’audience]** puis choisissez une audience existante ou créez-en une.

   Dans cet exemple, nous allons utiliser une audience existante ciblant des clients appartenant aux niveaux de points de fidélité argent et or.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Les audiences disponibles dans la liste proviennent soit de votre instance Campaign V8, soit de Adobe Experience Platform si l’intégration Destination/Sources a été implémentée sur votre instance. Découvrez comment sélectionner l’audience de courrier électronique

1. Une fois votre audience sélectionnée, vous pouvez modifier les règles si nécessaire. Vous pouvez également définir une population témoin afin d&#39;analyser le comportement des destinataires de l&#39;email par rapport au comportement des profils qui n&#39;ont pas été ciblés. Découvrez comment travailler avec les populations témoins

## Planifiez l&#39;envoi {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Planifiez l&#39;envoi"
>abstract="TBC"

Pour planifier l’envoi de l’email, cliquez sur Activer , puis indiquez la date et l’heure de votre choix.

= confirmer avant l’option d’envoi : ce qui se passe à la date planifiée : une notification pour confirmer l&#39;envoi du message ?

![](assets/schedule.png)

## Prévisualiser et tester l&#39;email {#preview-test}

Une fois votre email prêt, vous pouvez le prévisualiser et le tester avant de lancer son envoi.

1. Cliquez sur **[!UICONTROL Vérifier pour envoyer]**. Un aperçu de votre email s’affiche, ainsi que toutes les propriétés, l’audience et le planning configurés. Vous pouvez éditer l&#39;un de ces éléments à partir du bouton de modification .

   ![](assets/review-email.png)

1. Cliquez sur le bouton **[!UICONTROL Simulation du contenu]** pour prévisualiser l&#39;email et envoyer les bons à tirer.

1. Dans la zone de gauche, sélectionnez les profils à utiliser pour prévisualiser l&#39;email. Vous pouvez utiliser des profils ciblés ou des profils de test dédiés.

1. Un aperçu de l&#39;email s&#39;affiche dans la zone de droite en fonction du profil sélectionné. Si vous avez ajouté plusieurs profils, vous pouvez passer d’un profil à l’autre pour prévisualiser l’email correspondant.

   ![](assets/preview.png)

   >[!NOTE]
   >
   >En outre, la variable **[!UICONTROL Render Email]** vous permet de prévisualiser l’email à l’aide de plusieurs appareils ou fournisseurs de messagerie. Découvrez comment prévisualiser le rendu des emails

1. Pour envoyer des bons à tirer de votre email, cliquez sur le bouton **[!UICONTROL Test]** puis sélectionnez les profils qui recevront le BAT. Dans cet exemple, nous souhaitons envoyer les bons à tirer vers un profil de test spécifique.

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >Vous pouvez également tester vos messages en empruntant l’identité de certains des profils ciblés et en envoyant le message du BAT à l’adresse email de votre choix. Découvrez comment utiliser Substituer depuis le mode cible

1. Cliquez sur **[!UICONTROL Envoyer un email de test]** confirmez ensuite l’envoi.

   Une fois les BAT envoyés, vous pouvez vérifier leur statut en cliquant sur le bouton **[!UICONTROL Afficher le journal des emails de test]** bouton .

## Envoi et surveillance de l’email {#prepare-send}

Une fois que vous avez validé et testé votre email, vous pouvez lancer sa préparation et l&#39;envoyer.

1. Cliquez sur **[!UICONTROL Préparer]** pour lancer la préparation du message.

   Vous pouvez suivre la progression de la préparation en temps réel, ainsi que les statistiques. Une fois la préparation terminée, vous pouvez accéder aux logs détaillés pour une analyse plus approfondie. Découvrez comment surveiller les diffusions

   ![](assets/preparation.png)

1. Une fois que votre email est prêt à être envoyé, cliquez sur **[!UICONTROL Envoyer]** confirmez ensuite l’envoi.

   Vous pouvez suivre l’envoi en temps réel, ainsi que les statistiques. En outre, la variable **[!UICONTROL Journaux]** permet d&#39;accéder à des informations détaillées sur l&#39;envoi de l&#39;email. Découvrez comment surveiller les diffusions

   ![](assets/logs.png)

1. Une fois l&#39;email envoyé, vous pouvez accéder à des rapports dédiés à des fins d&#39;analyse ultérieure.

   ![](assets/reports.png)
