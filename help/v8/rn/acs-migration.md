---
audience: end-user
title: Transition du Campaign Standard au Web Adobe Campaign
description: Découvrir l’interface utilisateur web de Campaign
source-git-commit: 4c1f68f0e89b2b84b8845b2759ef3b0dc9b12033
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 12%

---


# Transition Campaign Standard vers Campaign v8{#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

Bienvenue dans Adobe Campaign Managed Cloud Services v8 !

Nous sommes ravis d’annoncer que les utilisateurs de Adobe Campaign Standard peuvent désormais passer à Adobe Campaign Managed Cloud Services v8. Cette transition présente de nombreux avantages :

* Une infrastructure informatique robuste : grâce aux Cloud Service gérés v8, les clients peuvent tirer parti d’une infrastructure informatique plus robuste, assurant des performances, une fiabilité et une évolutivité améliorées pour leurs campagnes.
* Amélioration de la prise en charge : notre équipe de Cloud Service gérés s’engage à fournir une assistance de pointe pour garantir une transition en douceur et une surveillance continue de votre plateforme. De la résolution des problèmes à la maintenance proactive, nous vous couvrons.
* Intégration à Adobe Experience Platform : Managed Cloud Service v8 se connecte de manière transparente à Adobe Experience Platform, ce qui permet aux clients d’exploiter tout le potentiel de leurs données et de diffuser des campagnes personnalisées et percutantes sur tous les canaux.
* Interface utilisateur et expérience cohérentes : rassurez-vous, la transition vers la version 8 des Cloud Service gérés ne perturbera pas votre workflow. Vous continuerez à profiter de l’interface utilisateur et de l’expérience utilisateur, ce qui vous garantit une courbe d’apprentissage minimale pour votre équipe.

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Fonctionnalités principales {#key-features}

Examinons plus en détail les principales fonctionnalités offertes par Campaign v8 :

* Expérience moderne, amicale et unifiée. [En savoir plus](../get-started/connect-to-campaign.md).
* Nouvelles fonctionnalités puissantes et processus transparents. [En savoir plus](../get-started/user-interface.md)
* Nouveau modèle de requête simplifié et intuitif. [En savoir plus](../query/query-modeler-overview.md)
* Fonctionnalités intégrées de gestion de campagne cross-canal. [En savoir plus](../msg/gs-messages.md)
* Activités de workflow de campagne nouvelles et repensées. [En savoir plus](../workflows/gs-workflows.md)
* Public cible avec le créateur de modèles de requête. [En savoir plus](../query/query-modeler-overview.md)
* Création et gestion aisées des profils. [En savoir plus](../audience/about-recipients.md)
* Aide contextuelle optimisée par l’IA [En savoir plus](../get-started/using-ai.md)
* Filtres prédéfinis. [En savoir plus](../get-started/predefined-filters.md)
* Convertisseur de HTMLs pour la conception d&#39;email. [En savoir plus](../email/existing-content.md)
* SMS avec des offres. [En savoir plus](../msg/offers.md)

## Console et interface web {#console}

En tant qu&#39;utilisateur de Campaign v8, vous avez accès à la nouvelle interface Web de Campaign et à la console v8. Les données et les paramètres sont synchronisés d’un environnement à un autre. Toutes les données et tous les paramètres disponibles dans la console cliente sont visibles dans l&#39;interface utilisateur Web de Campaign, à partir du volet de navigation de gauche de l&#39;Explorateur. [En savoir plus](../get-started/user-interface.md#user-interface-explorer)

Fonctionnalités prises en charge et non prises en charge et interopérabilité entre l’interface utilisateur Web de Campaign et la console cliente Campaign [dans cette page](../get-started/capability-matrix.md)

## Terminologie {#terminology}

La plupart des concepts sont similaires entre l&#39;interface web de Campaign et Campaign Standard. Cependant, il y a quelques différences. Voici quelques exemples de différences terminologiques entre Campaign Standard et l’interface web de Campaign :

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* Les ressources personnalisées **Schémas** dans l&#39;interface utilisateur Web de Campaign.
* Les activités marketing n&#39;existent plus.
* Messages is **Diffusions**.
* Les opérateurs sont **Utilisateurs**.
* Les droits nommés **Rôles**.
* Les groupes d’opérateurs sont **Groupes de sécurité**.
* Les autorisations de dossier sont **Entités organisationnelles**

## Nouveautés {#new-features}

Pour que vous puissiez effectuer une transition, nous avons ajouté [principales fonctionnalités](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html) de Campaign Standard à v8 :

* **Rapports dynamiques**: les rapports dynamiques fournissent des rapports en temps réel entièrement personnalisables pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, telles que le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Marque centralisée**: chaque entreprise dispose de directives visuelles et techniques sur la marque. Avec Adobe Campaign, vous pouvez définir un ensemble de spécifications afin de présenter une marque cohérente à vos clients, depuis les logos jusqu’aux aspects techniques, tels que l’expéditeur d’emails, l’URL ou les domaines. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **API REST** - En tant qu’utilisateur migré de Campaign Standard, vous pouvez utiliser les API REST pour créer des intégrations pour Adobe Campaign et créer votre propre écosystème en interfaçant Adobe Campaign avec le panneau de technologies que vous utilisez. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Landing pages** - De nombreuses améliorations ont été apportées à Campaign v8 pour vous assurer que vous ne perdez aucune fonctionnalité. En savoir plus dans la section [notes de mise à jour](../rn/release-notes.md#new-24-4) et la landing page [documentation](../landing-pages/get-started-lp.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->