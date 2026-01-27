---
audience: end-user
title: Créer des e-mails multilingues avec Adobe Experience Manager
description: Découvrez comment créer des diffusions par e-mail multilingues à l’aide de copies de langue Adobe Experience Manager dans Campaign Web.
feature: Email
topic: Content Management
role: User
level: Intermediate
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 2%

---


# Créer des e-mails multilingues avec Adobe Experience Manager {#aem-multilingual}

L’intégration de Adobe Experience Manager vous permet de créer des diffusions e-mail multilingues à l’aide de copies de langue Adobe Experience Manager. Vous pouvez ainsi gérer des variantes de contenu dans différentes langues et diffuser des e-mails personnalisés en fonction des préférences linguistiques des destinataires.

## Conditions préalables {#prerequisites}

Avant de créer une diffusion e-mail multilingue, vérifiez que vous disposez des éléments suivants :

* Accès à une instance Adobe Experience Manager configurée pour l&#39;intégration de l&#39;interface Web d&#39;Adobe Campaign.
* Un contenu Adobe Experience Manager avec des copies de langue a déjà été créé et approuvé. En savoir plus sur l&#39;Assistant Copie de la langue dans la documentation de [Adobe Experience Manager](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Modèle de diffusion d’e-mail configuré pour recevoir du contenu Adobe Experience Manager. Reportez-vous aux étapes détaillées dans la section [Activation du mode multilingue](#enable-multilingual).

## Création de votre diffusion multilingue

Pour créer une diffusion e-mail multilingue, vous devez d&#39;abord activer l&#39;option multilingue dans vos paramètres de diffusion. Le système détecte automatiquement les copies de langue disponibles et vous permet de choisir celles à ajouter.

### Activer le mode multilingue {#enable-multilingual}

Créez une nouvelle diffusion et activez l&#39;option multilingue dans les paramètres avancés.

1. Dans le menu **[!UICONTROL Diffusions]**, cliquez sur **[!UICONTROL Créer une diffusion]**.

   ![](assets/lg-copy-1.png)

1. Sélectionnez le modèle **[!UICONTROL Diffusion e-mail avec contenu AEM]** et cliquez sur **[!UICONTROL Créer une diffusion]**.

   ![](assets/lg-copy-2.png)

1. Saisissez un libellé pour la diffusion et configurez votre audience. [En savoir plus](../email/create-email.md)

1. Accédez à votre diffusion **[!UICONTROL Paramètres]**, puis à la section **[!UICONTROL Avancé]**.

1. Activez l’option **[!UICONTROL Activer le multilingue AEM]**.

   ![](assets/lg-copy-3.png)

1. Assurez-vous que :

   * Le **[!UICONTROL mode d’édition du contenu]** est défini sur **[!UICONTROL AEM]**.
   * Le Adobe Experience Manager correct **[!UICONTROL Compte externe]** est sélectionné.

1. Cliquez sur **[!UICONTROL Enregistrer et fermer]**.

### Créer des variantes de contenu {#create-variants}

Sélectionnez votre contenu Adobe Experience Manager et choisissez les variantes linguistiques à inclure dans la diffusion.

1. Cliquez sur **[!UICONTROL Modifier le contenu]**.

1. Sélectionnez **[!UICONTROL Créer une variante de contenu]**.

   ![](assets/lg-copy-4.png)

1. Sélectionnez votre contenu Adobe Experience Manager dans la liste.

   ![](assets/lg-copy-5.png)

1. Le système détecte toutes les copies de langue associées au contenu sélectionné (relation parent-enfant). Par exemple, si votre contenu Adobe Experience Manager comporte des variantes en français, en allemand et en italien, toutes les variantes sont disponibles pour la sélection.

   Sélectionnez les variantes linguistiques à inclure dans la diffusion.

   ![](assets/lg-copy-6.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

1. Vérifiez vos variantes de langue dans l’éditeur de contenu. Vous pouvez désormais [gérer chaque variante individuellement](#manage-variants) ou poursuivre [l’envoi de la diffusion](../monitor/prepare-send.md).

   ![](assets/lg-copy-7.png)

## Gérer les variantes linguistiques {#manage-variants}

Après avoir créé des variantes de contenu, vous pouvez les gérer directement dans la diffusion :

1. Pour définir une langue par défaut, accédez au menu avancé de la variante choisie et sélectionnez **[!UICONTROL Définir comme langue par défaut]**. La langue par défaut est utilisée lorsque la préférence linguistique d’un profil n’est pas définie ou ne correspond à aucune variante disponible.

   Cliquez sur **[!UICONTROL Supprimer]** pour supprimer toute variante de votre diffusion.

   ![](assets/lg-copy-8.png)

1. Dans le menu avancé Variantes de contenu , cliquez sur **[!UICONTROL Gérer les paramètres régionaux]** pour ajouter d’autres paramètres régionaux à votre diffusion.

   ![](assets/lg-copy-9.png)

1. Sélectionnez d’autres copies de langue pour inclure d’autres variantes et cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/lg-copy-11.png)

1. Si le contenu est mis à jour dans Adobe Experience Manager, cliquez sur **[!UICONTROL Actualiser le contenu AEM]** pour synchroniser toutes les variantes avec la dernière version.

   ![](assets/lg-copy-10.png)

1. Cliquez sur **[!UICONTROL Dissocier le contenu AEM]** si vous souhaitez modifier le contenu directement dans Campaign ou rompre le lien avec Adobe Experience Manager.

   >[!CAUTION]
   >
   >Après la dissociation, vous ne pouvez pas actualiser le contenu de Adobe Experience Manager ni créer de variantes. Le contenu devient indépendant de Adobe Experience Manager.


