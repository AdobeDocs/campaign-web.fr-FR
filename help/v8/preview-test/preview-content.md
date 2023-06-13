---
audience: end-user
title: Prévisualiser le contenu d’un e-mail
description: Découvrez comment prévisualiser le contenu de vos e-mails avec l’interface utilisateur web de Campaign.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 27%

---


# Prévisualiser le contenu d’un e-mail {#preview-content}

Utilisez la variable [!DNL Campaign] simulation de contenu permettant de prévisualiser le contenu de votre email avant son envoi. Vous pouvez ainsi contrôler la personnalisation et vérifier comment elle s&#39;affiche pour vos destinataires.

Pour prévisualiser le contenu de votre email, procédez comme suit.

1. Accédez à l’email [Modifier le contenu](../content/edit-content.md) ou au [Concepteur d&#39;email](../content/get-started-email-designer.md).

1. Cliquez sur le bouton **[!UICONTROL Simulation du contenu]** bouton .

   ![](assets/simulate-button.png)

1. Utilisez la variable **[!UICONTROL Ajouter un ou plusieurs profils de test]** pour sélectionner les profils qui seront utilisés pour prévisualiser votre contenu personnalisé.

1. Vous pouvez combiner les profils de test et les profils pour prévisualiser l’e-mail.

   * L’onglet **[!UICONTROL Profils de test]** répertorie les adresses de contrôle, qui sont des destinataires supplémentaires et fictifs dans la base de données.

     >[!NOTE]
     >
     >Les profils de test peuvent être créés dans la variable [!DNL Campaign] dans la console **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Adresses de contrôle]** dossier. En savoir plus dans [Documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * L’onglet **[!UICONTROL Profils]** répertorie tous les destinataires enregistrés dans le dossier **[!UICONTROL Profils et cibles]** à partir de la console [!DNL Campaign] [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

   ![](assets/simulate-select-profiles.png)

1. Cliquez sur **[!UICONTROL Sélectionner]** pour confirmer votre sélection dans les deux onglets.

   Un aperçu de l&#39;email s&#39;affiche dans le volet droit de la **[!UICONTROL Simuler]** écran. Les éléments personnalisés sont remplacés par les données du profil sélectionné dans le volet de gauche.

   ![](assets/simulate-preview.png)

1. Si vous avez ajouté plusieurs profils, vous pouvez passer d’un profil à l’autre dans la liste pour prévisualiser le contenu de l’e-mail correspondant. Vous pouvez également ajouter d’autres profils de test et effacer votre sélection à l’aide des boutons correspondants dans le volet de gauche.

1. Vous pouvez ajuster la variable **[!UICONTROL Niveau de zoom]** et prévisualisez votre contenu sur un ordinateur ou un appareil mobile à l’aide de l’icône dédiée dans le coin supérieur droit.

1. Dans la **[!UICONTROL Simuler]** vous pouvez également :
   * Vérifiez le rendu des emails dans les clients de messagerie les plus courants - [En savoir plus](email-rendering.md)
   * Envoyer des emails de test à des destinataires spécifiques pour validation - [En savoir plus](proofs.md)



