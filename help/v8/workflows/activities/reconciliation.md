---
audience: end-user
title: Utiliser l’activité de workflow Réconciliation
description: Découvrez comment utiliser l’activité de workflow Réconciliation
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '824'
ht-degree: 100%

---

# Réconciliation {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Activité Réconciliation"
>abstract="L’activité **Réconciliation** est une activité de **Ciblage** qui définit le lien entre les données dans la base de données Adobe Campaign et les données dans une table de travail. L’activité **Réconciliation** peut par exemple être placée après une activité **Charger un fichier** visant à importer des données non standard dans la base de données. Dans ce cas, l’activité **Réconciliation** définit le lien entre les données dans la base de données Adobe Campaign et les données dans la table externe."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Champ de sélection de la réconciliation"
>abstract="Champ de sélection de la réconciliation"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Condition de création de réconciliation"
>abstract="Condition de création de réconciliation"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Complément de génération de réconciliation"
>abstract="Complément de génération de réconciliation"

L’activité **Réconciliation** est une activité de **Ciblage** qui définit le lien entre les données dans la base de données Adobe Campaign et les données dans une table de travail, par exemple les données chargées à partir d’un fichier externe.

L’activité **Réconciliation** peut par exemple être placée après une activité **Charger un fichier** visant à importer des données non standard dans la base de données. Dans ce cas, l’activité **Réconciliation** définit le lien entre les données dans la base de données Adobe Campaign et les données dans la table de travail.

## Bonnes pratiques {#reconciliation-best-practices}

Tandis que l’activité **Enrichissement** définit les données additionnelles à traiter dans votre workflow (par exemple, combiner des données issues de plusieurs jeux ou créer des liens vers une ressource temporaire), l’activité **Réconciliation** lie des données non identifiées à des ressources existantes.

>[!NOTE]
>L’opération de réconciliation nécessite que les données des dimensions liées existent déjà dans la base de données. Par exemple, si vous importez un fichier d’achats indiquant quel produit a été acheté, à quelle heure, par quelle personne de la clientèle, le produit ainsi que la personne doivent déjà exister dans la base de données.

## Configurer l’activité Réconciliation {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Dimension de ciblage"
>abstract="Sélectionnez la nouvelle dimension de ciblage. Une dimension définit la population ciblée : destinataires, personnes abonnées à l’application, opérateurs et opératrices, personnes abonnées, etc. Par défaut, la dimension de ciblage actuelle est sélectionnée."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Règles de réconciliation"
>abstract="Sélectionnez les règles de réconciliation à utiliser pour la déduplication. Pour utiliser des attributs, sélectionnez l’option **Attributs simples** et choisissez les champs source et destination. Pour créer votre propre condition de réconciliation à l’aide du concepteur de requête, sélectionnez l’option **Conditions avancées de réconciliation**."
>additional-url="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/query-database/query-modeler-overview" text="Utiliser le concepteur de requête"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Sélectionner la dimension de ciblage"
>abstract="Sélectionnez la dimension de ciblage de vos données entrantes avec lesquelles vous souhaitez effectuer la réconciliation."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=fr#targeting-dimensions" text="Dimensions de ciblage"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Conserver les données non réconciliées"
>abstract="Par défaut, les données non réconciliées sont conservées dans la transition sortante et disponibles dans la table de travail pour une utilisation ultérieure. Pour supprimer les données non réconciliées, désactivez l’option **Conserver les données non réconciliées**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Attribut de réconciliation"
>abstract="Sélectionnez l’attribut à utiliser pour réconcilier les données, puis cliquez sur Confirmer."

Pour configurer l’activité **Réconciliation**, procédez comme suit :

1. Ajoutez une activité **Réconciliation** dans votre workflow. Cette activité doit être ajoutée à la suite d’une transition contenant une population dont la dimension de ciblage ne provient pas directement d’Adobe Campaign.

1. Sélectionnez la nouvelle dimension de ciblage. Une dimension définit la population ciblée : destinataires, personnes abonnées à l’application, opérateurs et opératrices, personnes abonnées, etc. [Découvrez les dimensions de ciblage](../../audience/about-recipients.md#targeting-dimensions).

1. Sélectionnez le ou les champs à utiliser pour la réconciliation. Vous pouvez utiliser un ou plusieurs critères de réconciliation.

   1. Pour utiliser des attributs afin de réconcilier des données, sélectionnez l’option **Attributs simples**. Le champ **Source** répertorie les champs disponibles dans la transition d’entrée qui doivent être réconciliés. Le champ **Destination** correspond aux champs de la dimension de ciblage sélectionnée. Les données sont réconciliées lorsque la source et la destination sont égales. Par exemple, sélectionnez les champs **E-mail** pour dédupliquer des profils en fonction de leur adresse e-mail.

      Pour ajouter un autre critère de réconciliation, cliquez sur le bouton **Ajouter une règle**. Si plusieurs conditions de jointure sont indiquées, elles doivent toutes être vérifiées pour que le lien entre les données puisse se faire.

      ![Exemple de critères de réconciliation](../assets/workflow-reconciliation-criteria.png)

   1. Pour utiliser d’autres attributs afin de réconcilier des données, sélectionnez l’option **Conditions avancées de réconciliation**. Vous pouvez ensuite créer votre propre condition de réconciliation à l’aide du concepteur de requête. [Découvrez comment utiliser le concepteur de requête](../../query/query-modeler-overview.md).

1. Filtrez les données à réconcilier à l’aide du bouton **Créer un filtre**. Vous pouvez ainsi créer une condition personnalisée à l’aide du concepteur de requête. [Découvrez comment utiliser le concepteur de requête](../../query/query-modeler-overview.md).

Par défaut, les données non réconciliées sont conservées dans la transition sortante et disponibles dans la table de travail pour une utilisation ultérieure. Pour supprimer les données non réconciliées, désactivez l’option **Conserver les données non réconciliées**.

## Exemple {#reconciliation-example}

L&#39;exemple suivant illustre un workflow permettant de créer une audience de profils directement à partir d&#39;un fichier importé contenant des nouveaux clients. Il comprend les activités suivantes :

Le workflow se présente comme suit :

![Exemple de workflow](../assets/workflow-reconciliation-sample-1.0.png)

Il est créé avec les activités suivantes :

* Une activité [Charger le fichier](load-file.md) charge un fichier contenant des données de profils extraites d’un outil externe.

  Par exemple :

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* Une activité **Réconciliation** identifie les données entrantes sous forme de profils, en utilisant les champs **E-mail** et **Date de naissance** comme critères de réconciliation.

  ![Exemple d’activité de réconciliation](../assets/workflow-reconciliation-sample-1.1.png)

* Une activité [Sauvegarder l’audience](save-audience.md) crée une audience à partir de ces mises à jour. Vous pouvez également remplacer l’activité **Sauvegarder l’audience** par une activité **Fin** si aucune audience spécifique ne doit être créée ou mise à jour. Dans tous les cas, les profils de destinataires sont mis à jour lorsque vous exécutez le workflow.

## Compatibilité {#reconciliation-compat}

L’activité **Réconciliation** n’existe pas dans la console cliente. Toutes les activités **Enrichissement** créées dans la console cliente avec les options de réconciliation activées s’affichent sous la forme d’activités **Réconciliation** dans l’interface d’utilisation web de Campaign.