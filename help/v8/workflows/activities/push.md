---
audience: end-user
title: Utilisation de l'activité de workflow Notification push
description: Découvrez comment utiliser l'activité de workflow Notification push
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 4%

---


# Push notification {#push-activity}

Le **Notification push** l&#39;activité de diffusion permet de paramétrer l&#39;envoi d&#39;une notification push dans un workflow.

>[!BEGINTABS]

>[!TAB Notification push (Android)]

1. Après avoir créé et configuré un nouveau workflow, ajoutez une activité Créer une audience pour sélectionner une audience existante ou utilisez le créateur de règles pour définir votre propre requête.

1. Ajoutez une activité de canal Notification push (Android) à votre workflow.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Sélectionnez votre activité. Dans le menu de la diffusion, sélectionnez les Modèles à utiliser pour cette diffusion. En savoir plus sur les modèles

1. Cliquez sur Créer une diffusion pour configurer votre diffusion de notification push. Pour plus d&#39;informations sur la diffusion Notification push (Android), consultez cette page.

1. Une fois que votre diffusion est prête à être envoyée, revenez à votre workflow et cliquez sur Démarrer pour lancer votre workflow.

1. Par défaut, le lancement d’un workflow de diffusion déclenche l’étape de préparation du message, sans envoyer immédiatement le message.

   Cliquez sur Réviser et envoyer dans le menu avancé de votre activité de canal Notification push (Android) pour confirmer l’envoi.

1. Dans le tableau de bord de la diffusion Notification push, cliquez sur Envoyer.

>[!TAB Notification push (iOS)]

1. Après avoir créé et configuré un nouveau workflow, ajoutez une activité Créer une audience pour sélectionner une audience existante ou utilisez le créateur de règles pour définir votre propre requête.

1. Ajoutez une activité de canal Notification push (iOS) à votre workflow.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Sélectionnez votre activité. Dans le menu de la diffusion, sélectionnez les Modèles à utiliser pour cette diffusion. En savoir plus sur les modèles

1. Cliquez sur Créer une diffusion pour configurer votre diffusion de notification push. Pour plus d&#39;informations sur la diffusion Notification push (iOS), consultez cette page.

1. Une fois que votre diffusion est prête à être envoyée, revenez à votre workflow et cliquez sur Démarrer pour lancer votre workflow.

1. Par défaut, le lancement d’un workflow de diffusion déclenche l’étape de préparation du message, sans envoyer immédiatement le message.

   Cliquez sur Réviser et envoyer dans le menu avancé de votre activité de canal Notification push (iOS) pour confirmer l’envoi.

1. Dans le tableau de bord de la diffusion Notification push, cliquez sur Envoyer.

>[!ENDTABS]