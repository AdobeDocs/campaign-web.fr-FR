---
title: Personnaliser votre contenu dans Campaign
description: Découvrez comment personnaliser votre contenu dans l’interface utilisateur web d’Adobe Campaign.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 100%

---


# Personnaliser votre contenu {#add-personalization}

Vous pouvez personnaliser n’importe quelle diffusion à l’aide de l’éditeur d’expression, accessible dans les champs de l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]**, comme l’objet, les liens d’e-mail et les composants de contenu texte/bouton. [Découvrez comment accéder à l’éditeur d’expression](gs-personalization.md/#access).

## Syntaxe de la personnalisation {#syntax}

Les balises de personnalisation suivent une syntaxe spécifique : `<%= table.field %>`. Par exemple, pour insérer le nom de la personne destinataire dans le tableau des destinataires, utilisez la syntaxe `<%= recipient.lastName %>`.

Pendant le processus de préparation de la diffusion, Adobe Campaign interprète automatiquement ces balises et les remplace par les valeurs de champ correspondantes pour chaque destinataire. Vous pouvez visualiser le remplacement réel en simulant votre contenu.

Lors du téléchargement de contacts depuis un fichier externe pour une diffusion e-mail autonome, tous les champs du fichier d’entrée peuvent être personnalisés. La syntaxe est la suivante : `<%= dataSource.field %>`.

## Ajouter des balises de personnalisation {#add}

Pour ajouter des balises de personnalisation dans une diffusion, procédez comme suit :

1. Ouvrez l’éditeur d’expression à l’aide de l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]** accessible à partir des champs de modification de type texte, tels que l’objet ou le corps du SMS. [Découvrez comment accéder à l’éditeur d’expression](gs-personalization.md/#access).

   ![](assets/perso-access.png){width="800" align="center"}

1. L’éditeur d’expression s’ouvre. Les champs de personnalisation disponibles dans la base de données d’Adobe Campaign sont organisés en plusieurs menus dans la partie gauche de l’écran :

   ![](assets/perso-insert-field.png){width="800" align="center"}

   | Menu | Description |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png) | Le menu **[!UICONTROL Application des abonnées et abonnés]** répertorie les champs liés aux abonnées et abonnés d’une application, tels que le terminal utilisé ou le système d’exploitation. *Ce menu est disponible uniquement pour les notifications push*. |
   | ![](assets/do-not-localize/perso-recipients-menu.png) | Le menu **[!UICONTROL Destinataire]** répertorie les champs définis dans le tableau des destinataires, tels que les noms, âges ou adresses des destinataires. Lors du [téléchargement des contacts depuis un fichier externe](../audience/file-audience.md) pour une diffusion e-mail autonome, ce menu répertorie tous les champs disponibles dans le fichier d’entrée. |
   | ![](assets/do-not-localize/perso-message-menu.png) | Le menu **[!UICONTROL Message]** répertorie les champs liés aux logs de diffusion, y compris tous les messages envoyés aux destinataires ou aux appareils sur tous les canaux, comme la date du dernier événement avec une personne destinataire donnée. |
   | ![](assets/do-not-localize/perso-delivery-menu.png) | Le menu **[!UICONTROL Diffusion]** répertorie les champs liés aux paramètres requis pour effectuer des diffusions, tels que le canal ou le libellé de la diffusion. |

   >[!NOTE]
   >
   >Par défaut, chaque menu répertorie tous les champs du tableau sélectionné (Destinataires/Message/Diffusion). Si vous souhaitez inclure des champs issus de tableaux liées au tableau sélectionné, activez l’option **[!UICONTROL Afficher les attributs avancés]** située sous la liste.

1. Pour ajouter un champ de personnalisation, positionnez-vous à l’emplacement souhaité dans votre contenu, puis cliquez sur le bouton `+` pour l’insérer.

1. Une fois votre contenu prêt, vous pouvez l’enregistrer et tester le rendu de la personnalisation en simulant votre contenu. L’exemple ci-dessous illustre la personnalisation d’un SMS avec les prénoms des destinataires.

   ![](assets/perso-preview1.png){width="800" align="center"}

   ![](assets/perso-preview2.png){width="800" align="center"}
