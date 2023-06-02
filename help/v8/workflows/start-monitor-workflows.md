---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 8aa76369-c9f3-4c5b-9a51-101b239727e6
source-git-commit: cc9566d1781d5a190b488182a8b05a99d396ac8c
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 18%

---

# Démarrer et suivre le workflow {#start-monitor}

Une fois que vous avez créé votre workflow et conçu les tâches à effectuer dans la zone de travail, vous pouvez le lancer et contrôler son exécution.

## Démarrez le workflow. {#start}

Pour démarrer le workflow, accédez à la **[!UICONTROL Workflows]** ou l&#39;opération associée, puis cliquez sur le bouton **[!UICONTROL Début]** dans le coin supérieur droit de la zone de travail.

Une fois le workflow en cours d’exécution, chaque activité de la zone de travail est exécutée dans un ordre séquentiel, jusqu’à ce que la fin du workflow soit atteinte.

Vous pouvez suivre la progression des profils ciblés en temps réel à l’aide d’un flux visuel. Vous pouvez ainsi identifier rapidement l’état de chaque activité et le nombre de profils en transition entre elles.

![](assets/workflow-execution.png)

>[!NOTE]
>
>Vous pouvez désactiver le flux visuel à l’aide de la méthode **[!UICONTROL Masquer la progression]** dans la barre d’actions supérieure de la zone de travail.

## Surveiller l’exécution des activités {#activities}

Les indicateurs visuels situés dans le coin supérieur droit de chaque activité vous permettent de vérifier leur exécution :

| Indicateur visuel | Description |
|-----|------------|
| ![](assets/activity-status-pending.png) | L’activité est en cours d’exécution. |
| ![](assets/activity-status-orange.png) | L’activité nécessite votre attention. Cela peut impliquer de confirmer l&#39;envoi d&#39;une diffusion ou de prendre une mesure nécessaire. |
| ![](assets/activity-status-red.png) | L’activité a rencontré une erreur. Pour résoudre ce problème, ouvrez les journaux de workflow pour plus d’informations. |
| ![](assets/activity-status-green.png) | L’activité a été exécutée avec succès. |

## Surveiller les journaux et les tâches {#logs-tasks}

La surveillance des logs et des tâches des workflows est une étape clé pour analyser vos workflows et s’assurer qu’ils s’exécutent correctement. Elles sont accessibles à partir du **[!UICONTROL Journaux]** qui est disponible dans la barre d’outils d’actions et dans le volet des propriétés de chaque activité.

Le **[!UICONTROL Logs et tâches]** fournit un historique de l’exécution du workflow, en enregistrant toutes les actions de l’utilisateur et les erreurs rencontrées. Cet historique est conservé pendant la durée spécifiée dans le workflow. [options d’exécution](workflow-settings.md). Pendant cette durée, tous les messages sont enregistrés, même après un redémarrage du workflow. Si vous ne souhaitez pas conserver les messages d’une exécution précédente, cliquez sur le bouton **[!UICONTROL Purge de l’historique]** bouton .

![](assets/workflow-logs.png)

Deux types d’informations sont disponibles :

* Le **[!UICONTROL Journal]** contient l&#39;historique d&#39;exécution de toutes les activités du workflow. Il répertorie par ordre chronologique les opérations réalisées et les erreurs d’exécution.
* L’onglet **[!UICONTROL Tâches]** permet de voir le séquencement de l’exécution des activités.

Dans les deux onglets, vous pouvez choisir les colonnes affichées et leur ordre, appliquer des filtres et utiliser le champ de recherche pour trouver rapidement les informations souhaitées.

## Commandes d’exécution des workflows {#execution-commands}

La barre d’actions située dans le coin supérieur droit fournit des commandes qui vous permettent de gérer l’exécution du workflow. Vous pouvez ainsi :

* **[!UICONTROL Début]** / **[!UICONTROL Reprendre]** l&#39;exécution du workflow, qui prend alors le statut En cours . Si le workflow était en pause, il s’agit d’une reprise, sinon il s’agit d’un démarrage et les activités initiales sont alors activées.

* **[!UICONTROL Pause]** l&#39;exécution du workflow, qui prend alors le statut En pause . Aucune nouvelle activité ne sera activée jusqu’à la prochaine reprise, mais les opérations en cours ne sont pas suspendues.

* **[!UICONTROL Arrêter]** un workflow en cours d&#39;exécution, qui prend alors le statut Terminé . Si possible, les opérations en cours sont interrompues. Il n’est pas possible de reprendre à l’endroit où le workflow s’est arrêté.
