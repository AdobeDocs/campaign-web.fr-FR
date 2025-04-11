---
audience: end-user
title: Filtrer des listes
description: Découvrez comment filtrer les listes Adobe Campaign Web à l’aide de filtres intégrés et personnalisés.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 65%

---

# Filtrer des listes {#filter-lists}

Adobe Campaign Web fournit des filtres dans chaque liste d’objets, ce qui vous permet de filtrer les informations en fonction de critères contextuels spécifiques. Par exemple, vous pouvez filtrer les diffusions en fonction de leur statut, de leur canal, de leur date de contact ou de leur dossier. Vous pouvez également masquer les BAT.

## Appliquer des filtres {#apply}

Pour appliquer des filtres à une liste, cliquez sur le bouton **[!UICONTROL Afficher les filtres]** situé dans le coin supérieur gauche de la liste, en regard de la barre de recherche.

Le volet des filtres s’ouvre, affichant les filtres disponibles pour la liste sélectionnée. Par exemple, vous pouvez filtrer les campagnes en fonction de leur statut, de leurs dates de début et de fin, ou de leur dossier de stockage, tandis que la liste des services d’abonnement peut être filtrée en fonction de leur canal et de leur dossier de stockage.

![Volet Filtres affichant les filtres disponibles pour les listes](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Pour filtrer une liste selon vos propres critères, créez un filtre personnalisé. Pour ce faire, accédez au bas du volet des filtres et cliquez sur le bouton **Ajouter des règles**. [Découvrez comment créer des filtres personnalisés](#custom).

Une fois appliqués à une liste, les filtres sont visibles dans la barre de recherche. Vous pouvez supprimer un filtre individuel à tout moment ou supprimer tous les filtres en cliquant sur le bouton **Tout effacer**.

## Créer des filtres personnalisés {#custom}

Les filtres personnalisés vous permettent d’affiner les listes en fonction de vos propres critères. Ils sont conçus à l’aide du concepteur de requête Campaign. Pour créer un filtre personnalisé, procédez comme suit :

1. Ouvrez le volet Filtres et cliquez sur le bouton **Ajouter des règles** situé en bas du volet.

1. Le concepteur de requête s’ouvre. Définissez et combinez vos critères de filtre en fonction de vos besoins. Des informations détaillées sur l’utilisation du concepteur de requête sont disponibles dans [cette section](../query/query-modeler-overview.md).

   L&#39;exemple ci-dessous montre un filtre personnalisé conçu pour s&#39;afficher dans la liste des campagnes des campagnes SMS exécutées par des opérateurs des départements Running ou Yoga.

   ![Exemple de filtre personnalisé affichant des campagnes SMS filtrées par service](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Une fois votre filtre personnalisé configuré, cliquez sur **[!UICONTROL Confirmer]** pour l’appliquer à la liste.