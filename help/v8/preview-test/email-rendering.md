---
audience: end-user
title: Tester le rendu des e-mails
description: Découvrez comment tester le rendu de vos e-mails dans l’interface utilisateur web de Campaign.
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 7%

---


# Tester le rendu des e-mails {#email-rendering}

Avant d&#39;envoyer votre email, vérifiez que l&#39;affichage de votre message est optimal pour les destinataires sur divers clients web et appareils.

Pour ce faire, vous pouvez utiliser vos **Litmus** compte dans [!DNL Adobe Campaign] pour prévisualiser instantanément le rendu de vos emails dans différents contextes et vérifier la compatibilité sur les principaux postes de travail et applications (webmail, service de messagerie, mobile, etc.).

>[!CAUTION]
>
>L’utilisation du rendu des emails dans Campaign envoie un email de test à un système tiers. En connectant votre compte Litmus à [!DNL Campaign], vous reconnaissez que l’Adobe n’est responsable d’aucune donnée que vous pouvez envoyer à ce tiers. La politique de conservation des données de Litmus s’applique à ces emails, y compris les données de personnalisation qui peuvent être incluses dans ces messages de test. Pour accéder à ces données ou les supprimer, vous devez contacter Litmus directement.

Pour accéder aux fonctionnalités de rendu des emails, vous devez :

* Posséder un compte Litmus
* Sélection de profils de test - Découvrez comment [cette section](preview-content.md)

Suivez ensuite les étapes ci-dessous.

1. Dans le [Modifier le contenu](../content/edit-content.md) ou dans le [Concepteur d&#39;email](../content/get-started-email-designer.md), cliquez sur le bouton **[!UICONTROL Simulation du contenu]** bouton .

1. Sélectionnez la **[!UICONTROL Render Email]** bouton .

   ![](assets/simulate-rendering-button.png)

1. Cliquez sur **Connexion à votre compte Litmus** dans la section supérieure droite.

   ![](assets/simulate-rendering-litmus.png)

1. Saisissez vos informations d’identification et connectez-vous.

   ![](assets/simulate-rendering-credentials.png)

1. Cliquez sur le bouton **Exécuter le test** pour générer des aperçus d’email.

1. Vérifiez le contenu de vos emails dans les clients populaires de bureau, de mobile et web.

   ![](assets/simulate-rendering-previews.png)

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png)

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
