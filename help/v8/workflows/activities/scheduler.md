---
audience: end-user
title: Utiliser l’activité de workflow Planificateur
description: Découvrez comment utiliser l’activité de workflow Planificateur.
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 058a9347329b35e49463b7d74bffa5b3c69b4a92
workflow-type: ht
source-wordcount: '505'
ht-degree: 100%

---

# Planificateur {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Activité Planificateur"
>abstract="L’activité **Planificateur** vous permet de planifier le démarrage du workflow. Cette activité est à considérer comme un démarrage planifié. Elle ne peut être utilisée que comme première activité du workflow."

L’activité **Planificateur** est une activité de **contrôle de flux**. Elle permet de planifier le démarrage du workflow. Cette activité est à considérer comme un démarrage planifié. Elle ne peut être utilisée que comme première activité du workflow.

## Bonnes pratiques {#scheduler-best-practices}

* Ne planifiez pas l’exécution d’un workflow à une fréquence supérieure à toutes les 15 minutes, car cela peut nuire aux performances générales du système et créer des blocages dans la base de données.
* Pour envoyer une diffusion ponctuelle dans votre workflow, ajoutez une activité Planificateur et configurez-la pour qu’elle s’exécute **une fois**. Définissez le **Planning** dans les paramètres de la diffusion.
* Pour envoyer une diffusion récurrente dans votre workflow, utilisez une activité **Planificateur** et définissez la fréquence d’exécution. L’activité de diffusion récurrente ne permet pas de définir de planning.

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

![Interface de configuration de l’activité Planificateur](../assets/workflow-scheduler.png)

1. Ajoutez une activité **Plafinicateur** à votre workflow.

1. Configurez la **Fréquence d’exécution** :

   * **Une seule fois** : le workflow n’est exécuté qu’une seule fois.
   * **Quotidienne** : le workflow est exécuté à une heure précise, une fois par jour.
   * **Plusieurs fois par jour** : le workflow est exécuté de manières régulière plusieurs fois par jour. Configurez des exécutions à des heures et dates spécifiques ou périodiquement.
   * **Hebdomadaire** : le workflow est exécuté à un moment défini, une ou plusieurs fois par semaine.
   * **Mensuelle** : le workflow est exécuté à un moment défini, une ou plusieurs fois par mois. Sélectionnez les mois pendant lesquels le workflow doit être exécuté. Vous pouvez également configurer des exécutions lors de jours de semaine spécifiés du mois, comme le deuxième mardi du mois.

1. Spécifiez les détails de l&#39;exécution selon la fréquence choisie. Les champs de détails peuvent varier en fonction de la fréquence sélectionnée (heure, fréquence de répétition, jours spécifiques et options similaires).

1. Cliquez sur **Prévisualiser les heures de lancement** pour vérifier le planning des dix prochaines exécutions de votre workflow.

1. Définissez la période de validité du planificateur :

   * **Permanent (n’expire jamais)** : le workflow est exécuté selon la fréquence définie, sans limite de période ou de nombre d’itérations.
   * **Période de validité** : le workflow est exécuté selon la fréquence définie, jusqu’à une date spécifique. Indiquez les dates de début et de fin.

>[!NOTE]
>Si vous souhaitez démarrer immédiatement le workflow, cliquez sur le bouton **Exécuter la tâche en attente** dans la barre d’actions supérieure du planificateur. Ce bouton n’est disponible que lorsque le workflow a été démarré.

## Exemple {#scheduler-example}

Dans l’exemple suivant, l’activité est configurée de sorte que le workflow s’exécute plusieurs fois par jour à 9h00 et 12h00, tous les jours de la semaine du 1er octobre 2023 au 1er janvier 2024.

![Exemple de configuration d’une activité Planificateur](../assets/workflow-scheduler2.png)
