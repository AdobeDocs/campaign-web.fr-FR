---
audience: end-user
title: Envoyer une diffusion par SMS
description: Découvrez comment envoyer des SMS à l’aide d’Adobe Campaign Web.
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 88%

---

# Prévisualiser et envoyer une diffusion par SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nouvelle mesure de quarantaines"
>abstract="Nombre total d’adresses mises en quarantaine à la suite d’un échec de diffusion (utilisateur ou utilisatrice inconnu(e), domaine non valide) par rapport au nombre de messages à diffuser."

## Prévisualiser votre diffusion par SMS{#preview-sms}

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des profils de test pour le prévisualiser et le tester. Si vous avez inséré du contenu personnalisé, vous pouvez vérifier son affichage dans le message à l’aide des données de profil de test. Vous pouvez ainsi vous assurer que le message s’affiche comme prévu et que toute information personnalisée est correctement présentée.

La diffusion par SMS comprend les étapes suivantes. Pour plus d’informations sur la prévisualisation des diffusions, consultez [cette section](../preview-test/preview-content.md).

1. Sur la page de contenu de la diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** pour prévisualiser le contenu que vous avez personnalisé.

   ![](assets/sms_send_1.png){zoomable=&quot;yes&quot;}

1. Cliquez sur **[!UICONTROL Ajouter un ou plusieurs profils de test]** pour sélectionner un ou plusieurs profils de test.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. Dans le volet de droite, vous trouverez un aperçu de la diffusion par SMS, où les éléments personnalisés sont remplacés dynamiquement par les données du profil sélectionné.

   ![](assets/sms_send_3.png){zoomable=&quot;yes&quot;}

Vous pouvez maintenant vérifier et envoyer votre SMS à votre audience.

## Tester votre diffusion par SMS {#test-sms}

Avec **Adobe Campaign**, vous avez la possibilité de tester un message avant de l’envoyer à l’audience principale, ce qui est une étape essentielle pour valider votre campagne par e-mail et identifier les problèmes potentiels.

L’envoi de BAT est une étape importante pour assurer la qualité et l’efficacité de votre diffusion. Les destinataires du BAT peuvent consulter divers éléments tels que des liens, des liens et des images d&#39;opt-out, mais aussi identifier les erreurs de rendu, de contenu, de paramètres de personnalisation et de configuration des SMS. Ce processus vous aide à évaluer et à optimiser minutieusement votre SMS avant d’atteindre votre audience principale.

![](../assets/do-not-localize/book.png) Découvrez comment envoyer des bons à tirer dans [cette section](../preview-test/test-deliveries.md).

![](assets/sms_send_6.png){zoomable=&quot;yes&quot;}

## Envoyer votre diffusion par SMS {#send-sms}

1. Après avoir personnalisé le contenu de votre SMS, cliquez sur **[!UICONTROL Vérifier et envoyer]** sur votre page **[!UICONTROL Diffusion]**.

   ![](assets/sms_send_4.png){zoomable=&quot;yes&quot;}

1. Cliquez sur **[!UICONTROL Préparer]** et suivez la progression et les statistiques fournies.

   En cas d’erreur, reportez-vous au menu Journaux pour obtenir des informations détaillées sur l’échec.

1. Envoyez les messages en cliquant sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final.

   ![](assets/sms_send_5.png){zoomable=&quot;yes&quot;}

   Si la diffusion SMS a été planifiée, cliquez sur le bouton **[!UICONTROL Envoyer comme prévu]**. Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#schedule-the-delivery-sending).


1. Confirmez l’action d’envoi en cliquant sur le bouton **[!UICONTROL Envoyer]**.

Une fois votre diffusion envoyée, vous pouvez suivre les données de vos KPI (indicateurs clés de performance) à partir de la page de diffusion et les données à partir du menu **[!UICONTROL Journaux]**.

Vous pouvez maintenant commencer à mesurer l’impact de votre message à l’aide de rapports intégrés. [En savoir plus](../reporting/sms-report.md)
