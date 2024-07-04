---
audience: end-user
title: Matrice des fonctionnalités de l’interface utilisateur web de Campaign/de la console cliente
description: Liste des fonctionnalités prises en charge dans l’interface utilisateur web de Campaign
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '2141'
ht-degree: 100%

---

# Campaign Web et console cliente Campaign {#capabilities-matrix}

Les fonctionnalités clés de Campaign sont disponibles dans l’interface utilisateur web de Campaign. Cette interface a été conçue en premier lieu pour que les personnes spécialisées dans le marketing puissent planifier, lancer et mesurer leurs campagnes marketing. Les différentes fonctionnalités sont répertoriés [sur cette page](../rn/whats-new.md).

La personnalisation de la plateforme Campaign en fonction des besoins de l’entreprise et des données, ainsi que la connexion à d’autres systèmes, sont gérées dans la console cliente Campaign. Par conséquent, vous pouvez accéder à certains paramètres et fonctionnalités, les créer ou les gérer uniquement depuis la console cliente Campaign. Certains paramètres et fonctionnalités seront disponibles dans une mise à jour ultérieure de l’interface utilisateur web de Campaign.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Gestion de campagne {#campaign-mgt-capabilities}

Avec l’interface utilisateur web de Campaign, vous pouvez créer des campagnes cross-canal, comme décrit [dans cette section](../campaigns/gs-campaigns.md). Les fonctionnalités suivantes ne sont disponibles que dans la console cliente Campaign. Elles ne sont pas accessibles dans l’interface utilisateur web de Campaign, bien que certaines s’affichent dans le menu [Explorateur](user-interface.md#user-interface-explorer).

Utilisez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et découvrir comment utiliser ces fonctionnalités.

* **Calendrier marketing**. Le calendrier des campagnes affiche l’ensemble des programmes, plans, campagnes et diffusions dans un journal global. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=fr#campaign-calendar){target="_blank"}
* **Programmes et plans**. Chaque campagne appartient à un programme qui appartient à son tour à un plan. Dans l’interface utilisateur web de Campaign, toutes les campagnes sont associées à un plan et à un programme intégrés par défaut. Vous pouvez uniquement créer et gérer des plans et des programmes dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=fr#work-with-plan-and-program){target="_blank"}
* **Gestion des fournisseurs, des budgets et des coûts**. Vous pouvez configurer les prestataires de services impliqués dans les traitements réalisés dans vos opérations, y compris les structures de coûts, et gérer vos budgets au sein de chaque programme et campagne. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=fr){target="_blank"}
* **Marketing distribué** (marketing central/local) Adobe Campaign propose une application Marketing distribué pour la mise en œuvre de campagnes de coopération entre entités centrales (sièges sociaux, services marketing, etc.) et les entités locales (points de vente, agences régionales, etc.). Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=fr){target="_blank"}
* **Gestion des ressources marketing** (MRM), objectifs, simulations et contrôle des coûts Adobe Campaign propose une application MRM (gestion des ressources marketing) qui permet de piloter les actions marketing sur un mode collaboratif, en assurant la gestion complète et le tracking en temps réel des tâches, ressources marketing et budgets impliqués. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=fr){target="_blank"}
* **Gestion des tâches**. Dans le cadre de l’application MRM, les tâches de Campaign peuvent être créées, affectées, suivies et surveillées à partir du tableau de bord de la campagne. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=fr){target="_blank"}

## Canaux de communication {#channels-capabilities}

Avec l’interface utilisateur web de Campaign, vous pouvez créer, concevoir et envoyer des **e-mails**, des **SMS**, des **notifications push** et du **courrier** puis mesurer leur impact à l’aide de divers rapports dédiés, comme indiqué [dans cette section](../msg/gs-messages.md). Toutefois, les canaux suivants ne sont actuellement **pas** disponibles : in-app, LINE, centre d’appels/canal personnalisé, marketing social avec X (Twitter).

Utilisez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur ces canaux.

* **Messagerie LINE**. LINE est une application gratuite de messagerie instantanée, d’appels vocaux et vidéo, disponible sur tous les appareils mobiles et sur PC. Adobe Campaign vous permet d’envoyer des messages LINE uniquement depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=fr){target="_blank"}
* **Centre d’appel et canaux personnalisés**. Le centre d’appel et d’autres canaux personnalisés peuvent être implémentés dans votre environnement Campaign. Ces canaux ne peuvent être disponibles que dans la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=fr#other-channels){target="_blank"}
* **Marketing social** avec X (Twitter). Vous interagissez avec vos clientes et clients via X (Twitter) en publiant des messages et en envoyant des messages directs. Cette fonctionnalité, fournie avec le module complémentaire de marketing social, n’est disponible que depuis la console cliente : [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=fr){target="_blank"}.

## Pages de destination et applications web {#Webapps-capabilities}

Adobe Campaign vous permet de créer, concevoir et partager des pages de destination. L’expérience des pages de destination a été entièrement repensée dans la nouvelle interface. Découvrez comment créer, concevoir et publier une page de destination dans l’interface utilisateur web de Campaign [dans cette section](../landing-pages/get-started-lp.md).

Par conséquent, dans la console cliente Campaign, vous ne pouvez pas modifier, mettre à jour ni changer une page de destination créée dans l’interface web, et inversement. Les types d’applications web suivants ne sont pas disponibles dans l’interface utilisateur web de Campaign. Ils sont toutefois visibles dans la liste des pages de destination. Utilisez les liens fournis pour parcourir la documentation de Campaign Classic v7 et en savoir plus sur ces applications web :

* **Applications web**. Adobe Campaign vous permet de créer et de publier des applications web dynamiques et interactives, composées de données issues de la base de données et dont le contenu est adapté en fonction des droits de la personne connectée. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=fr){target="_blank"}
* **Formulaires web**. Les pages web et de destination conçues dans la console cliente sont visibles dans l’interface utilisateur web de Campaign, mais ne peuvent être ni éditées ni modifiées. Certaines options peuvent différer entre le concepteur de page web de la console cliente et le concepteur de page de destination fourni avec l’interface utilisateur web de Campaign. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=fr){target="_blank"}
* **Questionnaires en ligne**. Vous pouvez créer des questionnaires en ligne et collecter les réponses à partir de la console cliente uniquement. Cette fonctionnalité n’est pas disponible dans l’interface utilisateur web de Campaign.  [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=fr){target="_blank"}


## Profils, profils de test et audiences {#profiles-audiences-capabilities}

Vous pouvez créer, gérer et mettre à jour des profils et des profils de test dans la console cliente Campaign et dans l’interface utilisateur web de Campaign. Toutes les modifications apportées dans une interface utilisateur sont visibles dans l’autre. Cependant, certains paramètres spécifiques à la personne destinataire et paramètres avancés peuvent être manquants dans la nouvelle interface utilisateur web de Campaign.

Notez que le terme « personne destinataire » a été remplacé par « profil » dans la nouvelle interface utilisateur web et que les « adresses de contrôle » sont désormais des « profils de test ».

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Toutes les audiences créées dans la console cliente Campaign ou dans Adobe Experience Platform sont disponibles dans l’interface utilisateur web de Campaign.

Les traitements d’import/export ponctuels, tels que décrits dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=fr#import-jobs){target="_blank"} ne sont pas disponibles dans l’interface utilisateur web de Campaign. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## Messages transactionnels {#mc-capabilities}

Les fonctionnalités de messages transactionnels fournies avec le package de produit Message Center ne sont actuellement pas disponibles dans la nouvelle interface utilisateur web de Campaign.

Parcourez la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html?lang=fr){target="_blank"} et apprenez-en davantage sur les fonctionnalités de messages en temps réel, telles que :

* Création et exécution de messages en temps réel par e-mail, SMS et notification push
* Enrichissement et personnalisation des messages
* Reporting et surveillance relatifs aux messages transactionnels

## Conception de contenu {#content-capabilities}

Le nouveau Concepteur d’e-mail fourni avec l’interface utilisateur web d’Adobe Campaign vous permet de créer facilement des e-mails attrayants et personnalisés au moyen d’une interface intuitive par glisser-déposer. Un monde de possibilités s’offre à vous : commencez à partir de zéro, importez un contenu précédent ou tirez parti de modèles existants. Vous pouvez concevoir et affiner le contenu de chaque e-mail. [En savoir plus](../email/edit-content.md)

Grâce à cette nouvelle interface utilisateur, vous pouvez gérer la synchronisation des modèles d’e-mail à partir d’Adobe Experience Manager et effectuer une intégration à Adobe Experience Manager as a Cloud Service.

Notez que les fonctionnalités suivantes ne sont pas disponibles pour l’instant dans l’interface utilisateur web de Campaign. Utilisez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur ces fonctionnalités.

* **Création de blocs de personnalisation personnalisés**. Outre les blocs de personnalisation par défaut, vous pouvez créer des blocs personnalisés à partir de la console cliente. Cette fonctionnalité n’est pas disponible dans l’interface utilisateur web de Campaign. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=fr#create-custom-personalization-blocks){target="_blank"}
* **Contenu des formulaires personnalisés**. Le module de gestion de contenu permet de créer et de gérer des formulaires destinés à assister les utilisateurs et utilisatrices lors de la création de contenu dans Campaign. Cette fonctionnalité est uniquement disponible avec la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=fr){target="_blank"}
* **AMP pour les e-mails**. Le nouveau format AMP pour les e-mails permet d’inclure des composants AMP dans vos messages et améliorer l’expérience par e-mail avec un contenu riche et exploitable. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=fr){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Typologies et règles de typologie {#rules-capabilities}

Les typologies sont des ensembles de règles de typologie qui sont exécutées pendant la phase de préparation afin d’appliquer facilement plusieurs règles de filtrage en même temps à une diffusion. Elles permettent aux personnes spécialisées dans le marketing de normaliser les pratiques commerciales pour toutes les diffusions, en contrôlant, filtrant et gérant la priorité de l’envoi des diffusions.

Les règles de typologie peuvent être sélectionnées pour une diffusion ou un modèle de diffusion dans l’interface utilisateur web de Campaign, comme indiqué [dans cette section](../advanced-settings/delivery-settings.md#typology). Toutefois, la création, la gestion et la personnalisation des règles et des règles de typologie ne sont disponibles que dans la console cliente Campaign.

Sélectionnez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur les règles de typologie :

* Création de règles de contrôle. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=fr){target="_blank"}
* Création de règles de fatigue/pression. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=fr){target="_blank"}
* Création de règles de filtrage. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=fr){target="_blank"}
* Gestion des règles de typologie. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=fr){target="_blank"}
* Simulation de campagne. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=fr){target="_blank"}
* Codage JavaScript pour la création de règles de typologie. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=fr#use-cases-on-pressure-rules){target="_blank"}

## Workflows {#wf-capabilities}

La nouvelle interface utilisateur web de Campaign offre une interface de zone de travail de workflow repensée pour concevoir et gérer vos processus. Les activités des workflows clés sont déjà disponibles dans leur nouvelle conception et certaines le seront dans une prochaine mise à jour. En savoir plus sur les fonctionnalités des workflows, y compris les mécanismes de sécurisation et les limitations [dans cette section](../get-started/guardrails.md).

Notez que les fonctionnalités suivantes ne sont disponibles que dans la console cliente Campaign :

* Script dans les workflows
* Activités ETL : export, édition de schéma, chargement de données, extraction de données, code SQL

En savoir plus sur les activités de workflow disponibles dans la documentation des workflows Adobe Campaign v8 (console) [ici](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=fr){target="_blank"}.

## Gestion des offres {#offer-capabilities}

Vous pouvez envoyer des offres dans vos diffusions créées dans l’interface utilisateur web d’Adobe Campaign. Ces offres doivent avoir été créées dans la console cliente à l’aide du module **[!UICONTROL Interaction]**. La conception des offres, les règles d’éligibilité et la gestion des offres ne sont disponibles que dans la console cliente Campaign. [En savoir plus](../msg/offers.md)

Découvrez comment gérer un catalogue d’offres dans la documentation de [Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=fr){target="_blank"}.

## Intégrations avec les solutions Adobe Experience Cloud {#exc-capabilities}

Cette nouvelle interface utilisateur moderne de Campaign simplifie la conception et la diffusion des campagnes marketing et offre une expérience cohérente avec d’autres solutions Adobe, notamment Adobe Experience Platform et Adobe Experience Manager.

Les fonctionnalités suivantes sont accessibles dans la console cliente Adobe Campaign, mais pas encore disponibles dans l’interface utilisateur web de Campaign. Sélectionnez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur ces intégrations :

* Utilisation des données Adobe Analytics et partage des KPI. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=fr){target="_blank"}
* Partage d’audiences avec Adobe Experience Cloud (Adobe Audience Manager). [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=fr){target="_blank"}
* Intégration avec Adobe Target. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=fr){target="_blank"}
* Intégration avec les Triggers Adobe Experience Cloud. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=fr){target="_blank"}

## Rapports {#reporting-capabilities}

La nouvelle interface utilisateur web de Campaign est fournie avec un ensemble de nouveaux rapports et KPI, pour tous les canaux : rapports de diffusion, rapports de campagne et rapports globaux. En savoir plus dans [cette section](../reporting/gs-reports.md)

Certaines fonctionnalités ne sont disponibles que depuis la console cliente. Suivez les liens fournis pour parcourir la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=fr){target="_blank"} et en savoir plus.

* Rapport de délivrabilité intégré et rendu des e-mails. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=fr){target="_blank"}
* Personnalisations des rapports. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=fr){target="_blank"}
* Analyse descriptive. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=fr){target="_blank"}
* Rapports d’analyse des campagnes / Cube. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=fr){target="_blank"}
* Partage des rapports selon un planning au format PDF et CSV ou lien. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=fr){target="_blank"}

## Modélisation des données et ingestion des données {#data-capabilities}

L’interface utilisateur web de Campaign ne présente pas les fonctionnalités suivantes. Elles ne sont disponibles que dans la console cliente :

### Comptes externes {#external}

Adobe Campaign est fourni avec un ensemble de comptes externes prédéfinis pour la connexion aux systèmes externes. En tant qu’administrateur ou administratrice système Campaign, vous ne pouvez créer et gérer des comptes externes qu’à partir de la console cliente.[En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html?lang=fr){target="_blank"}

### Création et extension de schéma {#schema}

La création, la modification et l’extension de schéma sont limitées aux utilisateurs et utilisatrices expérimentés. Ces fonctionnalités ne sont disponibles que depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=fr){target="_blank"}

### Fonctionnalités de gestion des données des workflows {#data}

Data Management combine un ensemble d’activités pour résoudre des problèmes de ciblage complexes en offrant des outils plus efficaces et plus flexibles tels que Chargement de données, Extraction (fichier), Mise à jour des données, Modifier le schéma ou Importer/exporter des workflows techniques. [Découvrir les fonctionnalités Data Management des workflows dans la console cliente](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=fr#data-management){target="_blank"}

>[!NOTE]
>
>Bien que certaines de ces activités ne soient disponibles que dans la console cliente, d’autres sont disponibles dans l’interface utilisateur web de Campaign, telles que les activités **Enrichissement**, **Charger un fichier**, **Changer la source des données** ou **Changement de dimension**. [En savoir plus sur les activités de ciblage et de gestion des données dans l’interface d’utilisation de Campaign Web](../workflows/activities/about-activities.md#targeting)

### Configuration de Federated Data Access {#fda}

La configuration de Campaign et la connexion à des systèmes externes sont limitées aux utilisateurs et utilisatrices expérimentés et ne sont disponibles que depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=fr){target="_blank"}

## Validations {#approvals-capabilities}

L’interface utilisateur web de Campaign ne présente pas la gestion de la validation du contenu, des diffusions, des workflows, des campagnes et des cibles. Elles ne sont disponibles que dans la console cliente.

Découvrez comment gérer les validations dans des workflows dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=fr){target="_blank"}.


Découvrez comment gérer les validations de diffusion, de contenu et de cible dans des campagnes dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=fr){target="_blank"}.


## Autorisations {#permissions-capabilities}

Les utilisateurs et utilisatrices de Campaign ne peuvent accéder à l’interface utilisateur web de Campaign qu’à l’aide de leur Adobe ID, via le système IMS (Adobe Identity Management System). Les autorisations accordées aux utilisateurs et utilisatrices s’appliquent également dans l’interface utilisateur web de Campaign.

Les autorisations sont définies dans Adobe Admin Console et la console cliente Adobe Campaign, comme décrit [dans cette section](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=fr). Aucune action sur les autorisations n’est possible à partir de l’interface utilisateur web d’Adobe Campaign.


## Surveillance {#monitoring-capabilities}

Les fonctionnalités de surveillance de la plateforme Campaign ne sont disponibles que dans la console cliente et le panneau de contrôle de Campaign. Elles ne s’affichent pas dans l’interface utilisateur web de Campaign.

Pour en savoir plus, parcourez les liens fournis vers la documentation de Campaign v8 (console cliente) et la documentation du panneau de contrôle.

* [Surveillance des workflows](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=fr){target="_blank"}
* [Carte thermique des workflows](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=fr){target="_blank"}
* [Surveillance des performances](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=fr){target="_blank"}
* [Surveillance de la délivrabilité](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=fr){target="_blank"}




