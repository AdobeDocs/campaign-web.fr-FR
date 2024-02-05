---
audience: end-user
title: Utiliser l’activité de workflow Planificateur
description: Découvrez comment utiliser l’activité de workflow Planificateur.
badge: label="Disponibilité limitée"
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 023777b88fa5c80e110fcf334517f7cef1c7f1ee
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 100%

---

# Planificateur {#scheduler}


>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Activité Planificateur"
>abstract="L’activité **Planificateur** vous permet de planifier le démarrage du workflow. Cette activité est à considérer comme un démarrage planifié. Elle ne peut être utilisée que comme première activité du workflow."


L’activité **Planificateur** est une activité de **contrôle de flux**. Elle permet de planifier le démarrage du workflow. Cette activité est à considérer comme un démarrage planifié. Elle ne peut être utilisée que comme première activité du workflow.

## Bonnes pratiques{#scheduler-best-practices}

* Ne planifiez pas l’exécution d’un workflow à une fréquence supérieure à toutes les 15 minutes, car cela peut nuire aux performances générales du système et créer des blocages dans la base de données.
* Pour envoyer une diffusion ponctuelle dans votre workflow, vous pouvez ajouter une activité Planificateur et la configurer pour qu’elle s’exécute **une fois**. Vous pouvez également définir le **Planning** dans les paramètres de la diffusion.
* Si vous souhaitez envoyer une diffusion récurrente dans votre workflow, vous devez utiliser une activité **Planificateur** et définir la fréquence d’exécution. L’activité de diffusion récurrente ne permet pas de définir de planning.

## Configurer l’activité Planificateur {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Validité du planificateur"
>abstract="Vous pouvez définir une période de validité pour le planificateur. Elle peut être permanente (par défaut) ou valide jusqu’à une date spécifique."


>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Options du planificateur"
>abstract="Définissez la fréquence du planificateur. Il peut être exécuté à un moment précis, ou encore une ou plusieurs fois par jour, semaine ou mois."

Pour configurer l’activité **Planificateur**, procédez comme suit :

![](../assets/workflow-scheduler.png)

1. Ajoutez une activité **Plafinicateur** à votre workflow.

1. Configurez la **Fréquence d’exécution** :

   * **Une seule fois** : le workflow n’est exécuté qu’une seule fois.

   * **Quotidienne** : le workflow est exécuté à une heure précise, une fois par jour.

   * **Plusieurs fois par jour** : le workflow est exécuté de manières régulière plusieurs fois par jour. Vous pouvez configurer des exécutions à des heures et dates spécifiques ou périodiquement.

   * **Hebdomadaire** : le workflow est exécuté à un instant défini, une ou plusieurs fois par semaine.

   * **Mensuelle** : le workflow est exécuté à un instant défini, une ou plusieurs fois par mois. Vous pouvez sélectionner les mois auxquels le workflow doit être exécuté. Vous pouvez également configurer des exécutions un jour de semaine spécifié du mois, comme le deuxième mardi du mois.

1. Spécifiez les détails de l&#39;exécution selon la fréquence choisie. Les champs du détail peuvent varier en fonction de la fréquence sélectionnée (heure, fréquence de répétition, jours spécifiques, etc.).

1. Cliquez sur **Prévisualiser les heures de lancement** pour vérifier le planning des dix prochaines exécutions de votre workflow.

1. Définissez la période de validité du planificateur :

   * **Permanent (n’expire jamais)** : le workflow est exécuté selon la fréquence définie, sans limite de période ou de nombre d’itérations.

   * **Période de validité** : le workflow est exécuté selon la fréquence définie, jusqu’à une date spécifique. Vous devez spécifier les dates de début et de fin.

>[!NOTE]
>
>Pour démarrer immédiatement le workflow, cliquez sur le bouton **Exécuter la tâche en attente** dans la barre d’actions supérieure du planificateur. Ce bouton n’est disponible que lorsque vous avez démarré le workflow.

## Exemple{#scheduler-example}

Dans l’exemple suivant, l’activité est configurée de sorte que le workflow s’exécute plusieurs fois par jour à 9h00 et 12h00, tous les jours de la semaine du 1er octobre 2023 au 1er janvier 2024.

![](../assets/workflow-scheduler2.png)
