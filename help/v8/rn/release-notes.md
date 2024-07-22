---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5b6843e57ac4160d943aac5aca5d86a9b4fa7783
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 100%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

## Notes de mise à jour de juin {#24-6-release}

**Date de publication** : 18-19 juin 2024

Les fonctionnalités et améliorations suivantes sont disponibles pour tous les utilisateurs et utilisatrices à compter de la version de juin.

### Alertes de diffusion {#24-6-3}

La fonctionnalité Alertes de diffusion est un système de gestion des alertes qui permet à un groupe d’utilisateurs et d’utilisatrices de recevoir automatiquement des notifications contenant des informations sur l’exécution de leurs diffusions. [En savoir plus](../msg/delivery-alerting.md)

### Plans et programmes {#24-6-4}

Vous pouvez désormais créer des plans et des programmes pour organiser vos campagnes. En définissant une hiérarchie des dossiers, vous pouvez organiser vos campagnes en programmes et vos programmes en plans. [En savoir plus](../administration/plans-programs.md)

### Améliorations {#improvements-24-6}

* **Réconciliation dans l’activité Enrichissement** : l’activité **Enrichissement** peut désormais être utilisée pour réconcilier des données du schéma de la base de données Campaign avec des données provenant d’un autre schéma, ou avec des données provenant d’un schéma temporaire tel que des données chargées à l’aide d’une activité Chargement de fichier. Par exemple, vous pouvez utiliser cette option pour réconcilier le pays d’un profil, indiqué dans un fichier chargé, avec l’un des pays disponibles dans le tableau dédié de la base de données Campaign. [En savoir plus](../workflows/activities/enrichment.md)

## Notes de mise à jour de mai {#24-5-release}

**Date de publication** : mercredi 21 mai 2024

Les fonctionnalités et améliorations suivantes sont disponibles pour tous les utilisateurs et utilisatrices à compter de la version de mai.

### Journal d’audit  {#24-5-1}

La nouvelle fonctionnalité **Journal d’audit** fournit un enregistrement détaillé et chronologique en temps réel de toutes les actions et tous les événements qui se sont produits dans votre instance Adobe Campaign. Elle offre une méthode pratique de suivi toutes les modifications apportées à vos données Campaign, en répondant à des requêtes telles que : le statut des workflows, les dernières personnes à les modifier ou les activités effectuées par les utilisateurs et utilisatrices dans l’instance. [En savoir plus](../reporting/audit-trail.md)

### Champs personnalisés {#24-5-2}

Les **Champs personnalisés** sont des attributs supplémentaires ajoutés aux schémas intégrés via la console Adobe Campaign. Dans l’interface d’utilisation de Campaign Web, ces champs personnalisés sont désormais visibles sur divers écrans, tels que les détails d’un profil ou d’un profil de test. Dans l’interface d’utilisation web, vous ne pouvez pas créer de champs personnalisés, mais vous pouvez désormais modifier leur mode d’affichage. [En savoir plus](../administration/custom-fields.md)

### Créer de liens entre les tables {#24-5-3}

Vous pouvez maintenant créer des liens avec une autre table de l’activité de workflow **Enrichissement**. Utilisez la nouvelle section **Définition du lien** dans les paramètres de l’activité afin de créer un lien entre les données de la table de travail et la base de données Adobe Campaign. Par exemple, si vous chargez les données d’un fichier contenant le numéro de compte, le pays et l’e-mail des personnes destinataires, vous pouvez maintenant créer un lien vers la table des pays afin de mettre à jour cette information dans leur profil. [En savoir plus](../workflows/activities/enrichment.md#create-links)

### Améliorations générales {#improvements-24-5}

* **Courrier** : vous pouvez désormais utiliser l’éditeur d’expression pour sélectionner les attributs à afficher dans les fichiers d’extraction de courrier. [En savoir plus](../direct-mail/content-direct-mail.md)

* **Gestion des dossiers** : vous pouvez désormais créer un sous-dossier d’un type différent de celui du dossier parent. [En savoir plus](../get-started/permissions.md#folders)

* **Harmonisation linguistique** : dans le cadre de nos efforts continus pour offrir une expérience client unifiée, nous harmonisons la terminologie utilisée dans les produits et applications Adobe Experience Cloud. Par exemple, le terme allemand « Titel » est remplacé par « Label » lorsqu’il se rapporte au nom d’un objet. Les modifications seront progressivement déployées dans l’interface d’utilisation et la documentation.


## Notes de mise à jour d’avril {#april-24-4-release}

**Date de publication** : 2 mai 2024

### Nouvelles fonctionnalités {#new-24-4}

Les fonctionnalités suivantes sont disponibles pour tous les utilisateurs et utilisatrices à compter de la version d’avril.

**Nouvelles activités de workflow**

* **Mettre à jour les données** : utilisez cette activité pour effectuer des mises à jour en masse des champs de la base de données. Plusieurs options vous permettent de personnaliser la mise à jour des données. [En savoir plus](../workflows/activities/update-data.md)
* **Services d’abonnement** : utilisez cette activité pour abonner plusieurs profils à un service ou les désinscrire d’un service en une seule action. [En savoir plus](../workflows/activities/subscription-services.md)
* **Extraire un fichier** : utilisez cette activité pour exporter des données à partir d’Adobe Campaign vers un autre système sous la forme d’un fichier externe. [En savoir plus](../workflows/activities/extract-file.md)
* **Transférer un fichier** : utilisez cette activité pour recevoir ou envoyer des fichiers, tester la présence de fichiers ou lister les fichiers présents sur un serveur. Le protocole utilisé peut être soit un protocole serveur à serveur, soit un protocole HTTP. [En savoir plus](../workflows/activities/transfer-file.md)
* **Test** : utilisez cette activité pour activer les transitions en fonction de conditions spécifiées. [En savoir plus](../workflows/activities/test.md)
* **Code JavaScript** : utilisez cette activité pour exécuter un fragment de code JavaScript dans le contexte d’un workflow. [En savoir plus](../workflows/activities/javascript-code.md)
* **Signal externe** : utilisez cette activité pour déclencher l’exécution d’un workflow à partir d’un autre workflow ou d’un appel API. [En savoir plus](../workflows/activities/external-signal.md)
* **Requête incrémentale** : utilisez cette activité pour interroger la base de données à des moments planifiés. À chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela vous permet de ne cibler que les nouveaux éléments. [En savoir plus](../workflows/activities/incremental-query.md)

**Modèles de notification push enrichies**

Vous pouvez désormais envoyer des notifications push enrichies via Android. La notification push enrichie est une forme améliorée de notification mobile qui va au-delà des messages texte simples en incorporant des éléments multimédias tels que des images, des boutons interactifs ou d’autres contenus multimédias enrichis. [En savoir plus](../push/rich-push.md)

Notez que cette fonctionnalité est en **Disponibilité limitée**.


### Nouvelles fonctionnalités en disponibilité limitée {#acs-24-4}

>[!AVAILABILITY]
>
>Les fonctionnalités suivantes sont en disponibilité limitée. Celles-ci sont limitées aux clientes et clients qui effectuent la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et elles ne peuvent pas être déployées dans un autre environnement.
>
>Consultez les pages de documentation suivantes : [Transition de Campaign Standard vers Campaign v8](../rn/acs-migration.md) et [Fonctionnalités pour les utilisateurs et les utilisatrices de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr).

* **Branding** : en tant qu’utilisateur ou utilisatrice ayant migré à partir de Campaign Standard, vos administrateurs et administratrices techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. Par exemple : le logo de la marque, le domaine d’URL d’accès aux pages de destination ainsi que les paramètres du tracking des messages. Vous pouvez créer ces marques et les associer à des messages ou à des pages de destination. Cette configuration est gérée dans des modèles. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=fr)

* **API REST** : en tant qu’utilisateur ou utilisatrice ayant effectué la migration depuis Campaign Standard, vous pouvez utiliser les API REST pour créer des intégrations pour Adobe Campaign et créer votre propre réseau en interfaçant Adobe Campaign avec le panneau de technologies que vous utilisez. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=fr)

* **Rapports dynamiques** : en tant qu’utilisateur ou utilisatrice ayant effectué la migration depuis Campaign Standard, vous pouvez accéder aux rapports dynamiques qui fournissent des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, telles que le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=fr)

* **Pages de destination** : les améliorations suivantes apportées aux pages de destination ne sont disponibles que pour les utilisateurs et utilisatrices effectuant la migration depuis Campaign Standard :

   * Vous pouvez désormais référencer une page de destination d’abonnement/de désinscription par défaut lors de la configuration d’un service. Lors de la conception d’un e-mail, si vous définissez un lien vers cette page de destination, les utilisateurs et utilisatrices qui envoient le formulaire de la page de destination sont automatiquement abonnés à ce service ou désinscrits de ce service. [En savoir plus](../audience/manage-services.md#create-service)
   * Une nouvelle option de configuration de page de destination permet aux visiteurs et visiteuses anonymes d’accéder à la page de destination. Si vous désélectionnez cette option, seuls les utilisateurs et les utilisatrices identifiés peuvent accéder au formulaire et l’envoyer. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option de configuration de page de destination permet de stocker des données internes supplémentaires lors de l’envoi de la page de destination. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option permet d’utiliser une page de destination pour plusieurs services, ce qui la rend dynamique. Lors de l’ajout d’un lien vers un e-mail, si vous sélectionnez une page de destination dynamique, vous pouvez sélectionner n’importe quel service. Si vous sélectionnez une page de destination associée à un service spécifique, ce service sera automatiquement utilisé (vous ne pouvez pas en sélectionner un autre). [En savoir plus](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Le contenu conditionnel est désormais pris en charge dans les pages de destination. [En savoir plus](../landing-pages/lp-content.md)

### Améliorations générales {#improvements-24-4}

Les améliorations ci-dessous sont disponibles pour l’ensemble des clientes et clients à compter de la version d’avril.

* L’activité **Charger un fichier** a été améliorée avec plusieurs sections qui vous permettent de charger un exemple de fichier, de gérer les erreurs et les rejets, et de supprimer les fichiers chargés une fois l’activité exécutée. [En savoir plus](../workflows/activities/load-file.md)


* Vous pouvez désormais **copier/coller des activités** d’un workflow à un autre à partir d’un autre onglet du navigateur. [En savoir plus](../workflows/orchestrate-activities.md#copy-activities-copy)

* Vous pouvez désormais gérer les **options d’exécution** de toutes les activités de workflow. Vous pouvez ainsi définir le mode d’exécution et le comportement de l’activité en cas d’erreur. [En savoir plus](../workflows/orchestrate-activities.md#execution-options-execution)

* L’option « Ne pas activer la transition si la population est vide » dans l’**Activité Partage** vous permet de choisir si le workflow doit passer à l’activité suivante lorsque le résultat du segment est vide. [En savoir plus](../workflows/activities/split.md)

## Notes de mise à jour de mars {#24-3-release}

>[!AVAILABILITY]
>
>Cette version est disponible pour l’ensemble des utilisateurs et utilisatrices à partir de la [version 8.6 de Campaign (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr). Apprenez-en davantage sur les versions et les mises à niveau de la console cliente d’Adobe Campaign dans la [documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=fr){target="_blank"}.

**Date de publication** : 19-20 mars 2024

### Canal Courrier {#24-3-dm}

Le canal **Courrier** est désormais disponible pour une utilisation dans les workflows et en tant que diffusions autonomes. Le canal Courrier est un canal hors ligne qui vous permet de créer, personnaliser et générer des fichiers d’extraction, et de les partager avec vos fournisseurs de services postaux pour envoyer du courrier à votre clientèle.

### Nouvelle activité de workflow Modifier la source de données {#24-3-change-data-source}

L’activité de ciblage **Modifier la source de données** permet de modifier la source de données de la table de travail d’un workflow. Cette activité offre davantage de flexibilité en vous permettant de gérer les données dans vos différentes bases de données et d’améliorer les performances.

### Amélioration de l’activité de workflow Partage {#24-3-split}

Vous pouvez désormais utiliser l’option **Générer tous les sous-ensembles dans le même tableau** dans l’activité de workflow **Partage** pour regrouper tous les sous-ensembles dans une seule transition de sortie.

### Concepteur de requête {#24-3-query-modeler}

* Le concepteur de requête est désormais disponible dans le concepteur d’e-mail. Cela vous permet de créer des conditions lorsque vous créez du contenu conditionnel.
* Des valeurs prédéfinies sont désormais disponibles pour les attributs de type date lors de la création d’une condition personnalisée.
* Les opérateurs ne peuvent plus être ajoutés sur une nouvelle transition du diagramme. Ils peuvent uniquement être ajoutés à une transition existante avant le filtrage des composants destiné à les regrouper.
