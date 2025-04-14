---
audience: end-user
title: Utiliser l’activité de workflow Planificateur
description: Découvrez comment utiliser l’activité de workflow Planificateur.
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 29%

---

# Planificateur {#scheduler}

>[!CONTEXTUALHELP]
>
>L’activité **Planificateur** est une activité de **contrôle de flux**. Elle permet de planifier le démarrage du workflow. Cette activité est à considérer comme un démarrage planifié. Elle ne peut être utilisée que comme première activité du workflow.

## Bonnes pratiques {#scheduler-best-practices}

* Ne planifiez pas l’exécution d’un workflow à une fréquence supérieure à toutes les 15 minutes, car cela peut nuire aux performances générales du système et créer des blocs dans la base de données.
* Pour envoyer une diffusion unique dans votre workflow, ajoutez une activité Planificateur et définissez-la pour qu’elle s’exécute **Une fois**. Définissez le **Planning** dans les paramètres de la diffusion.
* Pour envoyer une diffusion récurrente dans votre workflow, utilisez une activité **Planificateur** et définissez la fréquence d’exécution. L’activité de diffusion récurrente ne permet pas de définir de planning.

## Configurer l’activité Planificateur {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Scheduler validity"
>abstract="You can define a validity period for the scheduler. It can be permanent (default), or can be valid until a specific date."

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler options"
>abstract="Define the frequency of the scheduler. It can be executed at a specific moment, once or several times a day, week or month."

Pour configurer l’activité **Planificateur**, procédez comme suit :

![Interface de configuration de l’activité Planificateur](../assets/workflow-scheduler.png)

1. Ajoutez une activité **Plafinicateur** à votre workflow.

1. Configurez la **Fréquence d’exécution** :

   * **Une fois** : le workflow est exécuté une seule fois.
   * **Quotidien** : le workflow est exécuté à une heure spécifique, une fois par jour.
   * **Plusieurs fois par jour** : le workflow est exécuté régulièrement plusieurs fois par jour. Configurez les exécutions à des moments spécifiques ou de manière périodique.
   * **Hebdomadaire** : le workflow est exécuté à un moment spécifié, une ou plusieurs fois par semaine.
   * **Mensuel** : le workflow est exécuté à un moment précis, une ou plusieurs fois par mois. Sélectionnez les mois pendant lesquels le workflow doit être exécuté. Vous pouvez également configurer des exécutions les jours de la semaine spécifiés du mois, comme le deuxième mardi du mois.

1. Spécifiez les détails de l&#39;exécution selon la fréquence choisie. Les champs de détail peuvent varier en fonction de la fréquence utilisée (durée, fréquence de répétition, jours spécifiés et options similaires).

1. Cliquez sur **Prévisualiser les heures de lancement** pour vérifier le planning des dix prochaines exécutions de votre workflow.

1. Définissez la période de validité du planificateur :

   * **Permanent (n’expire jamais)** : le workflow est exécuté selon la fréquence spécifiée, sans limite de durée ni de nombre d’itérations.
   * **Période de validité** : le workflow est exécuté selon la fréquence spécifiée, jusqu&#39;à une date spécifique. Spécifiez les dates de début et de fin.

>[!NOTE]\
Si vous souhaitez démarrer le workflow immédiatement, cliquez sur **Exécuter la tâche en attente** dans la barre d’actions supérieure du planificateur. Ce bouton n’est disponible que lorsque le workflow a été démarré.

## Exemple {#scheduler-example}

Dans l’exemple suivant, l’activité est configurée de sorte que le workflow s’exécute plusieurs fois par jour à 9 h et 12 h, tous les jours de la semaine du 1er octobre 2023 au 1er janvier 2024.

![Exemple de configuration d’une activité Planificateur](../assets/workflow-scheduler2.png)