---
audience: end-user
title: Utilisation de l’activité de workflow Planificateur
description: Découvrez comment utiliser l’activité de workflow Planificateur
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 37%

---


# Planificateur {#scheduler}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler activity"
>abstract="The Scheduler activity allows you..."
-->

La variable **Planificateur** est une activité **Contrôle de flux** activité. Il permet de planifier le démarrage du workflow. Cette activité doit être considérée comme un début planifié. Il ne peut être utilisé que comme première activité du workflow.

## Bonnes pratiques

Ne planifiez pas l’exécution d’un workflow à une fréquence supérieure à toutes les 15 minutes, car cela peut nuire aux performances générales du système et créer des blocs dans la base de données.

## Configuration

Pour configurer la variable **Planificateur** activité :

1. Ajouter un **Planificateur** à votre workflow.

   ![](../assets/workflow-scheduler.png)

1. Configurez la variable **Fréquence d&#39;exécution**:

   * **Une seule fois** : le workflow n&#39;est exécuté qu&#39;une seule fois.

   * **Quotidienne** : le workflow est exécuté à une heure précise, une fois par jour.

   * **Plusieurs fois par jour :** le workflow est exécuté régulièrement plusieurs fois par jour. Vous pouvez configurer des exécutions à des heures et dates spécifiques ou périodiquement.

   * **Hebdomadaire** : le workflow est exécuté à un instant défini, une ou plusieurs fois par semaine.

   * **Mensuelle** : le workflow est exécuté à un instant défini, une ou plusieurs fois par mois. Vous pouvez sélectionner les mois auxquels le workflow doit être exécuté. Vous pouvez également configurer des exécutions les jours de semaine spécifiés du mois, comme le deuxième mardi du mois.

1. Spécifiez les détails de l&#39;exécution selon la fréquence choisie. Les champs du détail peuvent varier en fonction de la fréquence sélectionnée (heure, fréquence de répétition, jours spécifiques, etc.).

1. Cliquez sur **Aperçu des heures de lancement** pour vérifier le planning des dix prochaines exécutions de votre workflow.

1. Définissez la période de validité du planificateur :

   * **Permanent (n’expire jamais)**: le workflow est exécuté selon la fréquence d&#39;exécution définie, sans limite dans le temps ni au niveau du nombre d&#39;itérations.

   * **Période de validité**: le workflow est exécuté selon la fréquence d&#39;exécution définie, jusqu&#39;à une date spécifique. Vous devez spécifier les dates de début et de fin.

## Exemple

Dans l&#39;exemple suivant, l&#39;activité est paramétrée de sorte que le workflow démarre plusieurs fois par jour à 9h00 et 12h00, tous les jours de la semaine du 1er octobre 2023 au 1er janvier 2024.

![](../assets/workflow-scheduler2.png)



