---
audience: end-user
title: Modifier le contenu de l’e-mail
description: Découvrez comment commencer à créer votre contenu à l’aide du Concepteur d’email dans l’interface utilisateur web de Campaign
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 8%

---

# Prise en main du Concepteur d’e-mail {#get-started-email-designer}

Une fois que vous avez créé un email dans Adobe Campaign, vous devez en définir le contenu.

Le Concepteur d&#39;email vous permet de créer des emails attrayants et personnalisés grâce à une interface intuitive par glisser-déposer. Que vous commenciez à partir d’une page vierge, que vous importiez un contenu existant ou que vous utilisiez des modèles existants, concevez et affinez tout le contenu pour chaque email, qu’il soit promotionnel ou transactionnel.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Utilisation [!DNL Campaign] fonctionnalités de conception d’emails pour créer facilement des emails réactifs. [En savoir plus](create-email-content.md)

* Améliorez l’expérience des clients en créant des profils personnalisés en fonction de leurs attributs de profil. [En savoir plus](../personalization/personalize.md)

* Configurez des champs de contenu conditionnel pour créer une personnalisation dynamique basée sur le profil du destinataire. [En savoir plus](../personalization/conditions.md)

## Bonnes pratiques relatives à la conception d&#39;email {#best-practices}

Lors de l&#39;envoi d&#39;emails, il est important de tenir compte du fait que les destinataires peuvent les transférer, ce qui peut parfois entraîner des problèmes de rendu de l&#39;email. Ceci est particulièrement vrai lors de l’utilisation de classes CSS qui peuvent ne pas être prises en charge par le fournisseur de messagerie utilisé pour le transfert, par exemple, si vous utilisez la classe CSS &quot;is-desktop-hidden&quot; (est-masqué) pour masquer une image sur les périphériques mobiles.

Pour minimiser ces problèmes de rendu, nous vous recommandons de garder votre structure de conception d&#39;email aussi simple que possible. Essayez d’utiliser une conception unique qui fonctionne bien pour les ordinateurs de bureau et les appareils mobiles, et évitez d’utiliser des classes CSS complexes ou d’autres éléments de conception qui ne sont pas entièrement pris en charge par tous les clients de messagerie. En suivant ces bonnes pratiques, vous pouvez vous assurer que vos emails sont correctement rendus, quelle que soit la manière dont ils sont affichés ou transférés par les destinataires.

## Commencer à créer du contenu {#start-authoring}

Depuis le tableau de bord des diffusions email, accédez au [Modifier le contenu](edit-content.md) pour ouvrir la page d&#39;accueil du Concepteur d&#39;email. A partir de là, choisissez la façon dont vous souhaitez concevoir votre email parmi les options suivantes :

* **Concevoir entièrement votre email** via l’interface du concepteur d’email. Découvrez comment concevoir le contenu de votre email dans [cette section](create-email-content.md).

* **Code ou coller un HTML brut** directement dans le concepteur d&#39;email. Découvrez comment coder votre propre contenu dans [cette section](code-content.md).

* **Importer du contenu de HTML existant** à partir d’un fichier ou d’un dossier .zip. Découvrez comment importer un contenu d’email dans [cette section](existing-content.md).

* **Sélectionner un contenu existant** à partir d’une liste de modèles intégrés ou personnalisés. Découvrez comment utiliser des modèles d’email [cette section](email-sample-templates.md).

  ![](assets/email_designer_create_options.png)

