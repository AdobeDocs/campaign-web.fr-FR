---
audience: end-user
title: Parcourir, rechercher et filtrer les listes
description: Découvrez comment parcourir et filtrer les listes de Campaign Web v8
badge: label="Alpha" type="Positive"
source-git-commit: 31e5d314ed0b7792d6a28614699fbe6a41b8a783
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 14%

---


# Parcourir, rechercher et filtrer les listes {#list-screens}

La plupart des liens du menu de navigation de gauche affichent des listes d’objets, telles que la liste des **Diffusions** ou **Campagnes**. Certains de ces écrans de liste sont en lecture seule. Vous pouvez personnaliser l’affichage de la liste et filtrer ces listes, comme décrit ci-dessous.

Pour supprimer un filtre, cliquez sur le bouton **Effacer tout** bouton .

## Personnalisation des écrans de liste {#custom-lists}

Les listes sont affichées en colonnes. Vous pouvez également afficher des informations supplémentaires en modifiant la configuration des colonnes. Pour ce faire, cliquez sur le bouton **Configuration d’une colonne pour une disposition personnalisée** dans le coin supérieur droit de la liste.

![](assets/config-columns.png){width="70%" align="left" zoomable="yes"}

Dans le **Configuration des colonnes** , ajoutez ou supprimez des colonnes et modifiez l’ordre dans lequel elles s’affichent.

Par exemple, pour les paramètres suivants :

![](assets/columns.png){width="70%" align="left" zoomable="yes"}

La liste affiche les colonnes suivantes :

![](assets/column-sample.png){width="70%" align="left" zoomable="yes"}

Utilisez la variable **Afficher les attributs avancés** pour afficher tous les attributs de la liste active. [En savoir plus](#adv-attributes)

## Trier les données {#sort-lists}

Vous pouvez également trier les éléments de la liste en cliquant sur l’en-tête d’une colonne. Une flèche s’affiche (vers le haut ou vers le bas) pour indiquer que la liste est triée sur cette colonne.

Pour les colonnes numériques ou de date, la variable **Monter** la flèche indique que la liste est triée dans l’ordre croissant lorsque la variable **Descendre** la flèche indique un ordre décroissant. Pour les colonnes de type chaîne ou alphanumérique, les valeurs sont classées par ordre alphabétique.

## Filtres intégrés {#list-built-in-filters}

Pour trouver les éléments plus rapidement, vous pouvez utiliser la barre de recherche ou filtrer la liste selon des critères contextuels.

![](assets/filter.png){width="70%" align="left" zoomable="yes"}

Vous pouvez, par exemple, filtrer les diffusions selon leur état, canal, date de contact ou dossier. Vous pouvez également masquer les tests.

## Filtres personnalisés{#list-custom-filters}

Pour créer des filtres personnalisés sur les données, accédez au bas des filtres et cliquez sur le bouton **Ajouter des règles** bouton .

Faites glisser et déposez des attributs pour créer vos critères de filtre dans le **Filtres avancés** écran.

![](assets/custom-filter.png){width="70%" align="left" zoomable="yes"}

Utilisez la variable **Afficher les attributs avancés** pour afficher tous les attributs de la liste active. [En savoir plus](#adv-attributes)

## Utilisation d’attributs avancés {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Afficher les attributs avancés"
>abstract="Seuls les attributs les plus courants sont affichés par défaut dans la liste des attributs. Utilisez ce bouton pour créer un filtre avec des attributs avancés."

Seuls les attributs les plus courants sont affichés par défaut dans la liste des attributs et les écrans de configuration des filtres. Attributs définis comme `advanced` Les attributs du schéma de données sont masqués dans les écrans de configuration.

Activez la variable **Afficher les attributs avancés** bascule pour afficher tous les attributs disponibles pour la liste actuelle : la liste des attributs est mise à jour instantanément.
