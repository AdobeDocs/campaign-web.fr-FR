---
audience: end-user
title: Prise en main des canaux externes personnalisés
description: Découvrez comment créer et envoyer des diffusions de canal externe personnalisées avec Adobe Campaign Web
source-git-commit: 7438ce1805cde00cf5b76f05d72bd19d2ef2343a
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 6%

---

# Prise en main des canaux externes personnalisés {#gs-custom-channel}

Vous pouvez, directement à partir de l’interface utilisateur web d’Adobe Campaign, orchestrer et exécuter des diffusions en fonction de canaux externes personnalisés intégrés à des tiers. La création du canal externe personnalisé est effectuée dans la console cliente.

Vous pouvez configurer des diffusions externes de canal personnalisé dans des workflows ou en tant que diffusions autonomes, définir votre audience et générer des fichiers d’exportation personnalisables avec toutes les données de contact et de personnalisation nécessaires.

>[!NOTE]
>
>Le reporting n’est pas disponible dans l’interface utilisateur web pour les diffusions externes de canal personnalisé. Vous devez accéder à la console cliente pour accéder aux rapports.

Les étapes ci-dessous décrivent la procédure à suivre pour une diffusion autonome (ponctuelle). La plupart des étapes sont similaires aux diffusions du centre d’appels. Pour plus d’informations, consultez cette [page](../call-center/create-call-center.md).

Pour créer et envoyer une nouvelle diffusion externe personnalisée autonome, procédez comme suit :

1. Créer le canal externe personnalisé, [en savoir plus](#create-channel)
1. Créer la diffusion, [en savoir plus](#create-delivery)
1. Définir l&#39;audience, [en savoir plus](#select-audience)
1. Modifier le contenu, [en savoir plus](#edit-content)
1. Prévisualiser et envoyer la diffusion, [en savoir plus](#preview-send)

## Créer le canal externe personnalisé{#create-channel}

Tout d’abord, vous devez configurer le canal externe personnalisé. Les étapes principales à effectuer dans la console cliente sont les suivantes :

1. Configurez le schéma pour ajouter le nouveau canal à la liste des canaux disponibles.
1. Créez un compte externe de routage.
1. Créez un nouveau modèle de diffusion associé au nouveau canal.

Pour plus d’informations, consultez la documentation de la [console cliente](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html)

## Créer une diffusion{#create-delivery}

Pour créer la diffusion et configurer ses propriétés, procédez comme suit :

1. Sélectionnez le menu **[!UICONTROL Diffusions]** et cliquez sur le bouton **[!UICONTROL Créer une diffusion]**.

1. Sélectionnez le canal externe personnalisé de votre choix, le modèle associé, puis cliquez sur **[!UICONTROL Créer une diffusion]** pour confirmer.

   ![Capture d’écran montrant la création d’une diffusion personnalisée](assets/cus-create.png){zoomable="yes"}


1. Sous **[!UICONTROL Propriétés]**, saisissez un **[!UICONTROL Libellé]** pour la diffusion.

   ![Capture d’écran affichant la configuration des propriétés d’une diffusion personnalisée](assets/cus-properties.png){zoomable="yes"}

Pour plus d&#39;informations sur la création de diffusion, consultez la documentation du centre d&#39;appels [&#128279;](../call-center/create-call-center.md#create-delivery).

## Définir l’audience{#select-audience}

Vous devez maintenant définir l’audience qui sera ciblée pour le fichier d’extraction.

1. Dans la section **[!UICONTROL Audience]** de la page de diffusion, cliquez sur **[!UICONTROL Sélectionner une audience]**.

1. Choisissez une audience existante ou créez la vôtre.

   ![Capture d’écran affichant la sélection de l’audience pour une diffusion personnalisée](assets/cc-audience2.png){zoomable="yes"}

Pour plus d’informations sur la définition de l’audience, consultez la [documentation](../call-center/create-call-center.md#select-audience) du centre d’appels.

## Modifier le contenu{#edit-content}

Maintenant, modifions le contenu du fichier d’extraction qui sera généré par la diffusion du canal personnalisé.

1. Dans la page de diffusion, cliquez sur le bouton **[!UICONTROL Modifier le contenu]**.

1. Spécifiez un **[!UICONTROL Nom de fichier]**, sélectionnez un **[!UICONTROL Format de fichier]** et ajoutez autant de colonnes que nécessaire pour votre fichier d’extraction.

   ![Capture d’écran affichant les options de configuration des attributs pour le fichier d’extraction.](assets/cc-content-attributes.png)

Pour plus d’informations sur l’édition de contenu, consultez la documentation du centre d’appels [&#128279;](../call-center/create-call-center.md#edit-content).

## Prévisualiser et envoyer la diffusion{#preview-send}

Lorsque le contenu de la diffusion est prêt, vous pouvez le prévisualiser à l’aide de profils de test et envoyer des BAT. Vous pouvez ensuite envoyer la diffusion pour générer le fichier d’extraction.

1. Sur la page du contenu de la diffusion, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** et sélectionnez les profils de test.

   ![Capture d’écran montrant l’option Simuler du contenu dans la page du contenu de la diffusion](assets/cus-simulate.png){zoomable="yes"}

1. Dans la page de diffusion, cliquez sur **[!UICONTROL Vérifier et envoyer]** puis sur **[!UICONTROL Préparer]**. Ensuite, confirmez.

   ![Capture d’écran montrant l’option de préparation et le menu Logs](assets/cus-prepare.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final, puis confirmez.

Pour plus d’informations sur la prévisualisation et l’envoi, reportez-vous à la documentation du centre d’appel [&#128279;](../call-center/create-call-center.md#preview-send).
