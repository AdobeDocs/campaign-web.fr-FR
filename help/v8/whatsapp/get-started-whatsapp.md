---
audience: end-user
title: Commencer avec les messages WhatsApp
description: Découvrez comment créer et envoyer des messages WhatsApp à l’aide de l’interface d’utilisation d’Adobe Campaign Web.
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 100%
---
# Commencer avec les messages WhatsApp {#get-started-whatsapp}

Vous pouvez envoyer des messages WhatsApp à partir de l’**interface d’utilisation d’Adobe Campaign Web** à l’aide de l’[API Cloud](https://developers.facebook.com/docs/whatsapp/cloud-api/) de Meta. Utilisez WhatsApp dans des diffusions autonomes, dans des workflows de campagne ou dans des campagnes marketing, aux côtés de vos autres canaux.

* **[!UICONTROL Diffusions]** : dans l’interface d’utilisation d’Adobe Campaign Web, créez une diffusion WhatsApp autonome à partir du menu **[!UICONTROL Diffusions]** situé sur le rail de gauche, semblable à un SMS ou à une notification push. [En savoir plus](create-whatsapp.md).

* **[!UICONTROL Campagnes]** : dans l’interface d’utilisation d’Adobe Campaign Web, ouvrez une campagne et ajoutez une diffusion WhatsApp à partir de l’onglet **[!UICONTROL Diffusions]** ou orchestrez des envois avec un workflow associé à la campagne. [En savoir plus](../campaigns/create-campaigns.md).

* **[!UICONTROL Workflows]** : dans la zone de travail des workflows de l’interface d’utilisation d’Adobe Campaign Web, ajoutez une activité de canal **[!UICONTROL WhatsApp]**, choisissez un modèle de diffusion, puis définissez le contenu et les paramètres dans le tableau de bord de la diffusion. En savoir plus sur les activités de canal dans [cette page](../workflows/activities/channels.md).

## Conditions requises {#prereq}

Pour intégrer WhatsApp, vous devez disposer des éléments suivants :

* Compte Meta Business Manager
* [Compte WhatsApp Business avec nom d&#39;expéditeur ou d’expéditrice et numéro de téléphone vérifiés](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [Jeton d’autorisation de l’utilisateur ou de l’utilisatrice avec les autorisations appropriées](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Modèles Meta approuvés](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

Vous devez également tenir compte des points suivants avant de continuer :

* [Règles de contenu WhatsApp](https://www.whatsapp.com/legal/messaging-guidelines)
* [Conformité aux politiques de Meta](https://www.whatsapp.com/legal)
* [Limites de conversation sur 24 heures](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


