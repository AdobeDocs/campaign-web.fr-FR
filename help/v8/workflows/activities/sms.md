---
audience: end-user
title: Utiliser l’activité de workflow SMS
description: Découvrez comment utiliser l’activité de workflow SMS.
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 100%

---


# SMS {#sms}

L’activité **SMS** permet d’envoyer des messages SMS au sein d’un workflow. Les SMS sont alors envoyés automatiquement à une cible spécifique déterminée dans le même workflow.

Définissez les destinataires du SMS avant l’activité de diffusion SMS dans le workflow, à l’aide de l’activité Créer une audience. En savoir plus.

1. Une fosi que vous avez créé et configuré un workflow, ajoutez une activité Créer une audience pour sélectionner une audience existante ou utilisez le créateur de règles pour définir votre propre requête.

1. Ajoutez une activité de canal SMS à votre workflow.

   ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. Sélectionnez votre activité. Dans le menu de la diffusion, sélectionnez les modèles à utiliser pour la diffusion. En savoir plus sur les modèles

1. Cliquez sur Créer une diffusion pour configurer votre diffusion SMS. Pour plus d’informations sur les diffusions SMS, consultez cette page.

1. Une fois que votre diffusion est prête à être envoyée, revenez à votre workflow et cliquez sur Démarrer pour lancer votre workflow.

1. Par défaut, le lancement d’un workflow de diffusion déclenche l’étape de préparation du message, sans envoyer immédiatement le message.

   Cliquez sur Réviser et envoyer dans le menu avancé de votre activité SMS pour confirmer l’envoi.

1. Dans le tableau de bord de la diffusion SMS, cliquez sur Envoyer.
