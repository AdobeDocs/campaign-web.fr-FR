---
title: Barrières de sécurité et limites de l’interface utilisateur web de Campaign
description: Barrières de sécurité et limites de l’interface utilisateur web de Campaign
badge: label="Beta"
source-git-commit: ff95b563784ae507245e6690feedda33ea6a111b
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

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

* Les workflows, y compris les boucles, ne s’affichent pas dans l’interface utilisateur web. Un message d’erreur s’affiche.

**Réconciliation et enrichissement**

Dans la console cliente Campaign, le **Enrichissement** l’activité peut effectuer à la fois la réconciliation et l’enrichissement. Dans l’interface utilisateur web de Campaign, les fonctionnalités de réconciliation ne sont pas encore disponibles. Si vous avez défini la réconciliation dans l’activité de console, elle s’affichera comme une activité non compatible dans l’interface utilisateur web.

* Si la variable **Enrichissement** dans la console effectue uniquement un enrichissement, l’événement **Enrichissement** l’activité s’affiche sur le web.
* Si la variable **Enrichissement** une activité dans la console effectue uniquement une réconciliation, une activité incompatible est affichée.

## Filtres prédéfinis {#filters-guardrails-limitations}


Lors de la sélection de l&#39;audience d&#39;une diffusion, ou lors de la création d&#39;une audience dans un workflow, certains filtres prédéfinis ne sont pas disponibles. Un message d’erreur spécifique s’affiche. Vous pouvez toujours utiliser la requête et voir : la condition de filtrage et les résultats, mais vous ne pouvez pas afficher la requête exacte dans le créateur de règles et ne pouvez pas modifier le filtre.

![](assets/filter-unavailable.png)
