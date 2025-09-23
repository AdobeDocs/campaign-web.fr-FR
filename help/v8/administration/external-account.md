---
title: Gérer un compte externe
description: Découvrir comment configurer des comptes externes
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 97%

---

# Comptes externes spécifiques à Campaign {#external-account}

Suivez les étapes ci-dessous pour configurer les paramètres du compte en fonction du type de compte externe que vous avez sélectionné.

## E-mails rejetés (POP3) {#bounce}

Le compte externe « E-mails rejetés » spécifie le compte POP3 externe utilisé pour se connecter au service de messagerie. Tous les serveurs configurés pour l’accès POP3 peuvent recevoir les retours d’e-mails.

![Capture d’écran montrant les champs de configuration du compte externe E-mails rejetés (POP3).](assets/external_account_bounce.png)

Pour configurer le compte externe **[!UICONTROL E-mails rejetés (POP3)]**, renseignez les champs suivants :

* **[!UICONTROL Serveur]** - URL du serveur POP3.

* **[!UICONTROL Port]** : numéro de port de la connexion POP3 (port par défaut : 110)

* **[!UICONTROL Compte]** : nom de l’utilisateur ou de l’utilisatrice

* **[!UICONTROL Mot de passe]** : mot de passe du compte d’utilisateur.

* **[!UICONTROL Chiffrement]** : type de chiffrement, choisi parmi ce qui suit :
   * Par défaut (POP3 si port 110, POP3S si port 995).
   * POP3 qui bascule en SSL après envoi d’un STARTTLS.
   * POP3 non sécurisé (port 110 par défaut).
   * POP3 securisé au dessus de SSL (port 995 par défaut).

* **[!UICONTROL Fonction]** : sélectionnez **[!UICONTROL E-mail entrant]** pour configurer le compte de réception des e-mails entrants ou **[!UICONTROL routeur SOAP]** pour gérer les requêtes SOAP.

>[!IMPORTANT]
>
>Avant de configurer votre compte externe POP3 à l’aide de Microsoft OAuth 2.0, vous devez enregistrer votre application sur le portail Azure. Pour plus d’informations, consultez [cette page](https://learn.microsoft.com/fr-fr/entra/identity-platform/quickstart-register-app){target=_blank}.

Pour configurer un environnement externe POP3 à l’aide de Microsoft OAuth 2.0, cochez la case Microsoft OAuth 2.0 et renseignez les champs suivants :

* **[!UICONTROL Locataire Azure]**

  L’ID Azure (ou ID de répertoire, ou de locataire) se trouve dans le menu déroulant Essentiels de la vue d’ensemble de votre application dans le portail Azure.

* **[!UICONTROL Identifiant client Azure]**

  L’ID client (ou ID d’application, ou de client) se trouve dans le menu déroulant Essentiels de la vue d’ensemble de votre application dans le portail Azure.

* **[!UICONTROL Secret client Azure]**

  L’ID de secret client se trouve dans la variable Secrets clients du menu Certificats et secrets de votre application dans le portail Azure.

* **[!UICONTROL URL de redirection Azure]**

  L’URL de redirection se trouve dans le menu Authentification de votre application dans le portail Azure. Elle doit se terminer par la syntaxe suivante : nl/jsp/oauth.jsp, par exemple `https://redirect.adobe.net/nl/jsp/oauth.jsp`.

Un accès Internet est nécessaire pour la configuration et pour utiliser le bouton Tester la connexion dans la console cliente. Après la configuration, le processus inMail peut communiquer avec les serveurs Microsoft sans Internet.

Après avoir saisi les différentes informations d’identification, vous pouvez cliquer sur Configurer la connexion pour terminer la configuration de votre compte externe.

## Routage {#routing}

Pour configurer un compte externe spécifique pour les diffusions externes, procédez comme suit.

1. Créez un compte externe. [En savoir plus](create-external-account.md)

1. Sélectionnez le type **[!UICONTROL Routage]**.

   ![Capture d’écran montrant la sélection du type de compte externe Routage.](assets/external-account-routing.png){zoomable="yes"}

1. Sélectionnez le canal souhaité et cliquez sur **[!UICONTROL Créer]** :

1. Dans la section **[!UICONTROL Détails]** du compte externe, **[!UICONTROL Externe]** est sélectionné par défaut en tant que **[!UICONTROL Mode de diffusion]**.

   ![Capture d’écran montrant la configuration du mode de diffusion pour le routage des comptes externes.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Actuellement, **[!UICONTROL Externe]** est le seul mode disponible.

1. Pour gérer le processus après l’exécution de la diffusion, externalisez-le dans un workflow de post-traitement. Créez un workflow avec une activité [Signal externe](../workflows/activities/external-signal.md) et sélectionnez-le dans le champ **[!UICONTROL Post-traitement]**.

   ![Capture d’écran montrant la configuration des champs de post-traitement pour le routage des comptes externes.](assets/external-account-post-processing.png){zoomable="yes"}

1. Dans le champ **[!UICONTROL Activité]**, modifiez le nom de l’activité de workflow de post-traitement qui sera affiché dans les logs. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## Instance d’exécution {#instance-exec}

Dans le cas d’une architecture segmentée, identifiez les instances d’exécution associées à l’instance de pilotage et établissez des connexions entre elles. Les modèles de messages transactionnels sont déployés sur l’instance d’exécution.

![Capture d&#39;écran montrant les champs de configuration du compte externe de l&#39;instance d&#39;exécution.](assets/external_account_exec.png)

Pour configurer le compte externe d’**[!UICONTROL Instance d’exécution]** :

* **[!UICONTROL URL]** : URL du serveur sur lequel l’instance d’exécution est installée.

* **[!UICONTROL Compte]** : nom du compte correspondant à l’Agent Message Center tel qu’il a été défini dans le dossier de l’opérateur.

* **[!UICONTROL Mot de passe]** : mot de passe du compte tel qu&#39;il a été défini dans le dossier de l&#39;opérateur.

* **[!UICONTROL Méthode]** : choisissez entre Service web ou Federated Data Access (FDA).

  Sélectionnez votre compte FDA. Notez que la connexion de la campagne aux systèmes externes est réservée à une utilisation avancée et n’est disponible qu’à partir de la console cliente. [En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Créer un workflow d’archivage]** : pour chaque instance d’exécution enregistrée dans Message Center, qu’une ou plusieurs instances soient présentes, vous devez créer un workflow d’archivage distinct pour chaque compte externe associé à l’instance d’exécution.
