---
audience: end-user
title: Utiliser l’activité de workflow Requête incrémentale
description: Découvrir comment utiliser l’activité de workflow Requête incrémentale
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: fc872fd3975cd15a10845185c87152e2a473df8f
workflow-type: ht
source-wordcount: '794'
ht-degree: 100%

---

# Requête incrémentale {#incremental-query}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Activité Requête incrémentale"
>abstract="Utilisez la nouvelle activité Requête incrémentale pour interroger la base de données selon un calendrier précis. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela permet de ne cibler que les éléments nouveaux."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Requête incrémentale"
>abstract="L’activité **Requête incrémentale** est une activité de **Ciblage** qui vous permet d’interroger la base de données à l’aide du concepteur de requête. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela permet de ne cibler que les éléments nouveaux."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Historique des requêtes incrémentales"
>abstract="Historique des requêtes incrémentales"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Données traitées des requêtes incrémentales"
>abstract="Données traitées des requêtes incrémentales"

L’activité **Requête incrémentale** est une activité de **Ciblage** qui vous permet d’interroger la base de données à des moments planifiés. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela permet de ne cibler que les éléments nouveaux.

>[!NOTE]
>
>Tandis que la console cliente de Campaign intègre l’activité **[!UICONTROL Requête incrémentale]** avec un planificateur intégré, l’interface d’utilisation de Campaign Web traite cette fonctionnalité séparément. Pour planifier des exécutions de requêtes incrémentales, vous devez ajouter une activité **[!UICONTROL Planificateur]** dans le workflow avant l’activité **[!UICONTROL Requête incrémentale]**. [Découvrez comment configurer une activité Planificateur](scheduler.md).

L&#39;activité **[!UICONTROL Requête incrémentale]** peut être utilisée dans plusieurs cas d&#39;utilisation type :

* segmentation d’individus afin de définir la cible d’un message, une audience, etc.
* Exporter des données. Par exemple, vous pouvez utiliser l’activité pour exporter régulièrement les nouveaux journaux dans des fichiers. Cela peut s’avérer utile si vous souhaitez utiliser les données de vos journaux dans des rapports externes ou des outils BI.

La population déjà ciblée par les exécutions précédentes est stockée dans le workflow. Cela signifie que deux workflows démarrés à partir du même modèle ne partagent pas le même journal. Toutefois, deux tâches basées sur la même requête incrémentale dans le même workflow utilisent le même journal.

Si le résultat de la requête incrémentale est égal à 0 lors de l’une de ses exécutions, le workflow est mis en pause jusqu’à la prochaine exécution programmée de la requête. Les transitions et activités qui suivent la requête incrémentale ne sont alors pas traitée avant l’exécution suivante.

## Configurer l’activité Requête incrémentale {#incremental-query-configuration}

Pour configurer l’activité **Requête incrémentale**, procédez comme suit :

![](../assets/incremental-query.png)

1. Ajoutez une activité **Requête incrémentale** à votre workflow.

1. Dans la section **[!UICONTROL Audience]**, choisissez la **Dimension de ciblage** puis cliquez sur **[!UICONTROL Continuer]**.

   La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, la cible est sélectionnée parmi les destinataires. [En savoir plus sur les dimensions de ciblage](../../audience/about-recipients.md#targeting-dimensions)

1. Utilisez le concepteur de requêtes pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un nouvel e-mail. [Découvrez comment utiliser le concepteur de requêtes](../../query/query-modeler-overview.md).

1. Dans la section **[!UICONTROL Données traitées]**, sélectionnez le mode d’incrémentation à utiliser :

   * **[!UICONTROL Exclure les résultats de l’exécution précédente]** : à chaque exécution de l’activité, les résultats des exécutions précédentes sont exclus.

     Les enregistrements déjà ciblés dans les exécutions précédentes peuvent être consignés dans un journal selon un nombre maximum de jours à partir du jour où ils ont été ciblés. Pour ce faire, utilisez le champ **[!UICONTROL Historique en jours]**. Si cette valeur est égale à zéro, les personnes destinataires ne sont jamais purgées du journal.

   * **[!UICONTROL Utiliser un champ de date]** : cette option permet d’exclure les résultats des exécutions précédentes en fonction d’un champ de date spécifique. Pour cela, choisissez le champ de date souhaité dans la liste des attributs disponibles pour la dimension de ciblage sélectionnée. Lors des prochaines exécutions du workflow, seules les données qui auront été modifiées ou créées après la date de la dernière exécution seront récupérées.

     Après la première exécution du workflow, le champ **[!UICONTROL Date de dernière exécution]** est disponible. Celui-ci spécifie la date qui sera utilisée pour la prochaine exécution et est automatiquement mis à jour chaque fois que le workflow est exécuté. Vous avez toujours la possibilité de remplacer cette valeur en en saisissant une autre qui répond à vos besoins.

   >[!NOTE]
   >
   >Le mode **[!UICONTROL Utiliser un champ date]** offre davantage de flexibilité selon le champ date sélectionné. Par exemple, si le champ spécifié correspond à une date de modification, le mode du champ de date vous permet de récupérer les données qui ont été récemment mises à jour. L’autre mode, en revanche, exclut simplement les enregistrements qui ont déjà été ciblés dans une exécution précédente, même s’ils ont été modifiés depuis la dernière exécution du workflow.

## Exemple {#incremental-query-example}

L’exemple suivant présente la configuration d’un workflow qui filtre chaque semaine les profils de la base de données d’Adobe Campaign qui sont abonnés au service Yoga Newsletter, afin de leur envoyer un e-mail de bienvenue.

![](../assets/incremental-query-example.png)

Le workflow est constitué des éléments suivants :

* Un **[!UICONTROL Planificateur]**, afin que le workflow s’exécute chaque lundi à 6h.
* Une **[!UICONTROL Requête incrémentale]**, permettant de cibler tous les abonnés actuels lors de la première exécution, puis uniquement les nouveaux abonnés de la semaine lors des exécutions suivantes.
* Une activité **[!UICONTROL Diffusion e-mail]**.
