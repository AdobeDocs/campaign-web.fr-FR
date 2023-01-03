---
audience: end-user
title: Découvrir l’interface
description: Interface utilisateur web de Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 15ee9ea467f9243834374cfe1a3e411f929c2a77
workflow-type: ht
source-wordcount: '717'
ht-degree: 100%

---

# Découvrir l’interface {#user-interface}

>[!NOTE]
>
>Cette documentation est en cours d’élaboration et est fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Interface"
>abstract="TBC"

La nouvelle interface web de Campaign v8 offre une expérience utilisateur intégrée, intuitive et cohérente.

Les concepts clés lors de la navigation dans l’interface utilisateur sont communs à Adobe Experience Platform. Pour plus d’informations, reportez-vous à la [documentation Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html?lang=fr#adobe-experience-platform-ui-guide).

>[!NOTE]
>
>Cette documentation est fréquemment mise à jour pour prendre en compte les dernières modifications apportées à l’interface utilisateur du produit. Cependant, certaines captures d’écran peuvent légèrement différer de votre interface utilisateur.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Menu de navigation gauche

Parcourez les liens situés à gauche pour accéder aux fonctionnalités web de Campaign v8.

![](assets/home.png)

### Page d’accueil

La page d’accueil web de Campaign v8 contient des liens et des ressources importants pour bien démarrer. La liste **Récents** offre des raccourcis vers les diffusions récemment créées. Cette liste affiche les dates et statuts de création et de modification.

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Accédez aux pages principales d’aide concernant l’interface web de Campaign v8 depuis la section inférieure de la page d’accueil.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorateur

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorateur"
>abstract="TBC"

Le menu **Explorateur** affiche la même hiérarchie de dossiers que celle de la console cliente. Parcourez tous vos composants, dossiers et schémas Campaign v8. Tous les écrans de type Liste sont en lecture seule, à l’exception de la liste de diffusion e-mail.

Les éléments affichés dans l’Explorateur dépendent de vos autorisations utilisateur.

Comme dans n’importe quel écran de liste, vous pouvez configurer des colonnes afin d’afficher toutes les informations que vous souhaitez. Consultez cette [section](#list-screens).
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campagnes"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Diffusions"
>abstract="TBC"

* **Campagnes** - Il s’agit de la liste de vos campagnes. Vous pouvez afficher des informations utiles telles que leurs dates de début, de fin ou de dernière modification, ainsi que leur statut. Vous pouvez filtrer la liste par statut ou date de début/fin. Des modèles de campagne sont également disponibles. Ces listes sont en lecture seule.

* **Diffusions** - Parcourez votre liste de diffusions. Vous pouvez consulter leur état, date de dernière modification ainsi que les indicateurs clés de performance. Vous pouvez filtrer la liste par état, date de contact ou canal. Cliquez sur une diffusion e-mail pour ouvrir son tableau de bord. Les autres éléments sont en lecture seule. Des modèles de diffusion sont également disponibles.

### Gestion des clients

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Destinataires"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Listes d’abonnements"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Les workflows de ciblage"
>abstract="TBC"

* **Destinataires** - Accédez à la base de données des destinataires. Vous pouvez consulter des informations utiles telles que leur adresse e-mail, prénom et nom. Cette liste est en lecture seule.
* **Audiences** - Il s’agit de votre liste d’audiences. Vous pouvez consulter leur type, origine, date de création/dernière modification et libellé. Vous pouvez filtrer la liste par origine. Cette liste est en lecture seule.
* **Listes d’abonnements** - Parcourez vos listes d’abonnements. Vous pouvez consulter leur type, mode et libellé. Cette liste est en lecture seule.
* **Workflows de ciblage** - Accédez à votre liste de workflows de campagne. Vous pouvez afficher leur état, les dates de leur dernier/prochain traitement et leur environnement. Vous pouvez filtrer la liste par état, date de dernier traitement et type de workflow. Des modèles de workflow sont également disponibles. Ces listes sont en lecture seule.

### Gestion des décisions

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offres"
>abstract="TBC"

* **Offres** - Parcourez votre liste d’offres d’interaction. Vous pouvez consulter leur état, les dates de début/fin et leur environnement. Vous pouvez filtrer la liste par état et par date de début/fin. Des modèles d’offre sont également disponibles. Ces listes sont en lecture seule.

## Shell unifié

L’application web de Campaign v8 est intégrée à un shell unifié. Plusieurs boutons sont disponibles sur le côté droit de la barre supérieure.

![](assets/unified-shell.png){width="70%" align="left"}

Ces boutons vous permettent d’effectuer les opérations suivantes :

* partager vos commentaires en tant que client(e) Alpha,
* basculer entre les organisations IMS,
* basculer entre les applications Adobe Experience Cloud,
* accéder aux pages d’aide, contacter le support et partager vos commentaires. Vous pouvez rechercher des articles et des vidéos d’aide dans le champ de recherche.

<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Aide contextuelle et guide d’intégration

Une aide contextuelle est disponible dans l’interface. Lorsque cette option est disponible, cliquez sur l’icône **.Icône** pour afficher des informations d’aide et des liens vers une documentation connexe.

![](assets/context-help.png){width="70%" align="left"}

Un guide d’intégration est également disponible pour vous aider à commencer à utiliser l’application web de Campaign v8. Cliquez sur l’icône dans le coin inférieur droit, sélectionnez l’un des scénarios détaillés disponibles, puis suivez simplement les instructions.

![](assets/onboarding.png){width="70%" align="left"}

## Configurer les écrans de liste {#list-screens}

Tous les écrans de type Liste sont en lecture seule, à l’exception de la liste de diffusion e-mail.

Pour trouver les éléments plus rapidement, vous pouvez utiliser la barre de recherche ou filtrer la liste selon des critères contextuels.

![](assets/filter.png){width="70%" align="left"}

Les listes sont affichées en colonnes. Chaque colonne peut être triée dans un ordre croissant ou décroissant, une à la fois. Vous pouvez également afficher des informations supplémentaires en modifiant la configuration des colonnes. Pour ce faire, cliquez sur l’icône dans le coin supérieur droit de la liste. Vous pouvez ajouter ou supprimer des colonnes et modifier leur ordre d’affichage.

![](assets/columns.png){width="70%" align="left"}

<!--
## Supported browsers {#browsers}

Adobe [!DNL Journey Optimizer] interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->