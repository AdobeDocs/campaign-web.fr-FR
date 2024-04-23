---
audience: end-user
title: Consentement
description: En savoir plus sur le consentement dans Adobe Campaign Web
badge: label="Disponibilité limitée"
source-git-commit: 9a184d7558ca39be3afed4a7217a5e5687799c0d
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%

---

# Gestion du consentement {#manage-consent}

## Recommandations générales {#general-recommendations}

Adobe Campaign vous permet de collecter des données, y compris des informations personnelles et sensibles. Il est donc essentiel que vous obteniez et surveilliez le consentement de vos destinataires en conformité avec les réglementations de protection des données telles que le RGPD (Règlement général sur la protection des données) et d’autres lois sur la confidentialité applicables.

* Tout d&#39;abord, évitez d&#39;envoyer des emails, des notifications push et des SMS non sollicités (&quot;spam&quot;). Adobe croit fermement aux principes du consentement (permission marketing) pour fidéliser les clients et offrir une valeur ajoutée tout au long de leur vie et interdit donc strictement l’utilisation d’Adobe Campaign pour envoyer des messages non sollicités. [En savoir plus](#denylisted-profiles)

* Demandez toujours aux destinataires d&#39;accepter de recevoir des communications en leur offrant la possibilité de se désinscrire de vos diffusions<!-- and keep honoring opt-out requests as quickly as possible-->. [En savoir plus](#opt-out)

* Grâce au processus de gestion des abonnements, vous pouvez gérer les préférences de vos destinataires et déterminer quels destinataires ont choisi quel type d&#39;abonnement. [En savoir plus](../../delivery/using/about-services-and-subscriptions.md)

## Gérer le droit d’opposition {#opt-out}

Fournir aux destinataires la possibilité de se désabonner de la réception des communications d’une marque est une obligation légale, et s’assurer que ce choix est respecté. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**Pourquoi est-ce important ?**

* Le non-respect de ces réglementations entraîne des risques juridiques pour votre marque.
* Il permet d&#39;éviter d&#39;envoyer des communications non sollicitées à vos destinataires, ce qui pourrait les faire marquer vos messages comme du spam et nuire à votre réputation.

Lors de l&#39;envoi de diffusions à l&#39;aide du Web Adobe Campaign, vous devez toujours vous assurer que les clients peuvent se désabonner de futures communications. Une fois désabonnés, les profils sont automatiquement supprimés de l’audience des futurs messages marketing.

### Exclusion par e-mail {#email-opt-out}

Pour permettre aux destinataires de se désabonner de la réception des communications par e-mail, vous devez toujours inclure une **lien de désabonnement** dans chaque email envoyé aux destinataires.

Pour ce faire, suivez les étapes ci-après.

1. Créez une landing page externe et hébergez-la sur le système tiers de votre choix.

1. Créez une diffusion email. [Voici comment procéder](../email/create-email.md).

1. Insérez un lien vers le contenu de votre email. [Voici comment procéder](../email/message-tracking.md#insert-links).

   ![](../email/assets/message-tracking-insert-link.png)

1. Dans le **[!UICONTROL Url]** collez le lien vers votre page d’entrée tierce.

1. Cliquez sur l’icône **[!UICONTROL Liens]** dans le volet de gauche pour afficher la liste de toutes les URL du contenu à tracker.

1. Cliquez sur l’icône en forme de crayon en regard du nouveau lien pour l’éditer.

1. Modifiez la variable **[!UICONTROL Type de suivi]** et définissez-le sur **[!UICONTROL Exclusion]**.

   ![](../email/assets/message-tracking-edit-a-link.png)

1. Cliquez sur **[!UICONTROL Enregistrer]** et envoyez le message. [En savoir plus](../monitor/prepare-send.md)

1. Une fois le message reçu, si le destinataire clique sur le lien de désabonnement, votre landing page s&#39;affiche.

1. Lorsque le destinataire envoie le formulaire de landing page, les données de profil sont mises à jour. [En savoir plus](#denylisted-profiles)

<!--Any other option availabe such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Profils Placés sur la liste bloquée {#denylisted-profiles}

Après une désinscription (opt-out), les profils se trouvent sur la page **liste bloquée** pour un canal donné : cela signifie qu&#39;ils ne sont plus ciblés par aucune diffusion.

>[!NOTE]
>
>Si un profil de la liste bloquée pour le canal email comporte deux adresses email, les deux adresses seront exclues de la diffusion.

Vous pouvez vérifier si un profil se trouve en liste bloquée pour un ou plusieurs canaux dans la variable **[!UICONTROL Ne plus contacter]** section du profil **[!UICONTROL Détails]** . [En savoir plus](../audience/about-recipients.md#access)

![](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->



