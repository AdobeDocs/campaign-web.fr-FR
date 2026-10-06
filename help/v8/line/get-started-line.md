---
audience: end-user
title: Prise en main des messages LINE
description: Découvrez comment créer et envoyer des messages LINE avec l'interface utilisateur web d'Adobe Campaign
feature: Line App
topic: Content Management
role: User
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
subfeature_v2:
  - id: d9d413df-4e9e-4906-bbbc-28c06c2ccf59
    internal-label: LINE App
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 22%
---
# Prise en main des messages LINE {#get-started-line}

LINE est une application gratuite de messagerie instantanée, d’appels vocaux et vidéo, disponible sur tous les appareils mobiles et sur PC. Vous pouvez utiliser Adobe Campaign pour envoyer des messages LINE. Utilisez LINE dans des diffusions autonomes ou dans des workflows, aux côtés de vos autres canaux.

![Exemple de message LINE reçu sur un appareil mobile](assets/line-message.png)

* **[!UICONTROL Diffusions]** : créez une diffusion LINE autonome à partir du menu **[!UICONTROL Diffusions]** sur le rail de gauche, comme pour les SMS ou les notifications push. [En savoir plus](send-line.md).

* **[!UICONTROL Workflows]** : dans la zone de travail des workflows, ajoutez une activité de canal **[!UICONTROL LINE]**, choisissez un modèle de diffusion, puis définissez le contenu et les paramètres dans le tableau de bord de la diffusion. En savoir plus sur les activités de canal dans [cette page](../workflows/activities/channels.md).

  >[!NOTE]
  >
  >Dans l’activité **[!UICONTROL Créer une audience]** qui alimente votre activité de canal **[!UICONTROL LINE]**, modifiez la dimension de ciblage en **[!UICONTROL Abonnements des visiteurs]**. Veillez à activer l’option **[!UICONTROL Afficher tous les schémas]** dans le panneau latéral. Le sélecteur de modèles de diffusion n’est disponible qu’une fois cette dimension de ciblage définie.
