---
title: Configurer [!DNL Campaign] options
description: Découvrez comment configurer les options de Campaign et créer vos propres options personnalisées.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: 3bedb4562c5858cd6057fd8a17064ccac8303c39
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# Configurer les options de [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Options"
>abstract="Options"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Option Créer"
>abstract="Option Créer"

Adobe Campaign Web s’accompagne d’options techniques qui vous permettent de configurer l’application plus spécifiquement. Certaines de ces options sont intégrées, tandis que d’autres peuvent être ajoutées manuellement selon les besoins.

>[!IMPORTANT]
>
>Les options intégrées sont préconfigurées et ne doivent être modifiées que par les utilisateurs avancés. Si vous avez des questions ou des demandes, communiquez avec le représentant de votre Adobe.

## Accéder aux options de Campaign {#access}

Les options sont disponibles à partir du menu **[!UICONTROL Administration]** / **[!UICONTROL Options]**. Utilisez le volet de filtrage pour affiner la liste et trouver rapidement l’option dont vous avez besoin.

![](assets/options-list.png)

>[!NOTE]
>
>Bien que l’emplacement du menu des options diffère entre la console Adobe Campaign et l’interface utilisateur web, la liste est identique et fonctionne comme un miroir. Pour plus d&#39;informations sur les options disponibles, reportez-vous à la liste des options dans la documentation de [Campaign v7](https://experienceleague.adobe.com/fr/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}

Dans la liste des options, vous pouvez :

* **Dupliquer ou supprimer une option** : cliquez sur le bouton représentant des points de suspension et sélectionnez l’action souhaitée.
* **Modifier une option** : cliquez sur le nom de l’option pour ouvrir ses propriétés. Apportez vos modifications et enregistrez-les.
* **Créer une option personnalisée** : cliquez sur le bouton **[!UICONTROL Créer]**.

## Création d’une option {#create}

L’interface utilisateur web d’Adobe Campaign vous permet de créer vos propres options personnalisées en fonction de vos besoins. Cela s’avère particulièrement utile lorsque vous utilisez des activités de workflow **[!UICONTROL Code JavaScript]** pour stocker des données intermédiaires.

Pour créer une option :

1. Accédez à la liste des options et cliquez sur **[!UICONTROL Créer une option]**.
1. Attribuez un nom à l’option, sélectionnez son type et définissez la valeur souhaitée.
1. Cliquez sur **[!UICONTROL Créer]** pour créer l’option.

   ![](assets/options-create.png)

Les options peuvent servir d’espace de stockage temporaire des données et offrir les avantages suivants :

* Valeurs saisies : les options prennent en charge des types de données spécifiques, tels que des dates, des entiers, des chaînes...
* Flexibilité : les options permettent aux utilisateurs de stocker et de récupérer les données efficacement, sans avoir à gérer les tables de base de données.

Dans l’exemple ci-dessous, nous créons une option personnalisée nommée `sampleOption` avec la valeur initiale « a ». Une activité **[!UICONTROL Code JavaScript]** dans un workflow modifie la valeur de cette option et la stocke dans une variable. La valeur mise à jour s’affiche dans les logs de workflow et est reflétée dans le menu **[!UICONTROL Options]**.

1. Créez l’option .

   ![](assets/options-sample-create.png)

1. Configurez une activité **[!UICONTROL Code JavaScript]** et démarrez le workflow.

   ![](assets/options-sample-javascript.png)

1. Exécutez le workflow pour afficher la valeur mise à jour dans les logs de workflow.

   ![](assets/options-sample-logs.png)

1. La valeur mise à jour est désormais visible dans le menu **[!UICONTROL Options]**.

   ![](assets/options-sample-updated.png)
