---
audience: end-user
title: Utilisation d’une activité de workflow de diffusion
description: Découvrez comment ajouter une activité de workflow de diffusion (email, push, SMS)
badge: label="Alpha"
source-git-commit: d70c671e558613a27acc5252091e1e2836b675c7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 12%

---


# Email, SMS, Push {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur les canaux email, SMS et push. Vous pouvez combiner des activités de canal dans le canevas de workflow pour créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement et des données des clients.

Vous pouvez par exemple créer une campagne par e-mail de bienvenue qui comprend une série de messages sur différents canaux, tels que les e-mails, les SMS et les notifications push. Vous pouvez également envoyer un email de relance une fois qu’un client a effectué un achat, ou envoyer un message d’anniversaire personnalisé à un client par SMS.

Grâce aux activités de canal, vous pouvez créer des campagnes personnalisées et complètes qui impliquent des clients sur plusieurs points de contact et génèrent des conversions.

Voici les étapes à suivre pour ajouter une **Canal** activité dans un workflow :

1. Assurez-vous d’avoir ajouté une **Créer une audience** activité. L&#39;audience est la cible principale de votre diffusion : les destinataires qui reçoivent les messages. Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience du message n’est pas définie dans l’activité de canal, mais dans la variable **Créer une audience** activité. Consultez [cette section](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Sélectionnez une activité de diffusion : **[!UICONTROL e-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL notification push (Android)]** ou **[!UICONTROL notification push (iOS)]**.

1. Sélectionner une diffusion **Modèle**. Les modèles sont des paramètres de diffusion préconfigurés, spécifiques à un canal. Un modèle intégré est disponible pour chaque canal et prérempli par défaut. [En savoir plus](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)


   Vous pouvez sélectionner un autre modèle dans le volet de gauche de la configuration de l’activité des canaux. Si l’audience précédemment sélectionnée n’est pas compatible avec le canal, vous ne pouvez pas sélectionner de modèle. Pour résoudre ce problème, mettez à jour la variable **Créer une audience** pour sélectionner une audience avec le mapping de ciblage approprié. En savoir plus sur les mappings de ciblage dans [Documentation d’Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr){target="_blank"}.

1. Cliquez sur **Créer une diffusion**. Définissez les paramètres et le contenu de votre message de la même manière que vous créez une diffusion autonome. Vous pouvez également planifier et simuler le contenu. [En savoir plus](../../msg/gs-messages.md).

1. Revenez à votre workflow et enregistrez vos modifications.

1. Cliquez sur **Début** pour lancer votre workflow.

   Par défaut, le démarrage d’un workflow déclenche l’étape de préparation du message, sans envoyer immédiatement le message.

1. Ouvrez votre activité de diffusion pour confirmer l’envoi à partir de la **Réviser et envoyer** bouton .

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
