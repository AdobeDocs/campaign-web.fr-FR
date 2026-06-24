---
audience: end-user
title: Utiliser l’activité de workflow Jointure
description: Découvrez comment utiliser l’activité de workflow Jointure.
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: ht
source-wordcount: '473'
ht-degree: 100%

---

# Jointure {#join}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Branches de workflow multiples et activité Jointure"
>abstract="Plusieurs branches sont désormais prises en charge. Au lieu d’utiliser un branchement, vous pouvez cliquer sur Ajouter une branche dans la barre d’outils. L’activité Rendez-vous a également été améliorée. Il s’agit désormais d’une activité de jointure générique qui vous permet de choisir entre les options de jointure ET et OU."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Activité AND-join"
>abstract="L’activité **Rendez-vous** vous permet de synchroniser plusieurs branches d’exécution d’un workflow. Elle est déclenchée une fois toutes les activités précédentes terminées. Cela permet de s’assurer que certaines activités sont terminées avant de continuer à exécuter le workflow."

>[!CONTEXTUALHELP]
>id="acw_orchestration_join"
>title="Activité de jointure"
>abstract="L’activité **Jointure** permet de fusionner plusieurs transitions entrantes. Choisissez de continuer lorsque toutes les transitions entrantes sont terminées (ET) ou lorsqu’une transition entrante est terminée (OU)."

L’activité **Jointure** est une activité **Contrôle de flux**. Elle synchronise plusieurs branches d’exécution d’un workflow.
Vous pouvez choisir le mode d’évaluation des transitions entrantes :

* **ET** : se poursuit uniquement après l’activation de toutes les transitions entrantes sélectionnées.
* **OU** : se poursuit dès qu’une transition entrante sélectionnée est activée.

Lorsque **ET** est sélectionné, cette activité ne déclenche sa transition sortante qu’une fois toutes les transitions entrantes activées.En d’autres termes, elle s’active une fois toutes les activités précédentes terminées. Cela permet de s’assurer que certaines activités sont terminées avant de continuer à exécuter le workflow.

Lorsque **OU** est sélectionné, l’exécution se poursuit dès que l’une des transitions entrantes sélectionnées est activée.Elle n’attend pas chaque branche.

## Configurer l’activité Jointure {#join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Options de fusion"
>abstract="Sélectionnez les activités auxquelles vous souhaitez adhérer. Dans l’**Ensemble principal**, choisissez la population de transition entrante à conserver."

Pour configurer l’activité **Jointure**, procédez comme suit :

1. Ajoutez plusieurs activités telles que des activités de canal afin de former au moins deux branches d’exécution différentes. Vous pouvez utiliser un **Branchement** ou ajouter une branche distincte à l’aide du bouton de la barre d’outils **Ajouter une branche** (+).Voir [Orchestrer les activités](../orchestrate-activities.md#toolbar).

   ![Copie d’écran montrant deux branches.](../assets/workflow-join.png)

1. Ajoutez une activité **Jointure** à l’une des branches.

   ![Copie d’écran affichant l’activité Jointure ajoutée.](../assets/workflow-join2.png)

1. Dans les options de jointure, choisissez **ET** ou **OU** et cliquez sur **Continuer**.
1. Dans les **Options de fusion**, cochez les activités précédentes à joindre.
1. Dans l’**Ensemble principal**, choisissez la population de transition entrante à conserver. La transition sortante ne peut contenir que l’une des populations de la transition entrante.

   >[!NOTE]
   >
   >Le champ **Ensemble principal** n’est disponible que pour l’option de jointure **ET**.

   ![Copie d’écran affichant la jointure configurée.](../assets/workflow-join3.png)

## Exemple {#join-example}

L’exemple ci-après montre deux branches d’un workflow avec une diffusion e-mail et SMS. L’activité **Jointure**, définie sur **ET**, se déclenche lorsque les deux transitions entrantes sont activées.Les notifications push sont envoyées uniquement une fois les deux diffusions terminées. Si vous définissez l’option de jointure sur **OU**, les messages push sont envoyés dès que la première activité de diffusion entrante est terminée.

![Exemple de workflow avec deux branches, affichant la diffusion par e-mail et par SMS suivie de notifications push.](../assets/workflow-join4.png){zoomable="yes"}