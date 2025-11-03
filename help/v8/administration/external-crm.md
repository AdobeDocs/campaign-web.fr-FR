---
title: Gérer un compte externe
description: Découvrez comment configurer des comptes externes CRM
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 6%

---

# Compte externe CRM {#external-crm}

Utilisez un compte externe de type CRM pour connecter Adobe Campaign à une base de données tierce.

Les paramètres de configuration de ce compte externe dépendent du moteur de base de données spécifique auquel vous vous connectez. Des instructions de configuration détaillées pour chaque base de données prise en charge sont fournies dans les sections ci-dessous.

## Microsoft Dynamics CRM

Le compte externe Microsoft Dynamics CRM vous permet de connecter votre instance Campaign à votre base de données externe Microsoft Dynamics CRM.

Dans l’interface utilisateur web d’Adobe Campaign, configurez votre compte externe Microsoft Dynamics CRM.

1. [Créez votre compte externe](external-account.md) puis sélectionnez **[!UICONTROL Base de données externe]** comme **[!UICONTROL Type]** de votre compte externe et Microsoft Dynamics CRM comme **[!UICONTROL Type de fournisseur]**.

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Microsoft Dynamics CRM]**, renseignez les champs suivants :

   ![Capture d’écran affichant les champs de configuration du compte externe Microsoft Dynamics CRM.](assets/crm-microsoft-1.png)

   +++ Pour le type OAuth de CRM : mot de passe

   * **[!UICONTROL Serveur]** : saisissez l’URL de votre serveur CRM Microsoft.

     Pour localiser votre URL de serveur CRM Microsoft, connectez-vous à votre compte CRM Microsoft Dynamics, sélectionnez Dynamics 365, puis ouvrez votre application. L’URL du serveur s’affiche dans la barre d’adresse de votre navigateur, par exemple :`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Compte]** : indiquez le compte utilisé pour se connecter à Microsoft CRM.

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte spécifié.

   * **[!UICONTROL Identifiant du client]** : saisissez l’identifiant du client sur le portail de gestion Microsoft Azure.

   * **[!UICONTROL Version du CRM]** : sélectionnez la version du CRM Dynamics 365 CRM.

   +++

   </br>

   +++ Pour le type O-Auth de CRM : certificat

   * **[!UICONTROL Serveur]** : saisissez l’URL de votre serveur CRM Microsoft.

     Pour localiser votre URL de serveur CRM Microsoft, connectez-vous à votre compte CRM Microsoft Dynamics, sélectionnez Dynamics 365, puis ouvrez votre application. L’URL du serveur s’affiche dans la barre d’adresse de votre navigateur, par exemple :`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Clé privée (encodée en Base64)]** : indiquez la clé privée encodée au format Base64.

     Pour cela, vous pouvez utiliser l&#39;aide d&#39;un encodeur Base64 ou vous servir de la ligne de commande `base64 -w0 private.key` sous Linux.

   * **[!UICONTROL Identifiant de clé personnalisée]** : saisissez l’identifiant de clé personnalisée utilisé pour votre certificat.

   * **[!UICONTROL ID de clé]** : saisissez l’ID de clé associé à votre certificat.

   * **[!UICONTROL Identifiant du client]** : renseignez l&#39;identifiant du client dans la gestion Azure Microsoft

   * **[!UICONTROL Version du CRM]** : sélectionnez la version du CRM Dynamics 365 CRM.

   +++

1. Une fois la connexion établie, accédez à l&#39;assistant de configuration **[!UICONTROL Microsoft CRM]** pour générer votre liste de tables Microsoft CRM.

   Cliquez sur **[!UICONTROL Suivant]** pour sélectionner les tables souhaitées.

   ![Capture d’écran affichant les champs de configuration du compte externe Microsoft Dynamics CRM.](assets/crm-microsoft-2.png)

1. Sélectionnez les tables CRM Microsoft à récupérer ou ajoutez une table distante en spécifiant le **[!UICONTROL libellé de la table]** et le **[!UICONTROL nom interne de la table]**, puis activez le bouton bascule **[!UICONTROL Sélectionné]**.

   Cliquez sur **[!UICONTROL Suivant]**.

1. Cliquez sur **[!UICONTROL Démarrer]** pour lancer la création du schéma CRM Microsoft à partir des tables sélectionnées.

1. Suivez les instructions à l’écran pour insérer des pages de l’historique marketing Adobe Campaign et de la gestion des abonnements directement dans Microsoft Dynamics CRM.

1. Cliquez sur **[!UICONTROL Afficher les URL de l’historique marketing]** pour afficher les URL d’intégration des pages de l’historique marketing ou **[!UICONTROL Afficher les URL des abonnements des prospects]** pour afficher les URL d’intégration des pages de gestion des abonnements.

   ![Capture d’écran affichant les champs de configuration du compte externe Microsoft Dynamics CRM.](assets/crm-microsoft-3.png)

1. Cliquez sur **[!UICONTROL Enregistrer]** une fois votre compte externe Microsoft CRM configuré.

1. Une fois votre compte externe créé, vous pouvez cliquer sur **[!UICONTROL Synchronisation des énumérations...]** pour synchroniser automatiquement les énumérations entre le CRM Microsoft et l&#39;interface utilisateur web d&#39;Adobe Campaign.

   ![Capture d’écran affichant les champs de configuration du compte externe CRM Microsoft.](assets/crm-microsoft-4.png)

1. Sélectionnez l’énumération d’Adobe Campaign correspondant à l’énumération du CRM Microsoft.

   Pour remplacer les valeurs d’Adobe Campaign par les valeurs du CRM Microsoft, activez l’option **[!UICONTROL Remplacer]**.

## Salesforce {#salesforce}

Pour configurer le compte externe Salesforce afin de l’utiliser avec Adobe Campaign, vous devez fournir les détails suivants :

1. [Créez votre compte externe](external-account.md) puis sélectionnez **[!UICONTROL Base de données externe]** en tant que **[!UICONTROL Type]** de votre compte externe et Salesforce.com en tant que **[!UICONTROL Type de fournisseur]**.

   ![Capture d’écran affichant les champs de configuration du compte externe Salesforce.](assets/crm-salesforce-1.png)

1. Cliquez sur **[!UICONTROL Créer]**.

1. Pour configurer le compte externe **[!UICONTROL Salesforce]**, renseignez les champs suivants :

   * **[!UICONTROL Type O-Auth de CRM]** : **[!UICONTROL mot de passe]** ou **[!UICONTROL informations d’identification]**

   * **[!UICONTROL Compte]** : compte utilisé pour se connecter à Salesforce CRM

   * **[!UICONTROL Mot de passe]** : saisissez le mot de passe associé au compte spécifié.

   * **[!UICONTROL Jeton de sécurité]** : renseignez le jeton de sécurité Salesforce associé au compte.

   * **[!UICONTROL Version de l’API]** : sélectionnez la version 49.

   ![Capture d’écran affichant les champs de configuration du compte externe Salesforce.](assets/crm-salesforce-2.png)

1. Ouvrez l&#39;assistant de configuration **[!UICONTROL Salesforce CRM]** pour générer la liste des tables de votre CRM Salesforce, puis cliquez sur **[!UICONTROL Suivant]**.

   ![Capture d’écran affichant les champs de configuration du compte externe Salesforce CRM.](assets/crm-salesforce-3.png)

1. Sélectionnez les tables Salesforce à récupérer ou ajoutez une table distante en saisissant le **[!UICONTROL libellé de la table]** et le **[!UICONTROL nom interne de la table]**, puis activez le bouton bascule **[!UICONTROL Sélectionné]**.

   Cliquez sur **[!UICONTROL Suivant]**.

1. Cliquez sur **[!UICONTROL Démarrer]** pour lancer la création du schéma CRM Salesforce à partir des tables sélectionnées.

1. Cliquez sur **[!UICONTROL Assistant de création de liens Salesforce...]** pour générer les liens web dans Salesforce.

   Cliquez ensuite sur **[!UICONTROL Suivant]** pour récupérer les liens web pour **Leads** et **Contacts** à partir de Salesforce.

1. Sélectionnez les liens à exporter vers la liste des liens web Salesforce .

1. Suivez les instructions à l’écran pour insérer les pages **Historique marketing** et **Gestion des abonnements** de l’interface utilisateur web d’Adobe Campaign dans Salesforce CRM.

1. Cliquez sur **[!UICONTROL Enregistrer]** une fois votre compte externe Salesforce CRM configuré.

1. Une fois votre compte externe créé, vous pouvez cliquer sur **[!UICONTROL Synchronisation des énumérations...]** pour synchroniser automatiquement les énumérations entre Salesforce et l&#39;interface utilisateur web d&#39;Adobe Campaign.

   ![Capture d’écran affichant les champs de configuration du compte externe Salesforce CRM.](assets/crm-salesforce-4.png)

1. Sélectionnez l’énumération Adobe Campaign correspondant à l’énumération Salesforce.

   Pour remplacer les valeurs d’Adobe Campaign par des valeurs de Salesforce, activez l’option **[!UICONTROL Remplacer]**.

   ![Capture d’écran affichant les champs de configuration du compte externe Salesforce CRM.](assets/crm-salesforce-5.png)

