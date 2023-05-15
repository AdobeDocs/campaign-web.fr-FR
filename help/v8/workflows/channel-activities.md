---
audience: end-user
title: Utiliser les activités des canaux de workflows
description: Découvrez comment utiliser les activités des canaux dans les workflows Web Adobe Campaign.
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: ht
source-wordcount: '219'
ht-degree: 100%

---

# Activités des canaux {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux, tels que les e-mails, les SMS ou les notifications push. Avec les workflows Adobe Campaign, vous pouvez combiner des activités de canal dans la zone de travail afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement du client ou de la cliente.

Vous pouvez par exemple créer une campagne par e-mail de bienvenue qui comprend une série de messages sur différents canaux, tels que les e-mails, les SMS et les notifications push. Vous pouvez également envoyer un e-mail de relance une fois qu’un client ou une cliente a effectué un achat, ou encore envoyer un message d’anniversaire personnalisé par SMS.

Grâce aux activités de canal, vous pouvez créer des campagnes personnalisées et complètes qui impliquent des clients et clientes sur plusieurs points de contact et génèrent des conversions.

Les activités de canal sont disponibles à partir de la palette, dans la partie gauche de l’écran, dans la section Canaux.

## E-mail {#email}

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