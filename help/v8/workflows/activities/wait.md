---
audience: end-user
title: Utilisation de l’activité de workflow d’attente
description: Découvrez comment utiliser l’activité de workflow d’attente
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 75%

---


# Attente {#wait}

L&#39;activité **Attente** permet de suspendre momentanément l&#39;exécution d&#39;une partie d&#39;un workflow. Elle active sa transition sortante après un délai pouvant aller de quelques secondes à plusieurs mois, permettant l&#39;exécution des activités placées à la suite.

L&#39;activité **Attente** est utilisée pour permettre qu&#39;un certain temps s&#39;écoule entre l&#39;exécution de deux activités. Par exemple, attendre plusieurs jours après une activité de diffusion email puis analyser les ouvertures et les clics générés pendant ce laps de temps avant d&#39;appliquer d&#39;autres traitements (email de rappel, création d&#39;audience, etc.).

Procédez comme suit pour configurer la variable **Attente** activité :

1. Ajouter un **Attente** dans votre workflow.

1. Définissez la **Durée** de l&#39;attente entre l&#39;activation de la transition entrante et l&#39;activation de la transition sortante de l&#39;activité.

1. Sélectionner l’unité de temps **Période**: secondes, minutes, heures.





