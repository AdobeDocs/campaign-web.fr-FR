---
audience: end-user
title: Utilisation de l’activité de workflow Branchement
description: Découvrez comment utiliser l’activité de workflow Branchement
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Branchement {#fork}

L&#39;activité **Branchement** permet de créer des transitions sortantes afin de lancer plusieurs activités en parallèle.

L&#39;activité **Branchement** permet de réaliser, au sein d&#39;un même workflow, plusieurs exécutions distinctes de manière indépendante.

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

