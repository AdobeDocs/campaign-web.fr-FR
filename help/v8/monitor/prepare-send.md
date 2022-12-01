---
audience: end-user
title: Préparer et envoyer un email
description: Documentation web de Campaign v8
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 33%

---

# Préparez et envoyez votre email {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Préparez et envoyez votre email"
>abstract="Découvrez comment préparer votre email et en savoir plus sur l’envoi d’indicateurs de performance clés."

>[!NOTE]
>
>Cette documentation est en cours de construction et fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Préparer l&#39;envoi

Pendant la préparation, la population cible est calculée et le contenu du message généré pour chaque profil inclus dans la cible est calculé. Une fois la préparation terminée, les messages sont prêts à être envoyés, soit immédiatement, soit à la date et à l&#39;heure planifiées. Les règles de validation utilisées pendant l’analyse sont décrites dans cette section [section](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. Cliquez sur le bouton **Préparer** situé dans le coin supérieur droit.

1. La progression de la préparation s&#39;affiche. La durée de cette opération varie en fonction de la taille de la population ciblée.

   >[!NOTE]
   >
   >Vous pouvez arrêter la préparation à tout moment à l’aide de la variable **Arrêter la préparation** bouton . Pendant la phase de préparation, aucun message n&#39;est envoyé. Vous pouvez donc lancer ou annuler cette opération sans aucun risque.

1. Une fois la préparation terminée, vérifiez le **Ciblés**, **A envoyer** et **Pour exclure** IPC. Si le nombre de messages à envoyer ne correspond pas à vos attentes, modifiez votre audience et relancez la préparation.

1. Cliquez sur le bouton **Journaux** et vérifiez qu’il n’y a pas d’erreur. Toutes les étapes de validation, les avertissements et les erreurs sont répertoriés. Les icônes colorées indiquent le type de message :

   * L’icône grise indique un message informatif.
   * L’icône jaune indique une erreur de traitement non critique.
   * L’icône rouge indique une erreur critique qui empêche l’envoi de la diffusion.

1. Après avoir apporté les modifications, redémarrez la préparation.

Une fois la préparation terminée, votre message est prêt à être envoyé. Pour plus d&#39;informations, consultez la section Confirmer l&#39;envoi.


## Envoi du message

Une fois la préparation terminée, procédez comme suit pour envoyer votre message.

1. Cliquez sur le bouton **Bouton Envoyer** dans le coin supérieur droit et confirmez.

1. La progression de l&#39;envoi s&#39;affiche avec trois KPI : Distribué, Ouvre, Clics.

1. Finalisez l’envoi en cliquant sur le bouton OK.

LOGS

>[!NOTE]
>
>Si le message est planifié, il sera envoyé à l’heure d’envoi. Pour plus d’informations sur la planification des messages, consultez cette section.

