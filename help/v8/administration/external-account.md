---
title: Gérer le compte externe
description: Découvrir comment configurer des comptes externes
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 51%

---

# Gestion des comptes externes {#external-accounts}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Comptes externes"
>abstract="Vous pouvez désormais vous connecter à d’autres plateformes ou personnaliser les connexions pour qu’elles s’adaptent à votre workflow, et créer facilement des comptes externes pour répondre à vos besoins spécifiques et garantir un transfert de données fluide."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

>[!AVAILABILITY]
>
> Notez que les comptes externes ne sont actuellement disponibles que pour les e-mails bounce (POP3), le routage et l&#39;instance d&#39;exécution, avec d&#39;autres types de comptes à ajouter à l&#39;avenir.
> Les comptes externes non pris en charge créés dans la console Adobe Campaign sont visibles dans l’interface d’utilisation web, mais ne peuvent pas être modifiés et ne sont pas accessibles.

Adobe Campaign est fourni avec un ensemble de comptes externes préconfigurés pour faciliter l’intégration avec différents systèmes. Si vous devez vous connecter à d’autres plateformes ou personnaliser les connexions pour qu’elles s’adaptent à votre workflow, vous pouvez désormais facilement créer des comptes externes à l’aide de l’interface d’utilisation web pour répondre à vos besoins spécifiques et garantir des transferts de données transparents.

## Créer un compte externe {#create-ext-account}

Pour créer un compte externe, procédez comme suit : Les paramètres détaillés dépendent du type de compte externe. [En savoir plus](#campaign-specific)

1. Dans le menu du volet de gauche, sélectionnez **[!UICONTROL Comptes externes]** sous **[!UICONTROL Administration]**.

1. Cliquez sur **[!UICONTROL Créer un compte externe]**.

   ![](assets/external_account_create_1.png)

1. Saisissez votre **[!UICONTROL Libellé]** et sélectionnez le compte externe **[!UICONTROL Type]**.

   >[!NOTE]
   >
   >Les paramètres des types spécifiques à Campaign sont détaillés dans [cette section](#campaign-specific).

   ![](assets/external_account_create_2.png)

1. Cliquez sur **[!UICONTROL Créer]**.

1. Dans la liste déroulante **[!UICONTROL Options supplémentaires]**, vous pouvez modifier le chemin d’accès **[!UICONTROL Nom interne]** ou **[!UICONTROL Dossier]** si nécessaire.

   ![](assets/external_account_create_3.png)

1. Activez l&#39;option **[!UICONTROL Exporté automatiquement dans les packages]** si vous souhaitez que vos données gérées par ce compte externe soient automatiquement exportées. <!--Exported where??-->

   ![](assets/external_account_create_exported.png)

1. Dans la section **[!UICONTROL Détails]**, configurez l’accès au compte en spécifiant des informations d’identification en fonction du type de compte externe sélectionné. [En savoir plus](#bounce)

1. Cliquez sur **[!UICONTROL Tester la connexion]** pour vérifier que votre configuration est correcte.

1. Dans le menu **[!UICONTROL Plus...]** , vous pouvez dupliquer ou supprimer votre compte externe.

   ![](assets/external_account_create_4.png)

1. Une fois la configuration effectuée, cliquez sur **[!UICONTROL Enregistrer]**.

## Comptes externes spécifiques à Campaign {#campaign-specific}

Selon le type de compte externe que vous avez sélectionné, suivez les étapes ci-dessous pour configurer les paramètres du compte.

### E-mails rejetés (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 n’est actuellement pas pris en charge.

Le compte externe Mails rebonds spécifie le compte externe POP3 utilisé pour se connecter au service de messagerie. Tous les serveurs configurés pour l’accès POP3 peuvent recevoir les retours d’e-mails.

![](assets/external_account_bounce.png)

Pour configurer le compte externe **[!UICONTROL Mails rebonds (POP3)]** , renseignez les champs suivants :

* **[!UICONTROL Server]** - URL du serveur POP3

* **[!UICONTROL Port]** - Numéro de port de connexion POP3 (le port par défaut est 110)

* **[!UICONTROL Compte]** - Nom de l’utilisateur

* **[!UICONTROL Mot de passe]** - Mot de passe du compte utilisateur

* **[!UICONTROL Chiffrement]** - Type de chiffrement choisi entre :

   * Par défaut (POP3 si port 110, POP3S si port 995)
   * POP3 basculant en SSL après envoi d’un STARTTLS
   * POP3 non sécurisé (port 110 par défaut)
   * POP3 securisé au dessus de SSL (port 995 par défaut)

* **[!UICONTROL Fonction]** - E-mail entrant, lorsque le compte externe est configuré pour recevoir des e-mails entrants, ou routeur SOAP, pour traiter les demandes SOAP.

### Routage {#routing}

Pour configurer un compte externe spécifique qui sera utilisé dans vos diffusions externes, procédez comme suit.

1. Créez un compte externe. [En savoir plus](../administration/external-account.md#create-ext-account)

1. Sélectionnez le type **[!UICONTROL Routage]**.

   ![](assets/external-account-routing.png){zoomable="yes"}

1. Sélectionnez le canal de votre choix et cliquez sur **[!UICONTROL Créer]**.

1. Dans la section Compte externe **[!UICONTROL Détails]** , **[!UICONTROL Externe]** est sélectionné par défaut en tant que **[!UICONTROL Mode de diffusion]**.

   ![](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Actuellement, **[!UICONTROL externe]** est le seul mode disponible.

1. Pour gérer le processus après l’exécution de votre diffusion, vous pouvez l’externaliser dans un workflow de post-traitement. Pour ce faire, vous devez créer un workflow avec une activité [Signal externe](../workflows/activities/external-signal.md) et le sélectionner dans le champ **[!UICONTROL Post-traitement]**.

   ![](assets/external-account-post-processing.png){zoomable="yes"}

1. Dans le champ **[!UICONTROL Activité]**, vous pouvez modifier le nom de l’activité de workflow de post-traitement qui s’affichera dans les journaux. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->


### Instance d’exécution {#instance-exec}

Dans le cas d’une architecture segmentée, vous devez identifier les instances d’exécution associées à l’instance de pilotage et établir des connexions entre elles. Les modèles de messages transactionnels sont déployés sur l’instance d’exécution.

![](assets/external_account_exec.png)

Pour configurer le compte externe d’**[!UICONTROL Instance d’exécution]** :

* **[!UICONTROL URL]**

  URL du serveur sur lequel est installée l&#39;instance d&#39;exécution.

* **[!UICONTROL Compte]**

  Nom du compte qui doit correspondre à l&#39;Agent Message Center tel qu&#39;il a été défini dans le dossier de l&#39;opérateur.

* **[!UICONTROL Mot de passe]**

  Mot de passe du compte tel qu&#39;il a été défini dans le dossier de l&#39;opérateur.

* **[!UICONTROL Méthode]**

  Choisissez entre Service web ou Federated Data Access (FDA).
En cas de méthode FDA, sélectionnez votre compte FDA. Notez que la connexion de la campagne aux systèmes externes est réservée à une utilisation avancée et n’est disponible qu’à partir de la console cliente. [En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Créer un workflow d’archivage]**

  Pour chaque instance d’exécution enregistrée dans Message Center, qu’une ou plusieurs instances soient présentes, vous devez créer un workflow d’archivage distinct pour chaque compte externe associé à l’instance d’exécution.
