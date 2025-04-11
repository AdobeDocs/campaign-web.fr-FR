---
audience: end-user
title: Consentement
description: En savoir plus sur le consentement dans Adobe Campaign Web
badge: label="Disponibilité limitée"
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 38%

---

# Gérer le consentement {#manage-consent}

## Recommandations générales {#general-recommendations}

Adobe Campaign vous permet de collecter des données, y compris des informations personnelles et sensibles. Il est essentiel d’obtenir et de surveiller le consentement des destinataires en conformité avec les réglementations de protection des données telles que le RGPD (Règlement général sur la protection des données) et d’autres lois applicables en matière de confidentialité.

* Tout d’abord, évitez d’envoyer des e-mails, des notifications push et des SMS non sollicités (« spam »). Adobe soutient fermement les principes du consentement (autorisation marketing) pour fidéliser le client et offrir une valeur ajoutée tout au long de sa durée de vie. Adobe interdit strictement l&#39;utilisation d&#39;Adobe Campaign pour l&#39;envoi de messages non sollicités. [En savoir plus](#denylisted-profiles)

* Assurez-vous toujours que les destinataires acceptent de recevoir des communications en leur offrant la possibilité de se désinscrire de vos diffusions<!-- and keep honoring opt-out requests as quickly as possible-->. [En savoir plus](#opt-out)

* Utilisez le processus de gestion des abonnements pour gérer les préférences des destinataires et suivre les destinataires qui se sont inscrits à des types d’abonnements spécifiques. [En savoir plus](../../delivery/using/about-services-and-subscriptions.md)

## Gérer l’opt-out {#opt-out}

La possibilité pour les destinataires de se désabonner de la réception des communications d’une marque est une exigence légale. Il est également nécessaire de s’assurer que ce choix est respecté. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**Pourquoi est-ce important ?**

* Le non-respect de ces réglementations entraîne des risques juridiques pour votre marque.
* Cela permet d’éviter d’envoyer des communications non sollicitées aux destinataires, ce qui pourrait les amener à marquer vos messages comme spam et nuire à votre réputation.

Lors de l’envoi de diffusions à l’aide d’Adobe Campaign Web, assurez-vous que les clients peuvent se désabonner des communications futures. Une fois désabonnés, les profils sont automatiquement supprimés de l’audience des futurs messages marketing.

### Opt-out des e-mails {#email-opt-out}

Pour permettre aux destinataires de se désabonner des communications par e-mail, incluez un **lien de désabonnement** dans chaque e-mail envoyé aux destinataires.

Procédez comme suit :

1. Créez une page de destination externe et hébergez-la sur le système tiers de votre choix.

1. Créez une diffusion par e-mail. [Voici comment procéder](../email/create-email.md)

1. Insérez un lien dans le contenu de votre e-mail. [Voici comment procéder](../email/message-tracking.md#insert-links)

   ![Insérer un lien dans le contenu de l’e-mail](../email/assets/message-tracking-insert-link.png)

1. Dans le champ **[!UICONTROL URL]**, collez le lien vers votre page de destination tierce.

1. Cliquez sur l’icône **[!UICONTROL Liens]** dans le volet de gauche pour afficher la liste de toutes les URL du contenu à tracker.

1. Cliquez sur l’icône en forme de crayon en regard du nouveau lien pour le modifier.

1. Modifiez le **[!UICONTROL Type de tracking]** et définissez-le sur **[!UICONTROL Opt-out]**.

   ![Modifier le type de tracking pour le processus d’opt-out](../email/assets/message-tracking-edit-a-link.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**, puis envoyez le message. [En savoir plus](../monitor/prepare-send.md)

1. Une fois le message reçu, si la personne destinataire clique sur le lien de désinscription, votre page de destination s’affiche.

1. Lorsque la personne destinataire envoie le formulaire de la page de destination, les données de profil sont mises à jour. [En savoir plus](#denylisted-profiles)

<!--Any other option available such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Profils placés sur la liste bloquée {#denylisted-profiles}

Placer sur la liste bloquée Après une désinscription (opt-out), les profils sont ajoutés à la **** pour un canal donné. Cela signifie qu’elles ne sont plus ciblées par aucune diffusion.

>[!NOTE]
>
>Si un profil sur la liste bloquée pour le canal e-mail comporte deux adresses e-mail, les deux adresses sont exclues de la diffusion.

Vous pouvez vérifier si un profil est sur liste bloquée pour un ou plusieurs canaux dans la section **[!UICONTROL Ne plus contacter]** de l’onglet **[!UICONTROL Détails]** du profil. [En savoir plus](../audience/about-recipients.md#access)

![Vérifier le statut de la liste bloquée dans les détails du profil](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->