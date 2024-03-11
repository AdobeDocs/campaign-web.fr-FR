---
audience: end-user
title: Envoyer des BAT
description: Découvrir comment définir et envoyer des BAT
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 99%

---

# Envoyer des BAT {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Mode Aperçu"
>abstract="Prévisualisez et testez le message en incluant la population test à la cible principale."

Une fois le contenu de votre message défini, vous pouvez le prévisualiser et le tester en envoyant des BAT aux profils de test. Si vous avez inséré du contenu personnalisé, vous pouvez vérifier son contenu dans le message à l’aide des données de profil de test.

Pour détecter d’éventuelles erreurs dans le contenu du message ou les paramètres de personnalisation, envoyez des BAT aux profils de test avant de les envoyer à l’audience cible. Un BAT doit être envoyé à chaque modification afin de valider le contenu le plus récent. L’envoi de BAT est une étape importante pour valider votre campagne et identifier les problèmes potentiels. Les personnes destinataires d’un BAT peuvent vérifier différents éléments tels que des liens, des liens de désinscription, des images ou des pages miroir, ainsi que détecter toute erreur de rendu, de contenu, de paramètres de personnalisation et de configuration de la diffusion.

## Simulation du contenu avec des profils de test {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Population test"
>abstract="Sélectionnez un mode de population test."

Avant d’envoyer un BAT, assurez-vous de définir une audience cible pour votre diffusion. [En savoir plus](../audience/add-audience.md)

Pour commencer à tester le contenu de votre message :

1. Modifiez le contenu de votre diffusion.
1. Cliquez sur le bouton **[!UICONTROL Simuler le contenu]**.
1. Cliquez sur le bouton **[!UICONTROL Envoyer un BAT]** pour envoyer des BAT.

   ![](assets/simulate-test-button-email.png){zoomable=&quot;yes&quot;}

1. Sélectionnez les personnes destinataires de vos BAT.

   Selon le canal de message, les BAT peuvent être envoyés aux types de personnes destinataires suivants :

   * Pour les SMS et les e-mails, vous pouvez utiliser des [profils de test](#test-profiles), qui sont des profils destinataires supplémentaires spécifiques dans la base de données. Vous pouvez également utiliser le mode de [substitution de la cible principale](#substitution-profiles), qui envoie le BAT à l’adresse e-mail ou au numéro de téléphone test et utilise les données de personnalisation d’un profil existant. Vous pouvez ainsi consulter le message comme si vous étiez la personne destinataire, avec le contenu reproduit à l’identique pour le profil indiqué.

   * Pour les messages push, vous pouvez utiliser des [personnes abonnées](#subscribers) fictives ajoutées à la base de données. Elles sont créés dans la console [!DNL Campaign]. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=fr){target="_blank"}.

   La configuration détaillée de chaque mode est disponible ci-dessous.

## Utiliser des profils de test {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Cible du BAT"
>abstract="Vous pouvez télécharger un second fichier en tant que « cible du BAT » si vous souhaitez tester votre diffusion avant de l’envoyer à la cible principale."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Charger les profils"
>abstract="Vous pouvez charger un second fichier avec des profils supplémentaires si vous souhaitez tester votre diffusion avec un ensemble différent de celui utilisé pour la cible principale."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="Fichier modèle"
>abstract="La mise en forme du fichier doit être identique à celle du fichier d’origine.<br/>Formats de fichiers pris en charge : txt, csv. Taille maximale du fichier : 15 Mo. Utilisez la première ligne comme en-tête de colonne."

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Inclure les profils de test dans l’audience principale"
>abstract="Activez cette option pour envoyer également le message final aux personnes destinataires des BAT."

Les profils de test sont des personnes destinataires supplémentaires dans la base de données. Ils sont créés à partir du menu **[!UICONTROL Gestion des clientes et clients]** > **[!UICONTROL Profils]**. [En savoir plus](../audience/test-profiles.md#create-test-profiles)

Les étapes d’envoi de BAT aux profils de test sont détaillées ci-dessous.

1. Dans le contenu de votre diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]**, puis sur le bouton **[!UICONTROL Envoyer un BAT]**.

1. Dans la liste déroulante **[!UICONTROL Mode]**, choisissez les **[!UICONTROL Profils de test]** pour cibler les personnes destinataires fictives qui recevront le BAT ou la diffusion par SMS.

   ![](assets/simulate-profile-mode.png){zoomable=&quot;yes&quot;}

1. Si vous avez déjà sélectionné des profils pour [prévisualiser le message](preview-content.md) dans l’écran de simulation du contenu, ils sont présélectionnés comme profils destinataires des BAT. Vous pouvez effacer votre sélection et/ou ajouter des profils destinataires supplémentaires à l’aide du bouton **[!UICONTROL Ajouter un ou plusieurs profils de test]**.

1. Lorsque vous parcourez le profil de test ou la liste des profils, vous pouvez ajouter des filtres pour affiner votre recherche. Par exemple, vous pouvez définir une règle pour rechercher tous les profils de test dotés du statut **[!UICONTROL Prospect]**. Découvrez comment ajouter des règles à l’aide du [concepteur de requêtes](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. Si vous souhaitez envoyer le message final aux personnes destinataires du BAT, sélectionnez l’option **[!UICONTROL Inclure la population du test dans la cible principale]**.

   ![](assets/simulate-include-test.png){zoomable=&quot;yes&quot;}

1. Une fois les profils de test sélectionnés, vous pouvez [envoyer le BAT](#send-test).

## Substituer des données de profil {#substitution-profiles}

Utilisez la substitution de profils pour envoyer un BAT à une adresse e-mail ou un numéro de téléphone spécifique, tout en affichant les données d’un profil existant de la base de données [!DNL Adobe Campaign]. Ce mode ne peut être sélectionné que si l’audience de la diffusion a été définie.

Pour remplacer les données de profil de la cible principale, procédez comme suit :

1. Dans le contenu de votre diffusion, cliquez sur le bouton **[!UICONTROL Simuler le contenu]**, puis sur le bouton **[!UICONTROL Envoyer un BAT]**.

1. Dans la liste déroulante **[!UICONTROL Mode]**, choisissez l’option **[!UICONTROL Substituer à partir de la cible principale]** pour envoyer un BAT à une adresse e-mail ou un numéro de téléphone spécifique tout en affichant les données d’un profil existant.

   >[!CAUTION]
   >
   >Si vous n’avez pas sélectionné d’[audience](../audience/about-recipients.md) pour votre diffusion, l’option **[!UICONTROL Substituer à partir de la cible principale]** est grisée et vous ne pourrez pas sélectionner de profil de substitution.

1. Cliquez sur le bouton **[!UICONTROL Ajouter une adresse]** et indiquez l’adresse e-mail ou le numéro de téléphone qui recevra le BAT.

   ![](assets/simulate-add-substitution-address.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Vous pouvez saisir n’importe quelle adresse e-mail ou n’importe quel numéro de téléphone. Vous pouvez ainsi envoyer des BAT à n’importe quelle personne destinataire, même si elle est étrangère à [!DNL Adobe Campaign].

1. Sélectionnez le profil de la cible que vous avez définie pour votre diffusion à utiliser en remplacement. Vous pouvez également laisser [!DNL Adobe Campaign] sélectionner un profil aléatoire à partir de la cible. Les données du profil sélectionné seront affichées dans le BAT.

1. Confirmez la personne destinataire et renouvelez l’opération pour ajouter autant d’adresses e-mail ou de numéros de téléphone que nécessaire.

   ![](assets/simulate-profile-substitute.png){zoomable=&quot;yes&quot;}

1. Si vous souhaitez envoyer le message final aux personnes destinataires du BAT, sélectionnez l’option **[!UICONTROL Inclure la population du test dans la cible principale]**.

1. Une fois les profils de substitution sélectionnés, vous pouvez [envoyer le BAT](#send-test).

## Envoyer des BAT aux personnes abonnées de l’application {#subscribers}

Lorsque vous travaillez avec les notifications push, les BAT ne peuvent être envoyés qu’aux personnes abonnées de votre application. Pour les sélectionner, procédez comme suit.

1. Dans le contenu de votre diffusion push, cliquez sur le bouton **[!UICONTROL Simuler le contenu]**, puis sur le bouton **[!UICONTROL Envoyer un BAT]**.

   ![](assets/simulate-test-button-push.png){zoomable=&quot;yes&quot;}

1. Si vous avez déjà sélectionné des abonnés et abonnées pour [prévisualiser la diffusion](preview-content.md) dans l’écran de simulation du contenu, ces profils sont présélectionnés comme abonnés du test.

   Vous pouvez effacer votre sélection et/ou ajouter d’autres abonnés et abonnées à l’aide du bouton dédié.

   ![](assets/simulate-test-subscribers.png){zoomable=&quot;yes&quot;}

1. Si vous souhaitez envoyer la notification push finale aux personnes abonnées du test, sélectionnez l’option **[!UICONTROL Inclure la population du test dans la cible principale]**.

1. Une fois les personnes abonnées sélectionnées, vous pouvez [envoyer le BAT](#send-test).

## Envoyer le BAT {#send-test}

Pour envoyer le BAT aux personnes destinataires sélectionnées, procédez comme suit.

1. Cliquez sur le bouton **[!UICONTROL Envoyer un BAT]**.

1. Confirmez l’envoi.

   ![](assets/simulate-send-test.png){zoomable=&quot;yes&quot;}

1. Vous pouvez envoyer autant de BAT que nécessaire jusqu’à ce que le contenu de votre diffusion soit finalisé.

Une fois cette opération effectuée, vous pouvez préparer et envoyer la diffusion à la cible principale. Pour ce faire, consultez les sections dédiées ci-dessous :

* [Envoyer votre e-mail](../monitor/prepare-send.md)
* [Envoyer votre notification push](../push/send-push.md#send-push)
* [Envoyer votre diffusion par SMS](../sms/send-sms.md#send-sms)

## Accéder aux BAT envoyés {#access-test-deliveries}

Une fois les BAT envoyés, vous pouvez accéder à leurs logs à partir de l’écran **[!UICONTROL Simuler le contenu]**.

Ces logs permettent d’accéder à tous les BAT envoyés pour la diffusion sélectionnée et de visualiser des statistiques spécifiques relatives à leur envoi. [Découvrir comment surveiller les logs de diffusion](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png){zoomable=&quot;yes&quot;}

Vous pouvez également accéder aux BAT envoyés à partir de la [liste de diffusion](../msg/gs-messages.md), comme pour n’importe quelle diffusion.

![](assets/simulate-deliveries-list.png){zoomable=&quot;yes&quot;}
