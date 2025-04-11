---
audience: end-user
title: Utiliser l’activité de workflow Combiner
description: Découvrez comment utiliser l’activité de workflow Combiner.
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 35%

---

# Combiner {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Activité Combiner"
>abstract="L’activité **Combiner** permet d’effectuer une segmentation sur votre population entrante. Vous pouvez combiner plusieurs populations, en exclure une partie ou ne conserver que les données communes entre plusieurs cibles."

L’activité **Combiner** est une activité de **ciblage**. Cette activité vous permet d’effectuer une segmentation sur votre population entrante. Vous pouvez combiner plusieurs populations, en exclure une partie ou ne conserver que les données communes entre plusieurs cibles. Les types de segmentation disponibles sont les suivants :

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* L’**Union** regroupe le résultat de plusieurs activités dans une cible unique.
* Le **Intersection** ne conserve que les éléments communs aux différentes populations entrantes dans l&#39;activité.
* Le **Exclusion** exclut les éléments d’une population selon certains critères.

## Configurer l’activité Combiner {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Options de fusion des intersections"
>abstract="L’intersection conserve uniquement les éléments communs aux différentes populations entrantes dans l’activité. Dans la section Ensembles à joindre , cochez toutes les activités précédentes à joindre."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Options de fusion des exclusions"
>abstract="L’exclusion exclut les éléments d’une population selon certains critères. Dans la section Ensembles à joindre , cochez toutes les activités précédentes à joindre."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Sélectionner le type de segmentation"
>abstract="Sélectionnez comment combiner des audiences. L’**Union** regroupe le résultat de plusieurs activités dans une cible unique. Le **Intersection** ne conserve que les éléments communs aux différentes populations entrantes dans l&#39;activité. Le **Exclusion** exclut les éléments d’une population selon certains critères."

Pour configurer l’activité **Combiner**, procédez comme suit :

![](../assets/workflow-combine.png)

1. Ajoutez plusieurs activités, telles que les activités **Créer une audience**, pour former au moins deux branches d’exécution différentes.
1. Ajoutez une activité **Combiner** à l’une des branches précédentes.
1. Sélectionnez le type de segmentation : [union](#union), [intersection](#intersection) ou [exclusion](#exclusion).
1. Cliquez sur **Continuer**.
1. Dans la section **Ensembles à joindre**, cochez toutes les activités précédentes à joindre.

## Union {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Options de réconciliation"
>abstract="Sélectionnez le **type de réconciliation** pour définir comment gérer les doublons. Par défaut, l&#39;option **Keys** est activée, ce qui signifie que l&#39;activité ne conserve qu&#39;un seul élément lorsque les éléments des différentes transitions entrantes possèdent la même clé. Utilisez l’option **Une sélection de colonnes** pour définir la liste des colonnes sur lesquelles est appliquée la réconciliation des données."

Dans l&#39;activité **Combiner**, configurez une **Union** en sélectionnant le **Type de réconciliation** afin de définir le traitement des doublons :

* **Clés uniquement** : il s’agit du mode par défaut. L&#39;activité ne conserve qu&#39;un seul élément lorsque les éléments des différentes transitions entrantes ont la même clé. Cette option ne peut être utilisée que si les populations entrantes sont homogènes.
* **Une sélection de colonnes** : sélectionnez cette option pour définir la liste des colonnes sur lesquelles s&#39;applique la réconciliation des données. Sélectionnez d&#39;abord l&#39;ensemble principal (les données sources), puis les colonnes à utiliser pour la jointure.

## Intersection {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Options de réconciliation des interactions"
>abstract="Sélectionnez le **type de réconciliation** pour définir comment gérer les doublons. Par défaut, l&#39;option **Keys** est activée, ce qui signifie que l&#39;activité ne conserve qu&#39;un seul élément lorsque les éléments des différentes transitions entrantes possèdent la même clé. Utilisez l’option **Une sélection de colonnes** pour définir la liste des colonnes sur lesquelles est appliquée la réconciliation des données."

Dans l&#39;activité **Combiner**, configurez une **Intersection** en procédant comme suit :

1. Sélectionnez le **Type de réconciliation** pour définir la manière dont les duplicatas sont traités. Pour plus d’informations, consultez la section [Union](#union).
1. Cochez l&#39;option **Générer le complémentaire** si vous souhaitez exploiter la population restante. Le complémentaire contient l’union des résultats de toutes les activités entrantes, moins l’intersection. Une transition sortante supplémentaire est alors ajoutée à l’activité.

## Exclusion {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Règles d’exclusion"
>abstract="Si nécessaire, manipulez les tableaux entrants. Pour exclure une cible d’une autre dimension, ramenez cette cible à la même dimension de ciblage que la cible principale. Cliquez sur Ajouter une règle dans la section Règles d’exclusion et indiquez les conditions de changement de dimension. La réconciliation des données s’effectue au moyen d’un attribut ou d’une jointure."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Sélectionner des ensembles à combiner"
>abstract="Dans la section **Ensembles à joindre**, sélectionnez **Ensemble principal** parmi les transitions entrantes. C’est l’ensemble à partir duquel des éléments sont exclus. Les autres ensembles correspondent aux éléments devant être exclus de l’ensemble principal."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="Règles d’exclusion"
>abstract="Si nécessaire, manipulez les tableaux entrants. Pour exclure une cible d’une autre dimension, ramenez cette cible à la même dimension de ciblage que la cible principale. Cliquez sur Ajouter une règle dans la section Règles d’exclusion et indiquez les conditions de changement de dimension. La réconciliation des données s’effectue au moyen d’un attribut ou d’une jointure."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="Combiner la génération de complément"
>abstract="Activez l’option Générer un complément pour traiter la population restante dans une transition supplémentaire."

Dans l’activité **Combiner**, configurez une **Exclusion** en procédant comme suit :

1. Dans la section **Ensembles à joindre**, sélectionnez **Ensemble principal** parmi les transitions entrantes. C’est l’ensemble à partir duquel des éléments sont exclus. Les autres ensembles correspondent aux éléments devant être exclus de l’ensemble principal.
1. Si nécessaire, manipulez les tableaux entrants. Pour exclure une cible d’une autre dimension, ramenez cette cible à la même dimension de ciblage que la cible principale. Cliquez sur **Ajouter une règle** dans la section **Règles d’exclusion** et spécifiez les conditions de changement de dimension. La réconciliation des données s’effectue au moyen d’un attribut ou d’une jointure.
1. Cochez l&#39;option **Générer le complémentaire** si vous souhaitez exploiter la population restante. Pour plus d’informations, consultez la section [Intersection](#intersection).

## Exemples {#combine-examples}

Dans l’exemple suivant, une activité **Combiner** utilise une **Union** pour récupérer tous les profils des deux requêtes : personnes de 18 à 27 ans et personnes de 34 à 40 ans.

![](../assets/workflow-union-example.png)

L’exemple suivant illustre l’**Intersection** entre deux activités de requête. Il récupère les profils qui ont entre 18 et 27 ans et dont l’adresse e-mail a été fournie.

![](../assets/workflow-intersection-example.png)

L’exemple **Exclusion** suivant montre deux requêtes configurées pour filtrer les profils ayant entre 18 et 27 ans et ayant un domaine d’e-mail Adobe. Les profils avec un domaine d’e-mail Adobe sont exclus du premier ensemble.

![](../assets/workflow-exclusion-example.png)