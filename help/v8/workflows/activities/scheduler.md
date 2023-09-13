---
audience: end-user
title: Utilisation de l’activité de workflow Planificateur
description: Découvrez comment utiliser l’activité de workflow Planificateur
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 62%

---


# Planificateur {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Activité Planificateur"
>abstract="L&#39;activité Planificateur permet..."

L&#39;activité Planificateur permet de planifier le déclenchement d&#39;un workflow ou d&#39;une activité.

L&#39;activité Planificateur est à considérer comme un départ planifié. Cette activité ne peut être utilisée que comme première activité du workflow.

## Bonnes pratiques

* Ne planifiez pas l’exécution d’un workflow à une fréquence supérieure à toutes les 15 minutes, car cela peut nuire aux performances générales du système et créer des blocs dans la base de données.

## Configuration

Pour configurer la variable **Planificateur** activité :

1. Ajouter un **Planificateur** à votre workflow.

1. Configurez la variable **Fréquence d&#39;exécution**:

   * Une seule fois : le workflow n&#39;est exécuté qu&#39;une seule fois.

   * Quotidienne : le workflow est exécuté à une heure précise, une fois par jour.

   * Plusieurs fois par jour : le workflow est exécuté de manières régulière plusieurs fois par jour. Vous pouvez configurer des exécutions à des heures et dates spécifiques ou périodiquement.

   * Hebdomadaire : le workflow est exécuté à un instant défini, une ou plusieurs fois par semaine.

   * Mensuelle : le workflow est exécuté à un instant défini, une ou plusieurs fois par mois. Vous pouvez sélectionner les mois auxquels le workflow doit être exécuté. Vous pouvez également configurer des exécutions un jour de semaine spécifié du mois, comme le deuxième mardi du mois.
1. Spécifiez les détails de l&#39;exécution selon la fréquence choisie. Les champs du détail peuvent varier en fonction de la fréquence sélectionnée (heure, fréquence de répétition, jours spécifiques, etc.).

1. Cliquez sur **Aperçu des heures de lancement** pour vérifier le planning des dix prochaines exécutions de votre workflow.

1. Définissez la période de validité du planificateur :

   * Permanent (n&#39;expire jamais) : le workflow sera exécuté selon la fréquence d&#39;exécution définie, sans limite dans le temps ni au niveau du nombre d&#39;itérations.

   * Période de validité : le workflow sera exécuté selon la fréquence d&#39;exécution définie, jusqu&#39;à une date spécifique. Indiquez alors la date limite d&#39;exécution.

## Exemple


