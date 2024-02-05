---
audience: end-user
title: Envoyer une diffusion par notification push
description: Découvrez comment envoyer une diffusion par notification push dans Adobe Campaign Web.
badge: label="Disponibilité limitée"
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 100%

---

# Prévisualiser et envoyer une diffusion push {#send-push-delivery}

## Prévisualiser la diffusion par notification push {#preview-push}

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des abonnés et abonnées tests pour prévisualiser et tester le message. Si vous avez inséré du contenu personnalisé, vous pouvez vérifier son affichage dans le message à l’aide des données de profil de test. Vous pouvez ainsi vous assurer que le message est correctement rendu et que les éléments personnalisés sont bien intégrés.

Voici les étapes principales pour prévisualiser votre notification push. Pour plus d’informations sur la prévisualisation des diffusions, consultez [cette section](../preview-test/preview-content.md).

1. Sur la page de contenu de la diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** pour prévisualiser le contenu que vous avez personnalisé.

   ![](assets/push_send_1.png)

1. Cliquez sur **[!UICONTROL Ajouter un ou plusieurs abonnés]** pour sélectionner un ou plusieurs profils afin de prévisualiser leurs données dans le contenu de la notification push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. Dans le volet de droite, vous trouverez un aperçu de la notification push, où les éléments personnalisés sont remplacés dynamiquement par les données du profil sélectionné.

   ![](assets/push_send_7.png)

Vous pouvez maintenant vérifier et envoyer votre notification push à votre audience.

## Tester votre diffusion par notification push {#test-push}

**Adobe Campaign** vous offre la possibilité de tester les notifications push avant de les envoyer à votre audience principale. Cette étape est importante pour valider votre diffusion et identifier les problèmes éventuels.
Les destinataires du test vérifient alors divers éléments, tels que les liens, les images et les paramètres de personnalisation, détectent les erreurs éventuelles et garantissent des performances optimales. Ce processus vous permet d’affiner et d’optimiser vos notifications push avant d’atteindre votre audience principale.

![](../assets/do-not-localize/book.png) Découvrez comment envoyer des notifications push de test dans [cette section](../preview-test/test-deliveries.md#subscribers).

![](assets/push_send_6.png)

## Envoyer votre diffusion par notification push {#send-push}

1. Une fois le contenu de votre notification push personnalisé, cliquez sur **[!UICONTROL Réviser et envoyer]** sur la page de votre **[!UICONTROL Diffusion]**.

   ![](assets/push_send_2.png)

1. Cliquez sur **[!UICONTROL Préparer]** et suivez la progression et les statistiques fournies.

   En cas d’erreur, reportez-vous au menu Journaux pour obtenir des informations détaillées sur l’échec.

   ![](assets/push_send_3.png)

1. Envoyez les messages en cliquant sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final.

1. Confirmez l’action d’envoi en cliquant sur le bouton **[!UICONTROL Envoyer]**.

   Si la diffusion de notification push a été planifiée, cliquez sur le bouton **[!UICONTROL Envoyer comme prévu]**. Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![](assets/push_send_4.png)

Une fois votre diffusion envoyée, vous pouvez suivre les données de vos KPI (indicateurs clés de performance) à partir de la page de diffusion et les données à partir du menu **[!UICONTROL Journaux]**.

Vous pouvez maintenant commencer à mesurer l’impact de votre message à l’aide de rapports intégrés. [En savoir plus](../reporting/push-report.md)
