---
audience: end-user
title: Concevoir une diffusion de notification push iOS enrichie
description: Découvrez comment concevoir une diffusion de notification push iOS enrichie avec Adobe Campaign Web.
exl-id: e6058d60-9f34-412b-aac2-6e319a3ab898
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 48%

---

# Concevoir une diffusion de notification push iOS enrichie {#rich-push}

>[!IMPORTANT]
>
>Avant de concevoir une notification push enrichie, vous devez configurer votre connecteur V2. Consultez [cette page](https://experienceleague.adobe.com/fr/docs/campaign-classic/using/sending-messages/sending-push-notifications/configure-the-mobile-app/configuring-the-mobile-application) pour accéder à la procédure détaillée.

## Définir le contenu de la notification {#push-message}

Une fois votre diffusion push créée, définissez son contenu à l’aide de l’un des modèles suivants :

* Le **modèle par défaut** vous permet d’envoyer des notifications avec une simple icône et une image associée.
* Le **modèle de base** peut inclure du texte, des images et des boutons dans vos notifications.
* Le **carousel** vous permet d’envoyer des notifications avec du texte et plusieurs images que les utilisateurs et utilisatrices peuvent faire défiler.
* Le **retardateur** inclut un minuteur avec compte à rebours dynamique dans vos notifications.

Parcourez les onglets ci-dessous pour en savoir plus sur la personnalisation de ces modèles.

>[!BEGINTABS]

>[!TAB Par défaut]

1. Dans le menu déroulant **[!UICONTROL Modèle]**, sélectionnez **[!UICONTROL Par défaut]**.

   ![Écran de sélection des modèles par défaut](assets/rich_push_ios_default_1.png)

1. Dans le champ **[!UICONTROL Titre]**, saisissez le libellé du titre qui doit apparaître dans la liste des notifications disponibles depuis le centre de notifications.

   Ce champ définit la valeur du paramètre **title** de la payload de notification iOS.

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Sous-titre]**, qui correspond à la valeur du paramètre **sous-titre** du payload de notification iOS.

1. Saisissez le contenu du message dans le champ **[!UICONTROL Message]**.

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

   ![Écran de l’éditeur d’expression](assets/rich_push_ios_default_2.png)

1. Pour personnaliser davantage votre notification push, choisissez une URL **[!UICONTROL Image de Launch]** à ajouter à votre notification push.

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et pastille]** pour personnaliser des paramètres supplémentaires tels que les options de son et de pastille pour vos notifications. [En savoir plus](#sound-badge)

   ![Écran des paramètres Son et pastille](assets/rich_push_ios_default_3.png)

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL supplémentaires]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

   ![Écran Options supplémentaires](assets/rich_push_ios_default_4.png)

1. Dans le menu **[!UICONTROL Variables de l’application]**, vos **[!UICONTROL variables d’application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications, par exemple lors de la configuration d&#39;un écran spécifique à afficher lorsque l&#39;utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, utilisez tester les abonnés et abonnées pour prévisualiser et tester le message.

>[!TAB De base]

1. Dans le menu déroulant **[!UICONTROL Modèle]**, sélectionnez **[!UICONTROL De base]**.

   ![Écran de sélection des modèles de base](assets/rich_push_ios_basic_1.png)

1. Pour composer votre message, saisissez le texte dans les champs **[!UICONTROL Titre]**, **[!UICONTROL Titre développé]**, **[!UICONTROL Message]** et **[!UICONTROL Message développé]**.

   Le texte **[!UICONTROL Message]** apparaît dans la vue réduite, tandis que le texte **[!UICONTROL Message développé]** s’affiche lorsque la notification est développée.

   ![Écran de composition des messages](assets/rich_push_ios_basic_2.png)

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Sous-titre]**, qui correspond à la valeur du paramètre **sous-titre** du payload de notification iOS.

1. Ajoutez l’URL qui définit l’**[!UICONTROL action de clic]** associée à un clic de l’utilisateur sur votre notification. Cela détermine le comportement lorsque l’utilisateur ou l’utilisatrice interagit avec la notification, par exemple en ouvrant une fenêtre spécifique ou en effectuant une action spécifique dans votre application.

1. Pour personnaliser davantage votre notification push, choisissez une URL **[!UICONTROL Image de Launch]** à ajouter à votre notification push.

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et pastille]** pour personnaliser des paramètres supplémentaires tels que les options de son et de pastille pour vos notifications. [En savoir plus](#sound-badge)

   ![Écran des paramètres Son et pastille](assets/rich_push_ios_basic_3.png)

1. Dans le menu **[!UICONTROL Options de couleur]**, saisissez des codes couleur hexadécimaux pour les **[!UICONTROL Couleur d’arrière-plan de la notification]**, **[!UICONTROL Couleur d’arrière-plan de la notification]** et **[!UICONTROL Couleur du texte du message]**.

   ![Écran des options de couleur](assets/rich_push_ios_basic_4.png)

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL supplémentaires]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

1. Dans le menu **[!UICONTROL Variables de l’application]**, vos **[!UICONTROL variables d’application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications, par exemple lors de la configuration d&#39;un écran spécifique à afficher lorsque l&#39;utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, utilisez tester les abonnés et abonnées pour prévisualiser et tester le message.

>[!TAB Carousel]

1. Dans le menu déroulant **[!UICONTROL Modèle]**, sélectionnez **[!UICONTROL Carousel]**.

   ![Écran de sélection du modèle de carrousel](assets/rich_push_ios_carousel_1.png)

1. Pour composer votre message, saisissez le texte dans les champs **[!UICONTROL Titre]**, **[!UICONTROL Titre développé]**, **[!UICONTROL Message]** et **[!UICONTROL Message développé]**.

   Le texte **[!UICONTROL Message]** apparaît dans la vue réduite, tandis que le texte **[!UICONTROL Message développé]** s’affiche lorsque la notification est développée.

   ![Écran de composition des messages](assets/rich_push_ios_carousel_2.png)

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Sous-titre]**, qui correspond à la valeur du paramètre **sous-titre** du payload de notification iOS.

1. Ajoutez l’URL qui définit l’**[!UICONTROL action de clic]** associée à un clic de l’utilisateur sur votre notification. Cela détermine le comportement lorsque l’utilisateur ou l’utilisatrice interagit avec la notification, par exemple en ouvrant une fenêtre spécifique ou en effectuant une action spécifique dans votre application.

1. Choisissez le mode de fonctionnement du **[!UICONTROL carrousel]** :

   * **[!UICONTROL Auto]** : fait automatiquement défiler les images sous forme de diapositives, selon des transitions à intervalles prédéfinis.
   * **[!UICONTROL Manuel]** : permet de passer manuellement d’une diapositive à l’autre pour naviguer dans les images.

1. Cliquez sur **[!UICONTROL Ajouter une image]** et saisissez votre **[!UICONTROL Image]** URL, **[!UICONTROL Texte]** et **[!UICONTROL URI d’action]**.

   Veillez à inclure trois images minimum et cinq maximum.

   ![Écran d’ajout d’images au carrousel](assets/rich_push_ios_carousel_3.png)

1. Gérez l’ordre de vos images à l’aide des flèches haut et bas.

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et pastille]** pour personnaliser des paramètres supplémentaires tels que les options de son et de pastille pour vos notifications. [En savoir plus](#sound-badge)

1. Dans le menu **[!UICONTROL Options de couleur]**, saisissez des codes couleur hexadécimaux pour les **[!UICONTROL Couleur d’arrière-plan de la notification]**, **[!UICONTROL Couleur d’arrière-plan de la notification]** et **[!UICONTROL Couleur du texte du message]**.

   ![Écran des options de couleur](assets/rich_push_ios_carousel_4.png)

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL supplémentaires]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

1. Dans le menu **[!UICONTROL Variables de l’application]**, vos **[!UICONTROL variables d’application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications, par exemple lors de la configuration d&#39;un écran spécifique à afficher lorsque l&#39;utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, utilisez tester les abonnés et abonnées pour prévisualiser et tester le message.

>[!TAB Retardateur]

1. Dans le menu déroulant **[!UICONTROL Type de notification]**, sélectionnez **[!UICONTROL Retardateur]**.

   ![Écran de sélection du modèle de minuteur](assets/rich_push_ios_timer_1.png)

1. Pour composer votre message, saisissez le texte dans les champs **[!UICONTROL Titre]**, **[!UICONTROL Titre développé]**, **[!UICONTROL Message]** et **[!UICONTROL Message développé]**.

   Le texte **[!UICONTROL Message]** apparaît dans la vue réduite, tandis que le texte **[!UICONTROL Message développé]** s’affiche lorsque la notification est développée.

   ![Écran de composition des messages](assets/rich_push_ios_timer_2.png)

1. Utilisez l’éditeur d’expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique. [En savoir plus](../personalization/personalize.md)

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Sous-titre]**, qui correspond à la valeur du paramètre **sous-titre** du payload de notification iOS.

1. Ajoutez l’URL qui définit l’**[!UICONTROL action de clic]** associée à un clic de l’utilisateur sur votre notification. Cela détermine le comportement lorsque l’utilisateur ou l’utilisatrice interagit avec la notification, par exemple en ouvrant une fenêtre spécifique ou en effectuant une action spécifique dans votre application.

1. Pour personnaliser davantage votre notification push, choisissez une URL **[!UICONTROL Image de Launch]** à ajouter à votre notification push.

1. Définissez la **[!UICONTROL durée du retardateur]** en secondes ou l’**[!UICONTROL horodatage de fin du retardateur]** sur un horodatage d’époque spécifique.

   ![Écran des paramètres de durée du minuteur](assets/rich_push_ios_timer_3.png)

1. Saisissez le texte et l’image qui s’afficheront après l’expiration du minuteur dans les champs **[!UICONTROL Titre secondaire]**, **[!UICONTROL Message secondaire]** et **[!UICONTROL Image de lancement secondaire]**.

   ![Autre écran des paramètres du message](assets/rich_push_ios_timer_4.png)

1. Dans la liste déroulante **[!UICONTROL Paramètres avancés]**, accédez à l’onglet **[!UICONTROL Son et pastille]** pour personnaliser des paramètres supplémentaires tels que les options de son et de pastille pour vos notifications. [En savoir plus](#sound-badge)

1. Dans le menu **[!UICONTROL Options de couleur]**, saisissez des codes couleur hexadécimaux pour les **[!UICONTROL Couleur d’arrière-plan de la notification]**, **[!UICONTROL Couleur d’arrière-plan de la notification]** et **[!UICONTROL Couleur du texte du message]**.

1. Pour une personnalisation plus poussée, explorez les options **[!UICONTROL supplémentaires]** disponibles pour vos notifications push. [En savoir plus](#push-advanced)

1. Dans le menu **[!UICONTROL Variables de l’application]**, vos **[!UICONTROL variables d’application]** sont automatiquement ajoutées. Elles permettent de définir le comportement des notifications, par exemple lors de la configuration d&#39;un écran spécifique à afficher lorsque l&#39;utilisateur active la notification.

Une fois que vous avez défini le contenu de votre message, utilisez tester les abonnés et abonnées pour prévisualiser et tester le message.

>[!ENDTABS]

## Paramètres avancés des notifications push {#push-advanced}

### Options de son et pastille {#sound-badge}

| Paramètre | Description |
|-----------|-------------|
| **[!UICONTROL Mode d’alerte critique]** | Activez cette option pour ajouter du son à votre notification, même si le téléphone de l’utilisateur est en mode thème ou en mode silencieux. |
| **[!UICONTROL Actualiser la pastille]** | Activez cette option pour actualiser la valeur du badge. |
| **[!UICONTROL Son]** | Définissez le son à émettre lorsque l’appareil reçoit votre notification. |
| **[!UICONTROL Nombre de notifications]** | Définissez un nombre à afficher directement sur l’icône de l’application, indiquant le nombre de nouvelles notifications non lues. |
| **[!UICONTROL Volume]** | Réglez le volume de votre son de 0 à 100. Les sons doivent être inclus dans l’application et définis lors de la création du service. |

### Options de couleur {#color}

| Paramètre | Description |
|-----------|-------------|
| **[!UICONTROL Couleur d’arrière-plan de la notification]** | Définissez la couleur de l’arrière-plan de votre notification à l’aide des codes couleur hexadécimaux. |
| **[!UICONTROL Couleur du titre]** | Définissez la couleur de votre titre à l’aide des codes couleur hexadécimaux. |
| **[!UICONTROL Couleur du texte de message]** | Définissez la couleur de votre texte à l’aide des codes couleur hexadécimaux. |

### Options avancées {#notification-options}

| Paramètre | Description |
|-----------|-------------|
| **[!UICONTROL Contenu modifiable]** | Activez cette option pour permettre à l’application mobile de télécharger le contenu multimédia. |
| **[!UICONTROL Score de pertinence]** | Définissez un score de pertinence compris entre 0 et 100. Le système l’utilise pour trier les notifications dans le résumé de la notification. |
| **[!UICONTROL Niveau d&#39;interruption]** | <ul><li>**Actif** : défini par défaut, le système présente immédiatement la notification, illumine l’écran et peut émettre un son. Les notifications ne passent pas en mode thème.</li><li>**Passif** : le système ajoute la notification à la liste de notifications sans allumer l’écran ni émettre de son. Les notifications ne passent pas en mode thème.</li><li>**Sensible à l’heure** : le système présente immédiatement la notification, allume l’écran, peut émettre un son et passe en mode Concentration. Ce niveau ne nécessite pas d’autorisation spéciale de la part d’Apple.</li><li>**Critique** : le système présente immédiatement la notification, allume l’écran et contourne le bouton de désactivation ou le mode Concentration. Notez que ce niveau nécessite une autorisation spéciale de la part d’Apple.</li></ul> |
| **[!UICONTROL Thread-id]** | Définissez l’identifiant utilisé pour regrouper les notifications associées. |
| **[!UICONTROL Catégorie]** | Définissez le nom de votre ID de catégorie qui affichera les boutons d’action. Ces notifications permettent à la personne d’effectuer plus rapidement différentes tâches en réponse à une notification, sans ouvrir l’application ou la parcourir. |
| **[!UICONTROL Identifiant du contenu Target]** | Définissez l’identifiant utilisé pour cibler la fenêtre d’application qui est avancée à l’ouverture de la notification. |