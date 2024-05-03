---
title: Dernières notes de mise à jour
description: Découvrir les nouvelles fonctionnalités de l’interface utilisateur web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f6a1ebcb5a77798f738e2a4ac0b45454d941d7c7
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 28%

---

# Notes de mise à jour {#latest-release}

<!--Last update: **March 19, 2024**-->

Les versions de l’interface utilisateur web d’Adobe Campaign fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

## Notes de mise à jour d’avril {#april-24-4-release}

**Date de publication**: 2 mai 2024

### Nouveautés {#new-24-4}

Les fonctionnalités suivantes sont disponibles pour tous les utilisateurs à compter de la version d’avril.

**Nouvelles activités de workflow**

* **Mise à jour de données** - Utilisez cette activité pour effectuer des mises à jour en masse sur les champs de la base de données. Plusieurs options permettent de personnaliser la mise à jour des données. [En savoir plus](../workflows/activities/update-data.md)
* **Services d’inscriptions** - Utilisez cette activité pour abonner ou désabonner plusieurs profils à/à un service en une seule action. [En savoir plus](../workflows/activities/subscription-services.md)
* **Extraction de fichier** - Utilisez cette activité pour exporter des données d&#39;Adobe Campaign vers un autre système sous la forme d&#39;un fichier externe. [En savoir plus](../workflows/activities/extract-file.md)
* **Transfert de fichier** - Utilisez cette activité pour recevoir ou envoyer des fichiers, tester la présence de fichiers ou lister les fichiers sur un serveur. Le protocole utilisé peut être soit un protocole serveur à serveur, soit un protocole HTTP. [En savoir plus](../workflows/activities/transfer-file.md)
* **Test** - Utilisez cette activité pour activer les transitions en fonction de conditions spécifiées. [En savoir plus](../workflows/activities/test.md)
* **Code JavaScript** - Utilisez cette activité pour exécuter un fragment de code JavaScript dans le contexte d’un workflow. [En savoir plus](../workflows/activities/javascript-code.md)
* **Signal externe** - Utilisez cette activité pour déclencher l&#39;exécution d&#39;un workflow à partir d&#39;un autre workflow, ou un appel API. [En savoir plus](../workflows/activities/external-signal.md)
* **Requête incrémentale** - Utilisez cette activité pour interroger la base de données selon un calendrier précis. A chaque nouvelle exécution de cette activité, les résultats des exécutions précédentes sont exclus. Cela vous permet de ne cibler que les nouveaux éléments. [En savoir plus](../workflows/activities/incremental-query.md)

**Modèles de notification push enrichis**

Vous pouvez désormais envoyer des notifications push enrichies via Android. La notification push enrichie est une forme améliorée de notification mobile qui va au-delà des messages texte simples en incorporant des éléments multimédias tels que des images, des boutons interactifs ou d’autres contenus multimédias enrichis. [En savoir plus](../push/rich-push.md)

Notez que cette fonctionnalité est **Disponibilité limitée** (LA).

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### Nouvelles fonctionnalités à disponibilité limitée {#acs-24-4}

>[!AVAILABILITY]
>
>Les fonctionnalités suivantes sont en disponibilité limitée (LA). Ils sont limités aux clients effectuant la migration. **de Adobe Campaign Standard à Adobe Campaign v8** et ne peuvent pas être déployés dans un autre environnement.
>
>Reportez-vous aux pages de documentation suivantes : [Transition Campaign Standard vers Campaign v8](../rn/acs-migration.md) et [Fonctionnalités pour les utilisateurs de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Marques** - En tant qu’utilisateur migré par un Campaign Standard, vos administrateurs techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. par exemple : le logo de la marque, le domaine d&#39;URL d&#39;accès aux landing pages ainsi que les paramètres du tracking des messages. Vous pouvez créer ces marques et les associer à des messages ou à des landing pages. Cette configuration est gérée dans des modèles. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **API REST** - En tant qu’utilisateur migré Campaign Standard, vous pouvez utiliser les API REST pour créer des intégrations pour Adobe Campaign et créer votre propre écosystème en interfaçant Adobe Campaign avec le panneau de technologies que vous utilisez. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Rapports dynamiques** - En tant qu’utilisateur migré Campaign Standard, vous pouvez accéder aux rapports dynamiques qui fournissent des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, telles que le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. [En savoir plus](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Pages d’entrée** - Les améliorations suivantes apportées aux landing pages ne sont disponibles que pour les utilisateurs passant du Campaign Standard :

   * Vous pouvez désormais référencer une landing page d&#39;abonnement/désabonnement par défaut lors de la configuration d&#39;un service. Lors de la conception d&#39;un email, si vous définissez un lien vers cette landing page, les utilisateurs qui envoient le formulaire de landing page sont automatiquement abonnés ou désabonnés de ce service. [En savoir plus](../audience/manage-services.md#create-service)
   * Une nouvelle option de configuration de la landing page permet aux visiteurs anonymes d&#39;accéder à la landing page. Si vous désélectionnez cette option, seuls les utilisateurs identifiés peuvent accéder au formulaire et l’envoyer. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option de configuration de page d’entrée permet de stocker des données internes supplémentaires lors de l’envoi de la page d’entrée. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option permet d&#39;utiliser une landing page pour plusieurs services, ce qui la rend dynamique. Lors de l&#39;ajout d&#39;un lien vers un email, si vous sélectionnez une landing page dynamique, vous pouvez sélectionner n&#39;importe quel service. Si vous sélectionnez une landing page associée à un service spécifique, ce service sera automatiquement utilisé (vous ne pouvez pas en sélectionner un autre). [En savoir plus](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Le contenu conditionnel est désormais pris en charge dans les landing pages. [En savoir plus](../landing-pages/lp-content.md)

### Améliorations générales {#improvements-24-4}

Les améliorations ci-dessous sont disponibles pour tous les clients à compter de la version d’avril.
<!--**Workflow - Copy/Paste into another tab**: -->

* La variable **Chargement de fichier** l&#39;activité a été améliorée avec plusieurs sections permettant de télécharger un exemple de fichier, de gérer les erreurs et rejets, et de supprimer les fichiers téléchargés une fois l&#39;activité exécutée. [En savoir plus](../workflows/activities/load-file.md)


* Vous pouvez désormais **copier/coller des activités** d’un workflow à un autre à partir d’un autre onglet du navigateur. [En savoir plus](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Toutes les activités de workflow permettent désormais de gérer leurs **options d’exécution**. Vous pouvez ainsi définir le mode d&#39;exécution et le comportement de l&#39;activité en cas d&#39;erreur. [En savoir plus](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* L&#39;option &quot;Ne pas activer la transition si la population est vide&quot; dans la variable **Activité Partage** permet de choisir si le workflow doit passer à l’activité suivante lorsque le résultat du segment est vide. [En savoir plus](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* **Champs personnalisés** sont des attributs supplémentaires ajoutés aux schémas d’usine par le biais de la console Adobe Campaign. Dans l’interface utilisateur web de Campaign, ces champs personnalisés sont désormais visibles dans divers écrans, par exemple les détails d’un profil ou d’un profil de test. Dans l’interface utilisateur web, vous ne pouvez pas créer de champs personnalisés, mais vous pouvez désormais modifier leur mode d’affichage. [En savoir plus](../administration/custom-fields.md)


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

Vous pouvez désormais utiliser la variable **Générer tous les sous-ensembles dans la même table** dans le **Partage** activité de workflow pour regrouper tous les sous-ensembles dans une seule transition de sortie.

### Concepteur de requête {#24-3-query-modeler}

* Le concepteur de requête est désormais disponible dans le concepteur d’e-mail. Il vous permet de créer des conditions lors de la création de contenu conditionnel.
* Les valeurs prédéfinies sont désormais disponibles pour les attributs de type date lors de la création d’une condition personnalisée.
* Les opérateurs ne peuvent plus être ajoutés sur une nouvelle transition du diagramme. Ils ne peuvent être ajoutés que sur une transition existante avant de filtrer les composants pour les regrouper.
