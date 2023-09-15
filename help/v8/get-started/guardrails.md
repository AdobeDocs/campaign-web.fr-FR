---
title: Barrières de sécurité et limites de l’interface utilisateur web de Campaign
description: Barrières de sécurité et limites de l’interface utilisateur web de Campaign
badge: label="Beta"
source-git-commit: 68eb1529f6780682256f4b36bd77d336cf560d21
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 7%

---


# Mécanismes de sécurisation et limitations {#guardrails-limitations}

Lorsque vous utilisez l’interface utilisateur web de Campaign avec des composants créés ou modifiés dans la console cliente Campaign, les barrières de sécurité et les limitations répertoriées ci-dessous s’appliquent.

## Workflows {#wf-guardrails-limitations}

Le même workflow est accessible dans la console et dans l’interface utilisateur web. Toutefois, sachez que certaines restrictions s’appliquent.

**Édition d’activité**

* Lors de l’accès à un workflow de console dans l’interface utilisateur web, vous ne pouvez modifier que les activités compatibles.

**Modification du canevas**

* Si un workflow de console comporte plusieurs noeuds/branches de démarrage ou activités flottantes, vous devez ajouter une activité de démarrage et un branchement pour connecter les noeuds de démarrage au noeud principal. Vous devez également supprimer les activités flottantes.

**Positionnement de l’activité**

* Le positionnement des noeuds ne sera recalculé (le positionnement initial des activités sera donc modifié) que lorsqu’une activité a été ajoutée ou supprimée (ce qui n’est pas toujours le cas).

**Options de non-exposition**

* Les options non compatibles ne s’affichent pas dans l’interface utilisateur web.

**Boucles**

* Les boucles ne sont pas encore disponibles dans l’interface utilisateur web. Si vous avez créé un workflow comprenant une boucle à l’aide de la console, il ne sera pas accessible dans l’interface utilisateur web. Un message d’erreur s’affiche.

| Console | Interface utilisateur web |
| --- | --- |
| ![](assets/limitations-loops-console.png) | ![](assets/limitations-loops-web.png) |

<table>
<tr>
<th>Console</th>
<th>Interface utilisateur web</th>
</tr>
<tr>
<td><img src="assets/limitations-loops-console.png"></td>
<td><img src="assets/limitations-loops-web.png"></td>
</tr>
</table>

**Réconciliation et enrichissement**

Dans la console cliente Campaign, le **Enrichissement** l’activité peut effectuer à la fois la réconciliation et l’enrichissement. Dans l’interface utilisateur web de Campaign, les fonctionnalités de réconciliation ne sont pas encore disponibles. Si vous avez défini la réconciliation dans l’activité de console, elle s’affichera comme une activité non compatible dans l’interface utilisateur web.

* Si la variable **Enrichissement** dans la console effectue uniquement un enrichissement, l’événement **Enrichissement** l’activité s’affiche sur le web.
* Si la variable **Enrichissement** une activité dans la console effectue uniquement une réconciliation, une activité incompatible est affichée.

## Filtres prédéfinis {#filters-guardrails-limitations}

Lors de la sélection de l&#39;audience d&#39;une diffusion, ou lors de la création d&#39;une audience dans un workflow, certains filtres prédéfinis ne sont pas disponibles dans l&#39;interface utilisateur, dans cette version du produit.

Un message d’erreur spécifique s’affiche. Même si vous ne pouvez pas afficher la représentation graphique de la requête dans le créateur de règles et si vous ne pouvez pas modifier le filtre, vous pouvez toujours l’utiliser et afficher les conditions de filtrage et les résultats. Vous pouvez également accéder à la requête SQL pour vérifier les paramètres exacts.

![](assets/filter-unavailable.png){width="70%" align="left"}


Notez que si vous créez un filtre dans l’interface Web et que vous le modifiez dans la console avec des attributs non pris en charge, la représentation graphique ne peut plus être disponible dans l’interface Web. Dans tous les cas, vous pouvez toujours utiliser le filtre.

Les attributs non pris en charge sont répertoriés ci-dessous.

### Types de données non pris en charge {#unsupported-data-type}

Les types de données suivants disponibles dans la console cliente ne sont pas pris en charge lors de l’affichage d’un filtre ou d’une règle dans l’interface web :

* datetime
* time
* timespan
* double
* float

### Fonctionnalités de filtrage non prises en charge {#unsupported-filtering-capabilities}

Lorsqu&#39;un filtre est créé avec des expressions et fonctions complexes dans la console cliente, il ne peut pas être édité dans l&#39;interface Web.

En outre, les opérateurs suivants ne sont pas pris en charge :

* Type numérique
   * est compris dans
   * no dans

* Type de chaîne
   * supérieur à
   * inférieur à
   * supérieur ou égal à
   * inférieur ou égal à
   * comme
   * pas comme

* Type de date
   * après ou égal à
   * avant ou égal à
   * n’est pas égal à
   * est vide
   * n&#39;est pas vide
   * est compris dans
   * n&#39;est pas compris dans
   * in last

* Liens 1-N
   * COMPTAGE, SOMME, AVG, MIN, MAX