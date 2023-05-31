---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 696fa6192c16f8fd1d2dd77ad533203277f8a2dd
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 96%

---

# Configurer les paramètres du workflow {#workflow-settings}

contenu à déterminer

Définir les paramètres disponibles à partir du bouton dans la zone de travail du workflow
<!--à reformuler-->

## Propriétés de workflow  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriétés de workflow"
>abstract="À déterminer"

(= comme lors de la création du workflow ? à vérifier)

* Libellé
* Options additionnelles
* Nom interne
* Dossier
* Campagne liée > modification possible. Si tel est le cas, le workflow disparaîtra de la campagne en cours et apparaîtra dans la nouvelle campagne liée.

   Lors de la création d&#39;un workflow au sein d&#39;une opération, vous trouverez un champ Campaign supplémentaire qui vous permet d&#39;identifier facilement la campagne associée au workflow et d&#39;y accéder.

* Fuseau horaire : définissez un fuseau horaire spécifique à utiliser par défaut dans toutes les activités du workflow. Par défaut, le fuseau horaire du workflow est celui défini pour l’opérateur de Campaign actuel.
* Superviseur : lorsqu’un workflow est en erreur, la ou les personnes appartenant au groupe de supervision du workflow sont averties par e-mail, à condition que leur adresse e-mail soit indiquée dans leur profil. Ce groupe est sélectionné dans le champ **[!UICONTROL Superviseur(s)]** des propriétés de workflow.
* description

## Paramètres de segmentation

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Paramètres de segmentation"
>abstract="À déterminer"

* Dimension de ciblage :

   Lors des opérations de segmentation des données, la clé de ciblage est associée à une dimension de filtrage. La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, titulaires d’un contrat, opérateur ou opératrice, abonnées ou abonnés, etc. La dimension de filtrage permet de sélectionner la population selon certains critères : détention d’un contrat, inscription à une newsletter, etc.

* Conserver les résultats : l’option **Conserver le résultat des populations intermédiaires entre deux exécutions** permet de conserver les tables temporaires entre deux exécutions d’un workflow.  Elle est disponible dans l&#39;onglet **[!UICONTROL Général]** des propriétés du workflow et peut être utilisée à des fins de développement et de test pour surveiller les données et vérifier les résultats. Vous pouvez utiliser cette option dans les environnements de développement, mais ne l&#39;utilisez jamais dans les environnements de production. La conservation des tables temporaires peut entraîner une augmentation significative de la taille de la base de données et, par la suite, l&#39;atteinte de la limite de taille. De plus, cela ralentira la sauvegarde.

   Seules les tables de travail de la dernière exécution du workflow sont conservées. Celles des exécutions précédentes sont purgées par le workflow de **[!UICONTROL nettoyage]** qui s&#39;exécute tous les jours.

   >[!CAUTION]
   >
   >Ne cochez **jamais** cette option dans un workflow de **production**. Elle sert à analyser les résultats et est conçue uniquement à des fins de test. Elle ne doit donc être utilisée que dans les environnements de développement ou d&#39;évaluation.

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
