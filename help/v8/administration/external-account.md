---
title: Gérer un compte externe
description: Découvrir comment configurer des comptes externes
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 34%

---

# Gérer des comptes externes {#external-accounts}

>[!AVAILABILITY]
>
>* Actuellement, les comptes externes ne sont disponibles que pour les e-mails bounce (POP3), le routage et l&#39;instance d&#39;exécution. D’autres types de comptes seront ajoutés ultérieurement.
>
>* Les comptes externes non pris en charge créés dans la console Adobe Campaign sont visibles dans l’interface d’utilisation web, mais ne peuvent pas être modifiés et ne sont pas accessibles.

Adobe Campaign comprend des comptes externes préconfigurés pour une intégration facile à divers systèmes. Pour vous connecter à d’autres plateformes ou personnaliser les connexions en fonction de votre workflow, créez des comptes externes à l’aide de l’interface utilisateur web. Cela garantit des transferts de données transparents.

## Créer un compte externe {#create-ext-account}

Pour créer un compte externe, procédez comme suit. Les paramètres détaillés dépendent du type de compte externe. [En savoir plus](#campaign-specific)

1. Dans le menu du volet de gauche, sélectionnez **[!UICONTROL Comptes externes]** sous **[!UICONTROL Administration]**.

1. Cliquez sur **[!UICONTROL Créer un compte externe]**.

   ![Capture d’écran montrant l’option de création d’un compte externe dans l’interface utilisateur web.](assets/external_account_create_1.png)

1. Saisissez votre **[!UICONTROL Libellé]** et sélectionnez le **[!UICONTROL Type]** de votre compte externe.

   >[!NOTE]
   >
   >Les paramètres des types spécifiques à Campaign sont décrits dans [cette section](#campaign-specific).

   ![Capture d&#39;écran affichant les champs permettant de saisir le libellé et de sélectionner le type de compte externe.](assets/external_account_create_2.png)

1. Cliquez sur **[!UICONTROL Créer]**.

1. Dans la liste déroulante **[!UICONTROL Options supplémentaires]**, modifiez le chemin d’accès **[!UICONTROL Nom interne]** ou **[!UICONTROL Dossier]** si nécessaire.

   ![Capture d’écran montrant des options supplémentaires pour la configuration du nom interne et du chemin de dossier.](assets/external_account_create_3.png)

1. Activez l&#39;option **[!UICONTROL Exporté automatiquement dans les packages]** pour exporter automatiquement les données gérées par ce compte externe. <!--Exported where??-->

   ![Capture d’écran montrant l’option permettant d’activer l’exportation automatique dans les packages.](assets/external_account_create_exported.png)

1. Dans la section **[!UICONTROL Détails]**, configurez l’accès au compte en spécifiant les informations d’identification en fonction du type de compte externe sélectionné. [En savoir plus](#bounce)

1. Cliquez sur **[!UICONTROL Tester la connexion]** pour vérifier que votre configuration est correcte.

1. Dans le menu **[!UICONTROL Plus...]**, dupliquez ou supprimez votre compte externe.

   ![Capture d’écran affichant le menu Plus avec des options pour dupliquer ou supprimer le compte externe.](assets/external_account_create_4.png)

1. Une fois la configuration terminée, cliquez sur **[!UICONTROL Enregistrer]**.

## Comptes externes spécifiques à Campaign {#campaign-specific}

Selon le type de compte externe que vous avez sélectionné, suivez les étapes ci-dessous pour configurer les paramètres du compte.

### E-mails rejetés (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 n’est actuellement pas pris en charge.

Le compte externe « E-mails rejetés » spécifie le compte POP3 externe utilisé pour se connecter au service de messagerie. Tous les serveurs configurés pour l’accès POP3 peuvent recevoir les retours d’e-mails.

![Capture d’écran affichant les champs de configuration du compte externe E-mails bounce (POP3).](assets/external_account_bounce.png)

Pour configurer le compte externe **[!UICONTROL E-mails rejetés (POP3)]**, renseignez les champs suivants :

* **[!UICONTROL Serveur]** - URL du serveur POP3.

* **[!UICONTROL Port]** : numéro de port de la connexion POP3 (le port par défaut est 110).

* **[!UICONTROL Compte]** - Nom de l’utilisateur.

* **[!UICONTROL Mot de passe]** : mot de passe du compte d’utilisateur.

* **[!UICONTROL Chiffrement]** - Type de chiffrement choisi, notamment :
   * Par défaut (POP3 si port 110, POP3S si port 995).
   * POP3 qui bascule en SSL après envoi d&#39;un STARTTLS.
   * POP3 non sécurisé (port 110 par défaut).
   * POP3 sécurisé au-dessus de SSL (port 995 par défaut).

* **[!UICONTROL Fonction]** - Sélectionnez **[!UICONTROL E-mail entrant]** pour configurer le compte de réception des e-mails entrants ou le **[!UICONTROL routeur SOAP]** pour gérer les requêtes SOAP.

### Routage {#routing}

Pour configurer un compte externe spécifique pour les diffusions externes, procédez comme suit.

1. Créez un compte externe. [En savoir plus](../administration/external-account.md#create-ext-account)

1. Sélectionnez le type **[!UICONTROL Routage]**.

   ![Capture d’écran affichant la sélection du type de compte externe Routage.](assets/external-account-routing.png){zoomable="yes"}

1. Sélectionnez le canal souhaité et cliquez sur **[!UICONTROL Créer]** :

1. Dans la section **[!UICONTROL Détails]** du compte externe, **[!UICONTROL Externe]** est sélectionné par défaut en tant que **[!UICONTROL Mode de diffusion]**.

   ![Capture d’écran affichant la configuration du mode de diffusion pour le Routage des comptes externes.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Actuellement, le mode **[!UICONTROL Externe]** est le seul disponible.

1. Pour gérer le processus après l’exécution de la diffusion, externalisez-le dans un workflow de post-traitement. Créez un workflow avec une activité [Signal externe](../workflows/activities/external-signal.md) et sélectionnez-la dans le champ **[!UICONTROL Post-traitement]**.

   ![Capture d’écran montrant la configuration des champs de post-traitement pour le Routage des comptes externes.](assets/external-account-post-processing.png){zoomable="yes"}

1. Dans le champ **[!UICONTROL Activité]**, modifiez le nom de l’activité de workflow de post-traitement qui s’affiche dans les logs. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

### Instance d’exécution {#instance-exec}

Si vous disposez d&#39;une architecture segmentée, identifiez les instances d&#39;exécution associées à l&#39;instance de pilotage et établissez des connexions entre elles. Les modèles de messages transactionnels sont déployés sur l’instance d’exécution.

![Capture d&#39;écran affichant les champs de configuration du compte externe de l&#39;instance d&#39;exécution.](assets/external_account_exec.png)

Pour configurer le compte externe d’**[!UICONTROL Instance d’exécution]** :

* **[!UICONTROL URL]** - URL du serveur sur lequel l&#39;instance d&#39;exécution est installée.

* **[!UICONTROL Compte]** - Nom du compte correspondant à l’agent Message Center tel que défini dans le dossier de l’opérateur.

* **[!UICONTROL Mot de passe]** - Mot de passe du compte tel que défini dans le dossier de l’opérateur.

* **[!UICONTROL Méthode]** - Choisissez entre le service Web ou Federated Data Access (FDA).

  Sélectionnez votre compte FDA. Notez que la connexion de la campagne aux systèmes externes est réservée à une utilisation avancée et n’est disponible qu’à partir de la console cliente. [En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Créer un workflow d’archivage]** - Pour chaque instance d’exécution enregistrée dans Message Center, que vous disposiez d’une ou de plusieurs instances, créez un workflow d’archivage distinct pour chaque compte externe associé à l’instance d’exécution.