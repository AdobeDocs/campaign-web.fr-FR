---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 100%

---

# Configurer les paramètres de workflow {#workflow-settings}

Lors de l’orchestration des activités de workflow dans la zone de travail, vous pouvez accéder aux paramètres avancés du workflow. Par exemple, vous pouvez définir un fuseau horaire spécifique pour le workflow, gérer le comportement du workflow en cas d’erreur ou indiquer le délai après lequel l’historique du workflow doit être purgé.

Ces paramètres sont prédéfinis dans le modèle sélectionné lors de la création du workflow, mais peuvent être modifiés selon les besoins du workflow.

Pour ce faire, cliquez sur le bouton **[!UICONTROL Paramètres de workflow]** dans le coin supérieur gauche de la zone de travail, en regard du libellé du workflow.

![](assets/workflow-settings.png)

## Propriétés de workflow  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriétés de workflow "
>abstract="Cette section fournit des propriétés de workflow génériques, qui sont également accessibles lors de la création du workflow. Vous pouvez choisir le modèle à utiliser pour créer le workflow et indiquer un libellé. Développez la section Options supplémentaires pour configurer des paramètres spécifiques tels que le dossier de stockage du workflow ou le fuseau horaire."

La section **[!UICONTROL Propriétés]** fournit des paramètres génériques, qui sont également accessibles lors de la création du workflow.

* **[!UICONTROL Libellé]** : le libellé du workflow qui s’affiche dans la liste.
* **[!UICONTROL Nom]** : le nom interne du workflow.
* **[!UICONTROL Dossier]** : le dossier dans lequel le workflow doit être enregistré.
* **[!UICONTROL Campagne liée]** : ce champ s’affiche si le workflow a été créé dans une campagne. Il vous permet d’ouvrir la campagne associée.
* **[!UICONTROL Fuseau horaire]** : définissez un fuseau horaire spécifique à utiliser par défaut dans toutes les activités du workflow. Par défaut, le fuseau horaire du workflow est celui défini pour l’opérateur de Campaign actuel.
* **[!UICONTROL Superviseur(s)]** : lorsqu’un workflow rencontre une erreur, la ou les personnes appartenant au groupe de supervision du workflow sont averties par e-mail, à condition que leur adresse e-mail soit indiquée dans leur profil.
* **[!UICONTROL Description]** : ce champ permet d’indiquer une description du workflow.

## Paramètres de segmentation

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Paramètres de segmentation"
>abstract="Cette section vous permet de sélectionner la dimension de ciblage pour cibler les profils dans le workflow et de conserver ou non les résultats du workflow entre deux exécutions. Cette option ne doit être utilisée qu’à des fins de test. Elle ne doit en aucun cas être activée dans un workflow de production."

* **[!UICONTROL Dimension de ciblage]** : sélectionnez la dimension de ciblage à utiliser pour cibler les profils (destinataires, bénéficiaires d’un contrat, opérateur ou opératrice, abonnées et abonnés, etc.).
* **[!UICONTROL Conserver le résultat des populations intermédiaires entre deux exécutions]** : par défaut, seules les tables de travail de la dernière exécution du workflow sont conservées. Les tables de travail des exécutions précédentes sont purgées par un workflow technique qui s’exécute quotidiennement.

  Si cette option est activée, les tables de travail sont conservées même après l’exécution du workflow. Vous pouvez l’utiliser à des fins de test. N’utilisez donc cette option que dans les environnements de développement ou d’évaluation. Cette option ne doit jamais être activée dans un workflow de production.

## Paramètres d&#39;exécution

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Paramètres d&#39;exécution"
>abstract="Dans cette section, vous pouvez définir les paramètres relatifs à l’exécution du workflow, par exemple le nombre de jours pendant lesquels l’historique du workflow est conservé."

* **[!UICONTROL Jours d’historique]** : indique le nombre de jours après lesquels l’historique doit être purgé. L’historique contient des éléments liés au workflow : logs, tâches, événements (objets techniques liés à l’opération du workflow). La valeur par défaut est de 30 jours pour les modèles de workflow prêts à l’emploi. La purge de l’historique est effectuée par le workflow technique de nettoyage de la base de données, qui est exécuté par défaut tous les jours.

  >[!IMPORTANT]
  >
  >Si le champ **[!UICONTROL Jours d’historique]** n’est pas renseigné, la valeur prise en compte est « 1 », ce qui signifie que l’historique sera purgé après 1 jour.

* **[!UICONTROL Affinité par défaut]** : si votre installation comprend plusieurs serveurs de workflow, ce champ permet de choisir la machine sur laquelle le workflow sera exécuté. Si la valeur définie dans ce champ n’existe sur aucun serveur, le workflow reste en attente.

* **[!UICONTROL Enregistrer les requêtes SQL dans le log]** : permet d’enregistrer les requêtes SQL du workflow dans les logs. Cette fonctionnalité est réservée aux utilisateurs et utilisatrices avancés. Elle s’applique aux workflows qui contiennent des activités de ciblage, comme **[!UICONTROL Créer une audience]**. Lorsque cette option est activée, les requêtes SQL envoyées à la base de données lors de l’exécution du workflow sont affichées dans les logs du workflow, ce qui vous permet de les analyser afin d’optimiser les requêtes ou de diagnostiquer les problèmes.

## Paramètres de gestion des erreurs

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Paramètres de gestion des erreurs"
>abstract="Dans cette section, vous pouvez gérer le comportement du workflow lorsqu’une erreur se produit lors de son exécution (mettre en pause/arrêter son exécution ou ignorer les erreurs)."

* **[!UICONTROL Gestion des erreurs]** : ce champ vous permet de définir les actions à effectuer si une tâche de workflow rencontre une erreur. Deux choix s’offrent à vous :

   * **[!UICONTROL Suspendre le processus]** : le workflow est automatiquement mis en pause et adopte le statut **[!UICONTROL Échec]**. Une fois le problème résolu, reprenez l’exécution du workflow à l’aide des boutons **[!UICONTROL Reprendre]**.
   * **[!UICONTROL Ignorer]** : le statut de la tâche qui a déclenché l’erreur passe à **[!UICONTROL Échec]**, mais le workflow conserve le statut **[!UICONTROL Démarré]**.<!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abandonner le processus]** : le workflow est automatiquement arrêté et adopte le statut **[!UICONTROL Échec]**. Une fois le problème résolu, redémarrez le workflow à l’aide du bouton **[!UICONTROL Démarrer]**.

* **[!UICONTROL Erreurs consécutives]** : ce champ est disponible lorsque la valeur **[!UICONTROL Ignorer]** est sélectionnée dans le champ **[!UICONTROL En cas d’erreur]**. Vous pouvez indiquer le nombre d’erreurs qui peuvent être ignorées avant l’arrêt du processus. Une fois ce nombre atteint, le statut du workflow passe à **[!UICONTROL Échec]**. Si la valeur de ce champ est 0, le workflow ne sera jamais arrêté, quel que soit le nombre d’erreurs.
