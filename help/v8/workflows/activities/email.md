---
audience: end-user
title: Utilisation de l’activité de workflow de courrier électronique
description: Découvrez comment utiliser l’activité de workflow de courrier électronique
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 84%

---


# E-mail {#email}

description, les cas d’utilisation possibles (autres activités courantes que vous pouvez lier avant ou après l’activité)

comment ajouter et configurer l’activité

exemple d’activité configurée dans un workflow


L’activité Diffusion E-mail permet de paramétrer l’envoi d’un e-mail dans un workflow.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Les destinataires des e-mails sont définis en amont de l’activité dans le même workflow, via une activité de ciblage d’audience.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
