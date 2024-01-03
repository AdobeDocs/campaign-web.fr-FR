---
audience: end-user
title: Filtrer les listes
description: Découvrez comment filtrer les listes web Adobe Campaign à l’aide de filtres intégrés et personnalisés.
source-git-commit: 843f3ad906d81892f45281ef5734d512b4c8f3d6
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 6%

---


# Filtrer les listes {#filter-lists}

Adobe Campaign Web fournit des filtres dans chaque liste d’objets, ce qui vous permet de filtrer les informations en fonction de critères contextuels spécifiques. Vous pouvez, par exemple, filtrer les diffusions selon leur statut, leur canal, leur date de contact ou leur dossier. Vous pouvez également masquer les tests.

## Appliquer les filtres{#apply}

Pour appliquer des filtres à une liste, cliquez sur le bouton **[!UICONTROL Afficher les filtres]** situé dans le coin supérieur gauche de la liste, en regard de la barre de recherche.

Le volet Filtres s’ouvre, affichant les filtres disponibles pour la liste sélectionnée. Vous pouvez, par exemple, filtrer les campagnes selon leur état, leurs dates de début et de fin ou leur dossier de stockage, tandis que la liste des services d’abonnement peut être filtrée sur leur canal et leur dossier de stockage.

![](assets/filters-pane.png){width="70%" align="left" zoomable="yes"}

Pour filtrer une liste selon vos propres critères, créez un filtre personnalisé. Pour ce faire, accédez au bas du volet Filtres et cliquez sur le bouton **Ajouter des règles** bouton . [Découvrez comment créer des filtres personnalisés](#custom)

Une fois appliqués à une liste, les filtres sont visibles sous la barre de recherche. Vous pouvez supprimer un filtre individuel à tout moment ou tous les filtres en cliquant sur le bouton **Effacer tout** bouton .

## Création de filtres personnalisés {#custom}

Les filtres personnalisés vous permettent d’affiner les listes en fonction de vos propres critères. Elles sont conçues à l’aide du créateur de requêtes de Campaign. Pour créer un filtre personnalisé, procédez comme suit :

1. Ouvrez le volet Filtres et cliquez sur le bouton **Ajouter des règles** située au bas du volet.
1. Le créateur de modèles de requête s’ouvre. Définissez et combinez vos critères de filtre en fonction de vos besoins. Vous trouverez des informations détaillées sur l’utilisation du modèle de requête dans la section [cette section](../query/query-modeler-overview.md).

   L&#39;exemple ci-dessous illustre un filtre personnalisé conçu pour s&#39;afficher dans la liste des campagnes, les campagnes SMS exécutées par les opérateurs des départements d&#39;exécution ou de yoga.

   ![](assets/filters-sample.png){width="70%" align="left" zoomable="yes"}

1. Une fois votre filtre personnalisé configuré, cliquez sur **[!UICONTROL Confirmer]** pour l&#39;appliquer à la liste.
