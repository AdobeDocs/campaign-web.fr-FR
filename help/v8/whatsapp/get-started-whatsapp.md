---
audience: end-user
title: Prise en main des messages WhatsApp
description: Découvrez comment créer et envoyer des messages WhatsApp avec l’interface utilisateur web d’Adobe Campaign
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 2%

---

# Prise en main des messages WhatsApp {#get-started-whatsapp}

Vous pouvez envoyer des messages WhatsApp à partir de l’interface utilisateur web d’**** à l’aide de Meta [API Cloud](https://developers.facebook.com/docs/whatsapp/cloud-api/). Utilisez WhatsApp dans des diffusions autonomes, dans des workflows de campagne ou dans des campagnes marketing, aux côtés de vos autres canaux.

* **[!UICONTROL Diffusions]** : dans l’interface utilisateur web d’Adobe Campaign, créez une diffusion WhatsApp autonome à partir du menu **[!UICONTROL Diffusions]** sur le rail de gauche, semblable à SMS ou à une notification push. [En savoir plus](create-whatsapp.md).

* **[!UICONTROL Campagnes]** : dans l’interface utilisateur web d’Adobe Campaign, ouvrez une campagne et ajoutez une diffusion WhatsApp à partir de l’onglet **[!UICONTROL Diffusions]** ou orchestrez des envois avec un workflow associé à la campagne. [En savoir plus](../campaigns/create-campaigns.md).

* **[!UICONTROL Workflows]** : dans la zone de travail des workflows de l’interface utilisateur web d’Adobe Campaign, ajoutez une activité de canal **[!UICONTROL WhatsApp]**, choisissez un modèle de diffusion, puis définissez le contenu et les paramètres dans le tableau de bord de la diffusion. En savoir plus sur les activités des canaux dans [cette section](../workflows/activities/channels.md).

## Conditions requises    {#prereq}

Intégrer WhatsApp nécessite ce qui suit :

* Compte Meta Business Manager
* [Compte professionnel WhatsApp avec nom d&#39;expéditeur et numéro de téléphone vérifiés](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [Jeton d’autorisation utilisateur avec les autorisations appropriées](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [ Modèles Meta approuvés ](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

Vous devez également tenir compte des points suivants avant de continuer :

* [ Règles de contenu WhatsApp ](https://www.whatsapp.com/legal/messaging-guidelines)
* [Conformité aux politiques de Meta](https://www.whatsapp.com/legal)
* Limites de conversation de [24 heures](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


