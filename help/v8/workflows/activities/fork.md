---
audience: end-user
title: Utiliser l’activité de workflow Branchement
description: Découvrez comment utiliser l’activité de workflow Branchement.
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 71%

---


# Branchement {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Branchement  activité"
>abstract="La variable **Branchement** est une activité **Contrôle de flux** activité. Il permet de créer des transitions sortantes afin de lancer simultanément plusieurs activités."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Branchement  activité"
>abstract="L’activité Branchement permet de créer des transitions sortantes afin de démarrer plusieurs activités en parallèle."

La variable **Branchement** est une activité **Contrôle de flux** activité. Il permet de créer des transitions sortantes afin de lancer simultanément plusieurs activités.

## Configuration

Pour configurer l’activité **Branchement**, procédez comme suit :

1. Ajoutez une activité **Branchement** à votre workflow.
1. Cliquez sur **Ajouter une transition** pour ajouter une nouvelle transition sortante. Par défaut, deux transitions sont définies.
1. Ajoutez un libellé à chacune de vos transitions.

## Exemple

Dans l’exemple suivant, nous utilisons deux activités **Branchement** :

* Une avant les deux requêtes, pour les exécuter en même temps.
* Une après l’intersection, pour envoyer simultanément un e-mail et un SMS à la population ciblée.

![](../assets/workflow-fork-example.png)

