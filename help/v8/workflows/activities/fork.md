---
audience: end-user
title: Utilisation de l’activité de workflow Branchement
description: Découvrez comment utiliser l’activité de workflow Branchement
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 19%

---


# Branchement {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Branchement activité"
>abstract="L&#39;activité Branchement permet de créer des transitions sortantes afin de lancer plusieurs activités en parallèle."

## Configuration

Procédez comme suit pour configurer la variable **Branchement** activité :

1. Ajouter un **Branchement** à votre workflow.
1. Cliquez sur **Ajouter une transition** pour ajouter une nouvelle transition sortante. Par défaut, deux transitions sont définies.
1. Ajoutez un libellé à chacune de vos transitions.

## Exemple

L’exemple suivant, nous utilisons deux **Branchement** activités :

* Un avant les deux requêtes, pour les exécuter en même temps.
* Une fois l&#39;intersection terminée, pour envoyer simultanément un email et un SMS à la population ciblée.

![](../assets/workflow-fork-example.png)

