---
audience: end-user
title: Sélectionner des attributs et les ajouter aux favoris
description: Découvrez comment utiliser les attributs et accéder facilement aux attributs favoris et récemment utilisés.
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 7%

---

# Sélectionner des attributs et les ajouter aux favoris {#folders}

L’interface utilisateur web de Campaign vous permet de sélectionner des attributs de la base de données à différents emplacements, selon l’action que vous souhaitez effectuer. Par exemple, vous pouvez sélectionner des attributs lors de la définition des colonnes de sortie pour une diffusion courrier ou un fichier à extraire. De même, les attributs peuvent être sélectionnés lors de l’utilisation du requêteur pour créer des règles, des filtres ou des audiences.

![](assets/attributes-list.png)

Pour réutiliser rapidement les attributs fréquemment utilisés, vous pouvez les ajouter aux favoris. Cela permet de s’assurer qu’ils sont facilement accessibles pour les tâches futures. Outre les favoris, vous pouvez également afficher et utiliser les derniers attributs sélectionnés.

L’interface propose également un outil de distribution des valeurs, qui vous permet de visualiser la distribution des valeurs d’un attribut dans un tableau. Cet outil peut vous aider à identifier la plage et la fréquence des valeurs, assurant ainsi la cohérence des données lors de la création de requêtes ou d’expressions.

## Favoris et attributs récents {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Favoris et Récents"
>abstract="Le menu **[!UICONTROL Favoris et récents]** du sélecteur d’attributs fournit une vue organisée des attributs que vous avez ajoutés aux favoris, ainsi qu’une liste des attributs récemment utilisés. Les attributs favoris apparaissent en premier, suivis des attributs récemment utilisés, ce qui facilite la localisation des attributs dont vous avez besoin."

Le menu **[!UICONTROL Favoris et récents]** du sélecteur d’attributs fournit une vue organisée des attributs que vous avez ajoutés aux favoris, ainsi qu’une liste des attributs récemment utilisés. Les attributs favoris apparaissent en premier, suivis des attributs récemment utilisés, ce qui facilite la localisation des attributs dont vous avez besoin.

![](assets/attributes-favorites.png)

Pour ajouter un attribut aux favoris, passez la souris sur son bouton d’informations et sélectionnez l’icône en forme d’étoile. L’attribut sera alors automatiquement ajouté à votre liste de favoris. Si vous ne souhaitez plus conserver un attribut comme favori, vous pouvez le supprimer en sélectionnant à nouveau l’icône en forme d’étoile.

Vous pouvez ajouter jusqu’à 20 attributs favoris. Les attributs favoris et récents sont associés à chaque utilisateur au sein d’une organisation. Cela signifie qu’ils sont accessibles à partir de différentes machines, ce qui garantit une expérience transparente entre les appareils.

## Identifier la répartition des valeurs dans un tableau {#distribution}

Le bouton **Répartition des valeurs**, disponible dans le volet d’informations d’un attribut, vous permet d’analyser la répartition des valeurs de cet attribut dans le tableau. Cette fonctionnalité est particulièrement utile pour comprendre les valeurs disponibles, leur nombre et leurs pourcentages. Cela permet également d’éviter des problèmes tels que l’incohérence des majuscules ou de l’orthographe lors de la création de requêtes ou d’expressions.

![](assets/attributes-distribution-values.png)

Pour les attributs comportant un grand nombre de valeurs, l’outil affiche uniquement les vingt premières valeurs. Dans ce cas, une notification **[!UICONTROL Charge partielle]** s’affiche pour indiquer cette limitation. Vous pouvez appliquer des filtres avancés pour affiner les résultats affichés et mettre l’accent sur des valeurs ou des sous-ensembles de données spécifiques. Des conseils détaillés sur l’utilisation des filtres sont disponibles [ici](../get-started/work-with-folders.md#filter-the-values).

Pour plus d’informations sur l’utilisation de l’outil de distribution des valeurs dans différents contextes, consultez les sections suivantes :

- [Répartition des valeurs dans un dossier](../get-started/work-with-folders.md##distribution-values-folder)
- [Répartition des valeurs dans une requête](../query/build-query.md#distribution-values-query)
