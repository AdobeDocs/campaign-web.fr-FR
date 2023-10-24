---
audience: end-user
title: Utiliser une activité de workflow de diffusion
description: Découvrez comment ajouter une activité de workflow de diffusion (e-mail, notification push ou SMS).
badge: label="Beta"
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 100%

---

# Activités e-mail, SMS, notification push {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur les canaux e-mail, SMS et de notification push. Vous pouvez combiner des activités de canal dans la zone de travail du workflow afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement de la clientèle et des données.

Vous pouvez par exemple créer une campagne par e-mail de bienvenue qui comprend une série de messages sur différents canaux, tels que les e-mails, les SMS et les notifications push. Vous pouvez également envoyer un e-mail de relance une fois qu’un client ou une cliente a effectué un achat, ou envoyer un message d’anniversaire personnalisé par SMS.

Grâce aux activités de canal, vous pouvez créer des campagnes personnalisées et complètes qui impliquent la clientèle sur plusieurs touchpoints et génèrent des conversions.

>[!NOTE]
>
>Vous pouvez également créer une diffusion ponctuelle, en dehors du contexte d’un workflow de campagne. En savoir plus dans ces sections :
>* [Créer une diffusion par e-mail autonome](../../email/create-email.md)
>* [Créer une diffusion par SMS autonome](../../sms/create-sms.md)
>* [Créer une diffusion par notification push autonome](../../push/create-push.md)

## Créer votre workflow{#build-your-workflow}

Commencez à créer votre workflow avec les activités pertinentes avant de placer la diffusion :

* Pour envoyer une diffusion récurrente, démarrez votre workflow avec une activité **Planificateur**. Pour envoyer une diffusion ponctuelle, vous pouvez définir la date de contact à l’aide d’une activité **Planificateur** ou définir le planning dans les paramètres de la diffusion. Consultez [cette section](scheduler.md).

* Ajoutez une activité **Créer une audience**. L’audience est la cible principale de votre diffusion : il s’agit des destinataires qui reçoivent les messages. Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience du message n’est pas définie dans l’activité de canal, mais dans l’activité **Créer une audience**. Consultez [cette section](build-audience.md).

  ![](../../msg/assets/add-delivery-in-wf.png)

## Configurer l’activité Canal {#create-a-delivery-in-a-workflow}


>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="Activité e-mail"
>abstract="Automatisez et exécutez des campagnes marketing sur les canaux e-mail, SMS et notification push. Vous pouvez combiner des activités de canal dans la zone de travail du workflow afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement de la clientèle et des données."


>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="Activité SMS"
>abstract="Automatisez et exécutez des campagnes marketing sur les canaux e-mail, SMS et notification push. Vous pouvez combiner des activités de canal dans la zone de travail du workflow afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement de la clientèle et des données."


>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Activité notification push iOS"
>abstract="Automatisez et exécutez des campagnes marketing sur les canaux e-mail, SMS et notification push. Vous pouvez combiner des activités de canal dans la zone de travail du workflow afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement de la clientèle et des données."


>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Activité notification push Android"
>abstract="Automatisez et exécutez des campagnes marketing sur les canaux e-mail, SMS et notification push. Vous pouvez combiner des activités de canal dans la zone de travail du workflow afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement de la clientèle et des données."

Pour configurer une diffusion dans le cadre d’un workflow, procédez comme suit :

1. Sélectionnez une activité canal : **[!UICONTROL E-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Notification push (Android)]** ou **[!UICONTROL Notification push (iOS)]**.

1. Sélectionnez le **Type de diffusion** : unique ou récurrent.

   * **Diffusion unique** : il s’agit d’une diffusion ponctuelle, envoyée une seule fois, par exemple un e-mail pour le Black Friday.
   * **Diffusion récurrente** : pour ce type de diffusion, vous définissez la fréquence d’exécution à l’aide d’une [activité Planificateur](scheduler.md). À chaque exécution du workflow, l’audience est recalculée et la diffusion est envoyée avec le contenu mis à jour. Il peut s’agir d’une newsletter hebdomadaire ou d’un e-mail d’anniversaire récurrent.

1. Choisissez un **modèle** de diffusion. Les modèles sont des paramètres de diffusion préconfigurés, spécifiques à un canal. Un modèle intégré est disponible pour chaque canal et prérempli par défaut. [En savoir plus](../../msg/delivery-template.md).

   ![](../assets/delivery-activity-in-wf.png)

   Vous pouvez sélectionner un autre modèle dans le volet de gauche de la configuration de l’activité de canal. Si l’audience précédemment sélectionnée n’est pas compatible avec le canal, vous ne pouvez pas sélectionner de modèle. Pour résoudre ce problème, modifiez l’activité **Créer une audience** et sélectionnez une audience ayant le mapping de ciblage approprié. En savoir plus sur les mappings de ciblage dans la [documentation d’Adobe Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr){target="_blank"}.

1. Cliquez sur **Créer une diffusion**. Définissez les paramètres et le contenu de votre message de la même manière que vous créez une diffusion autonome. Vous pouvez également planifier et simuler le contenu. [En savoir plus](../../msg/gs-messages.md).

1. Revenez à votre workflow. Pour continuer votre workflow, choisissez **Générer une transition sortante** afin d’ajouter une transition après l’activité canal.

1. Cliquez sur **Démarrer** pour lancer le workflow.

   Par défaut, le lancement d’un workflow déclenche l’étape de préparation du message, sans envoyer immédiatement le message.

1. Ouvrez l’activité de diffusion pour confirmer l’envoi à partir du bouton **Vérifier et envoyer**.

1. Dans le tableau de bord de la diffusion, cliquez sur **Envoyer**.

## Exemples {#cross-channel-workflow-sample}

Voici un exemple de workflow cross-canal avec une segmentation et deux diffusions. Le workflow cible la clientèle qui vit à Paris et qui s’intéresse aux machines à café. Parmi cette population, un e-mail est envoyé à la clientèle régulière, et un SMS est envoyé à la clientèle VIP.

![](../assets/workflow-channel-example.png)

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->

Vous pouvez également créer un workflow récurrent pour envoyer un SMS personnalisé chaque premier jour du mois à 20 heures à tous les clientes et clients habitant à Paris.

![](../assets/workflow-channel-example2.png)

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
