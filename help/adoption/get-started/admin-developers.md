---
title: Commencer avec Adobe Campaign v8 pour les administrateurs et administratrices et les développeurs et développeuses
description: Ce tutoriel offre une vue d’ensemble des principales fonctionnalités administratives et de gestion des données de Campaign v8. Il est destiné aux administrateurs et administratrices et aux spécialistes du marketing technique qui migrent de Campaign Standard vers Campaign v8.
role: Admin, Developer
level: Beginner, Experienced
source-git-commit: a1c16a9ba5e5ca844eaf82ed3b587f4f7a0b0873
workflow-type: tm+mt
source-wordcount: '2667'
ht-degree: 16%

---


# Prise en main pour les administrateurs et les développeurs {#acs-gs-admin}

Cette page donne un aperçu des principales fonctionnalités administratives et de gestion des données de Campaign v8. Il est destiné aux administrateurs et aux spécialistes du marketing technique qui passent de Campaign Standard à Campaign v8.

Le changement majeur pour vous est l’introduction de la console cliente, l’application native qui communique avec le serveur applicatif Adobe Campaign.

La console cliente Campaign centralise toutes les fonctionnalités et tous les paramètres. Il reste synchronisé avec l’interface utilisateur Web de Campaign, assurant la cohérence entre les deux environnements.

![](assets/client_console.png){zoomable="yes"}

[En savoir plus sur l’interface utilisateur de la console cliente d’Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"} .

## Architecture de Campaign v8 {#acs-gs-admi-archi}

L&#39;architecture de Campaign est présentée dans la documentation de Campaign v8 (console). Découvrez les principes de base dans [cette page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"}.

Lien utile pour démarrer :

* Les composants Adobe Campaign et l’architecture globale sont décrits dans [cette page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"}.

* Reportez-vous à la section [Prise en main de l’architecture de Campaign](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} pour comprendre l’architecture de Campaign avant de commencer à structurer votre instance.

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* Les messages transactionnels (Message Center) sont le module Campaign v8 conçu pour gérer les messages déclenchés. Il repose sur un modèle d’architecture spécifique qui est présenté dans [cette section](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"}.

## Console cliente Campaign {#acs-gs-console}

### Installer la console cliente {#acs-gs-admin-console}

Les tâches d&#39;administration et de configuration sont effectuées dans la console cliente. La première étape consiste à configurer votre environnement.

La console cliente Campaign est une application native qui communique avec le serveur applicatif Adobe Campaign par le biais de protocoles Internet standard, tels que SOAP et HTTP. La console cliente Campaign centralise toutes les fonctionnalités et tous les paramètres et requiert une bande passante minimale, car elle repose sur un cache local. Conçue pour un déploiement facile, la console cliente Campaign peut être déployée à partir d&#39;un navigateur Internet, mise à jour automatiquement. Elle ne nécessite aucune configuration réseau spécifique, car elle ne génère que du trafic HTTP(S).

La vidéo suivante explique comment télécharger et installer la console cliente Adobe Campaign et gérer votre connexion à votre instance.

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

Pour plus d’informations, voir [Se connecter à Campaign avec la console cliente](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/new/connect){target="_blank"}.

Notez que la console cliente doit être installée dans un environnement pris en charge. En savoir plus dans la [matrice de compatibilité de Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"}.

### Découvrir l’interface de la console cliente  {#acs-gs-ui}

Découvrez l’interface utilisateur d’Adobe Campaign V8 et comment naviguer parmi les principales fonctionnalités grâce à ce tutoriel vidéo.

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

Voir [Utilisation de la console cliente](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"} pour plus d’informations.

## Administration de l’environnement {#acs-gs-admin-env}

Une fois la console cliente installée, suivez les étapes de cette documentation pour créer la connexion au serveur d’applications : [Connexion à la documentation du serveur d’applications](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}.

Les pratiques de sécurité sont profondément enracinées dans nos processus internes de développement logiciel et d’exploitation et nos outils, et sont rigoureusement suivies par nos équipes interfonctionnelles afin de prévenir, de détecter et de réagir rapidement aux incidents. En savoir plus dans [Bonnes pratiques de sécurité de Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security){target="_blank"}.

### Droits d’accès et autorisations {#acs-gs-admin-rights}

Adobe Campaign vous permet de définir et gérer les droits attribués aux utilisateurs. Ces autorisations sont définies en combinant les autorisations des groupes d’opérateurs, les droits nommés et les autorisations sur les dossiers.

En tant qu’utilisateur Campaign Standard passant à Campaign v8, vos autorisations et droits d’accès restent les mêmes. Les groupes de sécurité ont été déplacés par Adobe vers les groupes d&#39;opérateurs de Campaign v8, et vos permissions par entité organisationnelle ont été transférées vers les permissions de dossier. Utilisateurs de Campaign   utilisez leur Adobe ID pour vous connecter à Campaign v8, puis utilisez les mêmes identifiant et mot de passe que dans Campaign Standard.

Les [dossiers](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"} de Campaign sont des noeuds dans l’arborescence de l’explorateur de la console cliente. Selon leur type, ils contiennent certains types de données. Les programmes sont matérialisés par des dossiers dans Campaign v8. Vous pouvez créer des dossiers et gérer les autorisations leur permettant de restreindre l’accès. [En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Pour en savoir plus, consultez la [documentation sur les autorisations d’utilisateur](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.


### Panneau de contrôle Campaign {#acs-gs-admin-cp}

En ce qui concerne Campaign Standard, vous pouvez utiliser le Panneau de Contrôle pour administrer votre environnement. Notez que pour la version 8, le Panneau de Contrôle fournit des fonctionnalités supplémentaires.

Le Panneau de contrôle Campaign accroît votre efficacité en tant qu’administrateur de produit Adobe Campaign, en vous permettant de gérer les paramètres et de suivre l’utilisation de chacune de vos instances. Dans son interface intuitive, vous pouvez facilement surveiller l&#39;utilisation des principales ressources ou effectuer certaines tâches administratives telles que l&#39;ajout d&#39;adresses IP à la liste autorisée, la surveillance de l&#39;espace de stockage SFTP, la gestion des clés, etc.

Pour en savoir plus, consultez les [tutoriels sur le panneau de contrôle](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} et la [documentation sur le panneau de contrôle](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=fr){target="_blank"}.

* **Ajouter des adresses IP** - Le Panneau de Contrôle Campaign vous permet de configurer de nouvelles connexions à vos instances en ajoutant des plages d’adresses IP à la liste autorisée. En savoir plus dans la [documentation sur les listes autorisées d’adresses IP](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}

* **Configuration de sous-domaine** - Vous pouvez configurer une sous-section de votre domaine (techniquement, une &quot;zone DNS&quot;) à utiliser avec Adobe Campaign.
Pour en savoir plus, consultez la [documentation sur la délégation de sous-domaine](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}

* **Gérer les serveurs SFTP** : dans le Panneau de Contrôle, vous pouvez interagir avec tous les serveurs SFTP qui sont connectés aux instances Campaign auxquelles vous avez accès. En savoir plus dans la [documentation sur la gestion SFTP](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}


### Journal d’audit {#acs-gs-admin-audit-trail}

Comme déjà disponible dans Campaign Standard, le Suivi peut être utilisé dans Campaign v8 pour accéder à l’historique complet des modifications apportées à votre instance.

Dans l’interface utilisateur web d’Adobe Campaign, la fonctionnalité Suivi offre aux utilisateurs une visibilité complète de toutes les modifications apportées à des entités importantes de votre instance, généralement celles qui ont un impact significatif sur le bon fonctionnement de l’instance. En savoir plus dans la [documentation du Suivi](../../v8/reporting/audit-trail.md)

### Packages de données {#acs-gs-admin-audit-packages}

Tout comme dans Campaign Standard, les administrateurs peuvent définir des packages pour exchange des ressources entre différentes instances Adobe Campaign par le biais de fichiers XML structurés. Il peut s’agir de paramètres de configuration ou de données.

Vous pouvez utiliser des packages de données pour exporter et importer les données et paramètres personnalisés de votre plateforme. Un package peut contenir différents types de configurations et de composants, filtrés ou non. Découvrez comment utiliser les packages de données dans Campaign v8 dans [cette documentation](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/developer/packages){target="_blank"}.

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### Personnalisation de l’interface utilisateur {#acs-gs-admin-ui}

Plusieurs options permettent de personnaliser l’interface utilisateur dans la console cliente, telles que :

* **Affichage de liste et de données** - Des instructions pour gérer les paramètres de l’interface utilisateur tels que les listes, les unités ou l’affichage des données sont disponibles dans ce document : [Documentation sur les paramètres de l’interface utilisateur](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **Gestion des dossiers** - Les dossiers sont des objets dans Adobe Campaign qui vous permettent d’organiser vos composants et vos données. Ils sont également utilisés pour gérer les autorisations. Découvrez comment [travailler avec des dossiers](../../v8/get-started/work-with-folders.md).

* **Champs personnalisés** - Les champs personnalisés sont des attributs supplémentaires ajoutés aux schémas d’usine par le biais de la console Adobe Campaign. Ces champs personnalisés sont affichés dans divers écrans, par exemple les détails d&#39;un profil ou d&#39;un profil de test. Pour en savoir plus, consultez la [documentation sur la configuration des champs personnalisés](../../v8/administration/custom-fields.md).

## Configuration de la valorisation de marque {#acs-gs-admin-branding}

Chaque entreprise dispose de directives de marque qui définissent à la fois des éléments visuels et des détails techniques. En ce qui concerne Adobe Campaign Standard, Adobe Campaign v8 vous aide à gérer ces directives de manière centralisée, afin que vous puissiez présenter une image de marque cohérente à vos clients dans tous vos projets, depuis les logos contenus dans les emails jusqu’aux URL et domaines utilisés dans vos campagnes. En tant qu’administrateur technique, vous pouvez créer et gérer plusieurs marques dans Adobe Campaign.

En savoir plus dans la [documentation sur la marque](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}

## Présentation de la création d’un modèle de données {#acs-gs-admin-data-model-creation}

Comme Campaign Standard, Adobe Campaign v8 est fourni avec son modèle de données prédéfini. Adobe Campaign repose sur une base de données Cloud contenant des tables liées entre elles. Pour en savoir plus, consultez la [documentation du modèle de données](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}.

Un schéma est un document XML associé à une table de la base de données, il définit la structuration des données et décrit la définition SQL de la table. Voir la [documentation sur la création de schémas](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

Découvrez comment créer un schéma et comment étendre un schéma existant dans Campaign v8 dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

Tout comme les fonctionnalités disponibles dans Campaign Standard, vous pouvez créer des ressources personnalisées. Dans Campaign v8, les ressources personnalisées sont des **schémas** personnalisés ou étendus.

* Découvrez comment utiliser le schéma dans [cette page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

* Découvrez comment étendre un schéma existant dans [cette page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"}.

* Découvrez comment créer un nouveau schéma dans [cette page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"}.

* Lorsque vous créez ou étendez un schéma, vous devez créer ou modifier les formulaires de saisie associés afin que ces modifications soient visibles par les utilisateurs finaux. Un formulaire de saisie vous permet de modifier une instance associée à un schéma de données à partir de la console client Adobe Campaign. Le formulaire est identifié par son nom et son espace de noms. Voir la [documentation sur la création de formulaires d’entrée](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}.

## Workflows et gestion des données {#acs-gs-admin-data-management}

Comme avec Adobe Campaign Standard, Adobe Campaign v8 inclut un module de workflow qui vous permet d’orchestrer l’ensemble des processus et tâches dans les différents modules du serveur applicatif. Cet environnement graphique complet permet de concevoir des processus englobant segmentation, exécution de campagnes, traitement de fichiers, participation humaine, etc. Le moteur de workflow exécute et suit ces processus. Découvrez comment commencer avec des workflows dans Campaign v8 dans [cette documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"}.

Voir les liens vers d’autres ressources utiles ci-dessous :

* Découvrez les dimensions de ciblage et les tables de travail, ainsi que la manière dont Adobe Campaign gère les données entre différentes sources de données dans cette vidéo :

  >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* Campaign vous aide à ajouter des contacts à la base de données cloud. Vous pouvez charger un fichier, planifier et automatiser plusieurs mises à jour de contact, collecter des données sur le Web ou saisir des informations de profil directement dans la table des destinataires.  Pour en savoir plus, consultez la [documentation sur l&#39;import de données (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"}.

* Vous pouvez facilement exporter vos différents rapports au format PDF ou CSV, ce qui vous permet de les partager, de les manipuler ou de les imprimer. Pour en savoir plus, consultez la [documentation sur l&#39;export de données](../../v8/reporting/export-reports.md).

## API REST {#acs-gs-admin-apis}

Les API REST de Campaign ont pour but de vous permettre de créer des intégrations pour Adobe Campaign et de construire votre propre écosystème en interfaçant Adobe Campaign avec le panneau des technologies que vous utilisez.

En tant qu’utilisateur Campaign Standard passant à Campaign v8, les API REST sont à votre disposition.

Pour en savoir plus, consultez la [documentation sur l’API REST](https://experienceleague.adobe.com/fr/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"}.

Notez que certaines recommandations et limites s’appliquent aux API REST lors de la transition de Campaign Standard vers Campaign v8. Ils sont répertoriés dans [cette page](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"}. Des restrictions spécifiques s’appliquent également lors de la transition vers Campaign v8, comme indiqué dans la note de disponibilité ci-dessous :

>[!AVAILABILITY]
>
>* Les valeurs PKEY changent entre l’instance de Campaign Standard existante et l’instance Campaign v8 migrée. Si les PKEY sont stockés dans une base de données externe, l’implémentation doit changer de manière à ce qu’ils doivent appeler les API principales d’Adobe Campaign v8 qui fournissent des liens pkeys/hrefs avec les PKEY et les appels API suivants doivent être formés dynamiquement en utilisant les pkeys/hrefs des appels API précédents &#x200B;
>
>* Dans Campaign v8, pour le même corps où véhicule lié au profil, &#x200B; nous obtiendrions une propriété firstName d’erreur non valide pour `cusVehicle`, mais un corps de requête avec uniquement les attributs sans lien fonctionne correctement. `{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* Le fuseau horaire est présenté à l&#39;utilisateur dans le cadre de l&#39;appel de l&#39;API REST `profileAndServicesExt/profile` et non de l&#39;appel de l&#39;API REST `profileAndServices/profile`, car il est ajouté à un schéma étendu dans le cadre de la migration des données. &#x200B;
>
>* `ccpaOptOut` est présenté uniquement à l’utilisateur dans le cadre de l’appel de l’API REST `profileAndServicesExt/profile` et non de l’appel de l’API REST `profileAndServices/profile`, car il est ajouté à un schéma étendu dans le cadre de la migration des données.
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## Services d’abonnement {#acs-gs-admin-sub}

Comme dans Campaign Standard, en tant qu’administrateur, vous pouvez créer des services d’abonnement et les marketeurs peuvent envoyer des messages à leurs abonnés. Les concepts clés et les étapes de mise en oeuvre sont harmonisés avec Campaign Standard. Vous trouverez ci-dessous des liens et des vidéos utiles.

Découvrez comment configurer et gérer les abonnements et cibler les abonnés.

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

* Voir la [documentation de l&#39;interface utilisateur Web](../../v8/audience/manage-subscribers.md) des services d&#39;abonnement.

* Consultez également la documentation pour définir les services d&#39;abonnements dans la console cliente dans [cette section](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"}.

## Messages et diffusions{#acs-gs-msg}

### Configuration des canaux de diffusion {#acs-gs-admin-channels}

En tant que Campaign Standard, Adobe Campaign v8 vous permet d’envoyer des campagnes cross-canal, notamment des emails, des SMS, des notifications push et des courriers, et de mesurer leur efficacité à l’aide de différents rapports dédiés. Ces messages sont conçus et envoyés par le biais de diffusions, et peuvent être personnalisés pour chaque personne destinataire. Les principales fonctionnalités comprennent le ciblage, la définition et la personnalisation des messages, l&#39;exécution des communications et les rapports opérationnels associés. Le principal point d&#39;accès fonctionnel est l&#39;assistant de diffusion. Ce point d’accès permet d’accéder à de multiples fonctionnalités proposées par Adobe Campaign.

En tant qu’administrateur, vous devez définir les configurations de canal. Pour en savoir plus, consultez les liens ci-dessous.

* **Email** - Les paramètres d&#39;email sont tous détaillés dans [cette page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"}.
* **SMS** - Découvrez comment configurer votre canal SMS dans [cette documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.
* **Notifications push** - Les étapes de configuration du canal des notifications push sont détaillées [dans cette section](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
* **Messages transactionnels** - Les étapes de configuration de [Messages transactionnels](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"} dans Campaign v8 sont détaillées [dans cette section](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings)

### Comptes externes {#acs-gs-ext-accounts}

En tant qu&#39;administrateur, vous êtes responsable de la configuration et de la maintenance des comptes externes de Campaign. Comme dans Campaign Standard, les comptes externes sont utilisés par des processus techniques tels que des workflows techniques ou des workflows de campagne.

Le processus de transition vers Campaign v8 prend en charge vos comptes externes de Campaign Standard existants : ils sont désormais disponibles dans la console cliente.

En savoir plus sur la [configuration de compte externe](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/config/configuration/external-accounts){target="_blank"}.


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### Contenu dynamique {#acs-gs-dyn-content}

Utilisez Campaign pour créer du contenu dynamique et envoyer des messages personnalisés. Vous pouvez cumuler les fonctionnalités de personnalisation afin d’améliorer vos messages et créer une expérience utilisateur personnalisée.

Avec Campaign v8, en tant qu&#39;administrateur, vous pouvez définir des blocs de contenu dynamiques et les utiliser pour personnaliser le contenu de votre diffusion email dans cette vidéo :

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

Liens utiles :

* [Prise en main de la personnalisation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [Utiliser des blocs de personnalisation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [Créer du contenu conditionnel](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [Sources de données Personalization](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### Modèles de diffusion {#acs-gs-templates}

L&#39;utilisation de modèles de diffusion est obligatoire dans Campaign v8, comme en Campaign Standard.

Pour accélérer et améliorer le processus de conception, créez des modèles de diffusion afin de réutiliser facilement du contenu et des paramètres personnalisés dans vos campagnes. Cette fonctionnalité vous permet de normaliser l’aspect créatif afin d’être plus rapide dans l’exécution et le lancement des campagnes. Découvrez comment créer des modèles de diffusion dans l’ [interface utilisateur web de Campaign](../../v8/msg/delivery-template.md). Découvrez également comment créer des modèles de diffusion dans la console cliente dans [cette section](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/create-templates){target="_blank"}.

### Règles de typologie {#acs-gs-admin-rules}

En tant qu&#39;administrateur, vous êtes responsable de la création et de la gestion des règles de typologie pour vos diffusions. Comme dans Adobe Campaign Standard, dans Campaign v8, les règles de typologie sont des règles de fonctionnement qui vous permettent d&#39;effectuer des vérifications et filtrages sur votre message avant de l&#39;envoyer.

Lors de la transition de votre environnement de Campaign Standard vers Campaign v8, vos règles de typologie sont déplacées vers Campaign v8.

Dans Campaign v8, les règles de typologie sont fournies avec une fonction d’optimisation de campagne spécifique. Ce module permet de contrôler, filtrer et contrôler l&#39;envoi des diffusions. Pour éviter les conflits entre les campagnes, Adobe Campaign peut tester différentes combinaisons en appliquant des règles de contrainte spécifiques. Cela garantit que les messages envoyés répondent aux besoins et aux attentes des clients et des stratégies de communication de l&#39;entreprise. Pour en savoir plus, consultez la [documentation sur les règles de typologie](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}.

### Gestion des quarantaines {#acs-gs-admin-quarantine}

Toutes les adresses en quarantaine et règles de mise en quarantaine ont été migrées de votre environnement de Campaign Standard vers Campaign v8. Aucune action spécifique n&#39;est nécessaire pour la gestion des quarantaines.

En tant qu&#39;administrateur, familiarisez-vous avec la gestion des quarantaines dans Campaign v8 à partir de [cette page](../../v8/audience/quarantine.md). Consultez également la documentation détaillée de la console cliente sur la gestion des quarantaines dans [cette section](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"}.


## Gestion des intégrations Adobe Campaign {#acs-gs-integrations}

Vous pouvez connecter votre instance Campaign à des solutions Adobe Experience Cloud pour combiner des fonctionnalités. Adobe Campaign s’accompagne de plusieurs connecteurs qui vous permettent de communiquer avec des applications externes, de vous connecter à des moteurs de base de données, ainsi que de partager et de synchroniser des données. Découvrez comment combiner vos solutions dans [cette documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/integration){target="_blank"}.

En tant qu&#39;utilisateur Campaign Standard migrant vers Campaign v8, les conditions suivantes s&#39;appliquent à vous :

* Si vous utilisiez ces intégrations avec Campaign Standard, vos configurations et données **Adobe Analytics** et **Audience Manager** ont été migrées par Adobe.
* Si votre environnement de Campaign Standard a été intégré à **Adobe Experience Manager**, Adobe vous recommande de passer à **Adobe Experience Manager as a Cloud Service** afin que vous puissiez utiliser cette fonctionnalité lors de la conception d’emails dans l’interface utilisateur Web de Campaign et de faciliter la gestion simplifiée du contenu et des formulaires de diffusion d’emails directement dans votre environnement Adobe Experience Manager. En savoir plus dans [cette page](../../v8/integrations/aem-content.md).
Notez que Campaign peut également être intégré à Adobe Experience Manager 6.5. Pour configurer cette intégration, reportez-vous à [cette documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}.
* Si votre environnement de Campaign Standard a été intégré à **Triggers**, vous devez configurer cette intégration dans Campaign v8, comme indiqué dans [cette page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}.
* Si votre environnement de Campaign Standard a été intégré à **Adobe Target**, vous devez configurer cette intégration dans Campaign v8 comme indiqué dans [cette page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}.

