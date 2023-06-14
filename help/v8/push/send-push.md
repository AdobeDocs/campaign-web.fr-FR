---
audience: end-user
title: Envoyer une diffusion de notification push
description: Découvrez comment envoyer une diffusion de notification push avec Adobe Campaign Web
badge: label="Alpha"
source-git-commit: c24b53ee17e81805f0717682202d2d4154c96c1e
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Prévisualiser et envoyer une diffusion de notification push {#send-push-delivery}

## Prévisualiser la diffusion de la notification push {#preview-push}

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des abonnés au test pour prévisualiser et tester le message. Si vous avez inclus du contenu personnalisé, vous pouvez examiner l&#39;affichage de ce contenu dans le message à l&#39;aide des données de profil de test. Vous pouvez ainsi vous assurer que le message est correctement rendu et que les éléments personnalisés sont correctement intégrés.

Les principales étapes pour prévisualiser votre diffusion SMS sont les suivantes. Pour plus d’informations sur la prévisualisation des diffusions, reportez-vous à la section [cette section](../preview-test/preview-content.md).

1. Dans la page de contenu de votre diffusion, utilisez **[!UICONTROL Simulation du contenu]** pour prévisualiser votre contenu personnalisé.

   ![](assets/push_send_1.png)

1. Cliquez sur **[!UICONTROL Ajouter des abonnés]** pour sélectionner un ou plusieurs profils afin de prévisualiser leurs données dans le contenu de la notification push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. Dans le volet de droite, vous trouverez un aperçu de la notification push, où les éléments personnalisés sont remplacés dynamiquement par les données du profil sélectionné.

   ![](assets/push_send_7.png)

Vous pouvez maintenant passer en revue et envoyer votre notification push à votre audience.

## Tester votre diffusion de notification push {#test-push}

Utilisation **Adobe Campaign**, vous avez la possibilité de tester les notifications push avant de les envoyer à votre audience principale. Cette étape est importante pour valider votre diffusion et identifier les problèmes éventuels.
Les destinataires du test peuvent consulter des éléments tels que des liens, des images et des paramètres de personnalisation, assurant des performances optimales et détectant toutes les erreurs. Ce processus vous permet d’affiner et d’optimiser vos notifications push avant d’atteindre votre audience principale.

![](../assets/do-not-localize/book.png) Découvrez comment envoyer des notifications push de test dans [cette section](../preview-test/proofs.md#subscribers).

![](assets/push_send_6.png)

## Envoyer votre diffusion de notification push {#send-push}

1. Après avoir personnalisé le contenu de votre notification push, cliquez sur **[!UICONTROL Réviser et envoyer]** de votre **[!UICONTROL Diffusion]** page.

   ![](assets/push_send_2.png)

1. Cliquez sur **[!UICONTROL Préparer]**et suivre l&#39;état d&#39;avancement et les statistiques fournies.

   En cas d&#39;erreur, reportez-vous au menu Journaux pour obtenir des informations détaillées sur l&#39;échec.

   ![](assets/push_send_3.png)

1. Envoyer les messages en cliquant sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final.

1. Confirmez l&#39;action d&#39;envoi en cliquant sur le bouton **[!UICONTROL Envoyer]** ou **[!UICONTROL Envoyer comme prévu]** bouton .

   ![](assets/push_send_4.png)

Une fois votre diffusion envoyée, vous pouvez effectuer le suivi de vos données IPC (Indicateur de performance clé) provenant de votre page de diffusion et des données issues de la variable **[!UICONTROL Journaux]** .

Vous pouvez maintenant commencer à mesurer l’impact de votre message à l’aide de rapports intégrés. [En savoir plus](../reporting/push-report.md)
