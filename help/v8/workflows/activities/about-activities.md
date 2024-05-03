---
audience: end-user
title: Utiliser les activités de workflows
description: Découvrez les activités de workflows.
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 5947d7f6b2fd39ede6322273e7497744f9aff953
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 38%

---


# À propos des activités de workflows {#workflow-activities}

Les activités de workflows sont regroupées en trois catégories. Selon le contexte, les activités disponibles peuvent différer.

Toutes les activités sont présentées dans les sections ci-dessous :

* [Activités de ciblage et de gestion des données](#targeting)
* [Activités de canal](#channel)
* [Activités de contrôle de flux](#flow-control)

![](../assets/workflow-activities.png)

## Activités de ciblage {#targeting}

Ces activités sont spécifiques au ciblage. Elles permettent de construire une ou plusieurs cibles en définissant une audience, puis en partageant ou en combinant ces audiences à l’aide des opérations d’intersection, d’union ou d’exclusion.

* [Créer une audience](build-audience.md): définissez votre population cible. Vous pouvez sélectionner une audience existante ou utiliser le concepteur de requête pour définir votre propre requête.
* [Modification de la source de données](change-data-source.md): modifiez la source de données de la table de travail de votre workflow.&quot;
* [Changement de dimension](change-dimension.md): modifiez la dimension de ciblage à mesure que vous créez votre workflow.
* [Combiner](combine.md): effectuez une segmentation sur votre population entrante. Vous pouvez utiliser une union, une intersection ou une exclusion.
* [Déduplication](deduplication.md): supprimer les doublons dans le ou les résultats des activités entrantes.
* [Enrichissement](enrichment.md): définissez des données additionnelles à traiter dans votre workflow. Avec cette activité, vous pouvez utiliser la transition entrante et configurer l’activité pour ajouter des données supplémentaires à la transition sortante.
* [Requête incrémentale](incremental-query.md): interroger la base de données selon un calendrier précis. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela permet de ne cibler que les éléments nouveaux.
* [Réconciliation](reconciliation.md): définissez le lien entre les données de la base Adobe Campaign et les données d&#39;une table de travail, par exemple les données chargées à partir d&#39;un fichier externe.
* [Sauvegarde d’audience](save-audience.md): mettre à jour une audience existante ou créer une nouvelle audience à partir de la population calculée en amont dans un workflow.
* [Partage](split.md): segmentez la population entrante en plusieurs sous-ensembles.

## Activités de gestion des données {#data}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Activités d’extraction et de chargement de fichier"
>abstract="De nouvelles activités de Data Management sont disponibles dans les workflows. Utilisez l&#39;activité Extraction de fichier pour exporter des données d&#39;Adobe Campaign vers un autre système sous la forme d&#39;un fichier externe. Utilisez l&#39;activité Chargement de fichier pour utiliser les profils et les données stockés dans un fichier externe."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

Ces activités sont spécifiques à la manipulation et à l&#39;enrichissement des données sur la population.

* [Extraction de fichier](extract-file.md): exportez les données d’Adobe Campaign vers un autre système sous la forme d’un fichier externe.
* [Chargement de fichier](load-file.md): utilisation de profils et de données stockés dans un fichier externe.
* [Transfert de fichier](transfer-file.md): recevez ou envoyez des fichiers, testez la présence de fichiers ou listez les fichiers sur un serveur. Le protocole utilisé peut être soit un protocole serveur à serveur, soit un protocole HTTP.
* [Code JavaScript](javascript-code.md): exécutez un fragment de code JavaScript dans le contexte d’un workflow.
* [Services d’inscriptions](subscription-services.md): abonnez ou désabonnez plusieurs profils à/d’un service en une seule action.
* [Mise à jour de données](update-data.md): effectuez des mises à jour en masse sur les champs de la base de données. Plusieurs options permettent de personnaliser la mise à jour des données.

## Activités de canal {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux. Vous pouvez combiner des activités de canal dans la zone de travail afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement du client ou de la cliente. Les activités **Canal** suivantes sont disponibles : e-mail, SMS, notifications push Android et iOS. [Découvrez comment configurer une diffusion dans le contexte d’un workflow](channels.md).

## Activités de contrôle de flux {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Activités de workflow avancées"
>abstract="Vous pouvez maintenant configurer les activités Test, Code JavaScript et Signal externe dans un workflow. Utilisez l&#39;activité Test pour activer les transitions de workflow en fonction des conditions. Ajoutez une activité Code JavaScript pour exécuter un fragment de code JS dans le contexte de votre workflow. Configurez une activité Signal externe pour déclencher l’exécution de votre workflow à partir d’une API ou d’un autre workflow."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"



>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Activité Fin"
>abstract="L’activité **Fin** vous permet de marquer graphiquement la fin d’un workflow. Cette activité n’a aucun impact fonctionnel et est donc facultative."

Les activités ci-après sont spécifiques à l’organisation et à l’exécution du workflow. Leur principale tâche est de coordonner les autres activités :

* [Et rejoindre](and-join.md): synchroniser plusieurs branches d’exécution d’un workflow ;
* **Fin**: marque la fin d’un workflow sous forme graphique. Cette activité n’a aucun impact fonctionnel et est donc facultative.
* [Signal externe](external-signal.md): déclenchez l’exécution d’un workflow à partir d’un autre workflow ou d’un appel API.
* [Branchement](fork.md): créez des transitions sortantes afin de lancer simultanément plusieurs activités.
* [Planificateur](scheduler.md): planifiez le démarrage du workflow.
* [Test](test.md): activez les transitions en fonction de conditions spécifiées.
* [Attente](wait.md): suspendre momentanément l’exécution d’une partie d’un workflow.
