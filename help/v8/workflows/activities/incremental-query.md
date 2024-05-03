---
audience: end-user
title: Utilisation de l’activité de workflow de requête incrémentale
description: Découvrez comment utiliser l’activité de workflow de requête incrémentale
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 31%

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
>abstract="La variable **Requête incrémentale** est une activité **Ciblage** activité permettant d&#39;interroger la base de données à l&#39;aide du modeleur de requête. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela permet de ne cibler que les éléments nouveaux."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Historique des requêtes incrémentales"
>abstract="Historique des requêtes incrémentales"

La variable **Requête incrémentale** est une activité **Ciblage** activité permettant d&#39;interroger la base de données selon un calendrier précis. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela permet de ne cibler que les éléments nouveaux.

>[!NOTE]
>
>Pendant que la console cliente de Campaign intègre l’événement **[!UICONTROL Requête incrémentale]** avec un planificateur intégré, l’interface utilisateur web de Campaign traite cette fonctionnalité séparément. Pour planifier des exécutions de requête incrémentielles, vous devez ajouter une **[!UICONTROL Planificateur]** dans le workflow avant la **[!UICONTROL Requête incrémentale]** activité. [Découvrez comment configurer une activité Planificateur](scheduler.md)

L&#39;activité **[!UICONTROL Requête incrémentale]** peut être utilisée dans plusieurs cas d&#39;utilisation type :

* segmentation d’individus afin de définir la cible d’un message, une audience, etc.
* Exporter des données. Par exemple, vous pouvez utiliser l’activité pour exporter régulièrement de nouveaux logs dans des fichiers. Cela peut s’avérer utile si vous souhaitez utiliser vos données de journal dans des outils de reporting ou de BI externes.

La population déjà ciblée par les exécutions précédentes est stockée dans le workflow. Cela signifie que deux workflows démarrés à partir du même modèle ne partagent pas le même journal. Toutefois, deux tâches basées sur la même requête incrémentale dans le même workflow utilisent le même journal.

Si le résultat d&#39;une requête incrémentale est égal à 0 lors de l&#39;une de ses exécutions, le workflow est suspendu jusqu&#39;à la prochaine exécution programmée de la requête. Les transitions et activités qui suivent la requête incrémentale ne sont donc pas traitées avant l&#39;exécution suivante.

## Configuration de l&#39;activité Requête incrémentale {#incremental-query-configuration}

Pour configurer la variable **Requête incrémentale** activité :

![](../assets/incremental-query.png)

1. Ajoutez un **Requête incrémentale** dans votre workflow.

1. Dans le **[!UICONTROL Audience]** , choisissez la **Dimension de ciblage** puis cliquez sur **[!UICONTROL Continuer]**.

   La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, la cible est sélectionnée parmi les destinataires. [En savoir plus sur les dimensions de ciblage](../../audience/about-recipients.md#targeting-dimensions)

1. Utilisez le concepteur de requêtes pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un nouvel e-mail. [Découvrez comment utiliser le concepteur de requêtes](../../query/query-modeler-overview.md).

1. Dans le **[!UICONTROL Données traitées]** , sélectionnez le mode incrémentiel à utiliser :

   * **[!UICONTROL Exclure les résultats de l’exécution précédente]**: à chaque exécution de l’activité, les résultats des exécutions précédentes sont exclus.

     Les enregistrements déjà ciblés dans les exécutions précédentes peuvent être consignés un nombre maximum de jours à partir du jour où ils ont été ciblés. Pour ce faire, utilisez la méthode **[!UICONTROL Jours d&#39;historique]** champ . Si cette valeur est égale à zéro, les destinataires ne sont jamais purgés du journal.

   * **[!UICONTROL Utiliser un champ de date]**: cette option permet d’exclure les résultats des exécutions précédentes en fonction d’un champ de date spécifique. Pour cela, choisissez le champ de date de votre choix dans la liste des attributs disponibles pour la dimension de ciblage sélectionnée. Lors des prochaines exécutions du workflow, seules les données modifiées ou créées après la date de la dernière exécution seront récupérées.

     Après la première exécution du workflow, la variable **[!UICONTROL Date de dernière exécution]** devient disponible. Il spécifie la date qui sera utilisée pour la prochaine exécution et est automatiquement mis à jour chaque fois que le workflow est exécuté. Vous avez toujours la possibilité de remplacer cette valeur en en saisissant une autre qui répond à vos besoins.

   >[!NOTE]
   >
   >Le mode **[!UICONTROL Utiliser un champ date]** offre davantage de flexibilité selon le champ date sélectionné. Par exemple, si le champ spécifié correspond à une date de modification, le mode du champ date permet de récupérer les données récemment mises à jour, tandis que l&#39;autre mode exclut simplement les enregistrements déjà ciblés dans une exécution précédente, même s&#39;ils ont été modifiés depuis la dernière exécution du workflow.

## Exemple {#incremental-query-example}

L&#39;exemple suivant montre le paramétrage d&#39;un workflow qui filtre chaque semaine les profils de la base Adobe Campaign abonnés au service Newsletter Yoga, afin de leur envoyer un email de bienvenue.

![](../assets/incremental-query-example.png)

Le workflow est défini comme suit :

* Un **[!UICONTROL Planificateur]**, afin que le workflow s’exécute chaque lundi à 6h.
* Une **[!UICONTROL Requête incrémentale]**, permettant de cibler tous les abonnés actuels lors de la première exécution, puis uniquement les nouveaux abonnés de la semaine lors des exécutions suivantes.
* Un **[!UICONTROL Diffusion Email]** activité.
