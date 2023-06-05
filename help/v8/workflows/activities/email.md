---
audience: end-user
title: Utilisation de l’activité de workflow de courrier électronique
description: Découvrez comment utiliser l’activité de workflow de courrier électronique
badge: label="Alpha" type="Positive"
source-git-commit: fc920737aa336bbb92b2d2ef03f997ca2eefa0bb
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 31%

---


# Email, SMS, Push {#email}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux, tels que les emails, les SMS ou les notifications push. Vous pouvez combiner des activités de canal dans la zone de travail afin de créer des processus cross-canal pouvant déclencher des actions en fonction du comportement du client.

Vous pouvez par exemple créer une campagne par e-mail de bienvenue qui comprend une série de messages sur différents canaux, tels que les e-mails, les SMS et les notifications push. Vous pouvez également envoyer un e-mail de relance une fois qu’un client ou une cliente a effectué un achat, ou encore envoyer un message d’anniversaire personnalisé par SMS.

Grâce aux activités de canal, vous pouvez créer des campagnes personnalisées et complètes qui impliquent des clients sur plusieurs points de contact et génèrent des conversions.

Voici les étapes à suivre pour ajouter une **Canal** activité dans un workflow :

1. Assurez-vous d’avoir ajouté une **Créer une audience** activité. L&#39;audience est la cible principale de votre diffusion : les destinataires qui reçoivent les messages. Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience du message n’est pas définie dans l’activité de canal, mais dans la variable **Créer une audience** activité. Consultez [cette section](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Sélectionnez une activité de diffusion : **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Notification push (Android)]** ou **[!UICONTROL Notification push (iOS)]**.

1. Démarrez le workflow et vérifiez les logs.






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

When linked to a scheduler, you can define recurring emails.-->

Les destinataires des e-mails sont définis en amont de l’activité dans le même workflow, via une activité de ciblage d’audience.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
