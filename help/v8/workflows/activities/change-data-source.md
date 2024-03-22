---
audience: end-user
title: Utilisation de l’activité de workflow Modifier la source de données
description: Découvrez comment utiliser l’activité de workflow Modifier la source de données
source-git-commit: 9ec5483a5253d67110baf6a51b47ebe0c27574d5
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 12%

---

# Modifier la source de données {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Modifier la source de données"
>abstract="Utilisez la nouvelle activité de ciblage de workflow Modifier la source de données pour modifier la source de données utilisée par la table de travail de votre workflow. Cette activité offre davantage de flexibilité en vous permettant de gérer les données dans vos différentes bases de données et d’améliorer les performances."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Voir les notes de mise à jour"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Modifier la source de données"
>abstract="La variable **Modification de la source de données** L’activité vous permet de sélectionner une autre source de données pour la table de travail de votre workflow."

La variable **Modification de la source de données** est une activité **ciblage** activité. Cette activité permet de modifier la source de données utilisée par la table de travail de votre workflow. Vous bénéficiez ainsi d’une plus grande flexibilité grâce à la gestion des données dans vos différentes bases de données et à l’amélioration des performances.

Dans les workflows, les données transportées d&#39;une activité à l&#39;autre via les transitions sont stockées dans un emplacement temporaire. **Table de travail**. Par défaut, les tables de travail sont créées dans la même base que la source des données traitées. Par exemple, lors de l&#39;interrogation de la table &quot;Profils&quot;, stockée dans la base de données Cloud, une table de travail est créée sur la même base de données Cloud.

Dans certains cas, les données ne sont pas disponibles dans la base de données actuelle ou ne sont pas suffisamment efficaces pour effectuer des opérations unitaires. Vous devrez peut-être donc forcer le workflow à utiliser une autre base de données pour effectuer ces opérations en ajoutant une **[!UICONTROL Modification de la source de données]** activité.

Des informations détaillées sur l’architecture de Campaign sont disponibles dans la section [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)

<!--

Let's say you want to send to your  VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Configuration de l’activité Changer de source de données {#configure}

Pour configurer l’activité **Changement de dimension**, procédez comme suit :

![](../assets/workflow-change-data-source-add.png)

1. Ajouter un **Modification de la source de données** à votre workflow.

1. Définissez la source de données où déplacer le tableau de travail :

   * **[!UICONTROL Base de données Campaign par défaut (PostgreSQL)]**: utilisez la base de données locale Campaign par défaut.
   * **[!UICONTROL Compte externe FDA]**: utilisez des bases de données Cloud externes connectées à Adobe Campaign par le biais de la fonctionnalité Federated Data Access.

     >[!AVAILABILITY]
     >
     >La configuration de Campaign et la connexion à des systèmes externes sont limitées aux utilisateurs et utilisatrices expérimentés et ne sont disponibles que depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=fr){target="_blank"}

1. Configurez votre workflow pour effectuer les opérations souhaitées à l’aide de la nouvelle source de données.

<!--
## Example {#example}

The workflow belows illustrates the use case detailed earlier, i.e. sending VIP customers offer codes that they can redeem on our online store.

-->
