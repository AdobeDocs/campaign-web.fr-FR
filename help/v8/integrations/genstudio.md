---
title: Utiliser GenStudio for Performance Marketing dans Adobe Campaign
description: Découvrez comment utiliser GenStudio for Performance Marketing dans Adobe Campaign.
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 61e6dcf13fc6a405f5e25328bf336e863701b2fe
workflow-type: ht
source-wordcount: '504'
ht-degree: 100%

---

# Utiliser GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="Utiliser un modèle créé avec GenStudio"
>abstract="Grâce à l’intégration transparente à Adobe GenStudio for Performance Marketing, vous pouvez facilement importer un modèle GenStudio amélioré par la technologie d’IA Adobe."

## Commencer à utiliser GenStudio {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} est une application basée sur l’IA générative qui permet aux équipes marketing de créer leurs propres annonces et e-mails afin de générer des campagnes marketing personnalisées et percutantes, conformes aux normes de votre marque et à vos politiques d’entreprise. En tirant parti de la technologie d’IA d’Adobe, elle fournit une suite complète d’outils qui simplifient les complexités de la création et de la gestion du contenu afin que les personnes créatives puissent se concentrer sur l’innovation.

>[!AVAILABILITY]
>
>Cette fonctionnalité est disponible uniquement pour le canal E-mail.

Pour améliorer l’efficacité du marketing et maintenir la cohérence de la marque, vous pouvez intégrer les expériences [!DNL **GenStudio for Performance Marketing**] à [!DNL **Adobe Campaign**] de manière transparente. Cela vous permet de tirer parti de la création de contenu basée sur l’IA de [!DNL GenStudio] tout en bénéficiant des fonctionnalités d’orchestration avancées d’[!DNL Adobe Campaign].

>[!INFO]
>
>Pour en savoir plus, consultez cette [vue d’ensemble](https://business.adobe.com/fr/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} et une [démonstration](https://business.adobe.com/fr/products/genstudio-for-performance-marketing.html#demo){target="_blank"} d’[!DNL Adobe GenStudio for Performance Marketing].

## Utiliser les fonctionnalités de GenStudio dans Adobe Campaign {#use-genstudio}

L’intégration de [!DNL GenStudio for Performance Marketing] à [!DNL Adobe Campaign] vous permet de faire en sorte que les spécialistes marketing de votre entreprise travaillent mieux ensemble pour optimiser les processus.

Par exemple, un ou une spécialiste du marketing technique, qui utilise [!DNL Adobe Campaign] pour développer et automatiser des campagnes par e-mail, peut collaborer avec un ou une spécialiste du marketing de performance qui crée du contenu à l’aide de [!DNL GenStudio].

Grâce à cette intégration, ces deux personnes peuvent travailler ensemble pour intégrer facilement du contenu de marque provenant de [!DNL GenStudio] dans [!DNL Adobe Campaign], ce qui permet de créer des e-mails attrayants qui ciblent des segments de clientèle spécifiques et stimulent les ventes.

### Exporter un modèle HTML à partir d’Adobe Campaign vers GenStudio {#export-from-campaign-to-genstudio}

Tout d’abord, vous pouvez exporter un modèle HTML [!DNL Adobe Campaign] incluant les directives de votre marque vers [!DNL GenStudio for Performance Marketing]. Suivez les étapes ci-dessous.

1. Dans [!DNL Adobe Campaign], accédez au contenu de votre e-mail. [Voici comment procéder](../email/create-email.md#create-content)

1. Dans le Concepteur d’e-mail, sélectionnez **[!UICONTROL Exporter en HTML]** à l’aide du bouton **[!UICONTROL Plus]**.

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. Chargez le modèle HTML exporté dans [!DNL GenStudio for Performance Marketing]. <!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >Découvrez comment charger un modèle HTML dans [!DNL GenStudio] dans la section dédiée à ce sujet du [Guide d’utilisation d’Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"}.<!--GenStudio doc to be updated with Campaign-->

1. Dans GenStudio, utilisez ce modèle pour créer plusieurs variations d’e-mail à l’aide de prompts d’IA et enregistrez-les.

   >[!NOTE]
   >
   >Découvrez comment créer des expériences d’e-mail dans la [section](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"} dédiée à ce sujet pour GenStudio.

### Utiliser les expériences GenStudio dans Adobe Campaign {#leverage-genstudio-experiences}

Pour utiliser les variations d’e-mail [!DNL GenStudio] que vous venez de créer en les important dans [!DNL Adobe Campaign], procédez comme suit.

1. Dans [!DNL Adobe Campaign], [créez une diffusion e-mail](../email/create-email.md).

1. Dans le tableau de bord de la diffusion e-mail, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**. [En savoir plus](../email/create-email.md#create-content)

1. Dans la page d’accueil du Concepteur d’e-mail, sélectionnez **[!UICONTROL Importer du HTML]** et cliquez sur le bouton **[!UICONTROL Adobe GenStudio for Performance Marketing]**.

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. Parcourez les expériences GenStudio pour commencer à créer votre contenu. Vous pouvez filtrer les expériences selon plusieurs critères tels que les produits, les personas, les marques ou même les couleurs.

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. Sélectionnez une expérience et cliquez sur **[!UICONTROL Utiliser]**.

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. Sélectionnez le dossier dans lequel vous souhaitez importer l’expérience GenStudio.

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. Le contenu sélectionné s’affiche dans le Concepteur d’e-mail.

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >Les expériences GenStudio [créées à partir d’un modèle [!DNL Adobe Campaign] ](#export-from-ajo-to-genstudio) sont importées directement dans le Concepteur d’e-mail. Les expériences GenStudio créées sans modèle [!DNL Adobe Campaign] sont importées en [mode de compatibilité](../email/existing-content.md).

   Utilisez les [outils d’édition de contenu d’e-mail](../email/create-email-content.md) et les [champs de personnalisation](../personalization/personalize.md) pour modifier votre e-mail selon vos besoins. Enregistrez votre contenu.

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456038/?quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->