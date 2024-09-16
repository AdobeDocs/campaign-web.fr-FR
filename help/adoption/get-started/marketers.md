---
title: Commencer avec Adobe Campaign v8 pour les spécialistes du marketing
description: Découvrez les fonctionnalités clés de Campaign v8. Il est destiné aux spécialistes du marketing qui migrent de Campaign Standard vers Campaign v8.
role: User
level: Beginner, Experienced
source-git-commit: e68ad7ca3368165feb534363c36b03b510291e8a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Commencer pour les spécialistes du marketing {#acs-gs-marketers}

Ce guide présente les principales fonctionnalités de Campaign v8 pour les marketeurs qui passent de Campaign Standard à Campaign v8.

Vous pouvez accéder à Adobe Campaign v8 via la console cliente ou l&#39;interface utilisateur Web. L’interface web vous permet de créer, gérer et exécuter des actions marketing clés. La nouvelle interface d’Adobe Campaign Web offre une expérience utilisateur moderne et intuitive, afin de simplifier la conception et la diffusion des campagnes marketing. [En savoir plus](../../v8/get-started/user-interface.md).

Avec la migration, toutes vos données de Campaign Standard sont importées dans Campaign v8, ce qui garantit une transition fluide avec un minimum de perturbations dans vos opérations en cours.

Vous pouvez continuer à utiliser vos informations d’identification existantes pour vous connecter et vous connecter à votre nouvelle instance Adobe Campaign v8. Une fois connecté, vous pouvez trouver tous les profils et workflows migrés, ce qui vous permet de continuer à travailler sur vos campagnes.

La principale différence réside dans l’interface utilisateur de . Voici une comparaison du même workflow dans les 2 interfaces :

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Les mises à jour de l’interface d’utilisation d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continue qui permet une approche plus évolutive et plus progressive du déploiement des fonctionnalités. Consultez régulièrement les [notes de mise à jour](../../v8/rn/release-notes.md) pour connaître les dernières mises à jour.

## Découvrez l’interface utilisateur web de Campaign {#acs-gs-marketers-ui}

Dans la vidéo ci-dessous, découvrez comment accéder à l’interface utilisateur Web de Campaign et naviguer dans celle-ci, et comment personnaliser les listes de stock.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

Pour plus d’informations, consultez la documentation ci-dessous :

1. [Découvrez l&#39;interface utilisateur Web de Campaign](../../v8/get-started/user-interface.md)

1. [Parcourir et filtrer les listes](../../v8/get-started/list-filters.md)


## Créer et gérer des profils et des audiences {#acs-gs-marketers-profiles-and-audiences}

Les concepts généraux de création et de gestion des profils et des audiences dans Campaign v8 sont les mêmes que dans Adobe Campaign Standard. Découvrez comment commencer avec les profils et les audiences dans [cette section](../../v8/audience/gs-audiences-recipients.md).

Vous trouverez ci-dessous quelques liens utiles pour commencer.

### Gestion des profils {#acs-gs-marketers-profiles}

Dans Adobe Campaign, un profil est un enregistrement stocké dans la base de données. Il sert de composant clé pour créer des audiences pour les diffusions et ajouter des données de personnalisation à votre contenu.

1. Découvrez comment accéder aux profils, les gérer et les explorer à l’aide de l’interface utilisateur Web de Campaign dans cette vidéo :

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   Pour en savoir plus, consultez la documentation [Prise en main des profils](../../v8/audience/about-recipients.md) .

1. Découvrez comment [créer et gérer des profils de test](../../v8/audience/test-profiles.md) dans Campaign v8.

### Gérer des audiences {#acs-gs-marketers-audiences}

Les audiences sont des ensembles de profils qui partagent des comportements et/ou des caractéristiques similaires. Cette collection de personnes peut être générée, sélectionnée ou chargée. Une fois créées, les audiences peuvent être exploitées comme la population cible de vos diffusions.

Découvrez comment créer et gérer des audiences, comment sélectionner des audiences pour une diffusion et définir des populations témoins dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

Pour plus d’informations, voir [Prise en main des audiences](../../v8/audience/manage-audience.md){target="_blank"} .

Comme dans Campaign Standard, vous pouvez ajouter une population témoin à votre diffusion. Définissez une population témoin pour éviter d’envoyer des messages à une partie de votre audience et pour comparer le comportement de la cible principale après la diffusion. Cette option vous aide à mesurer l’impact de votre campagne.
Découvrez comment [définir une population témoin](../../v8/audience/control-group.md){target="_blank"}.

>[!AVAILABILITY]
>
>* Toutes les audiences créées via l&#39;activité Requête de Campaign Standard sont transformées en filtre prédéfini dans Campaign v8 lors de la transition. Campaign v8 prend également en charge l’activité Requête .
>
>* L’audience de lecture est transformée en activité de requête avec [filtre prédéfini](../../v8/query/build-query.md)
>
>* Le filtre prédéfini prend uniquement la dernière valeur après la migration de l’audience vers Campaign v8.
>
>* Les audiences de type fichier dans Campaign Standard sont migrées en tant que type Liste sans dimensions.

### Gérer les abonnements {#acs-gs-marketers-sub}

Vous pouvez gérer et créer vos services tels que des newsletters, et vérifier les abonnements ou désabonnements à ces services. Les étapes clés sont globalement les mêmes que dans Campaign Standard. Pour en savoir plus, consultez les pages ci-dessous :

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

## Utilisation des plans, programmes et campagnes {#acs-gs-marketers-plans}

Adobe Campaign v8 vous permet de configurer la hiérarchie de dossiers des plans et programmes marketing. Les plans, programmes et campagnes sont similaires à Campaign Standard et à Campaign v8.

Pour en savoir plus, consultez la [documentation sur les plans et les programmes](../../v8/administration/plans-programs.md).

Vous trouverez ci-dessous des liens utiles pour commencer. Les modifications susceptibles d’affecter votre expérience utilisateur sont mises en évidence dans les notes de disponibilité.


### Créer une campagne {#acs-gs-marketers-campaign}

Adobe Campaign vous permet d’orchestrer facilement vos initiatives marketing ciblées à l’aide de la fonctionnalité intégrée de gestion de campagne. Tirez parti de la possibilité de définir un planning pour planifier la durée et le lancement opportun de vos campagnes, sur la base de vos objectifs stratégiques, et optimisez l’engagement de votre audience.

![Flux de campagne](assets/campaign-flow.png)

Pour en savoir plus sur les campagnes, consultez la documentation ci-dessous :

1. [Prise en main des campagnes](../../v8/campaigns/gs-campaigns.md)
1. [Accéder aux campagnes et les gérer](../../v8/campaigns/manage-campaigns.md)
1. [Créer votre première campagne](../../v8/campaigns/create-campaigns.md)


### Créer un workflow {#acs-gs-marketers-wf}

L’interface utilisateur du workflow a été entièrement repensée dans l’interface utilisateur Web de Campaign afin de faciliter l’utilisation, la configuration, l’exécution et la résolution des problèmes. Comme vous l’avez déjà fait avec Campaign Standard, avec les workflows, vous pouvez orchestrer l’ensemble des processus et tâches, améliorer la vitesse et l’échelle de chaque aspect de vos campagnes marketing, de la création de segments à la préparation des messages en passant par la diffusion. Dans une interface unique et conviviale, vous pouvez coordonner vos canaux et orchestrer vos campagnes.

Découvrez le fonctionnement des workflows et comment créer un workflow de ciblage dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Pour plus d’informations, consultez la [documentation sur le workflow](../../v8/workflows/gs-workflows.md).

L’interface utilisateur web d’Adobe Campaign comporte un modèle de requête dans les workflows qui simplifie le processus de filtrage de la base de données selon différents critères. [En savoir plus sur le modeleur de requête](../../v8/query/query-modeler-overview.md)

Pour comprendre l’objectif et les fonctionnalités de chaque activité dans votre workflow, explorez les informations détaillées disponibles sur les [activités de workflow](../../v8/workflows/activities/about-activities.md)

Optimisez l&#39;efficacité de votre workflow en examinant les [Barrières de sécurité et limites des workflows](../../v8/get-started/guardrails.md).

>[!AVAILABILITY]
>
>* L&#39;exécution des workflows [history et logs](../../v8/workflows/start-monitor-workflows.md#logs-tasks) sont disponibles dans Adobe Campaign v8.
>
>* Les logs historiques des workflows exécutés sur votre instance de Campaign Standard ne sont pas migrés vers Campaign v8.
>
>* Les entités organisationnelles sont mappées au concept de dossier pour le mappage et la garantie d’un contrôle d’accès similaire.
>

## Créer et gérer des diffusions {#acs-gs-marketers-deliveries}

Avec l’interface utilisateur web de Campaign, en tant que marketeur, vous pouvez créer des diffusions autonomes à partir du menu de gauche **Diffusions** ou créer des diffusions dans le cadre d’un workflow, inclus ou non dans une campagne. Les étapes clés sont alignées sur votre expérience précédente dans Campaign Standard. Découvrez comment créer une diffusion dans la section suivante : [Documentation sur la création et la gestion des diffusions](../../v8/msg/gs-deliveries.md).

Liens utiles :

* **Modèles de diffusion** - Pour accélérer et améliorer le processus de conception, vous pouvez créer des modèles de diffusion afin de réutiliser facilement du contenu et des paramètres personnalisés dans vos campagnes. Cette fonctionnalité vous permet de normaliser l’aspect créatif afin d’être plus rapide dans l’exécution et le lancement des campagnes/ En savoir plus sur la page [Modèle de diffusion](../../v8/msg/delivery-template.md).

* **Paramètres de diffusion** - Les paramètres de diffusion sont des paramètres de diffusion techniques définis dans le modèle de diffusion. Ils peuvent être surchargés pour chaque diffusion. Ces paramètres sont disponibles à partir du bouton Paramètres disponible lors de l&#39;édition d&#39;une diffusion ou d&#39;un modèle de diffusion. Pour en savoir plus, consultez la section [Paramètres de diffusion](../../v8/advanced-settings/delivery-settings.md) .

* **Contenu dynamique** - Les fonctionnalités de contenu dynamique web d’Adobe Campaign vous permettent de personnaliser votre contenu en fonction des informations que vous avez rassemblées sur vos destinataires. L’utilisation de contenu dynamique vous permet de vous assurer que vos efforts marketing sont plus pertinents, en évitant de commercialiser des produits ou services indésirables ou inutiles. Pour en savoir plus, consultez la section [Contenu dynamique](../../v8/personalization/gs-personalization.md) .

* **Test et BAT** - Une fois le contenu de votre diffusion défini, vous pouvez utiliser des profils et des profils de test pour le prévisualiser et le tester avant d’envoyer le message. Cette étape est essentielle pour s’assurer qu’elle est exacte, mais également exempte d’erreurs dans les paramètres de contenu et de personnalisation. Voir [Aperçu et test](../../v8/preview-test/preview-test.md).

* **Planification** - Vous pouvez définir la date et l’heure exactes d’envoi de vos messages. En choisissant l’heure la plus appropriée pour votre message marketing, vous pouvez optimiser les taux d’ouverture.

   * Découvrez comment [planifier une diffusion autonome](../../v8/msg/gs-deliveries.md#gs-schedule)
   * Découvrez comment [planifier une diffusion dans un workflow](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)

* **AJOUTER des offres** - Vous pouvez ajouter des offres à vos diffusions dans l’interface utilisateur Web d’Adobe Campaign. Ces offres sont disponibles à partir du menu de gauche Offres , qui permet d&#39;accéder à la liste des offres.  Découvrez comment [ajouter des offres à vos messages](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* Les diffusions en état de brouillon ou à l’état terminé ont été migrées.
>
>* Les diffusions qui ont l&#39;un des statuts suivants ont été migrées vers Adobe Campaign v8, mais doivent être préparées à nouveau : En transit / En cours / Annulée / Reprise en cours / Erreur de préparation.
>
>* Les diffusions ayant l&#39;un des statuts suivants ont été migrées en tant que diffusions annulées : Pour annulées / Reprises en cours.
>
>* Les liens de tracking, URL de page miroir, liens d’abonnement/désabonnement fonctionnent comme dans Campaign Standard.
>
>Voir aussi les sections suivantes : [Tracking et surveillance](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Marque](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} dans Adobe Campaign.

### Diffusion par e-mail {#acs-gs-marketers-email}

Découvrez comment créer entièrement une diffusion email, définir l&#39;audience, concevoir le contenu, simuler l&#39;aperçu et envoyer un BAT dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Découvrez comment créer votre premier email ciblé dans la [documentation Créer votre premier email](../../v8/email/create-email.md)

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion email sont similaires à Campaign Standard.

1. **Concevoir et définir du contenu**

   Le Concepteur d’email de Campaign v8 est similaire à celui disponible dans Campaign Standard. Pour rappel, l’ancien éditeur d’email de Campaign Standard[a été abandonné ](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} il y a quelques années. Vous devez déjà être passé à Campaign Email Designer pour créer et personnaliser le contenu de votre email.

   Découvrez comment naviguer dans le Concepteur d’e-mail. Découvrez comment structurer et concevoir entièrement un email, comment personnaliser et tester votre email dans la vidéo suivante :

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   Le concepteur d’e-mail permet de créer des e-mails captivants et personnalisés au moyen d’une interface intuite par glisser-déposer. Pour en savoir plus, consultez la [documentation Designer par e-mail](../../v8/email/get-started-email-designer.md)

   Découvrez comment créer un email en téléchargeant un HTML, comment le rendre compatible avec le Designer d&#39;email et comment le convertir en modèle dans cette vidéo :

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   Un fragment de contenu est un composant réutilisable pouvant être référencé dans un ou plusieurs messages. En savoir plus sur les [fragments de contenu](../../v8/content/fragments.md) pour simplifier la création de votre diffusion email.

   Pour accélérer et améliorer le processus de conception, vous pouvez créer des modèles autonomes pour réutiliser facilement du contenu personnalisé dans Adobe Campaign. Voir [Créer des modèles d’email](../../v8/email/create-email-templates.md)

1. **Prévisualiser et tester**

   Découvrez comment prévisualiser le contenu et la personnalisation des emails, envoyer des diffusions de test (BAT) et vérifier le rendu des emails dans les clients de bureau, mobiles et web les plus populaires, dans cette vidéo :

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Envoyer un e-mail et consulter les journaux**

   Une fois que vous avez défini votre contenu, votre audience et votre planning, vous êtes prêt à préparer votre diffusion email. En savoir plus dans les sections suivantes :

   * [Préparer et envoyer un e-mail](../../v8/monitor/prepare-send.md)
   * [Surveiller les logs de diffusion](../../v8/monitor/delivery-logs.md)


### Diffusion SMS {#acs-gs-marketers-sms}

Les diffusions par SMS offrent un moyen pratique et efficace d’envoyer des SMS sur les appareils mobiles de vos clientes et clients. Grâce à cette fonctionnalité, vous pouvez créer, personnaliser et prévisualiser des SMS pour une communication efficace.

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion SMS sont similaires à Campaign Standard.


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

Les notifications push sont essentielles pour atteindre les utilisateurs de votre application mobile, même s’ils n’utilisent pas activement votre application. Ils ont diverses fonctions, comme fournir des mises à jour, mener des actions spécifiques et informer au sujet des offres.

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion de notification push sont similaires à Campaign Standard.


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
>* Adobe Campaign v8 prend en charge Android et le canal push iOS. Pour la transition des workflows et des diffusions existants à l’aide du canal push, connectez-vous à votre Gestionnaire de transition Adobe Campaign. En savoir plus sur la [configuration de canal](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
>
>* Notez que le SDK V4 pour les applications mobiles était [ obsolète en Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} il y a quelques années. Vous devez déjà passer au SDK Adobe Experience Platform, qui est le même que celui utilisé dans Campaign v8.
> 

### Courrier {#acs-gs-marketers-direct-mail}

Le canal Courrier est un canal hors ligne qui vous permet de produire des fichiers pour diffuser en masse des lettres personnalisées à vos clients, telles que des cartes postales, des prospectus ou des catalogues. Lors de la création d&#39;une diffusion courrier, Adobe Campaign génère automatiquement un fichier d&#39;extraction contenant tous les profils ciblés et les données sélectionnées, telles que les adresses postales et les attributs de profil.

Dans Campaign v8, les étapes détaillées pour créer, tester et envoyer une diffusion courrier sont similaires à Campaign Standard.


1. [Créer une diffusion courrier](../../v8/direct-mail/create-direct-mail.md)
1. [Définition du fichier d&#39;extraction](../../v8/direct-mail/content-direct-mail.md)
1. [Prévisualiser et envoyer](../../v8/direct-mail/send-direct-mail.md)

### Canal In-App {#acs-gs-marketers-in-app}

Notez que le canal In-App n&#39;est pas disponible dans Campaign v8. Si vous devez envoyer des notifications in-app, contactez votre représentant d’Adobe.

## Créer et gérer des pages de destination {#acs-gs-marketers-lp}

L’interface utilisateur web d’Adobe Campaign v8 s’accompagne d’une expérience utilisateur repensée pour les landing pages. Campaign vous permet de créer, concevoir et partager des landing pages. Les pages de destination vous permettent d’orienter vos utilisateurs et utilisatrices vers des formulaires en ligne sur lesquelles ils peuvent mettre à jour leurs données, s’abonner à vos communications ou à un service spécifique tel qu’une newsletter, ou s’en désabonner.

En tant qu’utilisateur Campaign Standard passant à Campaign v8, vos landing pages existantes ont été migrées vers l’interface utilisateur Web de Campaign. Vous pouvez accéder à la même gamme de fonctionnalités.

En savoir plus sur les landing pages dans les sections suivantes :

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

Adobe Campaign fournit un ensemble d’ [ outils de création de rapports ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}. En tant qu’administrateur, vous pouvez créer et configurer des rapports à partager avec d’autres utilisateurs de Campaign.

La suite d’outils de création de rapports d’Adobe Campaign fournit des informations précieuses sur l’efficacité de vos efforts marketing, ce qui vous permet d’optimiser vos campagnes pour un impact maximum. Pour en savoir plus, consultez la [documentation sur le reporting](../../v8/reporting/gs-reports.md).

En outre, conformément à l’expérience Adobe Campaign Standard, les rapports dynamiques sont à votre disposition dans Campaign v8 pour vos diffusions email. Il fournit des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, telles que le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. En savoir plus dans la [documentation sur les rapports dynamiques](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}

>[!AVAILABILITY]
>
>* La [création de rapports dynamiques](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} peut être utilisée pour la création de rapports sur les diffusions email, les campagnes avec diffusions email et les messages transactionnels. L’analyse démographique par dimension Profil est également disponible.
>
> * [La création de rapports sur l’interface utilisateur Web d’Adobe Campaign](../../v8/reporting/campaign-reports.md) est également disponible pour tous les utilisateurs qui passent de Adobe Campaign Standard à Adobe Campaign v8.

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
<p>Fournissez des informations détaillées sur les performances, l’efficacité et les résultats de vos diffusions individuelles, afin de vous offrir une vue d’ensemble exhaustive.</p>
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
<p>Offrir une analyse approfondie des performances de chaque diffusion, par canal : taux de succès, engagement de l’audience et autres mesures essentielles. Ils vous permettent d’évaluer l’efficacité globale et l’impact de votre campagne.</p>
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
<p>Fournissez un résumé global consolidé des mesures de trafic et d’engagement pour chaque canal de votre instance Campaign. Ces rapports se composent de différents widgets, chacun offrant une perspective différente des performances de vos campagnes ou diffusions.</p>
</div>
<p>
</td>
</tr>
</table>
