---
audience: end-user
title: Créer des messages transactionnels
description: Découvrir comment créer un message transactionnel dans l’interface d’utilisation de Campaign Web
exl-id: 74e468f5-d9c3-4470-8ff2-68648b5f396f
source-git-commit: 7185e1cbc8ce9dd325bebc20c0ac362d7067f3e9
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 100%

---

# Créer des messages transactionnels

Dans les messages transactionnels, un événement déclenche l’envoi d’un message personnalisé.
Pour activer cette fonctionnalité, vous devez créer un modèle de message pour chaque type d’événement. Ces modèles contiennent toutes les informations nécessaires à la personnalisation du message transactionnel.

## Créer un modèle de message transactionnel {#transactional-template}

Dans l’interface d’utilisation de Campaign Web, la première étape de la configuration des messages transactionnels correspond à la création du modèle ou à la création directe du message. Ceci diffère de [la configuration des messages transactionnels sur la console cliente](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/real-time/transactional).

Un modèle de message transactionnel peut être utilisé pour prévisualiser le contenu de la diffusion reçu par le profil avant d’atteindre l’audience finale. Par exemple, un administrateur ou une administratrice peut configurer les modèles, ce qui les rend prêts à l’emploi par les utilisateurs et utilisatrices marketing.

Pour créer un modèle de message transactionnel, procédez comme suit :

* Dans la section **[!UICONTROL Messages déclenchés]**, accédez à **[!UICONTROL Messages transactionnels]**. Dans l’onglet **[!UICONTROL Modèles]**, vous pouvez voir tous les modèles de diffusion des messages transactionnels. Cliquez sur le bouton **[!UICONTROL Créer un modèle de message transactionnel]** pour commencer la création de votre modèle.

  ![](assets/transactional-templates.png){zoomable="yes"}

* Dans la nouvelle page qui s’affiche, choisissez le canal de votre modèle. Dans notre exemple, nous sélectionnons le canal **[!UICONTROL E-mail]**. Vous pouvez également utiliser un autre modèle de message et le sélectionner dans la liste des modèles.

  ![](assets/transactional-template-channel.png){zoomable="yes"}

  Cliquez de nouveau sur le bouton **[!UICONTROL Créer un message transactionnel]** pour valider la création de votre modèle sur le canal sélectionné.

* Vous avez désormais accès à la configuration de votre modèle de messages transactionnels.

  ![](assets/transactional-template-configuration.png){zoomable="yes"}

### Propriétés du message transactionnel {#transactional-properties}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_properties"
>title="Propriétés des messages transactionnels"
>abstract="Renseigner ce formulaire pour configurer les propriétés des messages transactionnels"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_email_properties"
>title="Propriétés d’e-mail des messages transactionnels"
>abstract="Renseigner ce formulaire pour configurer les propriétés d’e-mail des messages transactionnels"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_sms_properties"
>title="Propriétés SMS des messages transactionnels"
>abstract="Renseigner ce formulaire pour configurer les propriétés SMS des messages transactionnels"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_push_properties"
>title="Propriétés de notification push des messages transactionnels"
>abstract="Renseigne ce formulaire pour configurer les propriétés de notification push des messages transactionnels"

La section **[!UICONTROL Propriétés]** d’un message transactionnel vous aidera à configurer les éléments suivants :

* Le **[!UICONTROL Libellé]** est le nom qui s’affiche dans la liste des messages transactionnels. Faites en sorte qu’il soit clair pour la recherche et l’utilisation ultérieure.
* Le **[!UICONTROL Nom interne]** est un nom unique qui différencie votre message des autres messages créés.
* Le **[!UICONTROL Dossier]** est l’emplacement où le modèle de message transactionnel est créé.
* Le **[!UICONTROL Dossier d’exécution]** est l’emplacement où le message est stocké après l’exécution.
* Le **[!UICONTROL Code de diffusion]** est un code qui aide à reconnaître le message pour le reporting, si nécessaire.
* **[!UICONTROL Description]**
* La **[!UICONTROL Nature]** est la nature de votre diffusion, comme indiqué dans l’énumération *deliveryNature*. [En savoir plus sur les énumérations](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/config/configuration/ui-settings#enumerations)

![](assets/template-properties.png){zoomable="yes"}

### Application mobile {#mobile-app}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_mobileapp"
>title="Application mobile de messages transactionnels"
>abstract="Dans cette section, vous pouvez sélectionner l’application dans laquelle vous souhaitez envoyer votre message."

Dans cette section, vous pouvez sélectionner l’application dans laquelle vous souhaitez envoyer votre message.

En cliquant sur l’icône de recherche, vous accédez à l’application mobile répertoriée dans votre instance Adobe Campaign.

![](assets/transactional-mobileapp.png){zoomable="yes"}

### Exemple de contexte {#context-sample}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_context"
>title="Contexte des messages transactionnels"
>abstract="L’exemple de contexte vous permet de créer un événement de test pour prévisualiser le message transactionnel reçu avec la personnalisation du profil."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_addcontext"
>title="Contexte des messages transactionnels"
>abstract="L’exemple de contexte vous permet de créer un événement de test pour prévisualiser le message transactionnel reçu avec la personnalisation du profil. "

L’exemple de contexte vous permet de créer un événement de test pour prévisualiser le message transactionnel reçu avec la personnalisation du profil.

Cette étape est facultative. Vous pouvez utiliser le modèle sans l’exemple de contexte. Notez toutefois que vous ne pourrez pas prévisualiser le contenu personnalisé.

Dans notre exemple de définition du mot de passe, l’événement envoie le prénom et le nom de la personne, ainsi qu’un lien personnalisé pour la réinitialisation du mot de passe. Le contexte peut être configuré comme illustré ci-dessous.

Le contenu du contexte dépend de la personnalisation dont vous avez besoin.

![](assets/transactional-context.png){zoomable="yes"}

### Contenu du modèle de message transactionnel {#transactional-content}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_content"
>title="Contenu des messages transactionnels"
>abstract="Découvrir comment créer le contenu des messages transactionnels"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_personalization"
>title="Personnalisation des messages transactionnels"
>abstract="Découvrir comment personnaliser le contenu des messages transactionnels"

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_event_context"
>title="Event context"
>abstract="Ce menu fournit des variables de l’événement déclencheur que vous pouvez exploiter pour personnaliser le contenu de votre message transactionnel."

Le travail sur le contenu d’un message transactionnel est comparable à la création de contenu d’une diffusion. Cliquez sur **[!UICONTROL Ouvrir le concepteur d’e-mail]** ou **[!UICONTROL Modifier le corps de l’e-mail]** et sélectionnez un contenu de modèle ou importez votre code HTML.

![](assets/template-content.png){zoomable="yes"}

Pour ajouter la personnalisation dans le contenu, cliquez sur la section où vous souhaitez l’ajouter et choisissez l’icône **[!UICONTROL Ajouter la personnalisation]**.

![](assets/template-perso.png){zoomable="yes"}

Vous aurez accès à la fenêtre **[!UICONTROL Modifier la personnalisation]**.
Pour ajouter les variables de l’événement déclencheur, cliquez sur l’icône **[!UICONTROL Contexte de l’événement]**. Vous pouvez parcourir le contexte que vous avez défini pour votre modèle ([en savoir plus sur le contexte](#context-sample)), puis cliquer sur le bouton **[!UICONTROL +]** pour insérer la variable nécessaire.

Vous pouvez voir sur l’image ci-dessous comment ajouter la personnalisation du prénom.

![](assets/template-firstname.png){zoomable="yes"}

Dans notre exemple, nous ajoutons le prénom et le nom, puis nous personnalisons le lien du bouton **[!UICONTROL Réinitialiser votre mot de passe]**.

![](assets/template-button.png){zoomable="yes"}

### Prévisualiser votre modèle

À ce stade de la création du modèle, vous pouvez prévisualiser le contenu du modèle et vérifier la personnalisation.

Pour ce faire, remplissez l’[exemple de contexte](#context-sample), puis cliquez sur le bouton **[!UICONTROL Simuler le contenu]**.

![](assets/template-preview.png){zoomable="yes"}

## Créer un message transactionnel {#transactional-message}

Vous pouvez créer un message transactionnel directement ou à l’aide d’un modèle de message transactionnel. [Découvrez comment créer un modèle de message transactionnel](#transactional-template).

Pour créer un message transactionnel, procédez comme suit :

* Dans la section **[!UICONTROL Messages déclenchés]**, accédez à **[!UICONTROL Messages transactionnels]**. Dans l’onglet **[!UICONTROL Parcourir]**, vous pouvez voir tous les messages transactionnels créés. Cliquez sur le bouton **[!UICONTROL Créer un message transactionnel]** pour commencer la création de votre message.

  ![](assets/transactional-browse.png){zoomable="yes"}

* Dans la nouvelle page affichée, choisissez le canal de votre message et le modèle à utiliser. Dans notre exemple, nous choisissons [le modèle que nous avons créé ici](#transactional-template).

  ![](assets/transactional-channel.png){zoomable="yes"}

  Cliquez de nouveau sur le bouton **[!UICONTROL Créer un message transactionnel]** pour valider la création de votre message sur le canal sélectionné.

* Vous avez désormais accès à la configuration de votre message transactionnel. Votre message hérite de la configuration du modèle. Cette page est presque identique à la page de configuration du modèle de message transactionnel, sauf qu’elle inclut également la configuration du type d’événement.

  ![](assets/transactional-configuration.png){zoomable="yes"}

  Renseignez la configuration de votre message comme pour un modèle :
   * [Propriétés des messages transactionnels](#transactional-properties)
   * [Exemple de contexte](#context-sample)
   * [Contenu du message](#transactional-content)
Et [configurez le type d’événement](#event-type) comme décrit ci-dessous.

* Après [validation de votre message transactionnel](validate-transactional.md), cliquez sur le bouton **[!UICONTROL Réviser et publier]** pour créer et publier votre message.
Les déclencheurs peuvent désormais envoyer une notification push de votre message transactionnel.

### À propos du type d’événement {#event-type}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_event"
>title="Événement des messages transactionnels"
>abstract="La configuration du type d’événement lie le message à l’événement déclencheur."

La configuration du type d’événement lie le message à l’événement déclencheur.

Dans l’interface d’utilisation de Campaign Web, vous pouvez sélectionner un type d’événement déjà créé ou le créer directement dans cette page de configuration.

![](assets/transactional-event-type.png){zoomable="yes"}

>[!CAUTION]
>
>Si vous sélectionnez un type d’événement actuellement utilisé par un autre message transactionnel, les deux messages seront déclenchés. Pour les bonnes pratiques, **il est vivement recommandé de lier UN type d’événement à UN seul message transactionnel.**

## Ajouter des offres à vos messages transactionnels {#transactional-offers}

Vous avez la possibilité d’inclure des offres dans vos messages transactionnels, ce qui vous permet de présenter des propositions pertinentes à vos utilisateurs et utilisatrices finaux, même lorsque le message est déclenché par un événement.

Cette fonctionnalité est accessible pendant la phase d’édition du contenu de votre message transactionnel. Cliquez simplement sur le bouton **[!UICONTROL Configurer les offres]** pour la configurer.

Le processus de configuration est identique à la configuration des offres pour les diffusions standard. [Découvrez comment ajouter des offres à votre message](../msg/offers.md).

![](assets/transactional-offers.png){zoomable="yes"}
