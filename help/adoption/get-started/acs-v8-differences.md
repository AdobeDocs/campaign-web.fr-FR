---
title: Différences entre Campaign Standard et Campaign v8
description: Découvrez ce qui change lorsque vous passez de Campaign Standard à Campaign v8 et où trouver les détails
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 25814ce1c70a139c9727b3bfccccd3efe056b441
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 2%
---
# Différences entre Campaign Standard et Campaign v8 {#acs-v8-differences}

La plupart des concepts sont identiques dans Campaign Standard et Campaign v8. Cette page rassemble les différences qui vous affectent après la transition et fournit des liens vers la page qui explique chacune d’elles. Il complète les guides destinés aux [professionnels du marketing](marketers.md) et aux [administrateurs et développeurs](admin-developers.md).

* Pour connaître les modifications terminologiques, voir [Principales différences entre Campaign Standard et Campaign v8](overview.md#experiences).
* Pour connaître les vérifications à exécuter et les problèmes signalés après une transition, voir [Vérifications et dépannage après la transition](post-transition-checks.md).
* Pour connaître les fonctionnalités disponibles uniquement dans la console cliente, voir [Console cliente Campaign Web et Campaign](../../v8/get-started/capability-matrix.md).

## Canaux et contenu {#channels}

Les étapes de création et d&#39;envoi des messages sont similaires dans les deux produits, comme décrit dans le [guide pour les professionnels du marketing](marketers.md). Les différences ci-dessous concernent la disponibilité du canal, les diffusions de test, les landing pages et les workflows de publipostage direct.

| Changements | En savoir plus |
|---|---|
| Le canal In-App n’est pas disponible dans Campaign v8. | [Canal In-App](marketers.md#acs-gs-marketers-in-app) |
| Pour effectuer la transition des workflows et des diffusions de notifications push existants, contactez votre gestionnaire de transition Adobe Campaign. | [Notifications push](marketers.md#acs-gs-marketers-push) |
| Dans Campaign Standard, un profil de test peut être marqué comme un **piège** pour recevoir l’envoi final. Dans Campaign v8, ajoutez un **groupe de pièges** dans les paramètres Audience de la diffusion. | [Groupe de pièges](../../v8/audience/trap-group.md) |
| Les landing pages créées dans l’interface utilisateur web de Campaign ne prennent pas en charge les champs de saisie masqués ou les JavaScript personnalisées. | [Landing pages](../../v8/landing-pages/get-started-lp.md) |
| Dans Campaign Standard, la transition sortante d’une activité de publipostage direct comportait également le fichier généré. Dans Campaign v8, elle ne transporte que la population ciblée. Pour envoyer le fichier à un serveur, ajoutez une activité **Extraction de données**, puis une activité **Transfert de fichier**. | [Publipostage direct](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Audiences, workflows et diffusions {#data-and-workflows}

Ces différences affectent les audiences et les workflows migrés depuis Campaign Standard, certaines options de diffusions récurrentes et de l&#39;activité **Transfert de fichier**, ainsi que la portée des rapports dynamiques.

| Changements | En savoir plus |
|---|---|
| Les audiences sont transformées pendant la transition. Par exemple, les audiences créées avec l&#39;activité Requête deviennent des filtres prédéfinis et les audiences de type fichier deviennent des audiences de type Liste sans dimensions. | [Gérer les audiences](marketers.md#acs-gs-marketers-audiences) |
| Les logs historiques des workflows exécutés dans Campaign Standard ne sont pas migrés. | [Créer un workflow](marketers.md#acs-gs-marketers-wf) |
| Dans Campaign Standard, vous pouvez sélectionner la période d’agrégation d’un e-mail récurrent. Cette option n’est pas disponible dans Campaign v8. | [Activités de canal](../../v8/workflows/activities/channels.md) |
| Les rapports dynamiques couvrent les diffusions par e-mail, les campagnes avec des diffusions par e-mail et les messages transactionnels. | [Reporting](marketers.md#acs-gs-marketers-reporting) |

## Accès et sécurité {#access}

Les groupes de sécurité, les rôles et les entités organisationnelles de Campaign Standard sont associés aux groupes d’opérateurs, aux droits nommés et aux autorisations de dossiers pendant la transition. Examinez les points ci-dessous, en particulier si certains utilisateurs disposent de droits plus larges ou plus étroits qu’auparavant.

| Changements | En savoir plus |
|---|---|
| Les groupes de sécurité, les rôles et les entités organisationnelles sont associés aux groupes d&#39;opérateurs, aux droits nommés et aux autorisations de dossiers. Les rôles personnalisés ne sont pas migrés. | [Gestion des accès utilisateur](user-management-acs.md) |
| Les utilisateurs dotés du rôle **Modèle de données** mais pas du rôle **Administration** obtiennent un accès **Administration**. | [Gestion des accès utilisateur](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Les utilisateurs affectés à des groupes de sécurité avec des entités organisationnelles parallèles peuvent bénéficier d&#39;un accès plus étendu dans Campaign v8. | [Affectation parallèle d’une entité organisationnelle](user-management-acs.md#parallel-assignments) |
| L&#39;accès aux API transactionnelles à partir de l&#39;instance d&#39;exécution nécessite un nouveau profil de produit. | [Mappage du profil de produit](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Les demandes d’accès à des informations personnelles peuvent arriver dans Campaign Standard et Campaign v8 pendant la période où votre environnement Campaign Standard reste actif. | [Informations personnelles et consentement](admin-developers.md#privacy-and-consent) |

## Administration, tracking et pages miroir {#admin-tracking}

Ces différences affectent les diffusions envoyées depuis Campaign Standard avant la transition et les informations administratives qui ne sont pas transférées vers Campaign v8.

| Changements | En savoir plus |
|---|---|
| Les pages miroir des diffusions envoyées depuis Campaign Standard avant la transition ne sont pas disponibles. Les pages miroir des diffusions envoyées à partir de Campaign v8 fonctionnent comme d’habitude. | [Pages miroir](../../v8/email/mirror-page.md) |
| Les données de tracking des diffusions transactionnelles en temps réel envoyées depuis Campaign Standard avant la transition ne sont pas capturées dans Campaign v8. Les liens de ces messages redirigent toujours. | [Surveiller les messages transactionnels](../../v8/transactional-messaging/monitor-transactional.md) |
| Les entités géographiques ne sont pas disponibles. Le contrôle d’accès basé sur les entités géographiques est perdu. | [Contrôle d’accès](../../v8/get-started/connect-to-campaign.md#access-control) |

## API et intégrations {#apis-and-integrations}

Ces différences affectent les intégrations qui appellent Campaign par le biais de son API REST, ainsi que les intégrations à d&#39;autres solutions et outils Adobe.

| Changements | En savoir plus |
|---|---|
| Les valeurs PKEY changent après la migration. Si vous stockez des PKEY en dehors de Campaign, suivez plutôt les arborescences renvoyées par l’API . | [API REST](admin-developers.md#acs-gs-admin-apis) |
| Certains champs de profil migrés, tels que le fuseau horaire et `ccpaOptOut`, sont renvoyés uniquement par l’API `profileAndServicesExt/profile`. | [API REST](admin-developers.md#acs-gs-admin-apis) |
| Les intégrations Dreamweaver et Adobe Experience Platform Data Connector de Campaign Standard ne sont pas disponibles dans Campaign v8. | [Utilisation de Campaign et d&#39;autres solutions Adobe](../../v8/integrations/integration.md) |
| Adobe migre vos configurations Adobe Analytics et Audience Manager. Vous devez configurer à nouveau les intégrations Triggers et Adobe Target. | [Gestion des intégrations Adobe Campaign](admin-developers.md#acs-gs-integrations) |
