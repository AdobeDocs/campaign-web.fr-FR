---
audience: end-user
title: Prévisualiser et envoyer une diffusion courrier
description: Découvrez comment prévisualiser et envoyer une diffusion courrier avec Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 18%

---

# Prévisualiser et envoyer une diffusion courrier {#send-direct-mail}

Une fois que vous avez configuré le fichier d&#39;extraction pour votre diffusion courrier, vous pouvez utiliser des profils de test pour le prévisualiser. Si vous avez inclus du contenu personnalisé, vous pouvez examiner l’affichage de ce contenu dans les colonnes à l’aide des données de profil de test. Vous pouvez ainsi vous assurer que le contenu du fichier est correctement rendu et que les éléments personnalisés sont correctement intégrés.

Lorsque le fichier d&#39;extraction est prêt, vous pouvez envoyer la diffusion courrier afin de générer le fichier et le partager avec votre opérateur de services postaux. [Découvrez comment envoyer votre diffusion courrier](#dm-send)

## Aperçu du fichier d&#39;extraction {#preview-dm}

Les principales étapes pour prévisualiser votre fichier d&#39;extraction sont les suivantes. Pour plus d’informations sur la prévisualisation des diffusions, consultez [cette section](../preview-test/preview-content.md).

1. Sur la page de contenu de la diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** pour prévisualiser le contenu que vous avez personnalisé.

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. Cliquez sur **[!UICONTROL Ajouter un ou plusieurs profils de test]** pour sélectionner un ou plusieurs profils afin de prévisualiser leurs données dans le contenu du fichier d&#39;extraction.

1. Dans le volet de droite, vous trouverez un aperçu du fichier d’extraction où les éléments personnalisés sont remplacés dynamiquement par les données du profil sélectionné.

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## Envoyer des BAT {#test-dm}

**Adobe Campaign** vous offre la possibilité d’envoyer des BAT avant de les envoyer à votre audience principale. Cette étape est importante pour valider votre diffusion et identifier les problèmes éventuels. Les destinataires du test peuvent consulter des éléments tels que les paramètres de personnalisation, en assurant des performances optimales et en détectant les erreurs. Ce processus vous permet d’affiner et d’optimiser votre fichier d’extraction avant d’atteindre votre audience principale.

Pour les diffusions courrier, l&#39;envoi de BAT génère un exemple du fichier d&#39;extraction à partir des données des profils de test sélectionnés. Pour y accéder, procédez comme suit :

1. Dans l’écran de simulation du contenu, cliquez sur le bouton **[!UICONTROL Envoyer un bon à tirer]** et procédez comme pour n&#39;importe quel type de diffusion pour envoyer un BAT. [Découvrir comment envoyer des BAT](../preview-test/test-deliveries.md)

1. Une fois le BAT envoyé, vous pouvez y accéder à partir de la **[!UICONTROL Affichage des bons à tirer]** ou dans la liste des diffusions. [Découvrez comment accéder aux BAT envoyés](../preview-test/test-deliveries.md#access-test-deliveries)

1. Dans le tableau de bord de la diffusion du BAT, cliquez sur l’icône **[!UICONTROL Aperçu du fichier]** pour accéder à un aperçu du fichier d&#39;extraction.

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Seules les 100 premières lignes sont affichées dans le fichier d&#39;aperçu.

## Envoyer votre diffusion courrier {#send-dm}

Une fois que le courrier est prêt à être envoyé à vos clients, vous pouvez envoyer la diffusion afin de démarrer l&#39;extraction des données dans le fichier d&#39;extraction spécifié. Pour ce faire, procédez comme suit :

1. Après avoir conçu le contenu de votre fichier d’extraction, cliquez sur **[!UICONTROL Réviser et envoyer]** de votre **[!UICONTROL Diffusion]** page.

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. Cliquez sur **[!UICONTROL Préparer]** et suivez la progression et les statistiques fournies.

   Si des erreurs se produisent, reportez-vous à la section **[!UICONTROL Journaux]** pour obtenir des informations détaillées sur l’échec.

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. Envoyez les messages en cliquant sur **[!UICONTROL Envoyer]** pour poursuivre le processus d’envoi final.

1. Confirmez l’action d’envoi en cliquant sur le bouton **[!UICONTROL Envoyer]**.

   Si la diffusion courrier a été planifiée, cliquez sur le bouton **[!UICONTROL Envoyer comme prévu]** bouton . Pour en savoir plus sur la planification des diffusions, consultez [cette section](../msg/gs-messages.md#schedule-the-delivery-sending).

Une fois votre diffusion envoyée, le fichier d&#39;extraction est automatiquement généré et exporté vers l&#39;emplacement spécifié dans la variable **[!UICONTROL Routage]** compte externe sélectionné dans le champ du modèle de diffusion [paramètres avancés](../advanced-settings/delivery-settings.md).

Vous pouvez effectuer le suivi de vos données IPC (Indicateur de performance clé) à partir de votre page de diffusion et des données issues du **[!UICONTROL Journaux]** .

Vous pouvez également commencer à mesurer l’impact de votre message à l’aide de rapports intégrés. [En savoir plus](../reporting/direct-mail.md)
