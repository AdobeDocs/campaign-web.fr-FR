---
title: Notes de mise à jour précédentes de l’interface d’utilisation web de Campaign v8
description: Versions de l’interface d’utilisation de Campaign Web 2024
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: ht
source-wordcount: '2532'
ht-degree: 100%

---

# Notes de mise à jour 2024 {#2024-release}

Cette page répertorie toutes les modifications et améliorations disponibles dans les **versions 2024**. Les dernières notes de mise à jour sont disponibles dans [cette page](release-notes.md).


## Version d’octobre 2024 {#24-10-release}

**Date de publication** : 29 octobre 2024

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version d’octobre.

### Fonctionnalités

<table>
<thead>
<tr>
<th><strong>Comptes externes</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais configurer et gérer des comptes externes directement via l’interface d’utilisation d’Adobe Campaign Web. Cette nouvelle fonctionnalité facilite la configuration de différents types de comptes externes, tels que les e-mails rejetés (POP3) ou les instances d’exécution.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Messages transactionnels</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les messages transactionnels (Message Center) sont désormais disponibles dans l’interface d’utilisation de Campaign Web. Ce module complémentaire est conçu pour les messages de déclenchement qui sont générés à partir d’événements déclenchés depuis des systèmes d’information et qui peuvent correspondre aux éléments suivants : facture, confirmation de commande, confirmation d’expédition, changement de mot de passe, notification d’indisponibilité d’un produit, relevé de compte, création d’un compte sur un site web, etc.</p>
<p>Pour plus d’informations, consultez la <a href="../transactional-messaging/transactional.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>


### Améliorations

* **Activités de workflows** : vous pouvez désormais déplacer une activité et tous ses nœuds enfant d’une transition vers une autre au sein d’un workflow. Un bouton **Déplacer** dédié est disponible dans le volet des propriétés de l’activité pour effectuer cette opération. [En savoir plus](../workflows/orchestrate-activities.md#move)

* **Activité d’enrichissement de workflow**

   * Vous pouvez désormais définir un Alias et un Libellé lors de la création d’un champ dans l’activité **Enrichissement**. [En savoir plus](../workflows/activities/enrichment.md#collection-settings)
   * Vous pouvez désormais ajouter des offres pour chaque profil dans l’activité **Enrichissement**. [En savoir plus](../workflows/activities/enrichment.md##add-offers)

* **Répartition des valeurs** : lorsque vous accédez à la liste des champs à personnaliser, vous pouvez désormais vérifier comment les valeurs sont distribuées pour chaque champ. Une fenêtre contextuelle dédiée indique le nombre et le pourcentage pour chaque valeur. [En savoir plus](../query/build-query.md#distribution-values-query)

* **Version et informations sur le système** : vous pouvez désormais accéder aux détails sur les versions de votre instance, à la fois pour la console cliente et l’interface d’utilisation web. Cette nouvelle section répertorie également tous les packages intégrés installés dans votre environnement. [En savoir plus](../get-started/user-interface.md#user-interface-about)

* **Listes** : vous pouvez désormais facilement réorganiser les valeurs d’une liste. [En savoir plus](../get-started/work-with-folders.md)

* **Diffusion** : les variables de diffusion sont désormais accessibles à partir des champs de personnalisation. [En savoir plus](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## Mises à jour de septembre {#9-2024}

<table>
<thead>
<tr>
<th><strong>Assistant IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Après avoir conçu et personnalisé votre message, améliorez-le avec l’assistant IA dans Adobe Campaign Web. Cet outil puissant vous permet d’optimiser l’impact de votre contenu en générant un éventail de textes attirants, de grands titres et d’images visuellement attrayantes.</p>
<p>Plongez dans une expérience pratique avec la <a href="https://experienceleague.adobe.com/fr/apps/journey-optimizer/ai-assistant-content-accelerator">prévisualisation de notre fonctionnalité en direct</a>, conçue pour explorer ses capacités en avant-première et comprendre pleinement ses possibilités.</a></p>
<p>Pour plus d’informations, consultez la <a href="../content/generative-gs.md">documentation détaillée</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Date de disponibilité : 12 septembre</p>
</td>
</tr>
</tbody>
</table>

## Version d’août {#24-8-release}

**Date de publication** : 3 septembre 2024

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version d’août.

* **Paramètres SMTP** : les paramètres SMTP sont désormais disponibles dans les paramètres de diffusion par e-mail. [En savoir plus](../advanced-settings/delivery-settings.md#smtp)

* **Variables globales**  : vous pouvez désormais définir des variables globales pour définir des valeurs pour vos diffusions. [En savoir plus](../advanced-settings/delivery-settings.md#variables-delivery)

### Nouvelles fonctionnalités en disponibilité limitée {#acs-24-8}

>[!AVAILABILITY]
>
>Les fonctionnalités suivantes sont en disponibilité limitée. Celles-ci sont limitées aux clientes et clients qui effectuent la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et elles ne peuvent pas être déployées dans un autre environnement.
>
>Consultez les pages de documentation suivantes : [Transition de Campaign Standard vers Campaign v8](../rn/acs-migration.md) et [Fonctionnalités pour les utilisateurs et les utilisatrices de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr){target="_blank"}.

* **Branding du publipostage direct** : les administrateurs et administratrices techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. Par exemple : le logo de la marque, le domaine d’URL d’accès aux pages de destination ainsi que les paramètres du tracking des messages. Vous pouvez à présent créer ces marques et les associer à des messages ou à des pages de destination. Cette configuration est gérée dans des modèles. [En savoir plus](../administration/branding/branding-assign.md)

* **Abonnements avec les pages de destination** : vous pouvez désormais lier une page de destination à un service, et envoyer un message de confirmation lorsque des utilisateurs ou utilisatrices la valident. [En savoir plus](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragments visuels** : vous pouvez désormais archiver des fragments de contenu visuel. [En savoir plus](../content/create-fragment.md#archive)

* **Captcha dans les pages de destination** : vous pouvez désormais ajouter un captcha pour protéger votre page de destination contre le spam et les abus causés par les robots. Cette action n’implique pas vos clients, car elle ne nécessite aucune interaction de leur part et repose sur les interactions avec votre site. [En savoir plus](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=fr){target="_blank"}.-->


## Notes de mise à jour de juillet {#24-7-release}

**Date de publication** : 30-31 juillet 2024

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version de juillet.

### Fragments de contenu {#24-7-1}

Vous pouvez désormais créer et utiliser des fragments de contenu. Un fragment de contenu est un composant réutilisable pouvant être référencé dans un ou plusieurs messages. Lors de la modification d’un fragment, chaque contenu qui l’utilise est mis à jour. Cette fonctionnalité permet de précréer plusieurs blocs de contenu personnalisés destinés aux utilisateurs et utilisatrices marketing et permettant d’assembler rapidement les contenus de messages dans un processus de conception amélioré.

Deux types de fragments sont disponibles :

* Les **fragments d’expression** sont des expressions prédéfinies disponibles à partir d’une entrée dédiée dans l’éditeur d’expression.
* Les **fragments visuels** sont des blocs visuels prédéfinis que vous pouvez réutiliser dans plusieurs diffusions e-mail ou dans des modèles de contenu. [En savoir plus](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >Les **fragments visuels** sont en disponibilité limitée (LA). Cette fonctionnalité est limitée aux clientes et clients qui effectuent la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et ne peut pas être déployée dans un autre environnement.

### Groupe de recouvrements {#24-7-2}

Un **groupe de recouvrements** est une liste d’adresses de contrôle. Elle est utilisée pour inclure des adresses spécifiques dans vos diffusions, puis pour cibler des profils qui ne correspondent pas aux critères de ciblage définis. Ainsi, les personnes destinataires qui ne font pas partie de l’audience de la diffusion peuvent la recevoir, comme toute autre personne destinataire cible. Vous pouvez utiliser des adresses de contrôle lors de l’envoi d’épreuves ou pour protéger votre liste de publipostage. [En savoir plus](../audience/trap-group.md)

### Modèles de notifications push enrichies {#24-7-3}

Vous pouvez désormais envoyer des notifications push enrichies. La notification push enrichie est une forme améliorée de notification mobile qui va au-delà des messages texte simples en incorporant des éléments multimédias tels que des images, des boutons interactifs ou d’autres contenus multimédias enrichis. Avec cette version, un ensemble de modèles pour les notifications push enrichies est désormais disponible pour vos applications iOS et Android.

[En savoir plus](../push/rich-push.md)

>[!AVAILABILITY]
>
>Cette fonctionnalité nécessite une mise à jour vers Campaign v8.6.3 <!--or v8.7.2-->. Pour en savoir plus, consultez les [notes de mise à jour](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/releases/release-notes){target="_blank"} de la console cliente Campaign v8.

### Améliorations {#improvements-24-7}

**Gestion des dossiers** : vous pouvez désormais gérer les autorisations et les restrictions sur les dossiers.

## Notes de mise à jour de juin {#24-6-release}

**Date de publication** : 18-19 juin 2024

Les fonctionnalités et améliorations suivantes sont disponibles pour tous les utilisateurs et utilisatrices à compter de la version de juin.


### Plans et programmes {#24-6-4}

Vous pouvez désormais créer des plans et des programmes pour organiser vos campagnes. En définissant une hiérarchie des dossiers, vous pouvez organiser vos campagnes en programmes et vos programmes en plans. [En savoir plus](../administration/plans-programs.md)

### Améliorations {#improvements-24-6}

* **Réconciliation dans l’activité Enrichissement** : l’activité **Enrichissement** peut désormais être utilisée pour réconcilier des données du schéma de la base de données Campaign avec des données provenant d’un autre schéma, ou avec des données provenant d’un schéma temporaire tel que des données chargées à l’aide d’une activité Chargement de fichier. Par exemple, vous pouvez utiliser cette option pour réconcilier le pays d’un profil, indiqué dans un fichier chargé, avec l’un des pays disponibles dans le tableau dédié de la base de données Campaign. [En savoir plus](../workflows/activities/enrichment.md)


### Nouvelle fonctionnalité en disponibilité limitée {#acs-24-6}

>[!AVAILABILITY]
>
>La fonctionnalité suivante est en disponibilité limitée. Elle est limitée aux personnes effectuant la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et ne peut pas être déployée dans un autre environnement.

* **Alertes de diffusion**

La fonctionnalité Alertes de diffusion est un système de gestion des alertes qui permet à un groupe d’utilisateurs et d’utilisatrices de recevoir automatiquement des notifications contenant des informations sur l’exécution de leurs diffusions. [En savoir plus](../msg/delivery-alerting.md)


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

* **Branding** : en tant qu’utilisateur ou utilisatrice ayant migré à partir de Campaign Standard, vos administrateurs et administratrices techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. Par exemple : le logo de la marque, le domaine d’URL d’accès aux pages de destination ainsi que les paramètres du tracking des messages. Vous pouvez créer ces marques et les associer à des messages ou à des pages de destination. Cette configuration est gérée dans des modèles. [En savoir plus](../administration/branding/branding-gs.md)

* **API REST** : en tant qu’utilisateur ou utilisatrice ayant effectué la migration depuis Campaign Standard, vous pouvez utiliser les API REST pour créer des intégrations pour Adobe Campaign et créer votre propre réseau en interfaçant Adobe Campaign avec le panneau de technologies que vous utilisez. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=fr)

* **Rapports dynamiques** : en tant qu’utilisateur ou utilisatrice ayant effectué la migration depuis Campaign Standard, vous pouvez accéder aux rapports dynamiques qui fournissent des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, comme le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. [En savoir plus](../reporting/dynamic-reporting/get-started-reporting.md)

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
>Cette version est disponible pour l’ensemble des utilisateurs et utilisatrices à partir de la [version 8.6 de Campaign (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr-FR). Pour en savoir plus sur les versions et les mises à niveau de la console cliente d’Adobe Campaign, consultez la [documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=fr){target="_blank"}.

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