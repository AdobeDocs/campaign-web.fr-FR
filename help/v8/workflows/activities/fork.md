---
audience: end-user
title: Utilisation de l’activité de workflow Branchement
description: Découvrez comment utiliser l’activité de workflow Branchement
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 5%

---


# Branchement {#fork}

Le **Branchement** est une activité **Contrôle de flux** activité. Il permet de créer des transitions sortantes afin de lancer simultanément plusieurs activités.

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

