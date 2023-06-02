---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 51648665-8400-426c-85cf-dbf5f4f81d20
source-git-commit: be7cdfbffbe5c3b1a7ec58e5c60856a6bdc56200
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 6%

---

# Accès et gestion des workflows {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Workflows"
>abstract="Dans cet écran, vous pouvez accéder à la liste complète des workflows de campagne et autonome, vérifier leur état actuel, les dates de dernière exécution/prochaine exécution et créer un nouveau workflow. Accédez à l&#39;onglet &quot;Modèle&quot; pour accéder aux modèles de workflow disponibles."

Le **[!UICONTROL Workflows]** vous permet d’accéder à la liste complète des workflows. Cette liste comprend les deux éléments suivants : **workflows autonomes** qui ont été créés à partir de cet écran ; et **workflows de campagne**, qui ont été créées dans une campagne.

![](assets/workflow-list.png)

Chaque workflow de la liste affiche des informations sur son [status](#status), la dernière exécution ou modification qu’il a effectuée, ainsi que la date et l’heure d’exécution planifiée suivantes.

Vous pouvez personnaliser les colonnes affichées en cliquant sur le **[!UICONTROL Configuration d’une colonne pour une disposition personnalisée]** située dans le coin supérieur droit de la liste. Vous pouvez ainsi ajouter des informations supplémentaires à la liste, telles que la dernière activité en erreur pour chaque workflow ou la dimension de ciblage appliquée.

En outre, une barre de recherche et des filtres sont disponibles pour faciliter la recherche dans la liste. Vous pouvez par exemple filtrer les workflows afin de n&#39;afficher que ceux appartenant à une campagne ou ceux traités au cours d&#39;une période spécifique.

Pour dupliquer ou supprimer un workflow, cliquez sur le bouton représentant des points de suspension puis sélectionnez **[!UICONTROL Dupliquer]** ou **[!UICONTROL Supprimer]**.

>[!NOTE]
>
>Vous pouvez dupliquer un workflow en cours, mais vous ne pouvez pas le supprimer.

## Statuts des workflows {#status}

Les workflows peuvent avoir plusieurs états :

* **[!UICONTROL Version préliminaire]**: Le workflow a été créé et enregistré.
* **[!UICONTROL En cours]**: Le workflow est en cours d’exécution.
* **[!UICONTROL Terminé]**: L’exécution du workflow est terminée.
* **[!UICONTROL En pause]**: Le workflow a été suspendu.
* **[!UICONTROL En erreur]**: Le workflow a rencontré une erreur. Ouvrez le workflow et accédez aux logs et tâches pour identifier l&#39;erreur et la résoudre. [Découvrez comment surveiller les logs et les tâches](start-monitor-workflows.md#logs-tasks)

Des informations détaillées sur le démarrage et le suivi de l&#39;exécution des workflows sont disponibles dans la section [cette page](start-monitor-workflows.md).

## Les modèles de workflows {#templates}

Le **[!UICONTROL Modèles]** répertorie tous les modèles de workflows disponibles.

Les modèles de workflow contiennent des activités préconfigurées et des configurations globales des propriétés qui peuvent être réutilisées pour créer de nouveaux workflows. Ils sont créés à partir de la console cliente. [Découvrez comment utiliser des modèles](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)
