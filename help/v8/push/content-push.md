---
audience: end-user
title: Concevoir une diffusion de notification push
description: Découvrez comment concevoir une diffusion de notification push avec Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: a9c9079a64dd7113aa7da1040aa30cef2c9c0aec
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 29%

---

# Concevoir une diffusion push {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Contenu de notification push pour Android"
>abstract="Définissez le contenu de la notification push Android."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Contenu de notification push pour iOS"
>abstract="Définissez le contenu de la notification push iOS."

## Message {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Firebase Cloud Messaging vous permet de choisir entre deux types de messages :

* Le **[!UICONTROL Message de données]e** est géré par l’application cliente. Ces messages sont envoyés directement à l’application mobile, qui génère et affiche une notification Android sur l’appareil. Les messages de données contiennent uniquement vos variables d&#39;application personnalisées.

  Pour définir le contenu, personnaliser les données et ajouter du contenu dynamique, cliquez sur l’icône **[!UICONTROL Message]** et utilisez l’éditeur d’expression. Vous pouvez accéder à cet éditeur pour personnaliser vos messages Dans **[!UICONTROL Variables d’application]** , vos variables d’application sont automatiquement ajoutées. Ces variables vous permettent de définir le comportement des notifications. Vous pouvez par exemple paramétrer un écran d&#39;application spécifique qui s&#39;affichera lorsque l&#39;utilisateur activera la notification.

  ![](assets/push_content_4.png)

* Le **[!UICONTROL Message de notification]**, géré automatiquement par le SDK FCM. FCM affiche automatiquement le message sur les appareils de vos utilisateurs pour le compte de l’application cliente. Les messages de notification contiennent un ensemble de paramètres et d&#39;options prédéfini, mais peuvent encore être personnalisés avec des variables d&#39;application personnalisées.

  Pour composer votre message, cliquez sur le bouton **[!UICONTROL Titre]** et **[!UICONTROL Corps]** champs. Utilisez l&#39;éditeur d&#39;expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique.

  Pour personnaliser davantage votre notification push, vous pouvez choisir une image à ajouter à votre notification push, l&#39;icône de la notification qui s&#39;affichera sur les appareils de vos profils et sa couleur.

  ![](assets/push_content_3.png)

>[!TAB iOS]

Pour composer votre message, cliquez sur le bouton **[!UICONTROL Titre]** et **[!UICONTROL Corps]** champs. Utilisez l&#39;éditeur d&#39;expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique.

Vous pouvez ajouter un **[!UICONTROL Sous-titre]**, valeur du paramètre sous-titre de la payload de notification iOS. Consultez cette section.

Le mode Silent push permet d&#39;envoyer une notification &quot;silencieuse&quot; à une application mobile. L’utilisateur n’est pas averti de l’arrivée de la notification. Elle est directement transférée à l&#39;application.

![](assets/push_content_1.png)

>[!ENDTABS]

## Paramètres avancés {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

![](assets/push_content_5.png)

| Paramètre | Description |
|---------|---------|
| **[!UICONTROL Son]** | Définissez le son à émettre lorsque l’appareil reçoit votre notification. |
| **[!UICONTROL Nombre de notifications]** | Définissez le nombre de nouvelles informations non lues à afficher directement sur l’icône de l’application. Cela permet à l’utilisateur de voir rapidement le nombre de notifications en attente. |
| **[!UICONTROL Identifiant du canal]** | Définissez l&#39;identifiant de canal de votre notification. L&#39;application doit créer un canal avec cet identifiant de canal avant la réception d&#39;une notification avec cet identifiant de canal. |
| **[!UICONTROL Action de clic]** | Définissez l&#39;action associée à un clic de l&#39;utilisateur sur votre notification. Cela détermine le comportement lorsque l’utilisateur interagit avec la notification, par exemple en ouvrant un écran spécifique ou en effectuant une action spécifique dans votre application. |
| **[!UICONTROL Balise]** | Définissez un identifiant utilisé pour remplacer les notifications existantes dans le tiroir de notifications. Cela permet d’éviter l’accumulation de plusieurs notifications et de s’assurer que seule la dernière notification pertinente est affichée. |
| **[!UICONTROL Priorité]** | Définissez le niveau de priorité de votre notification, qui peut être par défaut, minimum, faible ou élevé. Le niveau de priorité détermine l’importance et l’urgence de la notification, influençant son affichage et le fait qu’elle puisse contourner certains paramètres système. Pour plus d&#39;informations à ce propos, consultez la [documentation FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilité]** | Définissez le niveau de visibilité de votre notification, qui peut être publique, privée ou secrète. Le niveau de visibilité détermine la quantité de contenu de la notification qui s&#39;affiche sur l&#39;écran de verrouillage et dans d&#39;autres zones sensibles. Pour plus d’informations, reportez-vous à la section [Documentation FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Épinglé]** | Lorsqu&#39;elle est activée, la notification reste visible même après que l&#39;utilisateur a cliqué dessus. <br>Si cette option est désactivée, la notification est automatiquement ignorée lorsque l’utilisateur interagit avec celle-ci. Le comportement bascule permet à des notifications importantes de persister pendant de plus longues périodes à l’écran. |
| **[!UICONTROL Variables de l&#39;application]** | Permet de définir le comportement des notifications. Ces variables sont entièrement personnalisables et incluses dans la payload du message envoyée à l’appareil mobile. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Paramètre | Description |
|---------|---------|
| **[!UICONTROL Mode d’alerte critique]** | Activez cette option pour ajouter du son à votre notification, même si le téléphone de l&#39;utilisateur est en mode focus ou si iPhone est en mode muet. Cela permet de s’assurer que les alertes importantes sont remarquées par l’utilisateur. |
| **[!UICONTROL Nettoyer la pastille]** | Activez cette option pour actualiser la valeur du badge affichée sur l’icône de l’application. Cela permet de s’assurer que le badge reflète exactement le nombre de nouvelles informations non lues. |
| **[!UICONTROL Nombre de notifications]** | Définissez un nombre qui s’affichera directement sur l’icône de l’application, indiquant le nombre de nouvelles informations non lues. Vous obtenez ainsi une référence visuelle rapide pour l’utilisateur. |
| **[!UICONTROL Volume]** | Volume de votre son de 0 à 100. |
| **[!UICONTROL Contenu mutable]** | Activez cette option pour permettre à l&#39;application mobile de télécharger le contenu multimédia associé à la notification. Consultez à ce sujet la [Documentation développeur Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Score de pertinence]** | Définissez un score de pertinence compris entre 0 et 100 pour classer par priorité l’ordre des notifications dans la synthèse des notifications. Des scores plus élevés indiquent des notifications plus importantes. |
| **[!UICONTROL Niveau d&#39;interruption]** | <ul> <li>**[!UICONTROL Actif]** : défini par défaut, le système présente immédiatement la notification, illumine l’écran et peut émettre un son. Les notifications ne passent pas en mode Thème.</li><li>**[!UICONTROL Passif]** : le système ajoute la notification à la liste de notifications sans allumer l’écran ni émettre de son. Les notifications ne passent pas en mode Thème.</li><li>**[!UICONTROL Sensible à l’heure]** : le système présente immédiatement la notification, allume l’écran, peut émettre un son et passer en mode Concentration. Ce niveau ne nécessite pas d’autorisation spéciale de la part d’Apple.</li> <li>**[!UICONTROL Critique]** : le système présente immédiatement la notification, allume l’écran et contourne le bouton de désactivation ou le mode Concentration. Notez que ce niveau nécessite une autorisation spéciale de la part d’Apple.</ul> |
| **[!UICONTROL Thread-id]** | Identifiant utilisé pour regrouper les notifications associées. Les notifications avec le même identifiant de thread sont organisées en tant que conversation ou thread unique dans la liste de notifications. |
| **[!UICONTROL Catégorie]** | Indiquez le nom de l&#39;ID de catégorie associé à la notification. Cela permet d&#39;afficher des boutons d&#39;action, permettant à l&#39;utilisateur d&#39;effectuer différentes tâches directement depuis la notification sans ouvrir l&#39;application. |
| **[!UICONTROL Identifiant du contenu Target]** | Identifiant utilisé pour cibler la fenêtre d&#39;application à transférer à l&#39;ouverture de la notification. |
| **[!UICONTROL Image de Launch]** | Indiquez le nom du fichier image de lancement à afficher lorsque l’utilisateur choisit de lancer votre application à partir de la notification. L’image sélectionnée s’affiche au lieu de l’écran de lancement standard de votre application. |
| **[!UICONTROL Variables de l&#39;application]** | Permet de définir le comportement des notifications. Ces variables sont entièrement personnalisables et incluses dans la payload du message envoyée à l’appareil mobile. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



