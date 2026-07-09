---
title: Parcourir les schémas et y accéder
description: Découvrez comment parcourir les schémas et y accéder dans l’interface.
exl-id: deafd171-0a3f-4ba2-8fa4-09661d8cdb3e
source-git-commit: c6da1a4cb21c1346982303a29364cf97e26b4f4a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 90%

---

# Accéder aux schémas et les configurer {#access}

>[!CONTEXTUALHELP]
>id="acw_schema_action_data"
>title="Actions sur les données"
>abstract="Configurer les actions disponibles pour les écrans de détails et de listes du schéma. Activez **[!UICONTROL Lecture seule]** pour définir l’écran de détails en lecture seule et supprimer les actions de la liste. Activez **[!UICONTROL Ne pas autoriser la suppression]** pour supprimer l’action de suppression des écrans de détails et de liste."

Les schémas sont accessibles à partir du menu **[!UICONTROL Administration]** > **[!UICONTROL Schémas]**.

![Écran de liste des schémas affichant les schémas et les filtres disponibles](assets/schemas-list.png)

Depuis cet écran, vous pouvez afficher tous les schémas existants. Des filtres sont disponibles pour aider à affiner la liste, par exemple pour afficher uniquement les schémas modifiables.

Pour ouvrir un schéma, sélectionnez son nom. Une vue de schéma détaillée s’affiche.

![Écran de détails du schéma affichant les propriétés et le contenu du schéma](assets/schema-details.png)

## Vue d’ensemble du schéma {#overview}

L’onglet **[!UICONTROL Vue d’ensemble]** offre une vue générale du schéma :

* La section **[!UICONTROL Propriétés]** affiche des informations clés, telles que le nom du schéma, l’espace de noms et le nom de la table associée.

* La section **[!UICONTROL Définition du schéma]** affiche des détails sur la définition du schéma, comme la clé primaire utilisée pour la réconciliation des données et ses liens avec d’autres tables.

  Cliquez sur le bouton **[!UICONTROL Aperçu du schéma]** pour visualiser les différents champs et liens composant le schéma. Vous pouvez ainsi vérifier la structure complète d’un schéma. Si le schéma a été étendu avec des champs personnalisés, vous pouvez visualiser toutes ses extensions.

* La section **[!UICONTROL Contenu]** affiche le contenu XML du schéma, ce qui vous permet de basculer entre la source et la syntaxe générée.

## Données de schéma {#data}

L’onglet **[!UICONTROL Données]** fournit des informations sur les données du schéma.

![Onglet Données de schéma présentant la structure et les attributs des données](assets/schemas-data.png)

## Personnaliser l’affichage de l’écran {#screen-def}

La définition d’écran vous permet de configurer l’affichage et la modification des champs de schéma dans l’interface. Vous pouvez configurer les colonnes par défaut pour les vues de liste, personnaliser les champs personnalisés qui s’affichent dans les écrans de détail, ajouter des listes de collections pour afficher les données associées et organiser les champs en sections avec des séparateurs et des critères de visibilité.

Pour accéder à la définition d’écran :

1. Accédez au menu **[!UICONTROL Schémas]** et recherchez les schémas modifiables à l’aide des filtres.

   ![Écran de liste des schémas affichant les schémas et les filtres disponibles](assets/schemas-list2.png)

1. Sélectionnez le nom du schéma dans la liste pour l’ouvrir et cliquez sur le bouton **[!UICONTROL Modification d’écran]** dans la vue des détails du schéma pour accéder à la définition d’écran.

   ![Écran de liste des schémas affichant les schémas et les filtres disponibles](assets/schemas-list3.png)

   Les différentes listes vous permettent de réorganiser les éléments à l’aide des icônes de flèche vers le haut et vers le bas ou de les faire glisser et de les déposer. Pour supprimer des éléments, cliquez sur l’icône de la corbeille sur une ligne spécifique ou sélectionnez **[!UICONTROL Tout supprimer]** à partir de l’icône représentant des points de suspension.

   ![Section générale de la définition de l’écran](assets/schemas-general.png)

Dans l’onglet Définition d’écran, vous pouvez :

* [Configurer les colonnes de la liste par défaut](schemas-list-columns.md) : configurez les colonnes affichées par défaut dans les vues Liste.
* [Modifier les champs personnalisés](schemas-custom-fields.md) : configurez les champs personnalisés qui s’affichent dans les écrans de détails et organisez-les en sections.
* [Ajouter des listes de collections](schemas-collection-lists.md) : ajoutez des listes de collections pour afficher les données associées dans les écrans de profil.
