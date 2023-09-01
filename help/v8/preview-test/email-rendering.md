---
audience: end-user
title: Tester le rendu des e-mails
description: Découvrez comment tester le rendu de vos e-mails dans l’interface utilisateur web de Campaign.
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 100%

---


# Tester le rendu des e-mails {#email-rendering}

Avant d’envoyer votre e-mail, vérifiez que l’affichage de votre message est optimal pour les destinataires sur divers clients web et appareils.

Pour ce faire, tirez parti de votre compte **Litmus** dans [!DNL Adobe Campaign] pour prévisualiser instantanément le rendu de vos e-mails dans différents contextes et vérifier la compatibilité sur les principaux postes de travail et applications (messagerie web, service de messagerie, mobile, etc.).

>[!CAUTION]
>
>Lors de l’utilisation du rendu des e-mails dans Campaign, un e-mail de test est envoyé à un système tiers. En connectant votre compte Litmus à [!DNL Campaign], vous reconnaissez qu’Adobe n’est responsable d’aucune donnée que vous pouvez envoyer à ce tiers. La politique de conservation des données de Litmus s’applique à ces e-mails, y compris les données de personnalisation qui peuvent être incluses dans ces messages de test. Pour accéder à ces données ou les supprimer, contactez directement Litmus.

Pour accéder aux fonctionnalités de rendu des e-mails, vous devez remplir les conditions suivantes :

* disposer d’un compte Litmus
* sélectionner des profils de test. Découvrez comment procéder dans [cette section](preview-content.md).

Suivez ensuite les étapes ci-dessous.

1. Dans l’écran [Modifier le contenu](../content/edit-content.md) ou dans le [Concepteur d’e-mail](../content/get-started-email-designer.md), cliquez sur le bouton **[!UICONTROL Simuler le contenu]**.

1. Cliquez sur le bouton **[!UICONTROL Rendu d’e-mail]**.

   ![](assets/simulate-rendering-button.png)

1. Cliquez sur **Connecter votre compte Litmus** dans la section supérieure droite.

   ![](assets/simulate-rendering-litmus.png)

1. Saisissez vos informations d’identification et connectez-vous.

   ![](assets/simulate-rendering-credentials.png)

1. Cliquez sur le bouton **Exécuter le test** pour générer les aperçus d’e-mail.

1. Examinez le contenu des e-mails tel qu’il s’affiche sur les principaux clients de bureau, mobiles et web.

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
