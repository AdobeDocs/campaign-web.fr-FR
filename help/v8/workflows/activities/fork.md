---
audience: end-user
title: Utiliser l’activité de workflow Branchement
description: Découvrez comment utiliser l’activité de workflow Branchement.
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 66%

---


# Branchement {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Branchement  activité"
>abstract="L’activité **Branchement** permet de créer des transitions sortantes afin de lancer plusieurs activités en parallèle."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transitions de l&#39;activité Branchement"
>abstract="Par défaut, deux transitions sont créées avec un **Branchement** activité. Cliquez sur le bouton **Ajouter une transition** pour définir une transition sortante supplémentaire, et renseigner son libellé."

La variable **Branchement** est une activité **Contrôle de flux** activité. Il permet de créer des transitions sortantes afin de lancer simultanément plusieurs activités.

## Configuration de l’activité Branchement{#fork-configuration}

Pour configurer l’activité **Branchement**, procédez comme suit :

![](../assets/workflow-fork.png)

1. Ajoutez une activité **Branchement** à votre workflow.
1. Cliquez sur **Ajouter une transition** pour ajouter une nouvelle transition sortante. Par défaut, deux transitions sont définies.
1. Ajoutez un libellé à chacune de vos transitions.

## Exemple{#fork-example}

Dans l’exemple suivant, nous utilisons deux activités **Branchement** :

* Une avant les deux requêtes, pour les exécuter en même temps.
* Une après l’intersection, pour envoyer simultanément un e-mail et un SMS à la population ciblée.

![](../assets/workflow-fork-example.png)

