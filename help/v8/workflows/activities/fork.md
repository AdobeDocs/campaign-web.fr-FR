---
audience: end-user
title: Utiliser l’activité de workflow Branchement
description: Découvrez comment utiliser l’activité de workflow Branchement.
badge: label="Beta"
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 100%

---

# Branchement {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Branchement  activité"
>abstract="L’activité **Branchement** permet de créer des transitions sortantes afin de lancer plusieurs activités en parallèle."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transitions de l’activité Branchement"
>abstract="Par défaut, deux transitions sont créées avec une activité **Branchement**. Cliquez sur le bouton **Ajouter une transition** pour définir une transition sortante supplémentaire, puis renseignez son libellé."

L’activité **Branchement** est une activité de **contrôle de flux**. Elle permet de créer des transitions sortantes afin de démarrer plusieurs activités en parallèle.

## Configurer l’activité Branchement{#fork-configuration}

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
