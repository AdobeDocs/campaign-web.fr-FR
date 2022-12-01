---
audience: end-user
title: Tracker vos messages
description: Découvrez comment ajouter des liens et suivre les messages envoyés
source-git-commit: 9def5ea791e4ef42968cd34536f3ddeac7fc238c
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 8%

---


# Ajout de liens et suivi des messages {#tracking}

>[!NOTE]
>
>Cette documentation est en cours de construction et fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

Utilisation [!DNL Journey Optimizer] pour ajouter des liens à votre contenu et suivre les messages envoyés afin de suivre le comportement de vos destinataires.

## Activer le tracking {#enable-tracking}

Vous pouvez activer le tracking au niveau des emails en cochant la case **[!UICONTROL Ouverture d’email]** et/ou **[!UICONTROL Clic sur l’email]** lors de la création de votre message.

![](assets/message-tracking.png)

>[!NOTE]
>
>Les deux options sont activées par défaut.

Vous pourrez ainsi tracker le comportement de vos destinataires par :

* **[!UICONTROL Ouverture d’email]**: Messages ouverts.
* **[!UICONTROL Clic sur l’email]**: Clics sur les liens d’un email.

## Insérer des liens {#insert-links}

Lors de la conception d&#39;un message, vous pouvez ajouter des liens à votre contenu.

>[!NOTE]
>
>When [suivi activé](#enable-tracking), tous les liens inclus dans le contenu du message sont suivis.

Pour insérer des liens dans le contenu de votre email, procédez comme suit :

1. Sélectionnez un élément et cliquez sur **[!UICONTROL Insérer un lien]** dans la barre d&#39;outils contextuelle.

   ![](assets/message-tracking-insert-link.png)

1. Sélectionnez le type de lien que vous souhaitez créer :

   * **[!UICONTROL Lien externe]**: Insérez un lien vers une URL externe.

   * **[!UICONTROL Landing page]**: Insérez un lien vers une landing page.

   * **[!UICONTROL Exclusion en un clic]**: Insérez un lien pour permettre aux utilisateurs de se désabonner rapidement de vos communications sans avoir à confirmer leur désinscription.

   * **[!UICONTROL Abonnement/Opt-in externe]**: Insérez un lien pour accepter la réception de communications de votre marque.

   * **[!UICONTROL Désinscription/désinscription externe]**: Insérez un lien pour vous désabonner de la réception des communications de votre marque.

   * **[!UICONTROL Page miroir]**: Insérez un lien pour afficher le contenu de l&#39;email dans un navigateur web. En savoir plus dans [cette section](#mirror-page).

   ![](assets/message-tracking-links.png)

1. Vous pouvez personnaliser vos liens.

1. Enregistrez vos modifications.

1. Une fois le lien créé, vous pouvez toujours le modifier à partir de la fonction **[!UICONTROL Paramètres des composants]** sur la droite.

   * Vous pouvez éditer le lien et en modifier le type.
   * Vous pouvez souligner le lien ou non en cochant l&#39;option correspondante.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>Les messages électroniques de type marketing doivent inclure un lien d’exclusion, qui n’est pas obligatoire pour les messages transactionnels. La catégorie du message (**[!UICONTROL Marketing]** ou **[!UICONTROL Transactionnel]**) est défini à la surface du canal (c’est-à-dire au niveau du paramètre prédéfini du message) et lors de la création du message.

## Lien vers une page miroir {#mirror-page}

La page miroir est une page HTML accessible en ligne depuis un navigateur web. Son contenu est identique à celui de votre email.

Pour ajouter un lien vers une page miroir dans votre email, [insérer un lien](#insert-links) et sélectionnez **[!UICONTROL Page miroir]** comme type de lien.

![](assets/message-tracking-mirror-page.png)

La page miroir est automatiquement créée.

>[!IMPORTANT]
>
>Les liens de pages miroir sont générés automatiquement et ne peuvent pas être modifiés. Ils contiennent toutes les données personnalisées chiffrées requises pour générer l’email d’origine. Par conséquent, l’utilisation d’attributs personnalisés avec des valeurs élevées peut générer de longues URL de pages miroir, ce qui peut empêcher le fonctionnement du lien dans les navigateurs web dont la longueur est maximale.

Une fois l&#39;email envoyé, lorsque les destinataires cliquent sur le lien de la page miroir, le contenu de l&#39;email s&#39;affiche dans leur navigateur web par défaut.

>[!NOTE]
>
>Dans le BAT envoyé aux profils de test, le lien vers la page miroir n&#39;est pas principal. Elle n’est activée que dans les messages finaux.

La période de conservation d’une page miroir est de 60 jours. Après ce délai, la page miroir ne sera plus disponible.

## Gestion du suivi {#manage-tracking}

Le [Concepteur d&#39;email](create-email-content.md) permet de gérer les URL trackées, comme par exemple de modifier le type de suivi pour chaque lien.

1. Cliquez sur le bouton **[!UICONTROL Liens]** dans le volet de gauche pour afficher la liste de toutes les URL de votre contenu qui seront trackées.

   Cette liste permet d&#39;avoir une vue centrale et de localiser chaque URL dans le contenu de l&#39;email.

1. Pour éditer un lien, cliquez sur l&#39;icône de crayon correspondante.

   ![](assets/message-tracking-edit-links.png)

1. Vous pouvez modifier la variable **[!UICONTROL Type de suivi]** si nécessaire :

   ![](assets/message-tracking-edit-a-link.png)

   Pour chaque URL trackée, vous pouvez définir le mode de tracking sur l&#39;une de ces valeurs :

   * **[!UICONTROL Suivi]**: Active le tracking sur cette URL.
   * **[!UICONTROL Exclusion]**: Considère cette URL comme une URL d’opt-out ou de désabonnement.
   * **[!UICONTROL Page miroir]**: considère cette URL comme une URL de page miroir.
   * **[!UICONTROL Jamais]**: N’active jamais le suivi de cette URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

Les rapports sur les ouvertures et les clics sont disponibles dans le rapport En direct et dans le rapport Global .
