---
audience: end-user
title: Concevoir une diffusion de notification push enrichie iOS
description: Découvrez comment concevoir une diffusion de notification push enrichie iOS avec Adobe Campaign Web
source-git-commit: f48e9a6d75429d9038b4e6b0af65a15bcb6fe929
workflow-type: tm+mt
source-wordcount: '1546'
ht-degree: 46%

---

# Concevoir une diffusion push iOS enrichie {#rich-push}

>[!IMPORTANT]
>
>Avant de concevoir une notification push enrichie, vous devez d’abord configurer votre connecteur V2. Consultez [cette page](https://experienceleague.adobe.com/fr/docs/campaign-classic/using/sending-messages/sending-push-notifications/configure-the-mobile-app/configuring-the-mobile-application) pour accéder à la procédure détaillée.

## Définir le contenu de la notification {#push-message}

Une fois votre diffusion push créée, vous pouvez définir son contenu à l&#39;aide de l&#39;un des modèles suivants :

* **Par défaut** vous permet d’envoyer des notifications avec une simple icône et une image associée.

* **De base** peut inclure du texte, des images et des boutons dans vos notifications.

* **Carrousel** vous permet d’envoyer des notifications avec du texte et plusieurs images que les utilisateurs peuvent parcourir.

* **Timer** inclut un minuteur de compte à rebours en direct dans vos notifications.

Accédez aux onglets ci-dessous pour en savoir plus sur la personnalisation de ces modèles.

>[!BEGINTABS]

>[!TAB Par défaut]

1. Dans le menu déroulant **[!UICONTROL Modèle]**, sélectionnez **[!UICONTROL Par défaut]**.

   ![](assets/rich_push_ios_default_1.png)

1. Dans le champ **[!UICONTROL Titre]**, saisissez le libellé du titre qui doit apparaître dans la liste des notifications disponibles depuis le centre de notifications.

   Ce champ vous permet de définir la valeur du paramètre **Titre** de la payload de notification iOS.

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Subtitle]** qui correspond au paramètre **subtitle** de la payload de notification iOS.

1. Saisissez le contenu du message dans le champ **[!UICONTROL Message]** .

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

   ![](assets/rich_push_ios_default_2.png)

1. Pour personnaliser davantage votre notification push, vous pouvez choisir une URL **[!UICONTROL Image de lancement]** à ajouter à votre notification push.

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et badge]** pour personnaliser des paramètres supplémentaires tels que les options de son et de badge pour vos notifications. [En savoir plus](#sound-badge)

   ![](assets/rich_push_ios_default_3.png)

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL Additional]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

   ![](assets/rich_push_ios_default_4.png)

1. Dans le menu **[!UICONTROL Variables d&#39;application]**, vos **[!UICONTROL variables d&#39;application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications. Par exemple, vous pouvez configurer l’affichage d’un écran spécifique lorsque l’utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des abonnés et abonnées de test pour prévisualiser et tester le message.

>[!TAB De base]

1. Dans le menu déroulant **[!UICONTROL Modèle]**, sélectionnez **[!UICONTROL De base]**.

   ![](assets/rich_push_ios_basic_1.png)

1. Pour composer votre message, saisissez votre texte dans les champs **[!UICONTROL Titre]**, **[!UICONTROL Titre étendu]**, **[!UICONTROL Message]** et **[!UICONTROL Message étendu]**.

   Le texte **[!UICONTROL Message]** s’affiche dans la vue réduite, alors que le **[!UICONTROL Message étendu]** s’affiche lorsque la notification est développée.

   ![](assets/rich_push_ios_basic_2.png)

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Subtitle]** qui correspond au paramètre **subtitle** de la payload de notification iOS.

1. Ajoutez l’URL qui définit l’**[!UICONTROL Action de clic]** associée à un clic sur votre notification. Cela détermine le comportement lorsque l’utilisateur ou l’utilisatrice interagit avec la notification, par exemple en ouvrant une fenêtre spécifique ou en effectuant une action spécifique dans votre application.

1. Pour personnaliser davantage votre notification push, vous pouvez choisir une URL **[!UICONTROL Image de lancement]** à ajouter à votre notification push.

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et badge]** pour personnaliser des paramètres supplémentaires tels que les options de son et de badge pour vos notifications. [En savoir plus](#sound-badge)

   ![](assets/rich_push_ios_basic_3.png)

1. Dans le menu **[!UICONTROL Color options]**, saisissez des codes de couleur hexadécimaux pour la **[!UICONTROL Notification background color]**, la **[!UICONTROL Notification background color]** et la **[!UICONTROL Message text color]**.

   ![](assets/rich_push_ios_basic_4.png)

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL Additional]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

1. Dans le menu **[!UICONTROL Variables d&#39;application]**, vos **[!UICONTROL variables d&#39;application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications. Par exemple, vous pouvez configurer l’affichage d’un écran spécifique lorsque l’utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des abonnés et abonnées de test pour prévisualiser et tester le message.

>[!TAB Carrousel]

1. Dans le menu déroulant **[!UICONTROL Modèle]**, sélectionnez **[!UICONTROL Carrousel]**.

   ![](assets/rich_push_ios_carousel_1.png)

1. Pour composer votre message, saisissez votre texte dans les champs **[!UICONTROL Titre]**, **[!UICONTROL Titre étendu]**, **[!UICONTROL Message]** et **[!UICONTROL Message étendu]**.

   Le texte **[!UICONTROL Message]** s’affiche dans la vue réduite, alors que le **[!UICONTROL Message étendu]** s’affiche lorsque la notification est développée.

   ![](assets/rich_push_ios_carousel_2.png)

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Subtitle]** qui correspond au paramètre **subtitle** de la payload de notification iOS.

1. Ajoutez l’URL qui définit l’**[!UICONTROL Action de clic]** associée à un clic sur votre notification. Cela détermine le comportement lorsque l’utilisateur ou l’utilisatrice interagit avec la notification, par exemple en ouvrant une fenêtre spécifique ou en effectuant une action spécifique dans votre application.

1. Choisissez le mode de fonctionnement du **[!UICONTROL carrousel]** :

   * **[!UICONTROL Auto]** : fait automatiquement défiler les images sous forme de diapositives, selon des transitions à intervalles prédéfinis.
   * **[!UICONTROL Manuel]** : permet de passer manuellement d’une diapositive à l’autre pour naviguer dans les images.

1. Cliquez sur **[!UICONTROL Ajouter une image]** et saisissez votre URL **[!UICONTROL Image]**, **[!UICONTROL Texte]** et **[!UICONTROL URI d&#39;action]**.

   Veillez à inclure trois images minimum et cinq images maximum.

   ![](assets/rich_push_ios_carousel_3.png)

1. Gérez l’ordre de vos images à l’aide des flèches haut et bas.

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et badge]** pour personnaliser des paramètres supplémentaires tels que les options de son et de badge pour vos notifications. [En savoir plus](#sound-badge)

1. Dans le menu **[!UICONTROL Color options]**, saisissez des codes de couleur hexadécimaux pour la **[!UICONTROL Notification background color]**, la **[!UICONTROL Notification background color]** et la **[!UICONTROL Message text color]**.

   ![](assets/rich_push_ios_carousel_4.png)

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL Additional]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

1. Dans le menu **[!UICONTROL Variables d&#39;application]**, vos **[!UICONTROL variables d&#39;application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications. Par exemple, vous pouvez configurer l’affichage d’un écran spécifique lorsque l’utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des abonnés et abonnées de test pour prévisualiser et tester le message.

>[!TAB Timer]

1. Dans la liste déroulante **[!UICONTROL Type de notification]**, sélectionnez **[!UICONTROL Timer]**.

   ![](assets/rich_push_ios_timer_1.png)

1. Pour composer votre message, saisissez votre texte dans les champs **[!UICONTROL Titre]**, **[!UICONTROL Titre étendu]**, **[!UICONTROL Message]** et **[!UICONTROL Message étendu]**.

   Le texte **[!UICONTROL Message]** s’affiche dans la vue réduite, alors que le **[!UICONTROL Message étendu]** s’affiche lorsque la notification est développée.

   ![](assets/rich_push_ios_timer_2.png)

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Subtitle]** qui correspond au paramètre **subtitle** de la payload de notification iOS.

1. Ajoutez l’URL qui définit l’**[!UICONTROL Action de clic]** associée à un clic sur votre notification. Cela détermine le comportement lorsque l’utilisateur ou l’utilisatrice interagit avec la notification, par exemple en ouvrant une fenêtre spécifique ou en effectuant une action spécifique dans votre application.

1. Pour personnaliser davantage votre notification push, vous pouvez choisir une URL **[!UICONTROL Image de lancement]** à ajouter à votre notification push.

1. Définissez la **[!UICONTROL durée du minuteur]** en secondes ou l’**[!UICONTROL horodatage de fin du minuteur]** sur un horodatage d’époque spécifique.

   ![](assets/rich_push_ios_timer_3.png)

1. Saisissez le texte et l’image qui s’afficheront une fois le minuteur expiré dans les champs **[!UICONTROL Autre titre]**, **[!UICONTROL Autre message]** et **[!UICONTROL Autre image de lancement]**.

   ![](assets/rich_push_ios_timer_4.png)

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et badge]** pour personnaliser des paramètres supplémentaires tels que les options de son et de badge pour vos notifications. [En savoir plus](#sound-badge)

1. Dans le menu **[!UICONTROL Color options]**, saisissez des codes de couleur hexadécimaux pour la **[!UICONTROL Notification background color]**, la **[!UICONTROL Notification background color]** et la **[!UICONTROL Message text color]**.

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL Additional]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

1. Dans le menu **[!UICONTROL Variables d&#39;application]**, vos **[!UICONTROL variables d&#39;application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications. Par exemple, vous pouvez configurer l’affichage d’un écran spécifique lorsque l’utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, vous pouvez utiliser des abonnés et abonnées de test pour prévisualiser et tester le message.

>[!ENDTABS]

## Paramètres avancés des notifications push {#push-advanced}

### Options de son et de badge {#sound-badge}

| Paramètre | Description |
|---------|---------|
| **[!UICONTROL Mode d’alerte critique]** | Activez cette option pour ajouter du son à votre notification, même si le téléphone de l&#39;utilisateur est en mode focus ou si iPhone est en mode silencieux. |
| **[!UICONTROL Nettoyer la pastille]** | Activez ces options pour actualiser la valeur du badge. |
| **[!UICONTROL Son]** | Définissez le son à émettre lorsque l’appareil reçoit votre notification. |
| **[!UICONTROL Nombre de notifications]** | Définissez un nombre qui sera utilisé pour afficher directement sur l’icône de l’application le nombre de nouvelles informations non lues. |
| **[!UICONTROL Volume]** | Définissez le volume de votre son entre 0 et 100. Les sons doivent être inclus dans l’application et définis lors de la création du service. |

### Paramètres de couleur {#color}

| Paramètre | Description |
|---------|---------|
| **[!UICONTROL Couleur d’arrière-plan de la notification]** | Définissez la couleur de votre arrière-plan de notification avec vos codes couleur hexadécimaux. |
| **[!UICONTROL Couleur du titre]** | Définissez la couleur de votre titre avec vos codes couleur hexadécimaux. |
| **[!UICONTROL Couleur du texte de message]** | Définissez la couleur de votre texte avec vos codes couleur hexadécimaux. |

### Options avancées {#notification-options}

| Paramètre | Description |
|---------|---------|
| **[!UICONTROL Contenu mutable]** | Activez cette option pour permettre à l’application mobile de télécharger le contenu multimédia. |
| **[!UICONTROL Score de pertinence]** | Définissez un score de pertinence compris entre 0 et 100. Le système l’utilise pour trier les notifications dans le résumé de la notification. |
| **[!UICONTROL Niveau d&#39;interruption]** | <ul><li>Actif : défini par défaut, le système présente immédiatement la notification, illumine l’écran et peut émettre un son. Les notifications ne passent pas en mode Ciblage .</li><li>Passif : le système ajoute la notification à la liste de notifications sans allumer l&#39;écran ni émettre un son. Les notifications ne passent pas en mode Thème.</li><li> Temps sensible : le système présente immédiatement la notification, allume l&#39;écran, peut émettre un son et passer en mode Mise au point. Ce niveau ne nécessite pas d’autorisation spéciale de la part d’Apple.</li><li>Critique : le système présente immédiatement la notification, allume l’écran et contourne le bouton d’arrêt ou le mode de focus. Notez que ce niveau nécessite une autorisation spéciale de la part d’Apple.</li></ul> |
| **[!UICONTROL Thread-id]** | Définissez l’identifiant utilisé pour regrouper les notifications associées. |
| **[!UICONTROL Catégorie]** | Définissez le nom de votre ID de catégorie qui affichera les boutons d’action. Ces notifications permettent à la personne d’effectuer plus rapidement différentes tâches en réponse à celles-ci, sans ouvrir l’application ou la parcourir. |
| **[!UICONTROL Identifiant du contenu Target]** | Définissez l&#39;identifiant utilisé pour cibler la fenêtre d&#39;application à afficher à l&#39;ouverture de la notification. |

