---
audience: end-user
title: Préparer et envoyer un email
description: Documentation de l’application web de Campaign v8
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: 75d579975023639840f35f673e63aab2a2d3a811
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 18%

---

# Préparez et envoyez votre email {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Préparez et envoyez votre email"
>abstract="Découvrez comment préparer votre email et en savoir plus sur l’envoi d’indicateurs de performance clés."

>[!NOTE]
>
>Cette documentation est en cours d’élaboration et est fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Préparer l&#39;envoi{#prepare}

Lorsque vous avez défini votre contenu, votre audience et votre planning, vous êtes prêt à préparer votre message. Pendant la préparation, la population cible est calculée et le contenu du message généré pour chaque profil inclus dans la cible est calculé. Une fois la préparation terminée, les messages sont prêts à être envoyés, soit immédiatement, soit à la date et à l&#39;heure planifiées. Les règles de validation utilisées pendant l’analyse sont décrites dans cette section [section](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies).

Procédez comme suit :

1. Dans le tableau de bord de la diffusion, cliquez sur le bouton **Préparer** dans le coin supérieur droit et confirmez.

   ![](assets/prepare.png)

   La progression de la préparation s&#39;affiche. La durée de cette opération varie en fonction de la taille de la population ciblée.

   >[!NOTE]
   >
   >Vous pouvez arrêter la préparation à tout moment à l’aide de la variable **Arrêter la préparation** bouton . Pendant la phase de préparation, aucun message n&#39;est envoyé. Vous pouvez donc lancer ou annuler cette opération sans aucun risque.

1. Une fois la préparation terminée, vérifiez les KPI. Si le nombre de messages à envoyer ne correspond pas à vos attentes, modifiez votre audience et relancez la préparation.

   ![](assets/prepare2.png)

   Voici les différents indicateurs clés de performance affichés :

   * **Ciblés**: le nombre de destinataires ciblés
   * **A envoyer**: le nombre de messages qui seront envoyés ;
   * **Pour exclure**: le nombre de messages exclus par une règle de typologie

1. Cliquez sur le bouton **Journaux** et vérifiez qu’il n’y a pas d’erreur. Le dernier message de logs affiche les erreurs éventuelles et leur nombre. Voir à ce propos cette [section](#send).

   ![](assets/prepare-logs.png)

Si la préparation détecte une erreur critique qui empêche l&#39;envoi de la diffusion, l&#39;état de préparation apparaît comme ayant échoué dans le tableau de bord de la diffusion.

![](assets/prepare-error.png)

Si vous devez apporter des modifications à votre diffusion après la préparation, vous devez relancer la préparation pour que ces modifications soient prises en compte.

Une fois la préparation terminée sans erreur, votre message est prêt à être envoyé. Voir à ce propos cette [section](#send).

## Envoi du message{#send}

Une fois la préparation terminée, vous pouvez désormais envoyer votre message. Cette étape n’est nécessaire que pour les messages envoyés immédiatement. Si le message est planifié, il est envoyé à la date définie.

Procédez comme suit :

1. Dans le tableau de bord de la diffusion, cliquez sur le bouton **Envoyer** dans le coin supérieur droit et confirmez.

   ![](assets/send.png)

1. La progression de l&#39;envoi s&#39;affiche. Vérifiez les indicateurs de performance clés affichés. Vous pouvez également consulter les journaux. Voir à ce propos cette [section](#send).

   ![](assets/send2.png)

   Voici les différents indicateurs clés de performance affichés :

   * **Délivrés**: le nombre de messages envoyés avec succès. Le pourcentage est basé sur le nombre total de destinataires ciblés.
   * **Ouvertures**: le nombre de messages ouverts. Le pourcentage est basé sur le nombre de messages délivrés.
   * **Clics**: le nombre de destinataires ayant cliqué au moins une fois dans l&#39;email. Le pourcentage est basé sur le nombre de messages délivrés.

   >[!NOTE]
   >
   >Le **Ouvertures** et **Clics** Les indicateurs seront mis à jour en temps réel.

   Vous pouvez suspendre l’envoi à tout moment, puis reprendre. Si vous arrêtez la diffusion pendant son envoi, vous ne pourrez pas reprendre.
