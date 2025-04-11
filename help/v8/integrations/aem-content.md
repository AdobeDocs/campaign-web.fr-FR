---
audience: end-user
title: Gérer les ressources avec Adobe Experience Manager as a Cloud service
description: Découvrez comment gérer les ressources avec Adobe Experience Manager as a Cloud service.
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 40%

---

# Gérer les modèles avec [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Commencer avec [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

L’intégration de l’interface Web d’Adobe Campaign à Adobe Experience Manager permet une gestion rationalisée du contenu et des formulaires de diffusion des e-mails directement dans la plateforme Adobe Experience Manager.

![](assets/do-not-localize/book.png)[En savoir plus sur Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=fr)

## Créer un modèle dans [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Accédez à votre instance d’auteur [!DNL Adobe Experience Manager], puis cliquez sur Adobe Experience Manager dans le coin supérieur gauche de la page. Choisissez **[!UICONTROL Sites]** dans le menu.

1. Accédez à **[!UICONTROL Campagnes > Nom de votre marque > Zone principale > Nom de votre page]**.

1. Cliquez sur **[!UICONTROL Créer]**, puis sélectionnez **[!UICONTROL Page]** dans le menu déroulant.

   ![Capture d’écran affichant le bouton « Créer » et l’option « Page » dans le menu déroulant.](assets/aem_1.png)

1. Sélectionnez le modèle **[!UICONTROL Adobe Campaign Email]** et attribuez un nom à votre newsletter.

   ![[Capture d’écran affichant le champ de sélection et de dénomination du modèle « Adobe Campaign Email ».]](assets/aem_2.png)

1. Personnalisez le contenu de votre e-mail en ajoutant des composants, tels que des champs de personnalisation d’Adobe Campaign. [En savoir plus](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=fr#editing-email-content)

1. Une fois votre e-mail prêt, accédez au menu **[!UICONTROL Informations sur la page]**, puis cliquez sur **[!UICONTROL Démarrer le workflow]**.

   ![Capture d’écran affichant le menu « Informations sur la page » et l’option « Démarrer le workflow ».](assets/aem_3.png)

1. Dans la première liste déroulante, sélectionnez **[!UICONTROL Approuver Adobe Campaign]** comme modèle de workflow, puis cliquez sur **[!UICONTROL Démarrer le workflow]**.

1. Une clause de non-responsabilité s’affiche en haut de la page et indique : `This page is subject to the workflow Approve for Adobe Campaign`. Cliquez sur **[!UICONTROL Terminé]** en regard de la clause de non-responsabilité pour confirmer la révision, puis cliquez sur **[!UICONTROL Ok]**.

   ![Capture d’écran affichant la clause de non-responsabilité et le bouton « Terminé ».](assets/aem_4.png)

1. Cliquez de nouveau sur **[!UICONTROL Terminer]** et sélectionnez **[!UICONTROL Approbation de la newsletter]** dans le menu déroulant **[!UICONTROL Étape suivante]**.

Votre newsletter est maintenant prête et synchronisée dans Adobe Campaign.

## Importation d’un modèle Adobe Experience Manager as a Cloud Service{#aem-templates-perso}

Une fois que le modèle Experience Manager est disponible dans Adobe Campaign Web en tant que modèle de contenu, vous pouvez identifier et incorporer le contenu nécessaire à l’e-mail, y compris la personnalisation.

1. Dans Campaign Web, à partir du menu **[!UICONTROL Diffusions]**, cliquez sur **[!UICONTROL Créer une diffusion]**.

1. Dans la fenêtre du modèle d’e-mail, sélectionnez le modèle **[!UICONTROL Diffusion de contenu AEM par e-mail]**.

   ![Capture d’écran affichant la sélection du modèle « Diffusion e-mail avec contenu AEM ».](assets/aem_5.png)

1. Saisissez un **[!UICONTROL Libellé]** pour la diffusion et configurez les options supplémentaires en fonction de vos besoins :

   * **[!UICONTROL Nom interne]** : attribuez un identifiant unique à la diffusion.
   * **[!UICONTROL Dossier]** : stockez la diffusion dans un dossier spécifique.
   * **[!UICONTROL Code de diffusion]** : utilisez ce champ pour organiser vos diffusions selon votre propre convention de nommage.
   * **[!UICONTROL Description]** : spécifiez une description pour la diffusion.
   * **[!UICONTROL Nature]** : indiquez la nature de l’e-mail à des fins de classification.

1. Définissez une **[!UICONTROL audience]** pour votre e-mail. [En savoir plus](../email/create-email.md#define-audience)

1. Cliquez sur **[!UICONTROL Modifier le contenu]**.

1. Dans le menu **[!UICONTROL Modifier le contenu]**, cliquez sur **[!UICONTROL Sélectionner du contenu AEM]**.

   ![Capture d’écran affichant l’option « Sélectionner le contenu AEM » dans le menu « Modifier le contenu ».](assets/aem_6.png)

1. Parcourez votre modèle AEM et sélectionnez celui à importer dans Campaign Web.

   ![Capture d’écran montrant l’interface de sélection des modèles d’AEM.](assets/aem_8.png)

1. Notez que le contenu n’est pas automatiquement synchronisé. Si des modifications sont apportées à vos modèles directement dans Adobe Experience Manager, sélectionnez **[!UICONTROL Actualiser le contenu AEM]** pour mettre à jour vers la dernière version de votre modèle.

1. Pour supprimer la liaison entre Experience Manager et Campaign ou pour personnaliser davantage votre modèle Experience Manager dans le Concepteur d&#39;email, cliquez sur **[!UICONTROL Annuler le lien du contenu AEM]**.

   ![Capture d’écran affichant l’option « Annuler le lien du contenu AEM ».](assets/aem_9.png)

1. Si vous avez ajouté du contenu personnalisé à votre modèle Experience Manager, cliquez sur **[!UICONTROL Simuler du contenu]** pour prévisualiser l’affichage du message à l’aide de profils de test.

[En savoir plus sur la prévisualisation et les profils de test](../preview-test/preview-content.md)

1. Lors de l’affichage de l’aperçu du message, tout élément personnalisé est automatiquement remplacé par les données correspondantes du profil de test sélectionné.

   Si nécessaire, ajoutez des profils de test supplémentaires via le bouton **[!UICONTROL Gérer les profils de test]**.

Votre diffusion est maintenant prête à être envoyée.