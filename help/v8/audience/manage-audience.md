---
audience: end-user
title: Commencer avec les audiences
description: Découvrez comment utiliser des audiences dans Adobe Campaign Web
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: b330230a031a366b674ebac37681274ee89ec6c8
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 95%

---

# Commencer avec les audiences {#monitor-manage}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Propriétés"
>abstract="Vous trouverez ici un résumé des propriétés d’une audience, telles que son origine ou son dossier de stockage. Cliquez sur le lien dans la section **Dernier workflow** pour ouvrir le workflow qui a été utilisé pour créer l’audience."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Taille de l’audience"
>abstract="Vous trouverez ici le nombre total de profils que comporte l’audience. Cliquez sur le bouton **Calculer** pour mettre à jour et recalculer les résultats de l’audience."

>[!CONTEXTUALHELP]
>id="acw_audiences_targeting"
>title="Ciblage"
>abstract="Ciblage"

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Erreur d’audience"
>abstract="Données d’audience non disponibles Attendez la fin de l’exécution du workflow."

L’audience est la cible principale de votre diffusion : il s’agit des profils qui reçoivent les messages. La liste des audiences disponibles dans Campaign Web est accessible à partir du menu **[!UICONTROL Audiences]**.

![Capture d’écran affichant la liste des audiences disponibles dans Campaign Web.](assets/audiences-list.png){zoomable="yes"}

Les audiences peuvent provenir de plusieurs sources. La colonne **[!UICONTROL Origine]** indique l’emplacement de création d’une audience donnée :

* **[!UICONTROL Adobe Campaign]** : ces audiences ont été créées dans l’[interface d’utilisation d’Adobe Campaign Web](create-audience.md) ou dans la [console cliente d’Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=fr){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform :]** ces audiences ont été créées dans Adobe Experience Platform et intégrées à Campaign Web à l’aide de l’intégration sources et destinations d’Adobe. Découvrez comment configurer cette intégration dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=fr){target="_blank"}.

  ➡️ [Découvrez cette fonctionnalité en vidéo](#video)

Pour obtenir plus d’informations sur une audience, ouvrez-la dans la liste. Les propriétés de l’audience s’affichent, avec le nombre de profils inclus dans l’audience. Actualisez la taille de l’audiences à tout moment à l’aide du bouton **[!UICONTROL Calculer]**.

Pour prévisualiser le schéma temporaire d’une audience, cliquez sur le bouton **[!UICONTROL Aperçu du schéma]** sous la section Propriétés .

L’onglet **[!UICONTROL Données]** vous permet de visualiser les profils qui font partie de l’audience. Personnalisez cette vue en ajoutant d’autres colonnes ou utilisez des filtres avancés pour affiner les données affichées.

![Capture d’écran affichant les détails de l’audience, y compris les profils et les options de personnalisation.](assets/audiences-details.png){zoomable="yes"}

Pour dupliquer ou supprimer une audience, cliquez sur le bouton **[!UICONTROL Plus d’actions]** disponible dans la liste des audiences, en regard du nom de l’audience ou dans un écran détaillé de l’audience.

## Vidéo pratique {#video}

Découvrez comment créer une destination pour utiliser une audience Experience Platform dans l’interface utilisateur web d’Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Vous trouverez des informations détaillées sur la configuration de l’intégration Sources et destinations d’Adobe dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=fr){target="_blank"}.