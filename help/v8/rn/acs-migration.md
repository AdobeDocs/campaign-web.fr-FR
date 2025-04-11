---
audience: end-user
title: Transition de Campaign Standard vers Adobe Campaign Web
description: Interface d’utilisation d’Adobe Campaign Web
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 16%

---

# Transition de Campaign Standard vers Campaign v8 {#acs-to-ac}

Les utilisateurs de Adobe Campaign Standard peuvent désormais passer à Adobe Campaign Managed Cloud Services v8. Cette transition offre plusieurs avantages :

* **Infrastructure informatique robuste** : Managed Cloud Services v8 fournit une infrastructure informatique plus robuste, assurant des performances, une fiabilité et une évolutivité améliorées pour les campagnes.
* **Assistance améliorée** : l’équipe Managed Cloud Services offre une assistance de premier plan pour assurer une transition fluide et une surveillance continue de la plateforme. L’assistance comprend le dépannage et la maintenance proactive.
* **Intégration à Adobe Experience Platform** : Managed Cloud Services v8 se connecte de manière transparente à Adobe Experience Platform, ce qui permet aux utilisateurs d’exploiter entièrement leurs données et de diffuser des campagnes personnalisées et percutantes sur plusieurs canaux.
* **Interface utilisateur et expérience cohérentes** : la transition vers Managed Cloud Services v8 ne perturbe pas les workflows. Les utilisateurs continuent à profiter de l’interface et de l’expérience familières, ce qui réduit la courbe d’apprentissage pour les équipes.

**Si vous êtes utilisateur ou utilisatrice de Campaign Standard passant à Campaign v8, découvrez comment démarrer [grâce à ce document](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Fonctionnalités principales {#key-features}

Les utilisateurs de Campaign v8 ont accès à la fois à la nouvelle interface web de Campaign et à la console v8. Les données et les paramètres se synchronisent entre les environnements. L’ensemble des données et des paramètres disponibles dans la console cliente sont visibles dans l’interface utilisateur web de Campaign, accessible à partir du volet de navigation de gauche de l’explorateur. [En savoir plus](../get-started/user-interface.md#user-interface-explorer)

L’interface utilisateur web de Campaign est conçue pour que les marketeurs puissent facilement créer et orchestrer des campagnes. Les fonctionnalités clés de l’interface utilisateur web de Campaign v8 sont les suivantes :

* **Une expérience moderne, conviviale et unifiée**. [En savoir plus](../get-started/connect-to-campaign.md).
* **Nouvelles fonctionnalités puissantes et processus transparents**. [En savoir plus](../get-started/user-interface.md).
* **Modéliseur de requête simplifié et intuitif**. [En savoir plus](../query/query-modeler-overview.md).
* **Fonctionnalités intégrées de gestion de campagnes cross-canal**. [En savoir plus](../msg/gs-messages.md).
* **Activités de workflow de campagne repensées**. [En savoir plus](../workflows/gs-workflows.md).
* **Création et gestion faciles de profils**. [En savoir plus](../audience/about-recipients.md).
* **Filtres prédéfinis**. [En savoir plus](../get-started/predefined-filters.md).
* **convertisseur HTML pour la conception d’e-mails**. [En savoir plus](../email/existing-content.md).
* **SMS avec offres**. [En savoir plus](../msg/offers.md).

La console cliente Campaign est conçue pour permettre aux administrateurs et aux développeurs de configurer et de personnaliser leur environnement. Les fonctionnalités clés disponibles dans la console cliente Campaign sont présentées en détail dans [cette documentation](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Découvrez les fonctionnalités prises en charge et non prises en charge ainsi que l’interopérabilité entre l’interface utilisateur web de Campaign et la console cliente Campaign [sur cette page](../get-started/capability-matrix.md).

## Terminologie {#terminology}

La plupart des concepts sont similaires entre Campaign v8 et Campaign Standard. Cependant, il existe quelques différences terminologiques. Voici quelques exemples :

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Fonctionnalités spécifiques {#new-features}

Afin d’assurer une transition fluide vers Campaign v8, des fonctionnalités Campaign Standard essentielles ont été ajoutées à Campaign v8. Ces fonctionnalités sont détaillées dans [cette documentation](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr){target="_blank} et ne sont disponibles que pour les utilisateurs qui effectuent une transition à partir de Campaign Standard.

* **Rapports dynamiques** : les rapports dynamiques fournissent des rapports en temps réel personnalisables pour mesurer l’impact des activités marketing. Elle inclut l’accès aux données de profil pour l’analyse démographique par dimensions telles que le sexe, la ville et l’âge, ainsi qu’aux données fonctionnelles de campagne par e-mail telles que les ouvertures et les clics. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=fr){target="_blank"}.

* **Valorisation de marque centralisée** : Adobe Campaign permet aux entreprises de définir des directives visuelles et techniques pour la marque. Les utilisateurs peuvent présenter une marque cohérente aux clients, depuis les logos jusqu’aux aspects techniques tels que l’expéditeur de l’e-mail, l’URL ou les domaines. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=fr).

* **API REST** : les utilisateurs ayant migré vers Campaign Standard peuvent utiliser des API REST pour créer des intégrations pour Adobe Campaign et créer des écosystèmes en interfaçant Adobe Campaign avec d’autres technologies. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=fr){target="_blank"}.

* **Pages de destination** : les pages de destination de Campaign v8 incluent des améliorations pour assurer la parité des fonctionnalités avec Campaign Standard. En savoir plus dans la section [notes de mise à jour](../rn/release-notes.md#new-24-4) et dans la [documentation](../landing-pages/get-started-lp.md) des pages de destination.

* **Fragments visuels** : les fragments visuels sont des composants visuels réutilisables référencés dans une ou plusieurs diffusions d’e-mail ou modèles de contenu. La modification d’un fragment met à jour tout le contenu qui l’utilise. Cette fonctionnalité permet aux utilisateurs marketing de précréer plusieurs blocs de contenu personnalisés pour l’assemblage rapide de messages dans un processus de conception amélioré. [En savoir plus](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->