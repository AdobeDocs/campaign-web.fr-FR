---
title: Notes de mise à jour de l’interface d’utilisation web de Campaign v8
description: Découvrez les nouvelles fonctionnalités accompagnant la version suivante de l’interface d’utilisation de Campaign Web.
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 126ebed5066bbc8c20d58d24e237b13f096b9d02
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 35%

---

# Notes de mise à jour anticipées {#e-release}

L’interface d’utilisation d’Adobe Campaign Web fournit continuellement de nouvelles fonctionnalités, des améliorations des fonctionnalités existantes et des correctifs. Toutes les modifications sont consolidées à la fin de chaque mois dans les [notes de mise à jour](release-notes.md).

**Les notes de mise à jour anticipées ci-dessous peuvent être modifiées sans préavis jusqu’à la date de publication.**. Les liens, les écrans et la documentation mise à jour sont publiés dans les [notes de mise à jour](release-notes.md), à la date de publication.

## Version du 25 janvier {#25-1-release}

**Date de publication** : 5 février 2025

Les fonctionnalités et améliorations suivantes sont disponibles à partir de la version de janvier.

### Fonctionnalités {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Créer et utiliser des fragments visuels</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les fragments visuels sont des blocs visuels prédéfinis que vous pouvez réutiliser dans plusieurs diffusions d’e-mail ou dans des modèles de contenu. Cette fonctionnalité est désormais disponible pour tous les clients qui s’exécutent sur le serveur version 8.6.4 et ultérieures.</p>
<p>Pour plus d’informations, consultez la <a href="../content/use-visual-fragments.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Utiliser un système tiers pour envoyer des diffusions</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez maintenant définir des diffusions externes et des modèles de diffusion externes dans l'interface utilisateur web de Campaign. Avec ce mode, les messages sont générés dans un fichier d’entrée qui peut être partagé avec votre fournisseur externe. Le mode de diffusion externe est le mode par défaut du canal de publipostage direct.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Contrôler et filtrer l’envoi des diffusions avec des typologies</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer des typologies et des règles de typologie dans l’interface utilisateur web d’Adobe Campaign. Une typologie est un ensemble de règles de typologie qui permet de contrôler, filtrer et prioriser l’envoi des diffusions. Les typologies valident que vos diffusions contiennent toujours des éléments requis (tels qu’un lien de désinscription ou une ligne d’objet) ou des règles de filtrage pour exclure des groupes de votre cible prévue (tels que les clients et clientes désabonnés, les concurrents et les clientes et clients ne faisant pas partie du programme de fidélité).</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gestion des énumérations</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer des énumérations directement via l'interface utilisateur web d'Adobe Campaign. Une énumération est une liste de valeurs suggérées par le système pour renseigner les champs. Utilisez des énumérations pour normaliser les valeurs de ces champs, faciliter la saisie de données ou les utiliser dans des requêtes.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Création d’options personnalisées</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais accéder aux options techniques de l’interface utilisateur web d’Adobe Campaign et créer vos propres options personnalisées en fonction de vos besoins. Cela s’avère particulièrement utile lorsque vous travaillez avec des activités de workflow de code JavaScript pour stocker des données intermédiaires.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Définition et appel de codes JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer des codes JavaScript dans l’interface utilisateur web d’Adobe Campaign. Vous pouvez ainsi créer des fonctions réutilisables qui peuvent être utilisées dans les workflows, comme une bibliothèque.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#25-1-improvements}

* Personnalisez l’affichage des champs personnalisés dans l’interface :

   * Vous pouvez désormais sélectionner d’autres champs personnalisés à afficher dans l’interface
   * Vous pouvez désormais définir des règles pour l’affichage des champs personnalisés de type lien, telles que la restriction des valeurs de liste en fonction des entrées d’un autre champ
   * Vous pouvez désormais organiser les champs dans l’interface avec plus de flexibilité : les champs peuvent s’étendre sur une seule colonne ou être regroupés en sous-sections pour une meilleure organisation
   * Vous pouvez désormais définir des champs spécifiques en lecture seule.

* Filtres récents et Favoris : pour réutiliser rapidement des attributs fréquemment utilisés, vous pouvez désormais les ajouter aux favoris. Cela permet de s’assurer qu’elles sont facilement accessibles pour les tâches futures. Outre les favoris, vous pouvez également afficher et utiliser les attributs sélectionnés le plus récemment.


