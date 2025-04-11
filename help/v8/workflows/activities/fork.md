---
audience: end-user
title: Utiliser l’activité de workflow Branchement
description: Découvrez comment utiliser l’activité de workflow Branchement.
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 58%

---


# Branchement {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Activité Branchement"
>abstract="L’activité **Branchement** permet de créer des transitions sortantes afin de lancer plusieurs activités en parallèle."

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transitions de l’activité Branchement"
>abstract="Par défaut, deux transitions sont créées avec une activité **Branchement**. Cliquez sur le bouton **Ajouter une transition** pour définir une transition sortante supplémentaire, puis renseignez son libellé."

L’activité **Branchement** est une activité de **contrôle de flux**. Il permet de créer des transitions sortantes afin de lancer plusieurs activités simultanément.

## Configurer l’activité Branchement {#fork-configuration}

Pour configurer l’activité **Branchement**, procédez comme suit :

![Capture d’écran de la configuration de l’activité Branchement de workflow](../assets/workflow-fork.png)

1. Ajoutez une activité **Branchement** à votre workflow.
1. Cliquez sur **Ajouter une transition** pour ajouter une nouvelle transition sortante. Par défaut, deux transitions sont définies.
1. Ajoutez un libellé à chaque transition.

## Exemple {#fork-example}

Dans l&#39;exemple suivant, deux activités **Branchement** sont utilisées :

* Une avant les deux requêtes, pour les exécuter simultanément.
* Une après l’intersection, pour envoyer simultanément un e-mail et un SMS à la population ciblée.

![Capture d’écran d’exemple de formulaire de workflow](../assets/workflow-fork-example.png)
