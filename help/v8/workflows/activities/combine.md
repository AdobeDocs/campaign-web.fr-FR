---
audience: end-user
title: Utiliser l’activité de workflow Combiner
description: Découvrez comment utiliser l’activité de workflow Combiner.
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 80%

---


# Combiner {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Activité Combiner"
>abstract="La variable **Combiner** est une activité **Ciblage** activité. Cette activité vous permet d’effectuer une segmentation sur votre population entrante. Vous pouvez ainsi combiner plusieurs populations, en exclure une partie ou ne conserver que les données communes à plusieurs cibles."


La variable **Combiner** est une activité **Ciblage** activité. Cette activité vous permet d’effectuer une segmentation sur votre population entrante. Il est ainsi possible de regrouper plusieurs populations, d’en exclure une partie ou de ne conserver que les données communes entre plusieurs cibles. Les types de segmentation disponibles sont les suivants :

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* l’**Union** permet de regrouper le résultat de plusieurs activités dans une cible unique.
* l’**Intersection** permet de ne conserver que les éléments communs aux différentes populations entrantes dans l’activité.
* l’**Exclusion** permet d’exclure des éléments d’une population selon certains critères.

## Configuration générale {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Options de fusion des intersections"
>abstract="L’intersection permet de ne conserver que les éléments communs aux différentes populations entrantes dans l’activité. Dans la section Ensembles à joindre, cochez les activités précédentes à joindre."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Options de fusion des exclusions"
>abstract="L’exclusion permet d’exclure des éléments d’une population selon certains critères. Dans la section Ensembles à joindre, cochez les activités précédentes à joindre."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Sélection du type de segmentation"
>abstract="Choisissez comment combiner des audiences : union, intersection ou exclusion."

Pour commencer à configurer l’activité **Combiner**, procédez comme suit :

1. Ajoutez plusieurs activités, comme **Créer une audience**, pour former au moins deux branches d’exécution différentes.
1. Ajoutez une activité **Combiner** à l’une des branches précédentes.
1. Sélectionnez le type de segmentation : [union](#union), [intersection](#intersection) ou [exclusion](#exclusion).
1. Cliquez sur **Continuer**.
1. Dans la section **Ensembles à joindre**, cochez les activités précédentes à joindre.

## Union {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Options de réconciliation des interactions"
>abstract="Sélectionnez le type de réconciliation pour définir la manière dont les duplicatas sont traités :"

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Options de réconciliation"
>abstract="Sélectionnez la variable **Type de réconciliation** pour définir comment gérer les doublons."

Dans le **Combiner** vous pouvez configurer une activité **Union**. Pour cela, vous devez sélectionner la variable **Type de réconciliation** pour définir la gestion des doublons :

* **Uniquement les clés** : il s’agit du mode par défaut. Lorsque des éléments provenant des différentes transitions entrantes ont la même clé, l’activité ne conserve qu’un élément. Cette option ne peut être utilisée que si les populations entrantes sont homogènes.
* **Une sélection de colonnes** : sélectionnez cette option pour définir la liste des colonnes sur lesquelles sera appliquée la réconciliation des données. Vous devez d’abord sélectionner l’ensemble principal (celui qui contient les données sources), puis les colonnes à utiliser pour la jointure.

## Intersection {#intersection}

Dans le **Combiner** vous pouvez configurer une **Intersection**. Pour cela, vous devez suivre les étapes supplémentaires ci-dessous :

1. Sélectionnez le **Type de réconciliation** pour définir la manière dont les duplicatas sont traités. Pour plus d’informations, consultez la section [Union](#union).
1. Vous pouvez vérifier l’option **Générer le complémentaire** si vous souhaitez traiter la population restante. Le complémentaire contiendra l’union des résultats de toutes les activités entrantes, moins l’intersection. Une transition sortante supplémentaire sera alors ajoutée à l’activité.

## Exclusion {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Exclusion  règles"
>abstract="Le cas échéant, vous pouvez manipuler les tableaux entrants. En effet, pour exclure une cible d’une autre dimension, cette cible doit être replacée dans la même dimension de ciblage que la cible principale. Pour ce faire, cliquez sur Ajouter une règle dans la section Règles d’exclusion et indiquez les conditions de changement de dimension. La réconciliation des données s’effectue au moyen d’un attribut ou d’une jointure."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Sélectionner des ensembles à combiner"
>abstract="Dans la section **Ensembles à joindre**, sélectionnez **Ensemble principal** parmi les transitions entrantes. C’est l’ensemble à partir duquel des éléments sont exclus. Les autres ensembles correspondent aux éléments devant être exclus de l’ensemble principal."


Dans le **Combiner** vous pouvez configurer une **Exclusion**. Pour cela, vous devez suivre les étapes supplémentaires ci-dessous :

1. Dans la section **Ensembles à joindre**, sélectionnez **Ensemble principal** parmi les transitions entrantes. C’est l’ensemble à partir duquel des éléments sont exclus. Les autres ensembles correspondent aux éléments devant être exclus de l’ensemble principal.
1. Le cas échéant, vous pouvez manipuler les tableaux entrants. En effet, pour exclure une cible d’une autre dimension, cette cible doit être replacée dans la même dimension de ciblage que la cible principale. Pour ce faire, cliquez sur **Ajouter une règle** dans la section **Règles d’exclusion** et indiquez les conditions de changement de dimension. La réconciliation des données s’effectue au moyen d’un attribut ou d’une jointure.
1. Vous pouvez vérifier l’option **Générer le complémentaire** si vous souhaitez traiter la population restante. Pour plus d’informations, consultez la section [Intersection](#intersection).

## Exemples

Dans l’exemple suivant, nous utilisons une **Combiner** activité et nous ajoutons une **union** pour retrouver tous les profils des deux requêtes : les personnes âgées de 18 à 27 ans et les personnes âgées de 34 à 40 ans.

![](../assets/workflow-union-example.png)

L’exemple suivant montre l’**intersection** de deux activités de requête. Elle est utilisée ici pour récupérer les profils qui ont entre 18 et 27 ans et dont l’adresse e-mail a été renseignée.

![](../assets/workflow-intersection-example.png)

L’exemple d’**exclusion** suivant présente deux requêtes configurées pour filtrer les profils qui ont entre 18 et 27 ans et qui ont un domaine d’e-mail Adobe. Les profils avec un domaine d’e-mail Adobe sont ensuite exclus du premier ensemble.

![](../assets/workflow-exclusion-example.png)


