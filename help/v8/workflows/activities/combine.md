---
audience: end-user
title: Utilisation de l’activité de workflow Combiner
description: Découvrez comment utiliser l’activité de workflow Combiner
badge: label="Alpha" type="Positive"
source-git-commit: 3bbdd45571d09258bba34e22de39f5281c02d248
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 28%

---


# Combiner {#combine}

Cette activité permet de traiter des ensembles sur les données entrantes. Il est ainsi possible de regrouper plusieurs populations, d&#39;en exclure une partie ou de ne conserver que les données communes entre plusieurs cibles. Voici les types de segmentation disponibles :

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* Le **Union** permet de regrouper le résultat de plusieurs activités dans une seule cible.
* Le **Intersection** permet de ne conserver que les éléments communs aux différentes populations entrantes dans l&#39;activité.
* Le **Exclusion** permet d&#39;exclure des éléments d&#39;une population selon certains critères.

## Configuration

Procédez comme suit pour configurer la variable **Combiner** activité :

1. Ajoutez plusieurs activités, telles que **Créer une audience** pour former au moins deux branches d&#39;exécution différentes.
1. Ajouter un **Combiner** à l’une des transitions de segmentation précédentes.
1. Sélectionnez le type de segmentation : union, intersection ou exclusion.
1. Cliquez sur **Continuer**.
1. Dans le **Définit la jointure** , vérifiez toutes les activités précédentes que vous souhaitez rejoindre.

Pour le **Union** et **Intersection**, vous devez sélectionner la variable **Type de réconciliation** pour définir la gestion des doublons :

    * Uniquement les clés : c&#39;est le mode par défaut. L&#39;activité ne conserve qu&#39;un élément lorsque des éléments provenant des différentes transitions entrantes ont la même clé. Cette option ne peut être utilisée que si les populations en entrée sont homogènes.
    * Une sélection de colonnes : sélectionnez cette option pour définir la liste des colonnes sur lesquelles sera appliquée la réconciliation des données. Vous devez d&#39;abord sélectionner l&#39;ensemble principal (celui qui contient les données sources), puis les colonnes à utiliser pour la jointure.

Pour le **Intersection** et **Exclusion**, vous pouvez vérifier la variable **Générer l’achèvement** si vous souhaitez traiter la population restante. Le complémentaire contiendra l’union des résultats de toutes les activités entrantes, moins l’intersection. Une transition sortante supplémentaire sera alors ajoutée à l&#39;activité.

Pour le **Exclusion**, sélectionnez la variable **Principal** depuis les transitions entrantes, dans la **Définit la jointure** . C&#39;est l&#39;ensemble à partir duquel des éléments sont exclus. Les autres ensembles correspondent aux éléments devant être exclus de l&#39;ensemble principal.

## Exemples      

Dans l’exemple suivant, nous avons ajouté une **union** qui récupère tous les profils des deux requêtes : personnes de 18 à 27 ans et personnes de 34 à 40 ans.

![](../assets/workflow-union-example.png)

L’exemple suivant illustre la variable **intersection** entre deux activités de requête. Il est utilisé ici pour récupérer les profils qui ont entre 18 et 27 ans et dont l&#39;adresse email a été renseignée.

![](../assets/workflow-intersection-example.png)

Les éléments suivants **exclusion** exemple affiche deux requêtes configurées pour filtrer les profils qui ont entre 18 et 27 ans et ont un domaine de messagerie adobe. Les profils avec un domaine de messagerie Adobe sont ensuite exclus du premier ensemble.

![](../assets/workflow-exclusion-example.png)





