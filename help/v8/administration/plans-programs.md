---
audience: end-user
title: Plans et programmes
description: Découvrir comment créer et envoyer des plans et des programmes dans Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 100%

---

# Plans et programmes {#plan-and-programs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Plans et programmes"
>abstract="Vous pouvez maintenant paramétrer la hiérarchie des dossiers des plans marketing et des programmes dans l’interface d’utilisation de Campaign Web."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

Adobe Campaign permet de configurer la hiérarchie des dossiers des plans marketing et des programmes.

Pour mieux les organiser, Adobe recommande la hiérarchie suivante : Plan `>` Programmes `>` Campagnes.

* Un **plan** peut contenir plusieurs programmes. Il définit des objectifs stratégiques pour une période de temps.
* Un **programme** peut contenir d’autres programmes, des campagnes, des workflows et des pages de destination.
* Une **campagne** peut contenir des diffusions, des workflows et des pages de destination.

## Créer et configurer un plan {#create-plan}

Pour créer un plan, vous devez créer un dossier avec le type de dossier **[!UICONTROL Plan]**. [En savoir plus sur la création d’un dossier](create-manage-folder.md).

![](assets/plan_create.png){zoomable="yes"}

Accédez aux **[!UICONTROL Paramètres de dossier]** de votre plan pour le gérer.

![](assets/plan_settings.png){zoomable="yes"}

Vous pouvez définir des **[!UICONTROL Options personnalisées]** et définir la date de planification de votre plan.

![](assets/plan_options.png){zoomable="yes"}

Pour gérer les **[!UICONTROL Options personnalisées]**, procédez comme suit :

1. Accédez aux **[!UICONTROL Schémas]**.
1. Choisissez les schémas **[!UICONTROL Modifiables]** dans les filtres.
1. Cliquez sur l’icône **[!UICONTROL Modifier les détails personnalisés]**.

![](assets/plan_edit.png){zoomable="yes"}

Vous pouvez les configurer comme suit :

![](assets/plan_customfields.png){zoomable="yes"}

## Créer et configurer un programme

Pour créer un programme dans votre plan ([En savoir plus sur la création d’un plan.](#create-plan)), vous devez être dans votre plan et créer un dossier avec le type de dossier **[!UICONTROL Programme]**.[En savoir plus sur la création d’un dossier](create-manage-folder.md).

![](assets/program_create.png){zoomable="yes"}

Accédez aux **[!UICONTROL Paramètres de dossier]** de votre programme pour le gérer.

![](assets/program_settings.png){zoomable="yes"}

Vous pouvez définir des **[!UICONTROL Options personnalisées]** et définir la date de planification de votre programme.

![](assets/program_options.png){zoomable="yes"}

Pour gérer les **[!UICONTROL Options personnalisées]**, procédez comme suit :

1. Accédez aux **[!UICONTROL Schémas]**.
1. Choisissez les schémas **[!UICONTROL Modifiables]** dans les filtres.
1. Cliquez sur l’icône **[!UICONTROL Modifier les détails personnalisés]**.

![](assets/program_edit.png){zoomable="yes"}

Vous pouvez les configurer comme suit :

![](assets/program_customfields.png){zoomable="yes"}

## Comment lier une campagne à un programme

Vous pouvez lier une campagne à un programme de deux manières différentes :

### Méthode 1 : vous disposez déjà d’un programme et souhaitez créer une campagne qui lui est liée.

Pour lier une nouvelle campagne à votre programme, créez directement votre campagne dans le programme :

![](assets/program_campaign_create.png){zoomable="yes"}

Les paramètres **[!UICONTROL Dossier]** seront automatiquement renseignés avec le chemin d’accès à votre programme.

![](assets/program_campaign_folder.png){zoomable="yes"}

### Méthode 2 : vous avez déjà une campagne existante et souhaitez la lier à un programme existant.

Cliquez sur le bouton **[!UICONTROL Paramètres]** de la campagne que vous souhaitez lier à votre programme :

![](assets/campaign_settings.png){zoomable="yes"}

Dans ses **[!UICONTROL Propriétés]**, cliquez sur l’icône **[!UICONTROL Dossier]** dans les paramètres **[!UICONTROL Dossier]** pour choisir votre dossier **[!UICONTROL Programme]**.

![](assets/campaign_folder.png){zoomable="yes"}

Sélectionnez votre dossier **[!UICONTROL Programme]** et cliquez sur le bouton **[!UICONTROL Confirmer]**, puis sur le bouton **[!UICONTROL Enregistrer et fermer]**.

![](assets/campaign_linked.png){zoomable="yes"}

Votre campagne est maintenant répertoriée dans votre programme :

![](assets/campaign_in_program.png){zoomable="yes"}
