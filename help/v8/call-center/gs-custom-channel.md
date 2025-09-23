---
audience: end-user
title: Prise en main des canaux personnalisés
description: Découvrez comment créer et envoyer des diffusions de canal personnalisé avec Adobe Campaign Web
exl-id: b4336a0a-d845-4024-a06b-400fce1316a4
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 41%

---

# Prise en main des canaux personnalisés {#gs-custom-channel}

Vous pouvez, directement à partir de l’interface utilisateur web d’Adobe Campaign, orchestrer et exécuter des diffusions en fonction de canaux personnalisés intégrés à des tiers. La configuration du canal personnalisé s’effectue dans la console cliente.

Deux types de canaux personnalisés sont pris en charge : externe et API. Avec les canaux externes, Campaign génère des fichiers d&#39;export personnalisables avec toutes les données de contact et de personnalisation nécessaires. Avec les canaux API, les messages sont envoyés aux profils cibles via l’API configurée.

Vous pouvez ajouter des diffusions de canal personnalisé dans les workflows ou simplement les utiliser comme diffusions autonomes.

Les étapes ci-dessous détaillent la procédure d’une diffusion autonome (ponctuelle). La plupart des étapes sont similaires aux diffusions de centre d’appel. Pour plus d&#39;informations, consultez cette [page](../call-center/create-call-center.md).

Pour envoyer une nouvelle diffusion personnalisée autonome, procédez comme suit :

1. Configurez le canal personnalisé. [En savoir plus](#create-channel)
1. Créer la diffusion, [en savoir plus](#create-delivery)
1. Définir l’audience, [en savoir plus](#select-audience)
1. Modifier le contenu, [en savoir plus](#edit-content)
1. Prévisualiser et envoyer la diffusion, [en savoir plus](#preview-send)

## Configuration du canal personnalisé{#create-channel}

Tout d’abord, vous devez configurer le canal personnalisé. Les principales étapes à effectuer dans la console cliente sont les suivantes. Ces étapes sont communes aux canaux externes et API personnalisés :

1. Configurez le schéma pour ajouter le nouveau canal à la liste des canaux disponibles. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html#configure-schema){target="_blank"}
1. Créez un compte externe de routage. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html#reate-ext-account){target="_blank"}
1. Créez un nouveau modèle de diffusion associé au nouveau canal. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html#create-template){target="_blank"}

Les canaux d’API personnalisés nécessitent une configuration supplémentaire. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html#api-additional){target="_blank"}

## Créer la diffusion{#create-delivery}

Suivez ces étapes pour créer la diffusion et configurer ses propriétés :

1. Sélectionnez le menu **[!UICONTROL Diffusions]** et cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Choisissez le canal personnalisé de votre choix, sélectionnez le modèle associé et cliquez sur **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![Capture d’écran affichant la création d’une diffusion personnalisée](assets/cus-create.png){zoomable="yes"}

1. Sous **[!UICONTROL Propriétés]**, saisissez un **[!UICONTROL Libellé]** pour la diffusion.

   ![Capture d’écran affichant la configuration des propriétés d’une diffusion personnalisée](assets/cus-properties.png){zoomable="yes"}

Pour plus d’informations sur la création de diffusions, consultez la [documentation](../call-center/create-call-center.md#create-delivery) du centre d’appel.

## Définir l’audience{#select-audience}

Vous devez maintenant définir l’audience qui sera ciblée.

1. Dans la section **[!UICONTROL Audience]** du tableau de bord de la diffusion, cliquez sur **[!UICONTROL Sélectionner une audience]**.

1. Choisissez une audience existante ou créez la vôtre.

   ![Capture d’écran affichant la sélection de l’audience pour une diffusion personnalisée](assets/cc-audience2.png){zoomable="yes"}

Pour plus d’informations sur la définition d’une audience, consultez la [documentation](../call-center/create-call-center.md#select-audience) du centre d’appel.

## Modifier le contenu{#edit-content}

Maintenant, modifions le contenu de la diffusion.

>[!BEGINTABS]

>[!TAB  Canal externe personnalisé ]

1. Dans le tableau de bord de la diffusion, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

1. Spécifiez un **[!UICONTROL Nom de fichier]**, sélectionnez un **[!UICONTROL Format de fichier]** et ajoutez autant de colonnes que nécessaire pour votre fichier d’extraction.

   ![Capture d’écran affichant les options de configuration des attributs pour le fichier d’extraction](assets/cc-content-attributes.png)

>[!TAB Canal API personnalisé]

1. Dans le tableau de bord de la diffusion, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

1. Renseignez les champs selon vos besoins. Pour savoir comment configurer cet écran, consultez cette [page](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html#api-additional-screen){target="_blank"}.

   ![Capture d’écran affichant les options de configuration des attributs pour le canal API.](assets/cc-content-attributes-api.png)

>[!ENDTABS]

Pour plus d’informations sur l’édition de contenu, consultez la [documentation](../call-center/create-call-center.md#edit-content) du centre d’appel.

## Prévisualiser et envoyer la diffusion{#preview-send}

Lorsque le contenu de la diffusion est prêt, vous pouvez le prévisualiser à l’aide de profils de test. Vous pouvez ensuite envoyer la diffusion pour générer le fichier d’extraction ou envoyer le message via l’API.

>[!BEGINTABS]

>[!TAB  Canal externe personnalisé ]

1. Dans le tableau de bord de la diffusion, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

1. Dans la page du contenu de diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** et sélectionnez les profils de test.

   ![Capture d’écran montrant l’option Simuler du contenu dans la page du contenu de la diffusion](assets/cus-simulate.png){zoomable="yes"}

>[!TAB Canal API personnalisé]

1. Dans le tableau de bord de la diffusion, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

1. Dans la page du contenu de diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** et sélectionnez les profils de test.

1. Sur le côté droit, cliquez sur **Ouvrir l’aperçu**. Cette fonctionnalité doit être configurée à l’aide de JSSP. Consultez cette [page](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html#api-additional-preview){target="_blank"}.

   ![Capture d’écran montrant l’option Simuler du contenu dans la page de contenu de diffusion pour l’API](assets/cus-simulate-api.png){zoomable="yes"}

>[!ENDTABS]

Dans le tableau de bord de la diffusion, cliquez sur **[!UICONTROL Vérifier et envoyer]** puis sur **[!UICONTROL Préparer]**. Ensuite, confirmez. Cliquez sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final, puis confirmez.

![Capture d’écran montrant l’option de préparation et le menu Logs](assets/cus-prepare.png){zoomable="yes"}

Pour plus d’informations sur la prévisualisation et l’envoi, reportez-vous à la [documentation](../call-center/create-call-center.md#preview-send) du centre d’appel.
