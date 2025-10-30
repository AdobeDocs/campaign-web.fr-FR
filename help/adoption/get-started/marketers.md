---
title: Commencer avec Adobe Campaign v8 pour les spécialistes du marketing
description: Découvrez la fonctionnalité principale de Campaign v8. Il est destiné aux spécialistes du marketing qui migrent de Campaign Standard vers Campaign v8.
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 100%

---

# Commencer pour les spécialistes du marketing {#acs-gs-marketers}

Ce guide présente les principales fonctionnalités de Campaign v8 pour les spécialistes du marketing qui passent de Campaign Standard à Campaign v8.

Vous pouvez accéder à Adobe Campaign v8 à partir de la console cliente ou de l’interface d’utilisation web. L’interface web vous permet de créer, de gérer et d’exécuter des actions marketing clés. La nouvelle interface d’Adobe Campaign Web offre une expérience client moderne et intuitive, afin de simplifier la conception et la diffusion des campagnes marketing. [En savoir plus](../../v8/get-started/user-interface.md).

Avec la migration, toutes vos données de Campaign Standard sont importées dans Campaign v8, ce qui garantit une transition fluide avec un minimum de perturbations dans vos opérations en cours.

Vous pouvez continuer à utiliser vos informations d’identification existantes pour vous connecter à votre nouvelle instance Adobe Campaign v8. Une fois la connexion effectuée, vous pouvez trouver tous les profils et workflows migrés, ce qui vous permet de continuer à travailler sur vos campagnes.

La principale différence réside dans l’interface d’utilisation. Voici une comparaison du même workflow dans les 2 interfaces :

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Les mises à jour de l’interface d’utilisation d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continue qui permet une approche plus évolutive et plus progressive du déploiement des fonctionnalités. Consultez régulièrement les [notes de mise à jour](../../v8/rn/release-notes.md) pour connaître les dernières mises à jour.

## Découvrir l’interface d’utilisation de Campaign Web {#acs-gs-marketers-ui}

Dans la vidéo ci-dessous, découvrez comment accéder à l’interface d’utilisation de Campaign Web et y naviguer, et comment personnaliser les listes de stock.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

Pour plus de détails, consultez la documentation ci-dessous :

1. [Découvrir l’interface d’utilisation de Campaign Web](../../v8/get-started/user-interface.md)

1. [Parcourir et filtrer les listes](../../v8/get-started/list-filters.md)


## Créer et gérer des profils et des audiences {#acs-gs-marketers-profiles-and-audiences}

Les concepts généraux de création et de gestion des profils et des audiences dans Campaign v8 sont les mêmes que dans Adobe Campaign Standard. Découvrez comment commencer avec les profils et les audiences dans [cette section](../../v8/audience/gs-audiences-recipients.md).

Vous trouverez ci-dessous quelques liens utiles pour commencer.

### Gestion des profils {#acs-gs-marketers-profiles}

Dans Adobe Campaign, un profil désigne un enregistrement stocké dans la base de données. Il sert de composant clé pour créer des audiences pour les diffusions et ajouter des données de personnalisation à votre contenu.

1. Découvrez comment accéder aux profils, les gérer et les explorer à l’aide de l’interface d’utilisation de Campaign Web dans cette vidéo :

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   En savoir plus dans la documentation [Commencer avec les profils](../../v8/audience/about-recipients.md).

1. Découvrez comment [créer et gérer des profils de test](../../v8/audience/test-profiles.md) dans Campaign v8.

### Gérer des audiences {#acs-gs-marketers-audiences}

Les audiences désignent un ensemble de profils qui partagent des comportements et/ou des caractéristiques similaires. Cette collection de personnes peut être générée, sélectionnée ou chargée. Une fois créées, les audiences peuvent être exploitées comme la population cible de vos diffusions.

Découvrez comment créer et gérer des audiences, comment sélectionner des audiences pour une diffusion et définir des populations témoins dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

Pour plus d’informations, voir [Commencer avec les audiences](../../v8/audience/manage-audience.md){target="_blank"}.

Comme dans Campaign Standard, vous pouvez ajouter une population témoin à votre diffusion. Définissez une population témoin pour éviter d’envoyer des messages à une partie de votre audience et pour comparer le comportement de la cible principale après la diffusion. Cette option vous aide à mesurer l’impact de votre campagne.
Découvrez comment [définir une population témoin](../../v8/audience/control-group.md){target="_blank"}.

>[!AVAILABILITY]
>
>* Toutes les audiences créées via l’activité de requête de Campaign Standard sont transformées en filtre prédéfini dans Campaign v8 lors de la transition. Campaign v8 prend également en charge l’activité de requête.
>
>* L’activité de lecture d’audience est transformée en activité de requête avec [filtre prédéfini](../../v8/query/build-query.md)
>
>* Le filtre prédéfini prend uniquement la dernière valeur après la migration de l’audience vers Campaign v8.
>
>* Les audiences de type Fichier dans Campaign Standard sont migrées en tant que type Liste sans dimensions.

### Gérer les abonnements {#acs-gs-marketers-sub}

Vous pouvez gérer et créer vos services tels que les newsletters, ainsi que vérifier les abonnements et désabonnements relatifs à ces services. Les étapes clés sont globalement les mêmes que dans Campaign Standard. En savoir plus dans les pages ci-dessous :

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="Peu fréquent" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>Créer des services d’abonnement</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="Peu fréquent" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>Gérer les personnes abonnées<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="Validation" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/send-to-subscribers"><strong>Envoyer des messages aux personnes abonnées à un service</strong></a>
</div>
<p>
</td>
</tr>
</table>

## Utiliser des plans, des programmes et des campagnes {#acs-gs-marketers-plans}

Adobe Campaign v8 permet de configurer la hiérarchie des dossiers des plans marketing et des programmes. Les plans, programmes et campagnes sont similaires avec Campaign Standard et avec Campaign v8.

En savoir plus dans la [documentation sur les plans et les programmes](../../v8/administration/plans-programs.md).

Vous trouverez ci-dessous des liens utiles pour commencer. Les modifications susceptibles d’affecter votre expérience client sont mises en évidence dans les remarques sur la disponibilité.


### Créer une campagne {#acs-gs-marketers-campaign}

Grâce à la fonctionnalité de gestion de campagne intégrée, Adobe Campaign permet d’orchestrer en toute facilité vos initiatives marketing ciblées. Tirez parti de la possibilité de définir un planning pour planifier la durée et le lancement opportun de vos campagnes, sur la base de vos objectifs stratégiques, et optimisez l’engagement de votre audience.

![Flux de campagne](assets/campaign-flow.png)

Pour en savoir plus sur les campagnes, consultez la documentation ci-dessous :

1. [Commencer avec les campagnes](../../v8/campaigns/gs-campaigns.md)
1. [Accéder aux campagnes et les gérer](../../v8/campaigns/manage-campaigns.md)
1. [Créer votre première campagne](../../v8/campaigns/create-campaigns.md)


### Créer un workflow {#acs-gs-marketers-wf}

L’interface d’utilisation du workflow a été entièrement repensée dans l’interface d’utilisation de Campaign Web afin de faciliter l’utilisation, la configuration, l’exécution et la résolution des problèmes. Comme vous le faisiez déjà dans Campaign Standard, grâce aux workflows, passez à la vitesse supérieure : orchestrez l’ensemble des processus et tâches, améliorez la vitesse et l’échelle de chaque composante de vos campagnes marketing, de la création de segments jusqu’à la préparation des messages et leur diffusion. Dans une interface unique et conviviale, vous pouvez coordonner vos canaux et orchestrer vos campagnes.

Découvrez le fonctionnement des workflows et comment créer un workflow de ciblage dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Obtenez plus de détails dans la [documentation sur le workflow](../../v8/workflows/gs-workflows.md).

L’interface d’utilisation d’Adobe Campaign Web comporte un concepteur de requête qui simplifie le processus de filtrage de la base de données selon différents critères. [En savoir plus sur le concepteur de requête](../../v8/query/query-modeler-overview.md)

Pour comprendre l’objectif et la fonctionnalité de chaque activité dans votre workflow, explorez les informations détaillées disponibles sur les [activités de workflow](../../v8/workflows/activities/about-activities.md).

Optimisez l’efficacité de votre workflow en passant en revue les [Mécanismes de sécurisation et limitations des workflows](../../v8/get-started/guardrails.md).

>[!AVAILABILITY]
>
>* L’[historique et les logs](../../v8/workflows/start-monitor-workflows.md#logs-tasks) d’exécution des workflows sont disponibles dans Adobe Campaign v8.
>
>* Les logs historiques des workflows exécutés sur votre instance de Campaign Standard ne sont pas migrés vers Campaign v8.
>
>* Les unités organisationnelles sont mappées au concept de dossier pour le mapping et pour garantir un contrôle d’accès similaire.
>

## Créer et gérer des diffusions {#acs-gs-marketers-deliveries}

Avec l’interface d’utilisation de Campaign Web, en tant que spécialiste du marketing, vous pouvez créer des diffusions autonomes à partir du menu de gauche **Diffusions**, ou créer des diffusions dans le cadre d’un workflow, incluses ou non dans une campagne. Les étapes clés sont alignées sur votre expérience précédente dans Campaign Standard. Découvrez comment créer une diffusion dans la section suivante : [Documentation sur la création et la gestion des diffusions](../../v8/msg/gs-deliveries.md).

Liens utiles :

* **Modèles de diffusion** : pour un processus de conception accéléré et amélioré, vous pouvez créer des modèles de diffusion pour réutiliser facilement le contenu et les paramètres personnalisés dans vos campagnes. Cette fonctionnalité vous permet de normaliser l’aspect créatif afin d’être plus rapide dans l’exécution et le lancement des campagnes. En savoir plus sur la page [Modèle de diffusion](../../v8/msg/delivery-template.md).

* **Paramètres de diffusion** : les paramètres de diffusion sont des paramètres de diffusions techniques définis dans le modèle de diffusion. Ils peuvent être surchargés pour chaque diffusion. Ces paramètres sont disponibles depuis le bouton Paramètres disponible lors de la modification d’une diffusion ou d’un modèle de diffusion. En savoir plus dans la section [Paramètres de diffusion](../../v8/advanced-settings/delivery-settings.md).

* **Contenu dynamique** : les fonctionnalités de contenu dynamique d’Adobe Campaign Web vous permettent de personnaliser votre contenu en fonction des informations que vous avez collectées sur vos personnes destinataires. L’utilisation de contenu dynamique vous permet de vous assurer que vos efforts marketing sont plus pertinents, en évitant de commercialiser des produits ou services indésirables ou inutiles. En savoir plus dans la section [Contenu dynamique](../../v8/personalization/gs-personalization.md).

* **Test et BAT** : une fois le contenu de la diffusion rédigé, vous pouvez utiliser les profils et les profils de test pour le prévisualiser et le tester avant d’envoyer le message. Cette étape est cruciale pour s’assurer qu’il est exact, mais également exempt d’erreurs au niveau du contenu et des paramètres de personnalisation. Voir [Prévisualiser et tester](../../v8/preview-test/preview-test.md).

* **Planification** : vous pouvez définir la date et l’heure d’envoi exactes de vos messages. En choisissant l’heure la plus appropriée pour votre message marketing, vous pouvez optimiser les taux d’ouverture.

   * Découvrir comment [planifier une diffusion autonome](../../v8/msg/gs-deliveries.md#gs-schedule)
   * Découvrir comment [planifier une diffusion dans un workflow](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)

* **Ajouter des offres** : vous pouvez ajouter des offres à vos diffusions dans l’interface d’utilisation d’Adobe Campaign Web. Ces offres sont disponibles à partir du menu de gauche Offres qui vous permet d’accéder à la liste des offres.  Découvrir comment [ajouter des offres à vos messages](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* Les diffusions à l’état Brouillon ou à l’état Terminé ont été migrées.
>
>* Les diffusions dans l’un des statuts suivants ont été migrées vers Adobe Campaign v8, mais doivent être préparées à nouveau : En transit, En cours, Annulée, Reprise en cours, Erreur de préparation.
>
>* Les diffusions dans l’un des statuts suivants ont été migrées en tant que diffusions annulées : Annulée, Reprise en cours.
>
>* Les liens de tracking, d’URL de page miroir, d’abonnement/de désabonnement fonctionnent comme dans Campaign Standard.
>
>Consultez également les sections suivantes : [Tracking et surveillance](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Branding](https://experienceleague.adobe.com/fr/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} dans Adobe Campaign.

### Diffusion par e-mail {#acs-gs-marketers-email}

Découvrez comment créer entièrement une diffusion par e-mail, définir l’audience, concevoir le contenu, simuler l’aperçu et envoyer un BAT dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Découvrez comment créer votre premier e-mail ciblé dans la [documentation Créer votre premier e-mail](../../v8/email/create-email.md).

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion par e-mail sont similaires à Campaign Standard.

1. **Concevoir et définir du contenu**

   Le concepteur d’e-mail de Campaign v8 est similaire à celui disponible dans Campaign Standard. Pour rappel, l’[éditeur d’e-mail hérité de Campaign Standard a été abandonné](https://experienceleague.adobe.com/fr/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} il y a quelques années. Vous devez déjà avoir effectué la transition vers le concepteur d’e-mail de Campaign pour créer et personnaliser le contenu de votre e-mail.

   Découvrez comment naviguer dans le concepteur d’e-mail. Découvrez comment structurer et concevoir entièrement un e-mail et personnaliser et tester votre e-mail dans la vidéo suivante :

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   Le concepteur d’e-mail permet de créer des e-mails captivants et personnalisés au moyen d’une interface intuitive par glisser-déposer. En savoir plus dans la [documentation sur le concepteur d’e-mail](../../v8/email/get-started-email-designer.md)

   Découvrez comment créer un e-mail en chargeant un fichier HTML, le rendre compatible avec le concepteur d’e-mail et le convertir en modèle dans cette vidéo :

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   Un fragment de contenu est un composant réutilisable pouvant être référencé dans un ou plusieurs messages. En savoir plus sur les [fragments de contenu](../../v8/content/fragments.md) pour simplifier la création de votre diffusion par e-mail.

   Pour un processus de conception accéléré et amélioré, vous pouvez créer des modèles autonomes pour réutiliser facilement le contenu personnalisé dans Adobe Campaign. Voir [Créer des modèles d’e-mail](../../v8/content/create-email-templates.md)

1. **Prévisualiser et tester**

   Découvrez comment prévisualiser le contenu et la personnalisation des e-mails, envoyer des diffusions de test (BAT), ou encore vérifier le rendu des e-mails dans les clients populaires de bureau, mobiles et web dans cette vidéo :

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Envoyer un e-mail et consulter les logs**

   Lorsque vous avez défini le contenu, l’audience et le planning, vous pouvez préparer votre diffusion par e-mail. En savoir plus dans les sections suivantes :

   * [Préparer et envoyer un e-mail](../../v8/monitor/prepare-send.md)
   * [Surveiller les logs de diffusion](../../v8/monitor/delivery-logs.md)


### Diffusion SMS {#acs-gs-marketers-sms}

Les diffusions par SMS offrent un moyen pratique et efficace d’envoyer des SMS sur les appareils mobiles de vos clientes et clients. Grâce à cette fonctionnalité, vous pouvez créer, personnaliser et prévisualiser des SMS pour une communication efficace.

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion SMS sont similaires à Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="Lead" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/sms/create-sms"><strong>Créer une diffusion SMS</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="Peu fréquent" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/sms/content-sms"><strong>Concevoir une diffusion SMS<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="Validation" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/sms/send-sms"><strong>Prévisualiser et envoyer une diffusion par SMS</strong></a>
</div>
<p>
</td>
</tr></table>

### Notifications push {#acs-gs-marketers-push}

Les notifications push sont essentielles pour communiquer avec les utilisateurs et utilisatrices de votre application mobile, même lorsqu’ils ne l’utilisent pas activement. Elles ont plusieurs objectifs : fournir des mises à jour, inciter à des actions spécifiques et informer de l’existence d’offres.

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion par notification push sont similaires à Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/push/create-push">
<img alt="Lead" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/push/create-push"><strong>Créer une diffusion de notification push</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/push/content-push">
<img alt="Peu fréquent" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/push/content-push"><strong>Concevoir une diffusion de notification push<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/push/send-push">
<img alt="Validation" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/msg/push/send-push"><strong>Prévisualiser et envoyer une diffusion push</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* Adobe Campaign v8 prend en charge le canal de notification push Android et iOS. Pour la transition de workflows et de diffusions existants qui utilisent le canal de notification push, contactez la personne responsable de la transition Adobe Campaign. En savoir plus sur la [configuration de canal](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
>
>* Notez que le SDK V4 pour les applications mobiles a été [abandonné dans Campaign Standard](https://experienceleague.adobe.com/fr/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} il y a quelques années. Vous devez déjà avoir effectué la transition vers le SDK Adobe Experience Platform, qui est le même que celui utilisé dans Campaign v8.
> 

### Courrier {#acs-gs-marketers-direct-mail}

Le canal Courrier est un canal hors ligne qui vous permet de produire des fichiers pour diffuser en masse des lettres personnalisées à votre clientèle, comme des cartes postales, des prospectus ou des catalogues. Lors de la création d’une diffusion par courrier, Adobe Campaign génère automatiquement un fichier d’extraction contenant tous les profils ciblés et les données sélectionnées, comme les adresses postales et les attributs de profil.

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion par courrier sont similaires à Campaign Standard.


1. [Créer une diffusion par courrier](../../v8/direct-mail/create-direct-mail.md)
1. [Définir le fichier d’extraction](../../v8/direct-mail/content-direct-mail.md)
1. [Prévisualiser et envoyer](../../v8/direct-mail/send-direct-mail.md)

### Canal in-app {#acs-gs-marketers-in-app}

Notez que le canal in-app n’est pas disponible dans Campaign v8. Si vous devez envoyer des notifications in-app, contactez votre personne représentante Adobe.

## Créer et gérer des pages de destination {#acs-gs-marketers-lp}

L’interface d’utilisation web d’Adobe Campaign v8 est fournie avec une expérience client repensée pour les pages de destination. Campaign vous permet de créer, concevoir et partager des pages de destination. Les pages de destination vous permettent d’orienter vos utilisateurs et utilisatrices vers des formulaires en ligne sur lesquels ils peuvent mettre à jour leurs données, s’abonner à vos communications ou à un service spécifique tel qu’une newsletter, ou s’en désabonner.

En tant qu’utilisateur ou utilisatrice de Campaign Standard passant à Campaign v8, vos pages de destination existantes ont été migrées vers l’interface d’utilisation de Campaign Web. Vous pouvez accéder à la même gamme de fonctionnalités.

En savoir plus sur les pages de destination dans les sections suivantes :

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="Lead" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/landing-pages/create-lp"><strong>Créer des pages de destination</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="Validation" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/landing-pages/lp-content"><strong>Concevoir des pages de destination</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="Validation" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/landing-pages/lp-templates"><strong>Utiliser des modèles de page de destination</strong></a>
</div>
<p>
</td>
</tr></table>


## Rapports {#acs-gs-marketers-reporting}

Adobe Campaign fournit un ensemble d’[outils de reporting](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}. En tant qu’administrateur ou administratrice, vous pouvez créer et configurer des rapports à partager avec d’autres utilisateurs et utilisatrices de Campaign.

La suite complète d’outils de reporting d’Adobe Campaign fournit des informations précieuses sur l’efficacité de vos efforts marketing, ce qui vous permet d’optimiser vos campagnes pour un impact maximum. En savoir plus dans la [documentation sur le reporting](../../v8/reporting/gs-reports.md).

En outre, comme avec l’expérience d’Adobe Campaign Standard, les rapports dynamiques sont à votre disposition dans Campaign v8 pour vos diffusions par e-mail. Il propose des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Il offre la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, telles que le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. En savoir plus dans la [documentation sur les rapports dynamiques](https://experienceleague.adobe.com/fr/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}

>[!AVAILABILITY]
>
>* Les [rapports dynamiques](https://experienceleague.adobe.com/fr/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} peuvent être utilisés pour la création de rapports sur les diffusions par e-mail, les campagnes avec diffusions par e-mail et les messages transactionnels. L’analyse démographique par dimension de profil est également disponible.
>
> * Le [reporting de l’interface d’utilisation d’Adobe Campaign Web](../../v8/reporting/campaign-reports.md) est également disponible pour tous les utilisateurs et utilisatrices qui passent d’Adobe Campaign Standard à Adobe Campaign v8.

Adobe Campaign propose trois rapports différents :

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="Validation" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>Rapports de campagne</strong></a>
</div>
<p>
<div>
<p>Ils fournissent des informations détaillées sur les performances, l’efficacité et les résultats de vos diffusions individuelles, ce qui vous permet d’obtenir une vue d’ensemble complète.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="Lead" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>Rapports de diffusion</strong>
</div>
<p>
<div>
<p>Ils offrent une analyse approfondie des performances de chaque diffusion, pour chaque canal : taux de succès, engagement de l’audience et autres mesures essentielles. Ils vous permettent d’évaluer l’efficacité globale et l’impact de votre campagne.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="Rapports globaux" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/fr/docs/campaign-web/v8/reports/global-report/global-reports"><strong>Rapports globaux</strong></a>
</div>
<p>
<div>
<p>Ils offrent un résumé global consolidé des mesures de trafic et d’engagement pour chaque canal de votre instance Campaign. Ces rapports se composent de différents widgets, chacun offrant une perspective différente des performances de vos campagnes ou diffusions.</p>
</div>
<p>
</td>
</tr>
</table>
