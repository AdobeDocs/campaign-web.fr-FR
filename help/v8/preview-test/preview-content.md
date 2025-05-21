---
audience: end-user
title: Prévisualiser le contenu de la diffusion
description: Découvrez comment prévisualiser le contenu de votre diffusion avec l’interface utilisateur web de Campaign.
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Prévisualiser le contenu du message {#preview-content}

La fonctionnalité de simulation de contenu de [!DNL Campaign] permet de prévisualiser le contenu du message avant son envoi. Cette fonctionnalité vous permet de contrôler la personnalisation et de vérifier l’affichage du message pour vos destinataires.

Pour prévisualiser le contenu de votre diffusion, procédez comme suit :

1. Accédez à l’écran de modification du contenu de la diffusion ou au [Concepteur d’e-mail](../email/get-started-email-designer.md).

1. Cliquez sur le bouton **[!UICONTROL Simuler le contenu]**.

   ![Image affichant le bouton Simuler du contenu](assets/simulate-button.png){zoomable="yes"}

1. Sélectionnez les profils à utiliser pour prévisualiser votre contenu. Pour effectuer cette action, cliquez sur le bouton **[!UICONTROL Ajouter un ou des profils de test]** (pour les e-mails et les SMS) ou le bouton **[!UICONTROL Ajouter une ou des personnes abonnées]** (pour les notifications push).

1. Combinez les profils et les profils de test pour prévisualiser votre e-mail ou SMS.

   * L’onglet **[!UICONTROL Profils de test]** répertorie les profils de test, qui représentent des personnes destinataires supplémentaires et fictives dans la base de données. [Découvrez comment utiliser des profils test](../audience/test-profiles.md).

   * L’onglet **[!UICONTROL Profils]** répertorie les profils stockés dans votre base de données. [Découvrez comment utiliser des profils](../audience/about-recipients.md).

   ![Image montrant la sélection des profils](assets/simulate-select-profiles.png){zoomable="yes"}

1. Lorsque vous parcourez le profil de test ou la liste des profils, utilisez des filtres pour affiner votre recherche. Par exemple, définissez une règle pour rechercher tous les profils de test dotés du statut **[!UICONTROL Prospect]**. [Découvrez comment ajouter des règles à l’aide du concepteur de requête](../query/query-modeler-overview.md).

   ![Image montrant les filtres appliqués aux profils de test](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Sélectionner]** pour confirmer votre sélection.

   Un aperçu du contenu de la diffusion s’affiche dans le volet de droite de l’écran **[!UICONTROL Simuler]**. Les éléments personnalisés sont remplacés par les données du profil sélectionné dans le volet de gauche.

   ![Image affichant la prévisualisation du contenu de la diffusion](assets/simulate-preview.png){zoomable="yes"}

1. Si plusieurs profils ont été ajoutés, passez d’un profil à l’autre dans la liste pour prévisualiser le contenu de la diffusion correspondante. Aoutez d’autres profils de test et effacez votre sélection à l’aide des boutons correspondants dans le volet de gauche.

1. Pour les diffusions par e-mail, ajustez l’**[!UICONTROL Échelle]** et prévisualisez votre contenu sur un poste de travail ou un appareil mobile à l’aide de l’icône dédiée dans le coin supérieur droit.

1. L’écran **[!UICONTROL Simuler]** vous permet également d’effectuer les actions suivantes :
   * Envoyer des BAT à des destinataires spécifiques pour validation - [En savoir plus](test-deliveries.md)
   * Accéder aux logs des BAT envoyées - [En savoir plus](test-deliveries.md#access-test-deliveries)
   * Pour les e-mails uniquement, vérifiez le rendu du contenu des messages dans les clients de messagerie les plus courants - [En savoir plus](email-rendering.md)