---
audience: end-user
title: Envoyer une diffusion par notification push
description: Découvrez comment envoyer une diffusion par notification push dans Adobe Campaign Web.
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 100%

---

# Prévisualiser et envoyer une diffusion push {#send-push-delivery}

## Prévisualiser la diffusion par notification push {#preview-push}

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des personnes abonnées de test pour prévisualiser et tester le message. Si vous avez inséré du contenu personnalisé, vérifiez son affichage dans le message à l’aide des données de profil de test. Cela permet de s’assurer que le message est correctement rendu et que les éléments personnalisés sont correctement intégrés.

Voici les étapes principales pour prévisualiser votre notification push. Pour plus d’informations sur la prévisualisation des diffusions, consultez [cette section](../preview-test/preview-content.md).

1. Sur la page de contenu de la diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** pour prévisualiser le contenu que vous avez personnalisé.

   ![Prévisualisation de contenu personnalisé dans la page de contenu de la diffusion](assets/push_send_1.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Ajouter un ou plusieurs abonnés]** pour sélectionner un ou plusieurs profils afin de prévisualiser leurs données dans le contenu de la notification push.

   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. Dans le volet de droite, vous trouverez un aperçu de la notification push, où les éléments personnalisés sont remplacés dynamiquement par les données du profil sélectionné.

   ![Volet d’aperçu présentant les éléments personnalisés remplacés par des données de profil](assets/push_send_7.png){zoomable="yes"}

Vous pouvez maintenant vérifier et envoyer votre notification push à votre audience.

## Tester votre diffusion par notification push {#test-push}

À l’aide d’**Adobe Campaign**, envoyez des BAT avant de les diffuser à votre audience principale. Cette étape valide votre diffusion et identifie les problèmes éventuels.

Les profils de test sont les profils destinataires des BAT. Ceux-ci peuvent examiner et valider les composants et les paramètres tels que les liens, les images et la personnalisation, pour garantir des performances optimales et détecter les erreurs. Ce processus vous permet d’affiner et d’optimiser vos notifications push avant d’atteindre votre audience principale. [Découvrez comment envoyer des BAT](../preview-test/test-deliveries.md#subscribers).

![Test de la diffusion des notifications push avec les destinataires du BAT](assets/push_send_6.png){zoomable="yes"}

## Envoyer votre diffusion par notification push {#send-push}

1. Une fois le contenu de votre notification push personnalisé, cliquez sur **[!UICONTROL Réviser et envoyer]** sur la page de votre **[!UICONTROL Diffusion]**.

   ![Bouton Vérifier et envoyer sur la page de diffusion](assets/push_send_2.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Préparer]** et suivez la progression et les statistiques fournies.

   En cas d’erreur, reportez-vous au menu Logs pour obtenir des informations détaillées sur l’échec.

   ![Suivi des progrès de la préparation et des statistiques](assets/push_send_3.png){zoomable="yes"}

1. Envoyez les messages en cliquant sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final.

1. Confirmez l’action d’envoi en cliquant sur le bouton **[!UICONTROL Envoyer]**.

   Si la diffusion de notification push a été planifiée, cliquez sur le bouton **[!UICONTROL Envoyer comme prévu]**. Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![Bouton Envoyer comme prévu pour la diffusion de notifications push planifiée](assets/push_send_4.png){zoomable="yes"}

Une fois votre diffusion envoyée, suivez les données de vos KPI (indicateurs clés de performance) à partir de votre page de diffusion et les données à partir du menu **[!UICONTROL Journaux]**.

Commencez à mesurer l’impact de votre message à l’aide de rapports intégrés. [En savoir plus](../reporting/push-report.md).