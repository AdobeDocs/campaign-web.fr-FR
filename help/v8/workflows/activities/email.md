---
audience: end-user
title: Utilisation de l’activité de workflow de courrier électronique
description: Découvrez comment utiliser l’activité de workflow de courrier électronique
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 22%

---


# Email, SMS, Push {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux, tels que les emails, les SMS ou les notifications push. Vous pouvez combiner des activités de canal dans la zone de travail afin de créer des processus cross-canal pouvant déclencher des actions en fonction du comportement du client.

Vous pouvez par exemple créer une campagne par e-mail de bienvenue qui comprend une série de messages sur différents canaux, tels que les e-mails, les SMS et les notifications push. Vous pouvez également envoyer un e-mail de relance une fois qu’un client ou une cliente a effectué un achat, ou encore envoyer un message d’anniversaire personnalisé par SMS.

Grâce aux activités de canal, vous pouvez créer des campagnes personnalisées et complètes qui impliquent des clients sur plusieurs points de contact et génèrent des conversions.

Voici les étapes à suivre pour ajouter une **Canal** activité dans un workflow :

1. Assurez-vous d’avoir ajouté une **Créer une audience** activité. L&#39;audience est la cible principale de votre diffusion : les destinataires qui reçoivent les messages. Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience du message n’est pas définie dans l’activité de canal, mais dans la variable **Créer une audience** activité. Consultez [cette section](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Sélectionnez une activité de diffusion : **[!UICONTROL e-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL notification push (Android)]** ou **[!UICONTROL notification push (iOS)]**.

1. Sélectionnez une **Modèle**. Les modèles sont des paramètres de diffusion préconfigurés enregistrés en vue d’une utilisation ultérieure. [En savoir plus](../../msg/delivery-template.md)

1. Cliquez sur **Créer une diffusion** et définir votre message de la même manière que vous créez une diffusion autonome. C&#39;est également à cet endroit que vous définissez les paramètres de diffusion, planifiez et simulez le contenu. [En savoir plus](../../msg/gs-messages.md)

1. Revenez à votre workflow et cliquez sur **Début** pour lancer votre workflow.

   Par défaut, le lancement d’un workflow de diffusion déclenche l’étape de préparation du message, sans envoyer immédiatement le message.

1. Cliquez sur **Réviser et envoyer** de l’activité de canal pour confirmer l’envoi.

1. Dans le tableau de bord de la diffusion, cliquez sur **Envoyer**.

## Exemple

Voici un exemple de workflow cross-canal avec une segmentation et deux diffusions. Le workflow cible tous les clients qui vivent à Paris et qui s&#39;intéressent aux machines à café. Parmi cette population, un email est envoyé aux clients réguliers et un SMS est envoyé aux clients VIP.

![](../assets/workflow-channel-example.png)
<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
