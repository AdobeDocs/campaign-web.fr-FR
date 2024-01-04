---
audience: end-user
product: campaign
title: Utilisation de modèles de contenu
description: Découvrez comment créer des modèles pour réutiliser du contenu dans les emails Adobe Campaign
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="LA"
source-git-commit: cd7e2bb325b4e571018a8e04ffa0eaef74fe6768
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 12%

---

# Utilisation de modèles de contenu {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Définir votre propre contenu"
>abstract="Créez entièrement un modèle personnalisé autonome pour rendre votre contenu réutilisable sur plusieurs emails."

Pour accélérer et améliorer le processus de conception, vous pouvez créer des modèles autonomes pour réutiliser facilement du contenu personnalisé dans [!DNL Adobe Campaign].

Cette fonctionnalité permet aux utilisateurs orientés contenu de travailler sur des modèles autonomes afin que les utilisateurs marketing puissent les réutiliser et les adapter dans leurs propres campagnes par e-mail.

>[!NOTE]
>
>Actuellement uniquement **email** les modèles de contenu sont pris en charge.

## Accéder aux modèles et les gérer {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Modifier le contenu du modèle"
>abstract="Cliquez sur le bouton **Modifier le contenu** pour mettre à jour votre contenu avec le Concepteur d&#39;email."

Pour accéder à la liste des modèles de contenu, sélectionnez **[!UICONTROL Gestion de contenu]** > **[!UICONTROL Modèles de contenu]** dans le menu de gauche.

![](assets/content-template-list.png)

Tous les modèles qui ont été créés, à partir d’un email utilisant la variable [Enregistrer en tant que modèle](#save-as-template) de l’option **[!UICONTROL Modèles de contenu]** menu - s’affichent.

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

Vous pouvez filtrer selon un [folder](../get-started/permissions.md#folders) à l’aide de la liste déroulante ou en ajoutant des règles à l’aide de la fonction [query modeler](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

Pour modifier le contenu d’un modèle, cliquez sur l’élément de votre choix dans la liste. Vous pouvez ainsi effectuer les actions suivantes :

* Modifiez ses propriétés.

* Cliquez sur le bouton **[!UICONTROL Modifier le contenu]** pour mettre à jour votre contenu à l’aide du bouton [Concepteur d&#39;email](get-started-email-designer.md).

![](assets/content-template-edition.png)

Pour supprimer un modèle, sélectionnez l’option correspondante dans la **[!UICONTROL Autres actions]** .

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>Lorsqu&#39;un modèle est supprimé, les diffusions créées à l&#39;aide de ce modèle ne sont pas impactées.

## Créer des modèles de contenu {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Conception de modèle de contenu"
>abstract="Conception de modèle de contenu"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Sélection du modèle de contenu"
>abstract="Sélection du modèle de contenu"

Vous pouvez créer des modèles de contenu de deux manières différentes :

* Créez un modèle de contenu entièrement nouveau à l’aide du rail de gauche. **[!UICONTROL Modèles de contenu]** . [Voici comment procéder](#create-template-from-scratch).

* Lors de la conception d&#39;un email, enregistrez le contenu de votre email en tant que modèle. [Voici comment procéder](#save-as-template).

Une fois enregistré, qu’il soit entièrement créé ou à partir d’un email précédent, vous pouvez désormais utiliser ce modèle lors de la création d’un [email](../email/create-email.md) dans [!DNL Adobe Campaign]. [Voici comment procéder](use-email-templates.md).

>[!NOTE]
>
>* Les modifications apportées aux modèles de contenu ne sont pas propagées aux emails.
>
>* De même, lorsque des modèles sont utilisés dans un email, les modifications que vous apportez au contenu de votre email n’ont aucune incidence sur le modèle de contenu précédemment utilisé.

### Créer entièrement un modèle {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Définition des propriétés du modèle"
>abstract="Lors de la création d’un modèle à partir de zéro, définissez ses propriétés à récupérer facilement si nécessaire."

Pour créer entièrement un modèle de contenu, procédez comme suit.

1. Accédez à la liste des modèles de contenu via le **[!UICONTROL Gestion de contenu]** > **[!UICONTROL Modèles de contenu]** menu de gauche.

1. Sélectionner **[!UICONTROL Créer un modèle]**.

   ![](assets/content-template-create.png)

1. Renseignez les détails du modèle. Vous pouvez sélectionner le dossier dans lequel vous souhaitez stocker votre modèle. Par défaut, les modèles de contenu sont stockés dans un noeud dédié de la hiérarchie Adobe Campaign : **[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Modèles]** > **[!UICONTROL Modèles de contenu]**. [Découvrez comment créer des dossiers](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >Actuellement, seule la variable **Email** channel et **HTML** Les types sont pris en charge.

1. Cliquez sur **[!UICONTROL Créer]** et choisissez la manière dont vous souhaitez concevoir votre modèle parmi les différentes options suivantes :

   * [Concevoir entièrement votre email](create-email-content.md) via l&#39;interface du Concepteur d&#39;email.

   * [HTML brut de code ou de copier-coller](code-content.md) directement dans le Concepteur d&#39;email.

   * [Importer du contenu de HTML existant](existing-content.md) à partir d’un fichier ou d’un dossier .zip.

   * Utilisez du contenu existant à partir d’une liste de modèles intégrés ou personnalisés. Les étapes d&#39;utilisation d&#39;un modèle de contenu dans un email sont décrites dans la section [cette section](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. La variable [Concepteur d&#39;email](get-started-email-designer.md) s’affiche. Modifiez votre contenu selon vos besoins, comme vous le feriez pour n&#39;importe quel email, selon l&#39;option que vous avez sélectionnée.

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Une fois votre modèle prêt, cliquez sur **[!UICONTROL Enregistrer]**.

   Si nécessaire, cliquez sur la flèche en regard du nom du modèle pour revenir au **[!UICONTROL Détails]** et modifiez votre modèle.

   ![](assets/content-template-save-back.png)

Ce modèle est maintenant prêt à être utilisé lors de la création d’un courrier électronique dans [!DNL Adobe Campaign]. [Voici comment procéder](use-email-templates.md).

### Enregistrer le contenu de l’e-mail en tant que modèle {#save-as-template}

Une fois votre [e-mail conçu](create-email-content.md), vous pouvez enregistrer ce contenu en tant que modèle pour une réutilisation ultérieure. Les modèles enregistrés sont disponibles pour tous les utilisateurs et utilisatrices de votre environnement Adobe Campaign.

Pour enregistrer un contenu d’e-mail en tant que modèle, procédez comme suit :

1. Dans le concepteur d’email, cliquez sur le **[!UICONTROL Plus]** en haut à droite de l’écran.

1. Sélectionnez **[!UICONTROL Enregistrer comme modèle de contenu]** dans le menu déroulant.

   ![](assets/email_designer-save-template.png)

1. Saisissez le nom du modèle et enregistrez-le.

   ![](assets/email_designer-template-name.png)

Vous pouvez maintenant utiliser ce modèle pour créer un nouveau contenu : il est disponible dans la **[!UICONTROL Modèles enregistrés]** du Concepteur d’email. [Voici comment procéder](use-email-templates.md).

![](assets/email_designer-saved-template.png)

Le modèle est enregistré dans la variable **[!UICONTROL Modèles de contenu]** accessible à partir de la liste [!DNL Adobe Campaign] menu dédié. Il devient alors un modèle de contenu autonome, accessible, édité et supprimé comme tout autre élément de cette liste. [En savoir plus](#access-manage-templates)

>[!NOTE]
>
>Toute modification apportée à ce nouveau modèle n’est pas propagée dans l’e-mail d’où elle provient. De même, lorsque le contenu d’origine est modifié dans cet email, le nouveau modèle n’est pas modifié.

<!--
Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list through the **[!UICONTROL Content Management]** > **[!UICONTROL Content Templates]** menu and select any template.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view. [Learn more](../content-management/preview-test.md)

    ![](../email/assets/content-template-stimulate.png)

1. You can send a proof to test your content and have it approved by some internal users before using it in a journey or a campaign.

    * To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in [this section](../content-management/proofs.md).
    
    * Before sending the proof, you must select the [email surface](../configuration/channel-surfaces.md) that will be used to test your content.

        ![](../email/assets/content-template-stimulate-proof-surface.png)

>[!CAUTION]
>
>Currently tracking is not supported when testing email content templates, meaning that tracking events, UTM parameters and landing page links will not be effective in the proofs that are being sent from a template. To test tracking, [use the content template](
use-email-templates.md) in an email and [send a proof](../content-management/preview-test.md#send-proofs).-->


