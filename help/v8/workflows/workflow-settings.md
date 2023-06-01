---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 806e465b7c1df6cd26d68103c45b175371d73485
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 63%

---

# Configuration des paramètres avancés du workflow {#workflow-settings}

Lors de l’orchestration des activités de workflow dans la zone de travail, vous pouvez accéder aux paramètres avancés liés au workflow. Par exemple, vous pouvez définir un fuseau horaire spécifique pour le workflow, gérer le comportement du workflow en cas d’erreur ou gérer le délai après lequel l’historique du workflow doit être purgé.

Pour ce faire, cliquez sur le bouton **[!UICONTROL Paramètres de workflow]** dans le coin supérieur gauche de la zone de travail, en regard du libellé du workflow.

![](assets/workflow-settings.png)

## Propriétés de workflow  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriétés de workflow"
>abstract="À déterminer"

La section Propriétés du workflow fournit des propriétés génériques qui sont également accessibles lors de la création du workflow.

* **[!UICONTROL Libellé]**: Libellé du workflow qui s’affiche dans la liste.
* **[!UICONTROL Nom interne]**: Nom interne du workflow.
* **[!UICONTROL Dossier]**: Dossier dans lequel le workflow doit être enregistré.
* **[!UICONTROL Campagne liée]**: Ce champ s&#39;affiche si le workflow a été créé dans une campagne. Il vous permet d’ouvrir la campagne associée.
* **[!UICONTROL Fuseau horaire]**: Définissez un fuseau horaire spécifique à utiliser par défaut dans toutes les activités du workflow. Par défaut, le fuseau horaire du workflow est celui défini pour l’opérateur de Campaign actuel.
* **[!UICONTROL Superviseur]**: Lorsqu&#39;un workflow est en erreur, le ou les opérateurs appartenant au groupe de supervision du workflow sont avertis par email, sous réserve que leur adresse email soit indiquée dans leur profil.
* **[!UICONTROL Description]**: Utilisez ce champ pour fournir une description de votre workflow.

## Paramètres de segmentation

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Paramètres de segmentation"
>abstract="À déterminer"

* **[!UICONTROL Dimension de ciblage]**: Sélectionnez la dimension de ciblage à utiliser pour cibler les profils : destinataires, bénéficiaires d&#39;un contrat, opérateur, abonnés, etc.
* **[!UICONTROL Conserver le résultat des populations intermédiaires entre deux exécutions]**: Par défaut, seules les tables de travail de la dernière exécution du workflow sont conservées. Les tables de travail des exécutions précédentes sont purgées par un workflow technique qui s’exécute tous les jours.

   Si cette option est activée, les tables de travail seront conservées même après l&#39;exécution du workflow. Vous pouvez l’utiliser à des fins de test et par conséquent ne doit être utilisé que dans les environnements de développement ou d’évaluation. Il ne doit jamais être vérifié dans un workflow de production,

## Paramètres d’exécution du workflow

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Paramètres d’exécution"
>abstract="À déterminer"

* Jours d’historique : les tables de travail de la base de données conservent un historique des exécutions (tâches, événements, journal). Vous pouvez définir ici le nombre de jours à archiver pour ce workflow : le processus de nettoyage supprimera les archives les plus anciennes une fois par jour. Si la valeur de ce champ est zéro, l’archive ne sera jamais supprimée.

   indique le nombre de jours après lesquels l’historique doit être purgé. L’historique contient des éléments liés au workflow : logs, tâches, événements (objets techniques liés à l’opération du workflow), ainsi que les fichiers téléchargés par l’activité **[!UICONTROL Transfert de fichier]**. La valeur par défaut est de 30 jours pour les modèles de workflow d’usine.

   La purge de l’historique est effectuée par le workflow technique de nettoyage de la base de données, qui est exécuté par défaut tous les jours.

   >[!IMPORTANT]
   >
   >Si le champ **[!UICONTROL Jours d’historique]** n’est pas renseigné, la valeur prise en compte est « 1 », ce qui signifie que l’historique sera purgé après 1 jour.

* Affinité par défaut : ce champ permet de forcer l’exécution d’un workflow ou d’une activité de workflow sur une machine en particulier.   Si votre installation comprend plusieurs serveurs de workflow, utilisez ce champ pour choisir sur quelle machine le workflow s’exécutera. Si la valeur définie dans ce champ n’existe au niveau d’aucun serveur, le workflow restera en attente.

* Enregistrer les requêtes SQL dans le journal : permet d’enregistrer les requêtes SQL du workflow dans les journaux. (où accéder aux journaux SQL ?)

   Cette fonctionnalité est réservée aux utilisateurs experts. Elle concerne les workflows qui contiennent des activités de ciblage (requête, union, intersection, etc.). Lorsque cette option est cochée, les requêtes SQL envoyées vers la base lors de l&#39;exécution du workflow sont affichées dans Adobe Campaign : vous pouvez ainsi les analyser afin d&#39;optimiser les requêtes ou diagnostiquer d&#39;éventuels problèmes.

   Les requêtes sont affichées dans un onglet **[!UICONTROL Logs SQL]** qui est ajouté au workflow (sauf pour les workflows d&#39;opération) et à l&#39;activité **[!UICONTROL Propriétés]** lorsque l&#39;option est activée. L&#39;onglet **[!UICONTROL Suivi]** inclut également les requêtes SQL.

## Paramètres de gestion des erreurs

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Paramètres de gestion des erreurs"
>abstract="À déterminer"

* Ce champ vous permet de définir l’action à effectuer lorsqu’une tâche du workflow est en erreur. Deux options sont disponibles :

   Suspendre le processus : le workflow est automatiquement suspendu. Le statut du workflow est alors en Échec. Lorsque le problème est résolu, relancez le workflow en utilisant les boutons Démarrer ou Redémarrer.

   Ignorer : la tâche ayant provoqué l’erreur prend le statut en Échec, mais le workflow garde le statut Démarré. Ce paramétrage est pertinent dans le cas de tâches récurrentes : si la branche comporte un planificateur, celui-ci se déclenchera normalement à sa prochaine date d’exécution.

* Erreurs consécutives : ce champ devient disponible lorsque la valeur Ignorer est sélectionnée dans le champ En cas d’erreur. Vous pouvez indiquer le nombre d’erreurs qui peuvent être ignorées avant l’arrêt du processus. Une fois ce nombre atteint, le statut du workflow passe en mode Échec. Si la valeur de ce champ est 0, le workflow ne sera jamais arrêté, quel que soit le nombre d’erreurs.
