---
audience: end-user
title: Plans et programmes
description: Découvrir comment créer et envoyer des plans et des programmes dans Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 1a751aed6d5185e700dafb1de2afd88300dfcd79
workflow-type: ht
source-wordcount: '522'
ht-degree: 100%

---

# Plans et programmes {#plan-and-programs}

Adobe Campaign permet de configurer la hiérarchie des dossiers des plans marketing et des programmes.

Pour mieux organiser ces composants, Adobe recommande la hiérarchie suivante : Plan `>` Programmes `>` Campagnes.

* Un **plan** peut contenir plusieurs programmes. Il définit des objectifs stratégiques pour une période spécifique.
* Un **programme** peut contenir d’autres programmes, des campagnes, des workflows et des pages de destination.
* Une **campagne** peut contenir des diffusions, des workflows et des pages de destination.

## Créer et configurer un plan {#create-plan}

Pour créer un plan, créez un dossier avec le type de dossier **[!UICONTROL Plan]**. [En savoir plus sur la création d’un dossier](../get-started/work-with-folders.md)

![Capture d’écran montrant la création d’un dossier de plan](assets/plan_create.png){zoomable="yes"}

Accédez aux **[!UICONTROL Paramètres de dossier]** de votre plan pour le gérer.

![Capture d’écran montrant les paramètres de dossier d’un plan](assets/plan_settings.png){zoomable="yes"}

Définissez des **[!UICONTROL Options personnalisées]** et la date de planification de votre plan.

![Capture d’écran montrant les options personnalisées d’un plan](assets/plan_options.png){zoomable="yes"}

Pour gérer les **[!UICONTROL Options personnalisées]**, procédez comme suit :

1. Accédez aux **[!UICONTROL Schémas]**.
1. Choisissez les schémas **[!UICONTROL Modifiables]** dans les filtres.
1. Cliquez sur le schéma.

![Capture d’écran montrant la modification des détails personnalisés d’un plan](assets/plan_edit.png){zoomable="yes"}

1. Cliquez sur le bouton **[!UICONTROL Édition d’écran]**.

   ![](assets/plan_edit2.png){zoomable="yes"}

Configurez les options personnalisées :

![Capture d’écran affichant la configuration des champs personnalisés d’un plan](assets/plan_customfields.png){zoomable="yes"}

## Créer et configurer un programme

Pour créer un programme dans votre plan ([En savoir plus sur la création d’un plan](#create-plan)), accédez à votre plan et créez un dossier avec le type de dossier **[!UICONTROL Programme]**. [En savoir plus sur la création d’un dossier](../get-started/work-with-folders.md).

![Capture d’écran montrant la création d’un dossier de programme](assets/program_create.png){zoomable="yes"}

Accédez aux **[!UICONTROL Paramètres de dossier]** de votre programme pour le gérer.

![Capture d’écran montrant les paramètres de dossier d’un programme](assets/program_settings.png){zoomable="yes"}

Définissez des **[!UICONTROL Options personnalisées]** et la date de planification de votre programme.

![Capture d’écran montrant les options personnalisées d’un programme](assets/program_options.png){zoomable="yes"}

Pour gérer les **[!UICONTROL Options personnalisées]**, procédez comme suit :

1. Accédez aux **[!UICONTROL Schémas]**.
1. Choisissez les schémas **[!UICONTROL Modifiables]** dans les filtres.
1. Cliquez sur le schéma.

![Capture d’écran montrant la modification des détails personnalisés d’un programme](assets/program_edit.png){zoomable="yes"}

1. Cliquez sur le bouton **[!UICONTROL Édition d’écran]**.

   ![](assets/program_edit2.png){zoomable="yes"}

Configurez les options personnalisées :

![Capture d’écran montrant la configuration des champs personnalisés d’un programme](assets/program_customfields.png){zoomable="yes"}

## Comment lier une campagne à un programme

Vous pouvez lier une campagne à un programme de deux manières différentes :

### Méthode 1 : vous disposez déjà d’un programme et souhaitez créer une campagne qui lui est liée.

Pour lier une nouvelle campagne à votre programme, créez directement la campagne dans le programme.

![Capture d’écran montrant la création d’une campagne dans un programme](assets/program_campaign_create.png){zoomable="yes"}

Les paramètres **[!UICONTROL Dossier]** seront automatiquement renseignés avec le chemin d’accès à votre programme.

![Capture d’écran affichant les paramètres du dossier pour une campagne liée à un programme](assets/program_campaign_folder.png){zoomable="yes"}

### Méthode 2 : vous avez déjà une campagne existante et souhaitez la lier à un programme existant.

Cliquez sur le bouton **[!UICONTROL Paramètres]** de la campagne que vous souhaitez lier à votre programme.

![Capture d’écran montrant le bouton des paramètres d’une campagne](assets/campaign_settings.png){zoomable="yes"}

Dans ses **[!UICONTROL Propriétés]**, cliquez sur l’icône **[!UICONTROL Dossier]** dans les paramètres **[!UICONTROL Dossier]** pour choisir votre dossier **[!UICONTROL Programme]**.

![Capture d’écran montrant la sélection du dossier pour lier une campagne à un programme](assets/campaign_folder.png){zoomable="yes"}

Sélectionnez votre dossier **[!UICONTROL Programme]** et cliquez sur le bouton **[!UICONTROL Confirmer]**, puis sur le bouton **[!UICONTROL Enregistrer et fermer]**.

![Capture d’écran montrant une campagne liée à un programme](assets/campaign_linked.png){zoomable="yes"}

Votre campagne est maintenant répertoriée dans votre programme :

![Capture d’écran montrant une campagne répertoriée dans un programme](assets/campaign_in_program.png){zoomable="yes"}