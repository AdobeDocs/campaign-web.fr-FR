---
audience: end-user
title: Concevoir une diffusion de notification push
description: Découvrez comment concevoir une diffusion de notification push avec Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 965c2d72d81233c98beb4e4bc3c76692c7bf3990
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 58%

---

# Concevoir une diffusion push {#content-push}

## Message {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Firebase Cloud Messaging vous permet de choisir entre deux types de messages :

* Le **Message de données**, géré par l’application cliente. Les messages sont envoyés directement à l&#39;application mobile qui génèrera et affichera la notification Android sur l&#39;appareil. Les messages de données contiennent uniquement vos variables d&#39;application personnalisées.

   Cliquez sur le bouton **[!UICONTROL Message]** et utiliser l&#39;éditeur d&#39;expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique.

* Le message de notification, géré automatiquement par le SDK FCM. FCM affiche automatiquement le message sur les appareils de vos utilisateurs pour le compte de l’application cliente. Les messages de notification contiennent un ensemble de paramètres et d&#39;options prédéfini, mais peuvent encore être personnalisés avec des variables d&#39;application personnalisées.

   Pour composer votre message, cliquez sur le bouton **[!UICONTROL Titre]** et **[!UICONTROL Corps]** champs. Utilisez l&#39;éditeur d&#39;expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique.

   Pour personnaliser davantage votre notification push, vous pouvez choisir une image à ajouter à votre notification push, l&#39;icône de la notification qui s&#39;affichera sur les appareils de vos profils et sa couleur.

>[!TAB iOS]

Pour composer votre message, cliquez sur le bouton **[!UICONTROL Titre]** et **[!UICONTROL Corps]** champs. Utilisez l&#39;éditeur d&#39;expression pour définir le contenu, personnaliser les données et ajouter du contenu dynamique.

Vous pouvez ajouter un **[!UICONTROL Sous-titre]**, valeur du paramètre sous-titre de la payload de notification iOS. Consultez cette section.

Le mode Silent push permet d&#39;envoyer une notification &quot;silencieuse&quot; à une application mobile. L’utilisateur n’est pas averti de l’arrivée de la notification. Elle est directement transférée à l&#39;application.

>[!ENDTABS]

## Paramètres avancés {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

* **[!UICONTROL Son]** : définissez le son à émettre lorsque l&#39;appareil reçoit votre notification.

* **[!UICONTROL Nombre de notifications]** : définissez le nombre de nouvelles informations non lues à afficher directement sur l&#39;icône de l&#39;application.

* **[!UICONTROL Identifiant de canal]**: Définissez l&#39;identifiant de canal de votre notification. L&#39;application doit créer un canal avec cet identifiant de canal avant la réception d&#39;une notification avec cet identifiant de canal.

* **[!UICONTROL Action de clic]** : définissez l&#39;action associée à un clic de l&#39;utilisateur sur votre notification.

* **[!UICONTROL Balise]** : définissez l&#39;identifiant utilisé pour remplacer les notifications existantes dans le tiroir de notifications.

* **[!UICONTROL Priorité des notifications]** : définissez les niveaux de priorité de votre sur &#39;par défaut&#39;, &#39;minimum&#39;, &#39;basse&#39; ou &#39;élevée&#39;. Pour plus d&#39;informations à ce propos, consultez la documentation FCM.

* **[!UICONTROL Visibilité]** : définissez les niveaux de visibilité de votre notification sur public, privé ou secret. Pour plus d&#39;informations à ce propos, consultez la documentation FCM.

* **[!UICONTROL Attractif]**: En cas de désactivation, la notification est automatiquement ignorée lorsque l&#39;utilisateur clique dessus. Si cette option est activée, la notification reste affichée même lorsque l&#39;utilisateur clique dessus.

>[!TAB iOS]

* **[!UICONTROL Mode d’alerte critique]**: activez cette option pour ajouter du son à votre notification, même si le téléphone de l&#39;utilisateur est en mode focus ou si iPhone est en mode silencieux.

* **[!UICONTROL Nettoyer la pastille]** : activez cette option pour actualiser la valeur de la pastille.

* **[!UICONTROL Nombre de notifications]**: définissez un nombre qui sera utilisé pour afficher directement sur l’icône de l’application le nombre de nouvelles informations non lues.

* **[!UICONTROL Volume]** : volume de votre son de 0 à 100.

* **[!UICONTROL Contenu mutable]** (iOS uniquement) : Envoie l’indicateur de contenu mutable dans la payload push et permettra de modifier le contenu de la notification push par une extension de l’application de service de notification fournie dans le SDK iOS. Consultez à ce sujet la [Documentation développeur Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). activez cette option pour permettre à l’application mobile de télécharger le contenu multimédia.

* **[!UICONTROL Score de pertinence]** : définissez un score de pertinence compris entre 0 et 100. Le système l’utilise pour trier les notifications dans le résumé de la notification.

* **[!UICONTROL Niveau d&#39;interruption]**:

   * **[!UICONTROL Actif]** : défini par défaut, le système présente immédiatement la notification, illumine l’écran et peut émettre un son. Les notifications ne passent pas en mode Thème.

   * **[!UICONTROL Passif]** : le système ajoute la notification à la liste de notifications sans allumer l’écran ni émettre de son. Les notifications ne passent pas en mode Thème.

   * **[!UICONTROL Sensible à l’heure]** : le système présente immédiatement la notification, allume l’écran, peut émettre un son et passer en mode Concentration. Ce niveau ne nécessite pas d’autorisation spéciale de la part d’Apple.

   * **[!UICONTROL Critique]** : le système présente immédiatement la notification, allume l’écran et contourne le bouton de désactivation ou le mode Concentration. Notez que ce niveau nécessite une autorisation spéciale de la part d’Apple.

* **[!UICONTROL Thread-id]** : identifiant utilisé pour regrouper les notifications associées.

* **[!UICONTROL Catégorie]** : nom de votre identifiant de catégorie qui affichera les boutons d’action. Ces notifications permettent à l&#39;utilisateur d&#39;effectuer plus rapidement différentes tâches en réponse à celles-ci, sans ouvrir l&#39;application ou la parcourir.

* **[!UICONTROL Identifiant du contenu Target]** : identifiant utilisé pour cibler la fenêtre d&#39;application à afficher au premier plan à l&#39;ouverture de la notification.

* **[!UICONTROL Image de Launch]** : nom du fichier image de Launch à afficher. Si l’utilisateur choisit de lancer l’application, l’image sélectionnée s’affiche au lieu de l’écran de lancement de l’application.

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



