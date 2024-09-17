---
title: Prise en main d’Adobe Campaign v8 après la transition depuis Campaign Standard
description: Découvrez les étapes requises pour commencer à utiliser votre nouvelle application Campaign v8
role: User, Admin, Developer
level: Beginner
source-git-commit: a1c16a9ba5e5ca844eaf82ed3b587f4f7a0b0873
workflow-type: tm+mt
source-wordcount: '1560'
ht-degree: 35%

---


# De Campaign Standard vers v8 {#ac-acs}

Bienvenue dans Adobe Campaign v8.

En tant qu’utilisateur passant de Campaign Standard à Campaign v8, ce guide de référence est conçu pour vous. Il vous aide à vous familiariser avec votre nouvel environnement Campaign et à vous guider dans les étapes nécessaires pour commencer à utiliser votre rôle.

1. Commencez par apprendre [les nouveautés d’Adobe Campaign v8](#new).

1. Comprenez ensuite [les différences d’expérience entre Adobe Campaign Standard et Adobe Campaign v8 en fonction de votre rôle](#experiences).

## Nouveautés {#new}

Découvrez les améliorations les plus récentes de l’interface utilisateur Web d’Adobe Campaign dans cette page. Pour obtenir une liste complète des fonctionnalités clés et des mises à jour de version, consultez [cette section](../../v8/rn/whats-new.md).

### Améliorations apportées à Campaign v8 {#ac-enhancements}

Les améliorations clés apportées à Adobe Campaign v8 sont répertoriées ci-dessous.

* **Interface utilisateur web**

  Adobe Campaign v8 propose une console cliente et une interface utilisateur web, qui répond à différents besoins et préférences de l&#39;utilisateur. La console cliente offre une puissante expérience de l’application de bureau, tandis que l’interface utilisateur web est conçue pour être intuitive et accessible, ce qui en fait un choix idéal pour les spécialistes du marketing familiarisés avec Adobe Campaign Standard.

  L’interface utilisateur web partage de nombreuses similitudes avec Adobe Campaign Standard, bien que certaines terminologies puissent différer.

  Vous pouvez [en savoir plus sur l’interface utilisateur web d’Adobe Campaign ici](../../v8/campaign-web-home.md).

  ![](assets/home.png){zoomable="yes"}

  Toutes les nouvelles fonctionnalités et améliorations sont répertoriées dans les [notes de mise à jour](../../v8/rn/release-notes.md). Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.


* **Performance**

  Adobe Campaign v8 tire parti des technologies de base de données avancées à l’échelle du cloud, ce qui se traduit par une amélioration significative des performances et de l’efficacité. Cette architecture repensée offre plusieurs avantages clés :

   * *Échelle* : le système prend désormais en charge une augmentation substantielle des fonctionnalités de traitement, avec un débit de traitement par lot pouvant atteindre **20 millions d&#39;opérations par heure**. Avec cette nouvelle architecture, il est possible de gérer des profils encore plus élevés avec des performances prévisibles.
   * *Vitesse* : le système a été amélioré pour toute activité marketing : segmentation, préparation de diffusion ou débit pour les messages transactionnels qui est désormais **1 million par heure**.

  Les services cloud entièrement gérés fournissent aux utilisateurs les éléments suivants :

   * Exploration des données en temps réel : accédez instantanément aux données et analysez-les pour obtenir des informations rapides et une prise de décision plus éclairée.

   * Création rapide d’audiences : créez facilement des audiences ciblées en quelques minutes pour une segmentation des campagnes plus efficace.

  Dans l’ensemble, l’architecture robuste d’Adobe Campaign v8 constitue une base puissante pour la gestion de campagnes marketing complexes et étendues, avec une vitesse et une efficacité accrues.

### Nouvelles fonctionnalités d’Adobe Campaign v8 {#ac-new-features}

En tant qu’utilisateur Campaign Standard passant à Adobe Campaign v8, les fonctionnalités suivantes vous sont désormais disponibles :

* **Push enrichi**

  Adobe Campaign v8 offre la possibilité d’envoyer des notifications push enrichies, qui peuvent capter l’attention des utilisateurs et les encourager à agir. Ces notifications peuvent inclure divers éléments tels que du texte, des images, des boutons, des minuteurs de comptage, des sons, etc.

  ![](../../v8/push/assets/rich_push.png){zoomable="yes"}

  Pour faciliter la création de ces notifications enrichies, Adobe Campaign v8 fournit divers modèles qui vous permettent de concevoir et de personnaliser le contenu de notifications complexes, telles que des carrousels ou des minuteurs.

  Vous pouvez personnaliser vos notifications en fonction du système du client :

   * Pour les modèles [Android](../../v8/push/rich-push.md)

   * Pour les modèles [iOs](../../v8/push/rich-push.md)

  Les notifications push sont un outil essentiel pour impliquer les utilisateurs d’applications mobiles, ce qui vous permet de les atteindre même lorsqu’ils n’utilisent pas activement votre application.

* **Adobe Experience Manager as a Cloud Service**

  Adobe Campaign v8 est parfaitement intégré à Adobe Experience Manager as a Cloud Service, ce qui vous permet de proposer à vos clients des expériences personnalisées et riches en contenu. Cette intégration native simplifie la gestion de contenu et tire parti des puissantes fonctionnalités de Adobe Experience Manager pour optimiser vos efforts marketing.

  Voici les principales fonctionnalités activées par cette intégration :

   * *Gestion des ressources* : dans Adobe Campaign v8, le concepteur d’email fournit un sélecteur pour accéder aux ressources et les gérer. Cette fonctionnalité simplifie l’intégration des éléments de Adobe Experience Manager dans votre diffusion, rendant ainsi la gestion de contenu plus efficace. [En savoir plus sur la gestion des ressources](../../v8/integrations/aem-assets.md)

     ![](../../v8/integrations/assets/assets_6.png){zoomable="yes"}

   * *Import de modèle d&#39;email* : Adobe Campaign v8 vous permet de parcourir et d&#39;importer des modèles d&#39;email depuis Adobe Experience Manager directement dans Campaign. [En savoir plus sur l’import de modèle d’email](../../v8/integrations/aem-content.md)

     ![](../../v8/integrations/assets/aem_6.png){zoomable="yes"}

  Adobe Experience Manager as a Cloud Service offre une agilité native au cloud, ce qui vous permet d’accélérer votre temps à évaluer et à vous adapter à l’évolution des besoins de l’entreprise. Cette intégration permet non seulement d’améliorer vos fonctionnalités de gestion de contenu, mais également de proposer à vos clients des expériences plus personnalisées et plus attrayantes sur tous les points de contact.

* **Assistant IA - Accélérateur de contenu**

  L’assistant de Campaign AI rend la création et l’exécution de campagnes marketing sur différents canaux tels que Email, SMS et Push intuitifs, simples et faciles tout en gagnant du temps, en améliorant l’efficacité et en obtenant de meilleurs résultats.

  ![](../../v8/email/assets/full-email-1.png){zoomable="yes"}

  L’assistant d’IA révolutionne la manière dont vous créez du contenu professionnel et cohérent sur le plan de la marque sur plusieurs canaux. Grâce aux modèles avancés de GenAI et à une compréhension approfondie des directives de votre marque, l’assistant d’IA génère automatiquement du contenu personnalisé, attrayant et efficace en fonction de l’objectif marketing, avec un contenu optimisé pour les styles, les mises en page, le ton et bien plus encore.

  L’assistant d’IA rend la création et l’exécution de campagnes marketing intuitives, simples et faciles tout en gagnant du temps, en améliorant l’efficacité et en obtenant de meilleurs résultats.

  ![](../../v8/email/assets/full-email-2.png){zoomable="yes"}

  Il fournit une variante de modèles d&#39;email et génère et regénère des images. En savoir plus sur l’assistant d’IA - Accélérateur de contenu dans [cette section](../../v8/email/generative-content.md). Adobe Campaign v8 a un assistant d&#39;IA disponible pour [Email](../../v8/email/generative-content.md), [SMS](../../v8/email/generative-sms.md) et [Push](../../v8/email/generative-push.md).

* **Infrastructure SMS mise à niveau - SMS v2.0**

  La simplicité et la facilité d&#39;utilisation des SMS en font un canal de communication très précieux en plus de sa robustesse et de sa compatibilité inégalée sur des milliards de terminaux.

  Adobe Campaign v8 est livré avec une nouvelle infrastructure qui améliore l&#39;envoi de SMS. [En savoir plus sur les nouveaux paramètres SMS](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.

* **Infrastructure push mise à niveau**

  Adobe Campaign v8 propose son dernier service de notification push, optimisé par un cadre robuste reposant sur une technologie de pointe. Ce service est conçu pour atteindre des niveaux d’évolutivité supérieurs, afin que vos notifications puissent atteindre une audience plus large avec une efficacité optimale. Grâce à notre infrastructure améliorée et à nos processus optimisés, vous bénéficierez d’une plus grande échelle et d’une meilleure fiabilité. Vous pourrez ainsi communiquer avec vos utilisateurs et utilisatrices d’applications mobiles comme jamais auparavant.

  [En savoir plus sur l’infrastructure push mise à niveau](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.


## Managed Services {#ac-managed-services}

Adobe Campaign v8 est disponible en tant que Managed Cloud Service, offrant une supervision proactive, des alertes rapides et une gouvernance des services. Adobe Managed Cloud Service offre aux spécialistes marketing une solution de gestion de campagnes cross-canal plus agile, sécurisée et évolutive, avec un coût total de possession faible. La nouvelle offre associe des services à une supervision proactive et à des alertes opportunes.

## Fonctionnalités de Campaign Standard ajoutées à la v8 {#ac-v8-added}

Pour que vous puissiez passer facilement à Campaign v8, les fonctionnalités clés de Campaign Standard ont été ajoutées à Campaign v8. Elles sont présentées dans [cette documentation](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr){target="_blank"}.

* **Rapports dynamiques** : les rapports dynamiques fournissent des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, telles que le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=fr){target="_blank"}.

* **Branding centralisé** : chaque entreprise dispose de ses directives visuelles et techniques en ce qui concerne le branding. Avec Adobe Campaign, vous pouvez définir un ensemble de spécifications pour présenter à vos clientes et clients une marque cohérente, des logos aux aspects techniques, tels que l’identifiant expéditeur des e-mails, l’URL ou les domaines. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=fr)

* **API REST** : en tant qu’utilisateur ou utilisatrice ayant migré à partir de Campaign Standard, vous pouvez utiliser les API REST pour créer des intégrations pour Adobe Campaign et pour créer votre propre réseau en connectant Adobe Campaign avec les technologies que vous utilisez. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=fr){target="_blank"}.

* **Pages de destination** : certaines améliorations ont été apportées aux pages de destination de Campaign v8 pour garantir la parité des fonctionnalités avec Campaign Standard. En savoir plus dans la section [notes de mise à jour](../../v8/rn/release-notes.md#new-24-4) et dans la [documentation](../../v8/landing-pages/get-started-lp.md) des pages de destination.

* **Fragments visuels** : les fragments visuels sont des composants visuels réutilisables qui peuvent être référencés dans une ou plusieurs diffusions par e-mail ou dans des modèles de contenu. Lors de la modification d’un fragment, chaque contenu qui l’utilise est mis à jour. Cette fonctionnalité permet de précréer plusieurs blocs de contenu personnalisés destinés aux utilisateurs et utilisatrices marketing et permettant d’assembler rapidement les contenus de messages dans un processus de conception amélioré. [En savoir plus](../../v8//content/use-visual-fragments.md)

## Principales différences entre Campaign Standard et Campaign v8 {#experiences}

La plupart des concepts sont similaires entre Adobe Campaign v8 et Adobe Campaign Standard. Cependant, il existe quelques différences comme décrit ci-dessous.

### Changements de terminologie {#terminology-changes}

Vous trouverez ci-dessous quelques différences terminologiques entre Campaign Standard et Campaign v8.

* Les ressources personnalisées sont appelées **schémas**.
* Les messages sont appelés **diffusions**.
* Les utilisateurs et les utilisatrices des produits sont les **opérateurs et opératrices**.
* Les rôles sont configurés avec les **droits nommés**.
* Les groupes de sécurité sont les **groupes d’opérateurs et d’opératrices**.
* Les entités organisationnelles sont gérées au moyen des **autorisations de dossier**.

En outre, en tant qu’utilisateur Campaign existant, notez que certains concepts ont été renommés pour s’aligner sur les dernières normes terminologiques. Ces modifications concernent uniquement l’interface utilisateur web de Campaign et ne sont pas répercutées dans la console cliente. Elles sont résumées ci-dessous.

* Les personnes destinataires sont désormais des **Profils**. [En savoir plus](../../v8/audience/gs-audiences-recipients.md).
* Les adresses de contrôle sont désormais des **Profils de test**. [En savoir plus](../../v8/preview-test/test-deliveries.md).
* L’analyse de la diffusion s’appelle désormais **préparation de la diffusion**. Lorsque vous devez lancer la préparation des messages, cliquez sur le bouton **Préparer**. [En savoir plus](../../v8/monitor/prepare-send.md)
* L’aperçu de l’e-mail est désormais disponible via le bouton **Simuler le contenu.** [En savoir plus](../../v8/preview-test/preview-test.md).
* Les listes s’appellent désormais **Audiences**. [En savoir plus](../../v8/audience/gs-audiences-recipients.md).

## Nouvelle expérience utilisateur

Accès au guide de référence approprié pour votre rôle pour découvrir la nouvelle expérience utilisateur avec Adobe Campaign v8.

<table>
<tr>
  <td>
    <a href="marketers.md">
      <img alt="Personne gestionnaire de campagnes"src="./assets/digital_marketing.jpeg"/>
    </a>
    <div>
  </td>
  <td>
  <a href="admin-developers.md">
    <img alt="Administrateur ou administratrice ou développeur ou développeuse" src="./assets/admin.jpeg"/>
    </a>
    <div>
  </td>
  </tr>
  <tr>
    <td>
    <a href="marketers.md">
    <strong>Personne spécialiste du marketing</strong>
    </a>
    </td>
    <td>
      <a href="admin-developers.md">
      <strong>Administrateur ou administratrice ou développeur ou développeuse</strong>
      </a>
    </td>
  </tr>
    <td>
    <em>Personne gestionnaire de campagnes, personne spécialiste du marketing multimédia</em>
    </td>
    <td>
      <em>Administrateur ou administratrice système, personne spécialiste du marketing technique</em>
    </td>
  <tr>
    <td>
    <b>Les tâches/responsabilités clés sont les suivantes :</b>
    </td>
      <td>
    <b>Les tâches/responsabilités clés sont les suivantes :</b>
    </td>
  </tr>
  <tr>
    <td>
      <li>Création de campagnes marketing
      <li>Concevoir des workflows
      <li>Tester et exécuter les campagnes
      <li>Déployer les campagnes multicanal
      <li>Optimiser les campagnes
      <li>Optimiser les campagnes automatisées
    </td>
    <td>
        <li>Gestion des accès
        <li>Configuration du système
        <li>Personnalisation du système
    </td>
</tr>
</table>
</div>

<!--
## Deprecated items

Adobe constantly evaluates product capabilities to identify older features that should be replaced with more modern alternatives to improve overall customer value, always under careful consideration of backward compatibility.

Please refer to [this documentation for information on deprecated items](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features).-->

