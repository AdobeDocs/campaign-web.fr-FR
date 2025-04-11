---
audience: end-user
title: Utiliser l’activité de workflow Requête incrémentale
description: Découvrir comment utiliser l’activité de workflow Requête incrémentale
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 35%

---

# Requête incrémentale {#incremental-query}

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Requête incrémentale"
>abstract="L’activité **Requête incrémentale** est une activité de **Ciblage** qui vous permet d’interroger la base de données à l’aide du concepteur de requête. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela vous permet de ne cibler que les nouveaux éléments."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Historique des requêtes incrémentales"
>abstract="Historique des requêtes incrémentales"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Données traitées des requêtes incrémentales"
>abstract="Données traitées des requêtes incrémentales"

L&#39;activité **Requête incrémentale** est une activité **Ciblage** qui permet d&#39;interroger la base de données selon un calendrier précis. À chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Vous pouvez ainsi cibler uniquement les nouveaux éléments.

>[!NOTE]
>
>Tandis que la console cliente de Campaign intègre l’activité **[!UICONTROL Requête incrémentale]** avec un planificateur intégré, l’interface d’utilisation de Campaign Web traite cette fonctionnalité séparément. Pour planifier des exécutions de requête incrémentale, ajoutez une activité **[!UICONTROL Planificateur]** dans le workflow avant l’activité **[!UICONTROL Requête incrémentale]**. [Découvrez comment configurer une activité Planificateur](scheduler.md).

L’activité **[!UICONTROL Requête incrémentale]** peut être utilisée à diverses fins :

* Segmenter des individus pour définir la cible d’un message, d’une audience ou d’autres opérations.
* Exporter des données. Par exemple, utilisez l’activité pour exporter régulièrement de nouveaux journaux dans les fichiers . Cela s’avère utile pour les outils de reporting externe ou de Business Intelligence.

La population déjà ciblée par les exécutions précédentes est stockée dans le workflow. Deux workflows lancés à partir du même modèle ne partagent pas le même journal. Toutefois, deux tâches basées sur la même requête incrémentale dans le même workflow utilisent le même journal.

Si le résultat d’une requête incrémentale est égal à 0 lors de l’une de ses exécutions, le workflow se met en pause jusqu’à la prochaine exécution programmée de la requête. Les transitions et les activités qui suivent la requête incrémentale ne sont pas traitées avant la prochaine exécution.

## Configurer l’activité Requête incrémentale {#incremental-query-configuration}

Pour configurer l’activité **Requête incrémentale**, procédez comme suit :

[Description : capture d’écran montrant l’interface de configuration de l’activité de Requête incrémentale dans Adobe Campaign.]\
![](../assets/incremental-query.png)

1. Ajoutez une activité **Requête incrémentale** à votre workflow.

1. Dans la section **[!UICONTROL Audience]**, choisissez la **Dimension de ciblage**, puis cliquez sur **[!UICONTROL Continuer]**.

   La dimension de ciblage définit la population ciblée par l’opération, comme les destinataires, les bénéficiaires d’un contrat, les opérateurs ou les abonnés. Par défaut, la cible est sélectionnée parmi les destinataires. [En savoir plus sur les dimensions de ciblage](../../audience/about-recipients.md#targeting-dimensions)

1. Utilisez le modéliseur de requête pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un e-mail. [Découvrir comment utiliser le concepteur de requête](../../query/query-modeler-overview.md)

1. Dans la section **[!UICONTROL Données traitées]**, sélectionnez le mode d’incrémentation à utiliser :

   * **[!UICONTROL Exclure les résultats de l’exécution précédente]** : à chaque exécution de l’activité, les résultats des exécutions précédentes sont exclus.

     Les enregistrements déjà ciblés lors d&#39;exécutions précédentes peuvent être consignés pendant un nombre maximal de jours à compter du jour où ils ont été ciblés. Utilisez le champ **[!UICONTROL Jours d’historique]** pour définir cette valeur. Si cette valeur est égale à zéro, les personnes destinataires ne sont jamais purgées du journal.

   * **[!UICONTROL Utiliser un champ de date]** : cette option exclut les résultats d’exécutions précédentes en fonction d’un champ de date spécifique. Choisissez le champ de date de votre choix dans la liste des attributs disponibles pour la dimension de ciblage sélectionnée. Lors des exécutions suivantes du workflow, seules les données modifiées ou créées après la date de dernière exécution seront récupérées.

     Après la première exécution du workflow, le champ **[!UICONTROL Date de dernière exécution]** est disponible. Il spécifie la date utilisée pour la prochaine exécution et est automatiquement mis à jour chaque fois que le workflow est exécuté. Vous pouvez remplacer manuellement cette valeur en fonction de vos besoins.

   >[!NOTE]
   >
   >Le mode **[!UICONTROL Utiliser un champ de date]** offre plus de flexibilité en fonction du champ de date sélectionné. Par exemple, si le champ spécifié correspond à une date de modification, le mode de champ de date récupère les données récemment mises à jour. L&#39;autre mode exclut les enregistrements déjà ciblés lors d&#39;une exécution précédente, même s&#39;ils ont été modifiés depuis la dernière exécution du workflow.

## Exemple {#incremental-query-example}

L’exemple suivant illustre la configuration d’un workflow qui filtre les profils dans la base de données Adobe Campaign toutes les semaines. Il cible les personnes abonnées au service Newsletter Yoga et leur envoie un e-mail de bienvenue.

![Capture d’écran d’un exemple de configuration de workflow pour le filtrage des profils abonnés au service Newsletter de yoga.](../assets/incremental-query-example.png)

Le workflow comprend les éléments suivants :

* Une activité **[!UICONTROL Planificateur]**, qui exécute le workflow tous les lundis à 6 heures du matin.
* Une activité **[!UICONTROL Requête incrémentale]** qui cible tous les abonnés actuels lors de la première exécution et uniquement les nouveaux abonnés lors des exécutions suivantes.
* Une activité **[!UICONTROL Diffusion e-mail]**.