---
audience: end-user
product: campaign
title: Utiliser des modèles de contenu
description: Découvrez comment créer des modèles pour réutiliser du contenu dans les e-mails Adobe Campaign
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="Disponibilité limitée"
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 72899742daf04a0da6e2fb3d802b7841753b8c6c
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 89%

---

# Utiliser des modèles de contenu {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Définir votre propre contenu"
>abstract="Créez un modèle personnalisé autonome à partir de zéro pour rendre votre contenu réutilisable entre plusieurs e-mails."

Pour un processus de conception accéléré et amélioré, vous pouvez créer des modèles autonomes afin de réutiliser facilement le contenu personnalisé dans [!DNL Adobe Campaign].

Cette fonctionnalité permet aux personnes orientées contenu d’utiliser des modèles autonomes afin que les utilisateurs et utilisatrices marketing puissent les réutiliser et les adapter dans leurs propres campagnes par e-mail.

>[!NOTE]
>
>Actuellement, seuls les modèles de contenu d’**e-mail** sont pris en charge.

## Accéder aux modèles et les gérer {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Modifier le contenu de votre modèle"
>abstract="Cliquez sur le bouton **Modifier le contenu** pour mettre à jour votre contenu avec le Concepteur d’e-mail."

Pour accéder à la liste des modèles de contenu, sélectionnez **[!UICONTROL Gestion de contenu]** > **[!UICONTROL Modèles de contenu]** dans le menu de gauche.

![](assets/content-template-list.png)

Tous les modèles qui ont été créés, que ce soit à partir d’un e-mail à l’aide de l’option [Enregistrer en tant que modèle](#save-as-template) ou à partir du menu **[!UICONTROL Modèles de contenu]**, s’affichent.

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

Vous pouvez filtrer sur un [dossier](../get-started/permissions.md#folders) spécifique à l’aide de la liste déroulante ou ajouter des règles à l’aide du [concepteur de requête](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

Pour modifier le contenu d’un modèle, cliquez sur l’élément souhaité dans la liste. Vous pouvez ainsi effectuer les actions suivantes :

* Modifiez ses propriétés.

* Cliquez sur le bouton **[!UICONTROL Modifier le contenu]** pour mettre à jour votre contenu avec le [Concepteur d’e-mail](get-started-email-designer.md).

![](assets/content-template-edition.png)

Pour supprimer un modèle, sélectionnez l’option correspondante dans le menu **[!UICONTROL Plus d’actions]**.

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>Lorsqu’un modèle est supprimé, les diffusions créées à l’aide de ce modèle ne sont pas affectées.

## Créer des modèles de contenu {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Conception de modèle de contenu"
>abstract="Conception de modèle de contenu"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Sélection du modèle de contenu"
>abstract="Sélection du modèle de contenu"

Vous pouvez créer des modèles de contenu de deux manières différentes :

* Créez un modèle de contenu à partir de zéro à l’aide du menu **[!UICONTROL Modèles de contenu]** du rail de gauche. [Voici comment procéder](#create-template-from-scratch).

* Lors de la conception d’un e-mail, enregistrez le contenu de votre e-mail en tant que modèle. [Voici comment procéder](#save-as-template).

Une fois enregistré, qu’il soit créé à partir de zéro ou à partir d’un e-mail précédent, vous pouvez désormais utiliser ce modèle lors de la création d’un [e-mail](../email/create-email.md) dans [!DNL Adobe Campaign]. [Voici comment procéder](use-email-templates.md).

>[!NOTE]
>
>* Les modifications apportées aux modèles de contenu ne sont pas propagées aux e-mails.
>
>* De même, lorsque des modèles sont utilisés dans un e-mail, les modifications que vous apportez au contenu de votre e-mail n’ont aucune incidence sur le modèle de contenu précédemment utilisé.

### Créer un modèle à partir de zéro {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Définir les propriétés de votre modèle"
>abstract="Lors de la création d’un modèle à partir de zéro, définissez ses propriétés à récupérer facilement si nécessaire."

Pour créer un modèle de contenu à partir de zéro, procédez comme suit.

1. Accédez à la liste des modèles de contenu via le menu de gauche **[!UICONTROL Gestion de contenu]** > **[!UICONTROL Modèles de contenu]**.

1. Sélectionnez **[!UICONTROL Créer un modèle]**.

   ![](assets/content-template-create.png)

1. Renseignez les détails du modèle. Vous pouvez sélectionner le dossier dans lequel vous souhaitez stocker votre modèle. Par défaut, les modèles de contenu sont stockés dans un dossier dédié de la hiérarchie Adobe Campaign : **[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Modèles]** > **[!UICONTROL Modèles de contenu]**. [Découvrez comment créer des dossiers](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >Actuellement, seuls le canal **E-mail** et le type **HTML** sont pris en charge.

1. Cliquez sur **[!UICONTROL Créer]** et choisissez votre méthode de conception de modèle parmi les différentes options suivantes :

   * [Concevez votre e-mail à partir de zéro](create-email-content.md) dans l’interface du Concepteur d’e-mail.

   * [Codez ou collez du code HTML brut](code-content.md) directement dans le Concepteur d’e-mail.

   * [Importez du contenu HTML existant](existing-content.md) à partir d’un fichier ou d’un dossier .zip.

   * Utilisez du contenu existant à partir d’une liste de modèles intégrés ou personnalisés. Les étapes d’utilisation d’un modèle de contenu dans un e-mail sont décrites dans [cette section](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. Le [Concepteur d’e-mail](get-started-email-designer.md) s’affiche. Modifiez votre contenu selon vos besoins, comme vous le feriez pour n’importe quel e-mail, en fonction de l’option que vous avez sélectionnée.

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Lorsque votre modèle est prêt, cliquez sur **[!UICONTROL Enregistrer]**.

   Si nécessaire, cliquez sur la flèche en regard du nom du modèle pour revenir à l’écran **[!UICONTROL Détails]** et modifiez votre modèle.

   ![](assets/content-template-save-back.png)

Le modèle est enregistré dans le dossier par défaut de la hiérarchie Adobe Campaign (**[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Modèles]** > **[!UICONTROL Modèles de contenu]**). [En savoir plus sur les dossiers](../get-started/permissions.md#folders)

Elle s’affiche également dans la variable **[!UICONTROL Modèles de contenu]** liste. [En savoir plus](#access-manage-templates)

Vous pouvez désormais utiliser ce modèle pour créer un nouveau contenu : il est disponible sous l’onglet **[!UICONTROL Modèles enregistrés]** du Concepteur d’e-mail. [Voici comment procéder](use-email-templates.md).

### Enregistrer le contenu de l’e-mail en tant que modèle {#save-as-template}

Une fois votre [e-mail conçu](create-email-content.md), vous pouvez enregistrer ce contenu en tant que modèle pour une réutilisation ultérieure. Les modèles enregistrés sont disponibles pour tous les utilisateurs et utilisatrices de votre environnement Adobe Campaign.

Pour enregistrer un contenu d’e-mail en tant que modèle, procédez comme suit :

1. Dans le concepteur d’e-mail, cliquez sur le bouton **[!UICONTROL Plus]** en haut à droite de l’écran.

1. Sélectionnez **[!UICONTROL Enregistrer comme modèle de contenu]** dans le menu déroulant.

   ![](assets/email_designer-save-template.png)

1. Saisissez le nom du modèle et enregistrez-le.

   ![](assets/email_designer-template-name.png)

Le modèle est enregistré dans le dossier par défaut de la hiérarchie Adobe Campaign (**[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Modèles]** > **[!UICONTROL Modèles de contenu]**). [En savoir plus sur les dossiers](../get-started/permissions.md#folders)

Elle s’affiche également dans la variable **[!UICONTROL Modèles de contenu]** liste. Il devient alors un modèle de contenu autonome, pouvant être consulté, modifié et supprimé comme tout autre élément de cette liste. [En savoir plus](#access-manage-templates)

Vous pouvez désormais utiliser ce modèle pour créer un nouveau contenu : il est disponible sous l’onglet **[!UICONTROL Modèles enregistrés]** du Concepteur d’e-mail. [Voici comment procéder](use-email-templates.md).

![](assets/email_designer-saved-template.png)

>[!NOTE]
>
>Toute modification apportée à ce nouveau modèle n’est pas propagée dans l’e-mail d’où elle provient. De même, lorsque le contenu d’origine est modifié dans cet e-mail, le nouveau modèle n’est pas modifié.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->
