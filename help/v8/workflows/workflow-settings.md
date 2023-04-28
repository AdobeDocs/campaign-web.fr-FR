---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
badge: label="Alpha" type="Positive"
source-git-commit: 60cd0ed8dcbe3e6003c1cde674fe3441d6d88869
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 61%

---

# Configuration des paramètres du workflow {#workflow-settings}

contenu à déterminer

définir les paramètres disponibles à partir du bouton dans la zone de travail du workflow ;
<!--à reformuler-->

## Propriétés d&#39;exécution  {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriétés de workflow"
>abstract="À déterminer"

(= identique à lors de la création du workflow ? à vérifier)

* Libellé
* Options additionnelles
* Nom interne
* Dossier
* Campagne liée > peut la modifier. Si tel est le cas, le workflow disparaîtra de la campagne en cours et apparaîtra dans la nouvelle opération liée.
* Fuseau horaire : définir un fuseau horaire spécifique à utiliser par défaut dans toutes les activités du workflow ; Par défaut, le fuseau horaire du workflow est celui défini pour l’opérateur de Campaign actuel.
* Superviseur : Lorsqu&#39;un workflow est en erreur, le ou les opérateurs appartenant au groupe de supervision du workflow sont avertis par email, sous réserve que leur adresse email soit indiquée dans leur profil. Ce groupe est sélectionné dans la variable **[!UICONTROL Superviseur(s)]** champ des propriétés du workflow.
* description

## Paramètres de segmentation

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Paramètres de segmentation"
>abstract="À déterminer"

* dimension de ciblage :

   Lors des opérations de segmentation des données, la dimension de ciblage est associée à une dimension de filtrage. La dimension de ciblage permet de définir la population ciblée par l&#39;opération : destinataires, titulaires d&#39;un contrat, opérateur, abonnés, etc. La dimension de filtrage permet de sélectionner la population selon certains critères : détention d&#39;un contrat, inscription à une newsletter, etc.

* conserver les résultats : Le **Conserver le résultat des populations intermédiaires entre deux exécutions** conserve les tables temporaires entre deux exécutions d’un workflow.  Elle est disponible dans l&#39;onglet **[!UICONTROL Général]** des propriétés du workflow et peut être utilisée à des fins de développement et de test pour surveiller les données et vérifier les résultats. Vous pouvez utiliser cette option dans les environnements de développement, mais ne l&#39;utilisez jamais dans les environnements de production. La conservation des tables temporaires peut entraîner une augmentation significative de la taille de la base de données et, par la suite, l&#39;atteinte de la limite de taille. De plus, cela ralentira la sauvegarde.

   Seules les tables de travail de la dernière exécution du workflow sont conservées. Celles des exécutions précédentes sont purgées par le workflow de **[!UICONTROL nettoyage]** qui s&#39;exécute tous les jours.

   >[!CAUTION]
   >
   >Ne cochez **jamais** cette option dans un workflow de **production**. Elle sert à analyser les résultats et est conçue uniquement à des fins de test. Elle ne doit donc être utilisée que dans les environnements de développement ou d&#39;évaluation.

## Paramètres d&#39;exécution du workflow

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Paramètres d’exécution"
>abstract="À déterminer"

* Jours d’historique : Les tables de travail de la base conservent un historique des exécutions (tâches, événements, journal). Vous pouvez définir ici le nombre de jours à archiver pour ce workflow : le processus de nettoyage supprimera les archives les plus anciennes une fois par jour. Si la valeur de ce champ est zéro, l’archive ne sera jamais supprimée.

   indique le nombre de jours après lesquels l’historique doit être purgé. L’historique contient des éléments liés au workflow : logs, tâches, événements (objets techniques liés à l’opération du workflow), ainsi que les fichiers téléchargés par l’activité **[!UICONTROL Transfert de fichier]**. La valeur par défaut est de 30 jours pour les modèles de workflow d’usine.

   La purge de l&#39;historique est effectuée par le workflow technique Nettoyage de la base , qui est exécuté par défaut tous les jours.

   >[!IMPORTANT]
   >
   >Si le champ **[!UICONTROL Jours d’historique]** n’est pas renseigné, la valeur prise en compte est « 1 », ce qui signifie que l’historique sera purgé après 1 jour.

* affinité par défaut : ce champ vous permet de forcer l’exécution d’un workflow ou d’une activité de workflow sur une machine en particulier.   Si votre installation comprend plusieurs serveurs de workflow, utilisez ce champ pour choisir sur quelle machine le workflow s&#39;exécutera. Si la valeur définie dans ce champ n&#39;existe au niveau d&#39;aucun serveur, le workflow restera en attente.

* enregistrer sql queriesi dans le journal : permet d&#39;enregistrer les requêtes SQL du workflow dans les logs. (où accéder aux journaux sql ?)

   Cette fonctionnalité est réservée aux utilisateurs experts. Elle concerne les workflows qui contiennent des activités de ciblage (requête, union, intersection, etc.). Lorsque cette option est cochée, les requêtes SQL envoyées vers la base lors de l&#39;exécution du workflow sont affichées dans Adobe Campaign : vous pouvez ainsi les analyser afin d&#39;optimiser les requêtes ou diagnostiquer d&#39;éventuels problèmes.

   Les requêtes sont affichées dans un onglet **[!UICONTROL Logs SQL]** qui est ajouté au workflow (sauf pour les workflows d&#39;opération) et à l&#39;activité **[!UICONTROL Propriétés]** lorsque l&#39;option est activée. L&#39;onglet **[!UICONTROL Suivi]** inclut également les requêtes SQL.

## Paramètres de gestion des erreurs

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Paramètres de gestion des erreurs"
>abstract="À déterminer"

* Ce champ vous permet de définir l&#39;action à effectuer lorsqu&#39;une tâche du workflow est en erreur. Deux options sont disponibles :

   Suspendre le processus : le workflow est automatiquement suspendu. Le statut du workflow est alors En échec. Lorsque le problème est résolu, relancez le workflow en utilisant les boutons Démarrer ou Redémarrer.

   Ignorer : la tâche ayant provoqué l&#39;erreur prend le statut En échec, mais le workflow garde le statut Démarré. Ce paramétrage est pertinent dans le cas de tâches récurrentes : si la branche comporte un planificateur, celui-ci se déclenchera normalement à sa prochaine date d&#39;exécution.

* Erreurs consécutives : Ce champ devient disponible lorsque la valeur Ignorer est sélectionnée dans le champ En cas d’erreur . Vous pouvez spécifier le nombre d’erreurs qui peuvent être ignorées avant l’arrêt du processus. Une fois ce nombre atteint, le statut du workflow passe à En échec. Si la valeur de ce champ est 0, le workflow ne sera jamais arrêté quel que soit le nombre d&#39;erreurs.
