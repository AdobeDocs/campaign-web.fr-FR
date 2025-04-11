---
audience: end-user
title: Envoyer une diffusion par SMS
description: Découvrez comment envoyer des SMS à l’aide d’Adobe Campaign Web.
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 36%

---

# Prévisualiser et envoyer une diffusion par SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nouvelle mesure de quarantaines"
>abstract="Nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (utilisateur ou utilisatrice inconnu(e), domaine non valide) par rapport au nombre de messages à diffuser."

## Prévisualiser votre diffusion par SMS {#preview-sms}

Une fois que vous avez défini le contenu de votre message, utilisez des profils de test pour le prévisualiser et le tester. Si du contenu personnalisé est inclus, examinez comment ce contenu apparaît dans le message à l’aide des données de profil de test. Cela permet de s’assurer que le message s’affiche comme prévu et que les informations personnalisées sont correctement présentées.

La diffusion par SMS comprend les étapes suivantes. Pour plus d’informations sur la prévisualisation des diffusions, consultez [cette section](../preview-test/preview-content.md).

1. Sur la page de contenu de la diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** pour prévisualiser le contenu que vous avez personnalisé.

   ![Prévisualisation de contenu SMS personnalisé](assets/sms_send_1.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Ajouter un ou plusieurs profils de test]** pour sélectionner un ou plusieurs profils de test.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. Dans le volet de droite, affichez un aperçu de la diffusion par SMS, où les éléments personnalisés sont remplacés dynamiquement par les données du profil sélectionné.

   ![Volet d&#39;aperçu affichant la diffusion SMS personnalisée](assets/sms_send_3.png){zoomable="yes"}

Vérifiez et envoyez votre SMS à votre audience.

## Tester votre diffusion par SMS {#test-sms}

Avec **Adobe Campaign**, testez un message avant de l’envoyer à l’audience principale. Cette étape valide votre campagne par e-mail et identifie les problèmes potentiels.

L’envoi de BAT est essentiel pour garantir la qualité et l’efficacité de votre diffusion. Les destinataires du BAT examinent divers éléments tels que des liens, des liens d’opt-out et des images et identifient les erreurs de rendu, de contenu, de paramètres de personnalisation et de configuration des SMS. Ce processus évalue et optimise minutieusement votre SMS avant d’atteindre votre audience principale.

![Icône de livre pour l’envoi de BAT](../assets/do-not-localize/book.png) Découvrez comment envoyer des BAT dans [cette section](../preview-test/test-deliveries.md).

![Test de la diffusion des SMS](assets/sms_send_6.png){zoomable="yes"}

## Envoyer votre diffusion par SMS {#send-sms}

1. Après avoir personnalisé le contenu de votre SMS, cliquez sur **[!UICONTROL Vérifier et envoyer]** sur votre page **[!UICONTROL Diffusion]**.

   ![Vérifier et envoyer la diffusion par SMS](assets/sms_send_4.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Préparer]** et suivez la progression et les statistiques fournies.

   En cas d’erreur, reportez-vous au menu Journaux pour obtenir des informations détaillées sur l’échec.

1. Envoyez les messages en cliquant sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final.

   ![Envoi d&#39;une diffusion SMS](assets/sms_send_5.png){zoomable="yes"}

   Si la diffusion SMS est planifiée, cliquez sur le bouton **[!UICONTROL Envoyer comme prévu]**. Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#schedule-the-delivery-sending).

1. Confirmez l’action d’envoi en cliquant sur le bouton **[!UICONTROL Envoyer]**.

Une fois votre diffusion envoyée, suivez les données de vos KPI (indicateurs clés de performance) à partir de votre page de diffusion et les données à partir du menu **[!UICONTROL Journaux]**.

Commencez à mesurer l’impact de votre message à l’aide de rapports intégrés. [En savoir plus](../reporting/sms-report.md)