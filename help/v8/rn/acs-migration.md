---
audience: end-user
title: Transition de Campaign Standard vers Adobe Campaign Web
description: Interface d’utilisation d’Adobe Campaign Web
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 100%

---

# Transition de Campaign Standard vers Campaign v8 {#acs-to-ac}

Les utilisateurs et les utilisatrices d’Adobe Campaign Standard peuvent désormais passer à Adobe Campaign Managed Cloud Services v8. Cette transition offre plusieurs avantages :

* **Infrastructure informatique robuste** : grâce à Managed Cloud Services v8, les clients et clientes peuvent tirer parti d’une infrastructure informatique plus robuste qui garantit des performances, une fiabilité et une évolutivité améliorées pour leurs campagnes.
* **Assistance améliorée** : l’équipe Managed Cloud Services offre une assistance de premier plan pour assurer une transition fluide et une surveillance continue de la plateforme. L’assistance comprend le dépannage et la maintenance proactive.
* **Intégration à Adobe Experience Platform** : Managed Cloud Services v8 se connecte en tout simplicité à Adobe Experience Platform, ce qui permet aux utilisateurs et utilisatrices d’exploiter tout le potentiel de leurs données et de diffuser des campagnes personnalisées à fort impact sur tous les canaux.
* **Interface et expérience d’utilisation cohérentes** : la transition vers Managed Cloud Services v8 ne perturbe pas les workflows. Les utilisateurs et utilisatrices continuent de profiter de l’interface et de l’expérience qui leur sont familières, ce qui réduit la courbe d’apprentissage pour les équipes.

**Si vous êtes utilisateur ou utilisatrice de Campaign Standard et que vous passez à Campaign v8, découvrez comment démarrer [grâce à ce document](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Fonctionnalités principales {#key-features}

En tant qu’utilisateur ou utilisatrice de Campaign v8, vous avez accès à la nouvelle interface de Campaign Web et à la console v8. Les données et les paramètres se synchronisent entre les environnements. L’ensemble de vos données et paramètres déjà disponibles dans la console cliente sont visibles dans l’interface d’utilisation de Campaign Web, à partir du volet de navigation de gauche de l’explorateur. [En savoir plus](../get-started/user-interface.md#user-interface-explorer)

L’interface d’utilisation de Campaign Web est conçue pour que les équipes marketing puissent facilement créer et orchestrer les campagnes. Les fonctionnalités clés de l’interface d’utilisation de Campaign v8 Web sont les suivantes :

* **Expérience moderne, conviviale et unifiée** [En savoir plus](../get-started/connect-to-campaign.md)
* **Nouvelles fonctionnalités puissantes et processus fluides** [En savoir plus](../get-started/user-interface.md)
* **Nouveau concepteur de requête simplifié et intuitif** [En savoir plus](../query/query-modeler-overview.md).
* **Fonctionnalités intégrées de gestion de campagnes cross-canal** [En savoir plus](../msg/gs-messages.md)
* **Activités de workflow de campagne repensées** [En savoir plus](../workflows/gs-workflows.md)
* **Création et gestion simples des profils** [En savoir plus](../audience/about-recipients.md)
* **Filtres prédéfinis** [En savoir plus](../get-started/predefined-filters.md)
* **Convertisseur HTML pour la conception d’e-mail** [En savoir plus](../email/existing-content.md)
* **SMS avec des offres** [En savoir plus](../msg/offers.md)

La console cliente Campaign est conçue pour les équipes d’administration et de développement qui doivent configurer et personnaliser leur environnement. Les fonctionnalités clés disponibles dans la console cliente Campaign sont présentées dans [cette documentation](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Pour en savoir plus sur les fonctionnalités prises en charge et non prises en charge, ainsi que sur l’interopérabilité entre l’interface d’utilisation de Campaign Web et la console cliente Campaign, consultez [cette page](../get-started/capability-matrix.md).

## Terminologie {#terminology}

La plupart des concepts sont similaires entre Campaign v8 et Campaign Standard. Il existe toutefois quelques différences en matière de terminologie : Voici quelques exemples :

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

Pour que vous puissiez passer facilement à Campaign v8, les fonctionnalités clés de Campaign Standard ont été ajoutées à Campaign v8. Elles sont présentées dans [cette documentation](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr){target=&quot;_blank} et ne sont disponibles que pour les personnes qui font la transition depuis Campaign Standard.

* **Rapports dynamiques** : les rapports dynamiques fournissent des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil à des fins d’analyse démographique selon différents critères, tels que le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles telles que les ouvertures et les clics. [En savoir plus](../reporting/dynamic-reporting/get-started-reporting.md)

* **Branding centralisé** : Adobe Campaign permet aux entreprises de définir des directives visuelles et techniques pour la marque. Les utilisateurs et utilisatrices peuvent présenter une marque cohérente aux clientes et clients, depuis les logos jusqu’aux aspects techniques tels que l’expéditeur de l’e-mail, l’URL ou les domaines. [En savoir plus](../administration/branding/branding-gs.md)

* **API REST** : les personnes ayant migré vers Campaign Standard peuvent utiliser des API REST pour créer des intégrations pour Adobe Campaign et créer des écosystèmes en interfaçant Adobe Campaign avec d’autres technologies. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=fr){target="_blank"}

* **Pages de destination** : les pages de destination de Campaign v8 incluent des améliorations pour assurer la parité des fonctionnalités avec Campaign Standard. En savoir plus dans la section [notes de mise à jour](../rn/release-notes.md#new-24-4) et dans la [documentation](../landing-pages/get-started-lp.md) des pages de destination.

* **Fragments visuels** : les fragments visuels sont des composants visuels réutilisables qui peuvent être référencés dans une ou plusieurs diffusions par e-mail ou dans des modèles de contenu. La modification d’un fragment met à jour tout le contenu qui l’utilise. Cette fonctionnalité permet aux équipes marketing de créer à l’avance plusieurs blocs de contenu personnalisés pour l’assemblage rapide de messages dans un processus de conception amélioré. [En savoir plus](../content/use-visual-fragments.md)

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->