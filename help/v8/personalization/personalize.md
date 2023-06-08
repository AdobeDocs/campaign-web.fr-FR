---
title: Personnaliser votre contenu dans Campaign
description: Découvrez comment personnaliser votre contenu dans l’interface utilisateur web d’Adobe Campaign.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 551e6b9efa8b29475bd2f0a71ce016681bf70289
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 7%

---


# Personnaliser votre contenu {#add-personalization}

La personnalisation peut être ajoutée à n’importe quelle diffusion à l’aide de l’éditeur d’expression, accessible dans tous les champs de la fonction **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]** par exemple, le champ de ligne d’objet ou les liens d’e-mail et les composants de contenu texte/bouton. [Découvrez où ajouter du contenu dynamique](gs-personalization.md/#access)

## Syntaxe de la personnalisation {#syntax}

Une balise de personnalisation utilise toujours la syntaxe suivante : `<%=table.field%>`. Par exemple, pour insérer le nom du destinataire, stocké dans la table des destinataires, la balise de personnalisation utilise la syntaxe &lt;%= recipient.lastName %> .

Lors de la préparation d&#39;une diffusion, ces balises sont automatiquement interprétées par Adobe Campaign et remplacées par la valeur du champ pour un destinataire donné. Le remplacement physique peut ensuite être visualisé lors de la simulation de votre contenu.

## Ajout de balises de personnalisation {#add}

Pour ajouter des balises de personnalisation dans une diffusion, ouvrez l’éditeur d’expression à l’aide du **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]** icône accessible à partir des champs de modification de type texte, tels que l’objet ou le corps du SMS. [Découvrez où ajouter du contenu dynamique](gs-personalization.md/#access)

![](assets/perso-access.png)

L’éditeur d’expression s’affiche. Les champs de personnalisation sont organisés en plusieurs menus, situés à gauche de l&#39;écran. Ces menus donnent accès à tous les champs disponibles dans la base de données Adobe Campaign.

![](assets/perso-insert-field.png)

| Menu | Description |
|-----|------------|
| ![](assets/do-not-localize/perso-subscribers-menu.png) | Le **[!UICONTROL Application d’abonnements]** répertorie tous les champs liés aux abonnés d’une application, tels que le terminal ou le système d’exploitation utilisé. *Ce menu est disponible uniquement pour les notifications push* |
| ![](assets/do-not-localize/perso-recipients-menu.png) | Le **[!UICONTROL Destinataire]** répertorie tous les champs définis dans la table des destinataires, tels que le nom, l’âge ou l’adresse du destinataire. |
| ![](assets/do-not-localize/perso-message-menu.png) | Le **[!UICONTROL Message]** menu répertorie tous les champs liés aux logs de diffusion, c’est-à-dire tous les messages envoyés aux destinataires ou aux appareils sur tous les canaux, comme la date du dernier événement avec un destinataire donné. |
| ![](assets/do-not-localize/perso-delivery-menu.png) | Le **[!UICONTROL Diffusion]** répertorie tous les champs relatifs aux paramètres requis pour effectuer des diffusions, tels que le canal de diffusion, le libellé, etc. |

>[!NOTE]
>
>Par défaut, chaque menu affiche tous les champs de la table sélectionnée (Destinataires / Message / Diffusion). Si vous souhaitez inclure des champs issus de tables liées à la table sélectionnée, activez l’option **[!UICONTROL Afficher les attributs avancés]** située sous la liste.

Pour ajouter un champ de personnalisation, placez le curseur à l’emplacement souhaité dans votre contenu, puis cliquez sur le bouton + pour l’insérer.

Une fois votre contenu prêt, vous pouvez l’enregistrer et tester le rendu de la personnalisation en simulant votre contenu. Dans l&#39;exemple ci-dessous, nous personnalisons un SMS avec les prénoms des profils ciblés.

*Ajouter la balise de personnalisation dans le contenu du message*

![](assets/perso-preview1.png)

*Simuler le rendu de la personnalisation pour un profil de test donné*

![](assets/perso-preview2.png)
