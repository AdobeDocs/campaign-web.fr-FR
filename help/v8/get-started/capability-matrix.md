---
audience: end-user
title: Matrice des fonctionnalités de l’interface utilisateur web de Campaign/de la console cliente
description: Liste des fonctionnalités prises en charge dans l’interface utilisateur web de Campaign
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '2102'
ht-degree: 50%

---

# Campaign Web et console cliente Campaign {#capabilities-matrix}

Les principales fonctionnalités de Campaign sont disponibles dans l’interface utilisateur web de Campaign. Cette interface est principalement conçue pour que les professionnels du marketing puissent planifier, lancer et mesurer leurs campagnes marketing. Toutes les fonctionnalités sont répertoriées [sur cette page](../rn/whats-new.md).

La personnalisation de la plateforme Campaign en fonction des besoins de l’entreprise et des données, ainsi que la connexion à d’autres systèmes, est gérée dans la console cliente Campaign. Par conséquent, certains paramètres et fonctionnalités ne sont accessibles, créés ou gérés qu’à partir de la console cliente Campaign. Certaines seront disponibles lors d’une mise à jour ultérieure de l’interface utilisateur web de Campaign.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Gestion de campagne {#campaign-mgt-capabilities}

L’interface utilisateur web de Campaign vous permet de créer des campagnes cross-canal, comme décrit [dans cette section](../campaigns/gs-campaigns.md). Les fonctionnalités suivantes ne sont disponibles que dans la console cliente Campaign. Ils ne sont pas accessibles dans l&#39;interface utilisateur web de Campaign, mais certains sont visibles à partir du menu [Explorateur](user-interface.md#user-interface-explorer).

Utilisez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et découvrir comment utiliser ces fonctionnalités.

* **Calendrier marketing**. Le calendrier des campagnes affiche tous les programmes, plans, campagnes et diffusions dans une chronologie globale. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=fr#campaign-calendar){target="_blank"}
* **Programmes et plans**. Chaque campagne appartient à un programme, qui appartient à un plan. Dans l’interface utilisateur web de Campaign, toutes les campagnes sont associées à un plan et à un programme intégrés par défaut. Vous pouvez uniquement créer et gérer des plans et des programmes dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=fr#work-with-plan-and-program){target="_blank"}
* **Prestataires, budget et gestion des coûts**. Vous pouvez configurer les prestataires de services impliqués dans les traitements réalisés dans vos opérations, y compris les structures de coûts, et gérer vos budgets au sein de chaque programme et campagne. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=fr){target="_blank"}
* **Marketing distribué** (marketing central/local) Adobe Campaign propose une application de marketing distribué qui permet de mettre en place des opérations collaboratives entre les entités centrales (siège social, services marketing, etc.) et les entités locales (points de vente, agences régionales, etc.). Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=fr){target="_blank"}
* **Gestion des ressources marketing** (MRM), objectifs, simulations et contrôle des coûts Adobe Campaign propose une application de gestion des ressources marketing (MRM) qui permet de piloter les actions marketing sur un mode collaboratif, en assurant la gestion complète et le tracking en temps réel des tâches, budgets et ressources marketing impliquées. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=fr){target="_blank"}
* **Gestion des tâches**. Dans le cadre de l’application MRM, les tâches de Campaign peuvent être créées, affectées, suivies et surveillées à partir du tableau de bord de la campagne. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=fr){target="_blank"}

## Canaux de communication {#channels-capabilities}

Grâce à l’interface utilisateur web de Campaign, vous pouvez créer, concevoir et envoyer des **e-mails**, **SMS**, **notifications push**, **courrier** et mesurer leur impact à l’aide de différents rapports dédiés, comme décrit [dans cette section](../msg/gs-messages.md). Toutefois, les canaux suivants ne sont actuellement **pas** disponibles : in-app, LINE, centre d’appels/canal personnalisé, marketing social avec X (Twitter).

Utilisez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur ces canaux.

* **Messagerie LINE**. LINE est une application gratuite de messagerie instantanée, d&#39;appels vocaux et vidéo, disponible sur tous les appareils mobiles et sur PC. Adobe Campaign vous permet d’envoyer des messages LINE uniquement depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=fr){target="_blank"}
* **Centre d’appel et canaux personnalisés**. Le centre d’appel et d’autres canaux personnalisés peuvent être implémentés dans votre environnement Campaign. Ces canaux ne peuvent être disponibles que dans la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=fr#other-channels){target="_blank"}
* **Marketing social** avec X (Twitter). Vous interagissez avec vos clientes et clients via X (Twitter) en publiant des messages et en envoyant des messages directs. Cette fonctionnalité, fournie avec le module complémentaire Marketing social , n’est disponible que depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=fr){target="_blank"}

## Pages de destination et applications web {#Webapps-capabilities}

Adobe Campaign vous permet de créer, concevoir et partager des pages de destination. L’expérience des pages de destination a été entièrement repensée dans la nouvelle interface. Découvrez comment créer, concevoir et publier des landing pages dans l&#39;interface utilisateur web de Campaign [dans cette section](../landing-pages/get-started-lp.md).

Par conséquent, dans la console cliente Campaign, vous ne pouvez pas modifier, mettre à jour ou modifier une landing page créée dans l’interface web, et vice versa. Les types d’applications web suivants ne sont pas disponibles dans l’interface utilisateur web de Campaign. Ils sont toutefois visibles dans la liste des pages de destination. Utilisez les liens fournis pour parcourir la documentation de Campaign Classic v7 et en savoir plus sur ces applications web :

* **Applications web**. Adobe Campaign vous permet de créer et de publier des applications web dynamiques et interactives, composées de données préchargées issues de la base de données et dont le contenu est adapté en fonction des droits de l’utilisateur connecté. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=fr){target="_blank"}
* **Formulaires web**. Les pages web et de destination conçues dans la console cliente sont visibles dans l’interface utilisateur web de Campaign, mais ne peuvent être ni éditées ni modifiées. Certaines options peuvent différer entre le concepteur de pages web de la console cliente et le concepteur de pages de destination fourni avec l’interface utilisateur web de Campaign. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=fr){target="_blank"}
* **Questionnaires en ligne**. Vous pouvez créer des questionnaires en ligne et collecter les réponses à partir de la console cliente uniquement. Cette fonctionnalité n’est pas disponible dans l’interface utilisateur web de Campaign. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=fr){target="_blank"}

## Profils, profils de test et audiences {#profiles-audiences-capabilities}

Vous pouvez créer, gérer et mettre à jour des profils et des profils de test dans la console cliente Campaign et l’interface utilisateur web Campaign. Toutes les modifications effectuées dans une interface sont visibles dans l’autre. Cependant, certains paramètres spécifiques aux destinataires et paramètres avancés peuvent être absents de la nouvelle interface utilisateur web de Campaign.

Notez que le terme « destinataire » a été remplacé par « profil » dans la nouvelle interface utilisateur web et que les « Adresses de contrôle » sont désormais des « Profils de test ».

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Toutes les audiences créées dans la console cliente Campaign ou dans Adobe Experience Platform sont disponibles dans l’interface utilisateur web de Campaign.

Les traitements d’import/export ponctuels, comme décrit dans la documentation [Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=fr#import-jobs){target="_blank"} ne sont pas disponibles dans l’interface utilisateur web de Campaign. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## Conception de contenu {#content-capabilities}

Le nouveau Concepteur d’e-mail fourni avec l’interface utilisateur web d’Adobe Campaign vous permet de créer facilement des e-mails attrayants et personnalisés au moyen d’une interface intuitive par glisser-déposer. Que vous commenciez à partir de zéro, que vous importiez du contenu existant ou que vous utilisiez des modèles existants, vous pouvez concevoir et affiner tout le contenu de chaque e-mail. [En savoir plus](../email/edit-content.md)

Cette nouvelle interface utilisateur vous permet de gérer la synchronisation des modèles d’e-mail à partir de Adobe Experience Manager et de l’intégrer à Adobe Experience Manager as a Cloud Service.

Notez que les fonctionnalités suivantes ne sont pas disponibles pour l’instant dans l’interface utilisateur web de Campaign. Utilisez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur ces fonctionnalités.

* **Création de blocs de personnalisation personnalisés**. Outre les blocs de personnalisation par défaut, vous pouvez créer des blocs personnalisés à partir de la console cliente. Cette fonctionnalité n’est pas disponible dans l’interface utilisateur web de Campaign. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=fr#create-custom-personalization-blocks){target="_blank"}
* **Contenu des formulaires personnalisés**. Le module de gestion de contenu permet de créer et de gérer des formulaires destinés à assister les utilisateurs et utilisatrices lors de la création de contenu dans Campaign. Cette fonctionnalité est uniquement disponible avec la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=fr){target="_blank"}
* **AMP pour les e-mails**. Le format AMP for Email vous permet d’inclure des composants AMP dans vos messages et d’améliorer l’expérience par e-mail avec du contenu riche et exploitable. Cette fonctionnalité est disponible uniquement dans la console cliente. [En savoir plus en consultant la documentation de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=fr){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Typologies et règles de typologie {#rules-capabilities}

Les typologies sont des ensembles de règles de typologie exécutées pendant la phase de préparation pour appliquer facilement plusieurs règles de filtrage à une diffusion à la fois. Ils permettent aux professionnels du marketing de normaliser les pratiques commerciales sur toutes les diffusions en contrôlant, en filtrant et en hiérarchisant l’envoi des diffusions.

Vous pouvez sélectionner des règles de typologie pour une diffusion ou un modèle de diffusion dans l’interface utilisateur web de Campaign, comme décrit [dans cette section](../advanced-settings/delivery-settings.md#typology). Cependant, la création, la gestion et la personnalisation des règles et des règles de typologie ne sont disponibles que dans la console cliente Campaign.

Sélectionnez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur les règles de typologie :

* Création de règles de contrôle. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=fr){target="_blank"}
* Création de règles de fatigue/pression. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=fr){target="_blank"}
* Création de règles de filtrage. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=fr){target="_blank"}
* Gestion des règles de typologie. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=fr){target="_blank"}
* Simulation de campagne. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=fr){target="_blank"}
* Codage JavaScript pour la création de règles de typologie. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=fr#use-cases-on-pressure-rules){target="_blank"}

## Workflows {#wf-capabilities}

La nouvelle interface utilisateur web de Campaign offre une interface de zone de travail de workflow repensée pour concevoir et gérer vos processus. Les principales activités de workflow sont déjà disponibles dans leur nouvelle conception et certaines le seront dans une prochaine mise à jour. En savoir plus sur les fonctionnalités des workflows, y compris les mécanismes de sécurisation et les limitations, [dans cette section](../get-started/guardrails.md).

Notez que les fonctionnalités suivantes ne sont disponibles que dans la console cliente Campaign :

* Script dans les workflows
* Activités ETL : export, édition de schéma, chargement de données, extraction de données, code SQL

En savoir plus sur les activités de workflow disponibles dans la documentation des workflows Adobe Campaign v8 (console) [ici](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=fr){target="_blank"}.

## Gestion des offres {#offer-capabilities}

Vous pouvez envoyer des offres dans vos diffusions créées dans l’interface utilisateur web d’Adobe Campaign. Ces offres doivent avoir été créées dans la console cliente à l’aide du module **[!UICONTROL Interaction]**. La conception des offres, les règles d’éligibilité et la gestion des offres ne sont disponibles que dans la console cliente Campaign. [En savoir plus](../msg/offers.md)

Découvrez comment gérer un catalogue d’offres dans la documentation de [Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=fr){target="_blank"}.

## Intégrations avec les solutions Adobe Experience Cloud {#exc-capabilities}

La nouvelle interface utilisateur moderne de Campaign simplifie la conception et la diffusion des campagnes marketing et offre une expérience cohérente avec d’autres solutions Adobe, notamment Adobe Experience Platform et Adobe Experience Manager.

Les intégrations suivantes sont disponibles à partir de la console cliente Adobe Campaign et ne sont pas encore disponibles dans l’interface utilisateur web de Campaign. Sélectionnez les liens fournis pour parcourir la documentation de Campaign v8 (console cliente) et en savoir plus sur ces intégrations :

* Utilisation des données Adobe Analytics et partage des KPI. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=fr){target="_blank"}
* Partage d’audiences avec Adobe Experience Cloud (Adobe Audience Manager). [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=fr){target="_blank"}
* Intégration avec Adobe Target. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=fr){target="_blank"}
* Intégration avec les Triggers Adobe Experience Cloud. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=fr){target="_blank"}

## Rapports {#reporting-capabilities}

La nouvelle interface utilisateur web de Campaign est fournie avec un ensemble de nouveaux rapports et de KPI pour tous les canaux : rapports de diffusion, rapports de campagne et rapports globaux. En savoir plus dans [cette section](../reporting/gs-reports.md)

Certaines fonctionnalités ne sont disponibles que depuis la console cliente. Parcourez les liens fournis vers la documentation [Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=fr){target="_blank"} et en savoir plus.

* Rapport de délivrabilité et inbox rendering natifs. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=fr){target="_blank"}
* Personnalisations des rapports. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=fr){target="_blank"}
* Analyse descriptive. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=fr){target="_blank"}
* Rapports d’analyse/de cube de campagne. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=fr){target="_blank"}
* Partage des rapports selon un planning au format PDF et CSV ou lien. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=fr){target="_blank"}

## Modélisation des données et ingestion des données {#data-capabilities}

L’interface utilisateur web de Campaign ne présente pas les fonctionnalités suivantes. Elles ne sont disponibles que dans la console cliente :

### Comptes externes {#external}

Adobe Campaign est fourni avec un ensemble de comptes externes prédéfinis pour la connexion aux systèmes externes. En tant qu’administrateur ou administratrice système de Campaign, vous pouvez créer et gérer des comptes externes. [En savoir plus](../administration/external-account.md)

### Création et extension de schéma {#schema}

La création, la modification et l’extension de schéma sont limitées aux utilisateurs et utilisatrices expérimentés. Ces fonctionnalités ne sont disponibles que depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=fr){target="_blank"}

### Fonctionnalités de gestion des données des workflows {#data}

Data Management combine un ensemble d’activités pour résoudre des problèmes de ciblage complexes en offrant des outils plus efficaces et plus flexibles tels que Chargement de données, Extraction (fichier), Mise à jour des données, Modifier le schéma ou Importer/exporter des workflows techniques. [Découvrir les fonctionnalités Data Management des workflows dans la console cliente](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=fr#data-management){target="_blank"}

>[!NOTE]
>
>Bien que certaines de ces activités ne soient disponibles que dans la console cliente, d’autres sont disponibles dans l’interface utilisateur web de Campaign, telles que les activités **Enrichissement**, **Chargement de fichier**, **Modification de la source de données** ou **Modification de la dimension**. [En savoir plus sur les activités de ciblage et de gestion des données dans l’interface utilisateur web de Campaign](../workflows/activities/about-activities.md#targeting)

### Configuration de Federated Data Access {#fda}

La configuration de Campaign et la connexion à des systèmes externes sont limitées aux utilisateurs et utilisatrices expérimentés et ne sont disponibles que depuis la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=fr){target="_blank"}

## Validations {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="Gestion des validations"
>abstract="La gestion des validations n’est disponible que depuis la console cliente. "

L’interface utilisateur web de Campaign ne fait pas apparaître la gestion de la validation du contenu, des diffusions, des workflows, des campagnes et des cibles. Elles ne sont disponibles que dans la console cliente.

Découvrez comment gérer les validations dans des workflows dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=fr){target="_blank"}.

Découvrez comment gérer les validations de diffusion, de contenu et de cible dans les campagnes dans la documentation de [Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=fr){target="_blank"}.

## Autorisations {#permissions-capabilities}

Les utilisateurs de Campaign peuvent uniquement accéder à l’interface utilisateur web de Campaign avec leur Adobe ID, via le système Adobe Identity Management (IMS). Les autorisations accordées aux utilisateurs s’appliquent également à l’interface utilisateur web de Campaign.

Les autorisations sont définies dans Adobe Admin Console et la console cliente Adobe Campaign, comme décrit [dans cette section](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=fr). Aucune action sur les autorisations n’est possible à partir de l’interface utilisateur web d’Adobe Campaign.

## Surveillance {#monitoring-capabilities}

Les fonctionnalités de surveillance de la plateforme Campaign ne sont disponibles que dans la console cliente et le panneau de contrôle Campaign. Elles ne sont pas visibles dans l’interface utilisateur web de Campaign.

Pour en savoir plus, parcourez les liens fournis vers la documentation de Campaign v8 (console cliente) et la documentation du panneau de contrôle.

* [Surveillance des workflows](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=fr){target="_blank"}
* [Carte thermique des workflows](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=fr){target="_blank"}
* [Surveillance des performances](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=fr){target="_blank"}
* [Supervision de la délivrabilité](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=fr){target="_blank"}