---
title: Personnaliser votre contenu dans Campaign
description: Découvrez comment personnaliser votre contenu dans l’interface utilisateur web d’Adobe Campaign.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: d12c3019fb47164864259ecc40225fcb04de0e6c
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 8%

---


# Personnaliser votre contenu{#add-personalization}

La personnalisation peut être ajoutée à n&#39;importe quelle diffusion à l&#39;aide de l&#39;éditeur d&#39;expression.

Une balise de personnalisation utilise toujours la syntaxe suivante : `<%=table.field%>`.Par exemple, pour insérer le nom du destinataire, stocké dans la table des destinataires, la balise de personnalisation utilise la syntaxe &lt;%= recipient.lastName %> .

Lors de la préparation d&#39;une diffusion, ces balises sont automatiquement interprétées par Adobe Campaign et remplacées par la valeur du champ pour un destinataire donné. Le remplacement physique peut ensuite être visualisé lors de la simulation de votre contenu.

Pour ajouter des balises de personnalisation dans une diffusion, cliquez sur l&#39;icône Ouvrir la boîte de dialogue de personnalisation accessible à partir des champs d&#39;édition de type texte, tels que la ligne d&#39;objet ou le corps du SMS.

![](assets/perso-access.png)

L’éditeur d’expression s’affiche. Les champs de personnalisation sont organisés en trois menus, situés à gauche de l&#39;écran. Ces menus donnent accès à tous les champs disponibles dans la base de données Adobe Campaign.

| Menu | Description |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | Le **[!UICONTROL Destinataire]** répertorie tous les champs définis dans la table des destinataires, tels que le nom, l’âge ou l’adresse du destinataire. |
| ![](assets/do-not-localize/perso-message-menu.png) | Le **[!UICONTROL Message]** menu répertorie tous les champs liés aux logs de diffusion, c’est-à-dire tous les messages envoyés aux destinataires ou aux appareils sur tous les canaux, comme la date du dernier événement avec un destinataire donné. |
| ![](assets/do-not-localize/perso-delivery-menu.png) | Le **[!UICONTROL Diffusion]** répertorie tous les champs relatifs aux paramètres requis pour effectuer des diffusions, tels que le canal de diffusion, le libellé, etc. |

>[!NOTE]
>
>Par défaut, la liste affiche tous les champs de la table sélectionnée (Destinataires / Message / Diffusion). Si vous souhaitez inclure des champs issus de tables liées à la table sélectionnée, activez l’option **[!UICONTROL Afficher les attributs avancés]** située sous la liste.

Pour ajouter un champ de personnalisation, placez le curseur à l’emplacement souhaité dans votre contenu, puis cliquez sur le bouton + pour l’insérer.

![](assets/perso-insert-field.png)
