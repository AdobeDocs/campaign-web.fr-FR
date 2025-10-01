---
title: Gérer un compte externe
description: Découvrir comment configurer des comptes externes
exl-id: 8f41312e-422f-4be1-b874-1b143c500912
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: ht
source-wordcount: '3892'
ht-degree: 100%

---

# Comptes de la base externe {#external-accounts}

Utilisez un compte externe de type base de données externe pour connecter Adobe Campaign à une base de données tierce.

Les paramètres de configuration du compte externe varient en fonction du moteur de base de données auquel vous vous connectez. Vous trouverez des instructions détaillées pour chaque base de données prise en charge dans les sections ci-dessous.

## Amazon Redshift

Le compte externe Amazon Redshift permet de connecter l’instance Campaign à la base de données externe Amazon Redshift.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Amazon Redshift.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Amazon Redshift comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Amazon Redshift]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Amazon Redshift

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Redshift.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Redshift à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Schéma de travail]** : saisissez le nom du schéma dans lequel Adobe Campaign fonctionnera.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Amazon Redshift.](assets/ext-account-amazon.png)

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Redshift distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

1. Liez votre **[!UICONTROL compte de stockage]** pour optimiser les performances et permettre des processus de chargement de données plus rapides entre Adobe Campaign et Amazon Redshift.

1. Saisissez votre **[!UICONTROL rôle de compte]** qui détermine les autorisations qu’Adobe Campaign utilisera lors de l’interaction avec votre environnement Redshift.

## Amazon Redshift (hérité)

Le compte externe Amazon Redshift (hérité) permet de connecter l’instance Campaign à la base de données externe Amazon Redshift.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Amazon Redshift (hérité).

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Amazon Redshift (hérité) comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Amazon Redshift (hérité)]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Amazon Redshift (hérité)

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Redshift.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Redshift à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Schéma de travail]** : saisissez le nom du schéma dans lequel Adobe Campaign fonctionnera.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Amazon Redshift (hérité).](assets/ext-account-amazon-legacy.png)

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Redshift distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## Azure Synapse Analytics

Le compte externe Azure Synapse Analytics permet de connecter l’instance Campaign à la base de données externe Azure Synapse.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Azure Synapse Analytics.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Azure Synapse Analytics comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Azure Synapse Analytics]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Azure Synapse Analytics

   * **[!UICONTROL Serveur]** : saisissez l’URL du serveur Azure Synapse.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice qui s’authentifiera avec la base de données Synapse.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte.

   * **[!UICONTROL Base de données]** : indiquez la base de données cible à laquelle Adobe Campaign doit se connecter.

   * **[!UICONTROL Préfixe des tables et fonctions]** : par défaut, il est défini sur le nom du compte. Vous pouvez le modifier si vous préférez utiliser un préfixe différent pour identifier les objets liés à Campaign.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Azure Synapse Analytics.](assets/ext-account-azure.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

   ![Copie d’écran montrant les champs de configuration du compte externe Azure Synapse Analytics.](assets/ext-account-azure-2.png)

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Azure Synapse Analytics distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## Databricks

Le compte externe Databricks permet de connecter l’instance Campaign à la base de données externe Databricks.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Databricks.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Databricks comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Databricks]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Databricks

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Databricks.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Databricks à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Catalogue]** : indiquez le catalogue à utiliser.

   * **[!UICONTROL Schéma de travail]** : renseignez le nom du schéma dans lequel Adobe Campaign va créer et gérer ses objets de travail.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   ![Copie d’écran montrant les champs de configuration du compte externe Databricks.](assets/ext-account-databricks.png)

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Databricks distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

1. Liez votre **[!UICONTROL compte de stockage]** pour optimiser les performances et permettre des processus de chargement de données plus rapides entre Adobe Campaign et Databricks.

## Google BigQuery

Le compte externe Google BigQuery permet de connecter l’instance Campaign à la base de données externe Google BigQuery.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Google BigQuery.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et BigQuery Google comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Google BigQuery]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Google BigQuery.

   * **[!UICONTROL Compte]** : saisissez le nom d’utilisateur ou d’utilisatrice ou le compte de service qu’Adobe Campaign utilisera pour se connecter à BigQuery.

   * **[!UICONTROL Méthode de chargement du fichier de connexion]** : choisissez comment fournir la clé de compte de service, soit en saisissant manuellement le chemin d’accès au fichier de clé, soit en chargeant directement le fichier de clé sur le serveur.

   * **[!UICONTROL Serveur]** : si vous sélectionnez l’option de saisie manuelle, indiquez l’URL du serveur.

   * **[!UICONTROL Projet]** : indiquez l’ID de projet Google Cloud associé à votre instance BigQuery.

   * **[!UICONTROL Jeu de données]** : saisissez le nom du jeu de données dans lequel Adobe Campaign stockera et interrogera les données.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   ![Copie d’écran montrant les champs de configuration du compte externe Google BigQuery.](assets/ext-account-google.png)

1. Sous **[!UICONTROL Paramètres]**, collez le contenu du fichier JSON de clé de compte de service pour authentifier Adobe Campaign auprès de Google BigQuery.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Google BigQuery distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

1. Si votre environnement nécessite un accès proxy pour se connecter au serveur BigQuery, configurez les paramètres du proxy.

   Commencez par sélectionner votre type de proxy : http, http_no_tunnel, socks4 ou socks5.

1. Renseignez les champs de configuration de proxy suivants pour établir un accès sécurisé :

   * **[!UICONTROL Hôte du proxy]** : adresse du serveur proxy.
   * **[!UICONTROL Port du proxy]** : port utilisé par le serveur proxy.
   * **[!UICONTROL UID du proxy]** : ID de l’utilisateur ou de l’utilisatrice pour l’authentification auprès du serveur proxy, si nécessaire.
   * **[!UICONTROL Mot de passe du proxy]** : mot de passe correspondant à l’UID du proxy (le cas échéant).

   ![Copie d’écran montrant les champs de configuration du compte externe Google BigQuery.](assets/ext-account-google-2.png)

## Microsoft SQL Server

Le compte externe Microsoft SQL Server permet de connecter l’instance Campaign à la base de données externe Microsoft SQL Server.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Microsoft SQL Server.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Microsoft SQL Server comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Microsoft SQL Server]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Microsoft SQL Server.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur SQL Microsoft Server.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Microsoft SQL Server à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Préfixe des tables et fonctions]** : par défaut, il est défini sur le nom du compte. Vous pouvez le modifier si vous préférez utiliser un préfixe différent pour identifier les objets liés à Campaign.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Microsoft SQL Server.](assets/ext-account-microsoft-sql.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Microsoft SQL Server distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## MySQL

Le compte externe MySQL permet de connecter l’instance Campaign à la base de données externe MySQL.
Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe MySQL.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et MySQL comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL MySQL]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : MySQL.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur MySQL.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice MySQL à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe MySQL.](assets/ext-account-mysql.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données MySQL distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## Netezza

Le compte externe Netezza vous permet de connecter l’instance Campaign à la base de données externe Netezza.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Netezza.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Netezza comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Netezza]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Netezza

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Netezza.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Netezza à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Netezza.](assets/ext-account-netezza.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Netezza distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## ODBC (Sybase ASE, Sybase IQ).

Le compte externe ODBC (Sybase ASE, Sybase IQ) permet de connecter l’instance Campaign à la base de données externe ODBC (Sybase ASE, Sybase IQ).
Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe ODBC (Sybase ASE, Sybase IQ).

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et ODBC (Sybase ASE, Sybase IQ) comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL ODBC (Sybase ASE, Sybase IQ)]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : ODBC (Sybase ASE, Sybase IQ)

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur ODBC (Sybase ASE, Sybase IQ).

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice ODBC (Sybase ASE, Sybase IQ) à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Outil d’insertion en masse]** : indiquez le chemin d’accès complet à l’exécutable de l’outil d’insertion en masse.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe ODBC.](assets/ext-account-odbc.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données ODBC distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## Relais HTTP vers base distante

Le compte externe Relais HTTP vers base distante permet de connecter l’instance Campaign à votre relais HTTP vers base externe distante.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Relais HTTP vers base distante.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Relais HTTP vers base distante comme **[!UICONTROL Type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Relais HTTP vers base distante]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Relais HTTP vers base distante.

   * **[!UICONTROL Serveur]** : saisissez l’URL complète du serveur relais HTTP qui se connecte à votre base de données distante.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice utilisé pour l’authentification auprès du serveur relais HTTP.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé à ce compte.

   * **[!UICONTROL Source de données]** : indiquez la base de données cible à laquelle Adobe Campaign doit se connecter via le relais.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   ![Copie d’écran montrant les champs de configuration du compte externe Relais HTTP vers base distante.](assets/ext-account-azure.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre relais HTTP distant vers la base distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## Oracle

Le compte externe Oracle permet de connecter l’instance Campaign à la base de données externe Oracle.
Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Oracle.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Oracle comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Oracle]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Oracle

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Oracle.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Oracle à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Oracle.](assets/ext-account-oracle.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Oracle distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## PostgreSQL

Le compte externe PostgreSQL permet de connecter l’instance Campaign à la base de données externe PostgreSQL.
Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe PostgreSQL.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et PostgreSQL comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL PostgreSQL]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : PostgreSQL.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur PostgreSQL.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice PostgreSQL à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Schéma de travail]** : renseignez le nom du schéma dans lequel Adobe Campaign va créer et gérer ses objets de travail.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe PostgreSQL.](assets/ext-account-postgresql.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données PostgreSQL distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## SAP HANA

Le compte externe SAP HANA permet de connecter l’instance Campaign à la base de données externe SAP HANA.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe SAP HANA.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et SAP HANA comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL SAP HANA]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : SAP HANA.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur SAP HANA.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice SAP HANA à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Schéma de travail]** : renseignez le nom du schéma dans lequel Adobe Campaign va créer et gérer ses objets de travail.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe SAP HANA.](assets/ext-account-saphana.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données SAP HANA distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## Snowflake

Le compte externe Snowflake permet de connecter l’instance Campaign à la base de données externe Snowflake.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Snowflake.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Snowflake comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Snowflake]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Snowflake.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Snowflake.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Snowflake à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Schéma de travail]** : renseignez le nom du schéma dans lequel Adobe Campaign va créer et gérer ses objets de travail.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Snowflake.](assets/ext-account-snowflake.png)

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Snowflake distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

1. Si vous utilisez l’authentification par paire de clés, dans le menu **[!UICONTROL keypair.auth]**, saisissez les valeurs requises pour :

   * **[!UICONTROL Mot de passe]** : phrase secrète protégeant la clé privée, le cas échéant.

   * **[!UICONTROL Clé privée]** : clé privée utilisée pour authentifier le compte Snowflake.

## Teradata

Le compte externe Teradata vous permet de connecter votre instance Campaign à votre base de données externe Teradata.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Teradata.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Teradata comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Teradata]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Teradata.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Teradata.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Teradata à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Teradata.](assets/ext-account-teradata.png)

1. Vous pouvez choisir d’activer l’option **[!UICONTROL Utiliser un tablespace de travail pour les tables]**, puis spécifier le **[!UICONTROL tablespace des tables]** où vos tables de travail seront stockées.

1. Si nécessaire, activez l’option **[!UICONTROL Utiliser un tablespace de travail pour les index]**, puis fournissez le **[!UICONTROL tablespace des index]**.

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Teradata distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

1. Si nécessaire, saisissez votre **[!UICONTROL script PostConnect]** si vous souhaitez qu’un script s’exécute automatiquement après l’établissement de chaque connexion. Si vous souhaitez que le script s’exécute à chaque fois, activez l’option **[!UICONTROL Exécuter à chaque fois]**.

## Vertica Analytics

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Vertica Analytics.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Vertica Analytics comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Vertica Analytics]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Vertica Analytics.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Vertica Analytics.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Vertica Analytics à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte d’utilisateur ou d’utilisatrice.

   * **[!UICONTROL Base de données]** : indiquez le nom de la base de données s’il n’est pas déjà défini dans le DSN. Laissez ce champ vide si le DSN inclut la base de données.

   * **[!UICONTROL Schéma de travail]** : renseignez le nom du schéma dans lequel Adobe Campaign va créer et gérer ses objets de travail.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   * **[!UICONTROL Fuseau horaire]** : sélectionnez ou saisissez le fuseau horaire du serveur pour garantir la précision des opérations temporelles.

   ![Copie d’écran montrant les champs de configuration du compte externe Vertica Analytics.](assets/ext-account-vertica.png)

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Vertica Analytics distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

## Microsoft Fabric {#fabric}

Le compte externe Microsoft Fabric permet de connecter l’instance Campaign à la base de données externe Microsoft Fabric.

Dans l’interface d’utilisation d’Adobe Campaign Web, configurez votre compte externe Microsoft Fabric.

1. [Créez votre compte externe](external-account.md), puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL type]** de votre compte externe et Microsoft Fabric comme **[!UICONTROL type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Microsoft Fabric]**, renseignez les champs suivants :

   * **[!UICONTROL Type]** : Microsoft Fabric.

   * **[!UICONTROL Serveur]** : saisissez le nom DNS de votre serveur Microsoft Fabric.

   * **[!UICONTROL Compte]** : indiquez le nom d’utilisateur ou d’utilisatrice Microsoft Fabric (ou le principal de service) à utiliser pour l’authentification.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe ou le secret associé au compte.

   * **[!UICONTROL Options]** : ajoutez toutes les options de configuration avancées qui peuvent être requises par votre environnement.

   ![Copie d’écran montrant les champs de configuration du compte externe Microsoft Fabric.](assets/ext-account-fabric.png)

1. Après avoir configuré la connexion, créez les fonctions SQL Adobe Campaign dans votre base de données Redshift distante. Une fois ces fonctions disponibles, cliquez sur **[!UICONTROL Déployer les fonctions]** pour les activer.

1. Liez votre **[!UICONTROL compte de stockage]** pour optimiser les performances et permettre des processus de chargement de données plus rapides entre Adobe Campaign et Microsoft Fabric.

1. Saisissez votre **[!UICONTROL rôle de compte]** qui détermine les autorisations qu’Adobe Campaign utilisera lors de l’interaction avec votre environnement Microsoft Fabric.
