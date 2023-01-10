---
audience: end-user
title: Tracker les messages
description: Découvrez comment ajouter des liens et tracker les messages envoyés.
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: c1d433ba1d12e840c5ae219b319e80c1bcdc7686
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 92%

---

# Ajouter des liens et tracker les messages {#tracking}

>[!NOTE]
>
>Cette documentation est en cours d’élaboration et est fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

Utilisez le Concepteur d’e-mail pour ajouter des liens à votre contenu et tracker les messages envoyés afin de surveiller le comportement de vos destinataires.

## Insérer des liens {#insert-links}

Lors de la conception d’un message, vous pouvez ajouter des liens à votre contenu.

>[!NOTE]
>
>Lorsque le tracking est activé, tous les liens inclus dans le contenu du message sont trackés.

Pour insérer des liens dans le contenu de votre e-mail, procédez comme suit :

1. Sélectionnez un élément et cliquez sur **[!UICONTROL Insérer un lien]** dans la barre d’outils contextuelle.

   ![](assets/message-tracking-insert-link.png)

1. Ajoutez un **[!UICONTROL Libellé]** et un **[!UICONTROL Lien]**.

1. Enregistrez vos modifications.

1. Une fois le lien créé, vous pouvez encore le modifier à partir du volet **[!UICONTROL Paramètres des composants]** à droite.

   * Vous pouvez modifier le lien ainsi que sa **[!UICONTROL Cible]**.
   * Vous pouvez choisir de souligner le lien en cochant l’option correspondante.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>Les e-mails de type marketing doivent inclure un lien d’exclusion, qui n’est pas obligatoire pour les messages transactionnels. La catégorie du message (**[!UICONTROL Marketing]** ou **[!UICONTROL Transactionnel]**) est définie au niveau de la surface du canal (c’est-à-dire le paramètre prédéfini du message) et lors de la création du message.

## Lien vers une page miroir {#mirror-page}

La page miroir est une page HTML accessible en ligne via un navigateur web. Son contenu est identique à celui de l’e-mail.

Pour ajouter un lien vers une page miroir dans l’e-mail :

1. Sélectionnez un élément et cliquez sur **[!UICONTROL Insérer un lien]** dans la barre d’outils contextuelle.

   ![](assets/message-tracking-mirror-page.png)

1. Sélectionnez l’icône **[!UICONTROL Insérer un lien]** pour accéder au menu de personnalisation.

   ![](assets/message-tracking-mirror-page_2.png)

1. Dans le menu **[!UICONTROL Bloc de contenu]**, sélectionnez **[!UICONTROL URL de la page miroir]** et cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/message-tracking-mirror-page_3.png)

La page miroir est automatiquement créée.

>[!IMPORTANT]
>
>Les liens de pages miroir sont générés automatiquement et ne peuvent pas être modifiés. Ils contiennent toutes les données personnalisées chiffrées requises pour générer l’e-mail original. Par conséquent, l’utilisation d’attributs personnalisés avec des valeurs élevées peut générer de longues URL de pages miroir. Cela peut empêcher le lien de fonctionner dans les navigateurs web qui imposent des limites de longueur d’URL.

Une fois l’e-mail envoyé, lorsque les destinataires cliquent sur le lien de la page miroir, le contenu de l’e-mail s’affiche dans leur navigateur web par défaut.

>[!NOTE]
>
>Dans le BAT envoyé aux profils de test, le lien vers la page miroir est inactif. Il n’est actif que dans les messages finaux.

La période de conservation d’une page miroir est de 60 jours. Une fois ce délai écoulé, la page miroir n’est plus disponible.

## Gérer le tracking {#manage-tracking}

Le [Concepteur d’e-mail](create-email-content.md) permet de gérer les URL trackées : par exemple, vous pouvez modifier le type de tracking de chaque lien.

1. Cliquez sur l’icône **[!UICONTROL Liens]** dans le volet de gauche pour afficher la liste de toutes les URL du contenu qui feront l’objet d’un tracking.

   Cette liste permet d’avoir une vue centrale et de localiser chaque URL dans le contenu de l’e-mail.

1. Pour éditer un lien, cliquez sur l’icône représentant un crayon correspondante.

   ![](assets/message-tracking-edit-links.png)

1. Vous pouvez modifier le **[!UICONTROL Type de tracking]** si nécessaire :

   ![](assets/message-tracking-edit-a-link.png)

   Pour chaque URL trackée, vous pouvez définir le mode de tracking sur l’une des valeurs suivantes :

   * **[!UICONTROL Trackée]** : active le tracking de cette URL.
   * **[!UICONTROL Exclusion]** : traite cette URL comme une URL d’exclusion ou de désinscription.
   * **[!UICONTROL Page miroir]** : traite cette URL comme une URL de page miroir.
   * **[!UICONTROL Jamais]** : n’active jamais le tracking de cette URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Ajouter un **[!UICONTROL Catégorie]** à votre lien pour regrouper les liens trackés, puis cliquez sur **[!UICONTROL Enregistrer]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. Une fois votre diffusion envoyée, accédez à votre rapport de diffusion. Sous , **[!UICONTROL Tracking]** , **[!UICONTROL URL et flux de clics]** Le rapport affiche les URL de votre diffusion les plus visitées. [En savoir plus](../reporting/reports.md)
