---
title: Branding
description: Découvrir comment configurer votre marque
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 5c9d3db95905f77dddffaf824156c87b9d79013c
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 37%

---

# Configurer des marques {#branding-configure}

Les administrateurs techniques peuvent créer et gérer plusieurs marques directement à partir de l’interface utilisateur web. Vous pouvez ainsi définir tous les éléments qui constituent votre identité de marque, y compris les logos et même les paramètres de tracking e-mail.

>[!NOTE]
>
>Cette fonctionnalité nécessite le package de branding sur votre instance. Contactez votre représentant Adobe si le menu **Branding** ne s’affiche pas.

## Créer ou modifier une marque {#create-edit-brand}

>[!CONTEXTUALHELP]
>id="acw_branding_create"
>title="Création d’une marque"
>abstract="Cliquez sur **Créer une marque** pour définir une nouvelle identité de marque. Renseignez les détails de la marque dans les onglets de configuration, puis cliquez sur **Créer une marque** pour enregistrer. La marque peut être liée à des modèles de diffusion et à des diffusions autonomes."

Pour créer une nouvelle marque, procédez comme suit :

1. Accédez à **[!UICONTROL Administration > Image de marque]** dans le menu de gauche, ou à **[!UICONTROL Administration > Plateforme > Image de marque]** dans l’**[!UICONTROL Explorateur]**.

1. Cliquez sur le bouton **[!UICONTROL Créer une marque]** au-dessus de la liste.

   ![Capture d’écran montrant la création de la marque](assets/branding-create.png)

1. Renseignez les détails sur la marque dans les différentes sections. Chaque champ est décrit dans la section [Attributs de marque](#brand-attributes) ci-dessous.

   ![Capture d’écran affichant les champs de création de marque](assets/branding-create2.png)

1. Cliquez sur **[!UICONTROL Créer une marque]** pour enregistrer. La marque peut désormais être liée aux modèles de diffusion et aux diffusions autonomes. [Découvrez comment attribuer une marque](branding-assign.md).

Pour modifier une marque existante, sélectionnez-la dans la liste, mettez à jour les champs et enregistrez vos modifications.

## Attributs de marque {#brand-attributes}

Un **[!UICONTROL Brand]** est configuré en quatre sections : **[!UICONTROL Identité]**, **[!UICONTROL Configurations de marque]**, **[!UICONTROL Paramètres d’en-tête d’e-mail]** et **[!UICONTROL Paramètres de suivi des URL]**.

### Identité {#identity}

La section **[!UICONTROL Identité]** vous permet de définir et de personnaliser votre marque.

![Capture d’écran affichant l’onglet Identité lors de la création d’une marque](assets/branding-create3.png)

Cette section contient les champs suivants :

* **[!UICONTROL Nom de la marque]** : le nom de votre marque. Ce champ est obligatoire.
* **[!UICONTROL Libellé]** : libellé visible dans l’interface.
* **[!UICONTROL ID]** : identifiant interne généré automatiquement. Tu peux le changer. Seuls les lettres, chiffres et traits de soulignement sont autorisés. Les caractères spéciaux sont remplacés par des traits de soulignement.
* **[!UICONTROL URL du logo]** : URL de l’image du logo de la marque.
* **[!UICONTROL URL du site web]** et **[!UICONTROL libellé du site web]** : URL du site web et libellé associé à la marque.


### Configurations de la marque {#brand-configs}

Dans la section **[!UICONTROL Configurations de marque]**, vous définissez les protocoles de sous-domaine et d’URL utilisés pour le suivi et l’accès aux pages de destination.

![Capture d’écran affichant l’onglet Configurations de marque](assets/branding-create4.png)

Cette section contient les champs suivants :

* **[!UICONTROL Sous-domaine de marque]** : URL de sous-domaine spécifique à cette marque, demandée pour la délégation à partir d’Adobe.
* **[!UICONTROL Protocole d’URL de tracking]**, **[!UICONTROL Protocole d’URL de page miroir]** et **[!UICONTROL Protocole d’URL d’application]** : protocole utilisé pour chaque type d’URL (par exemple, **Sécurisé (https)**).

>[!NOTE]
>
>La configuration des serveurs de suivi, de mise en miroir et d’application est stockée dans des comptes externes distincts associés au routage. Ces paramètres sont appliqués pendant l’approvisionnement et ne doivent pas être modifiés. Pour afficher les URL, accédez à l’onglet **[!UICONTROL Préfixes de branding]** à partir de votre compte externe.

### Paramètres d&#39;en-tête des emails {#header-param}

Les **[!UICONTROL paramètres d’en-tête des e-mails]** vous permettent de personnaliser ce que les destinataires verront dans la section d’en-tête de vos campagnes.

![Capture d’écran affichant l’onglet Paramètres d’en-tête avec les champs d’en-tête des e-mails](assets/branding-create5.png)

Cette section contient les champs suivants :

* **[!UICONTROL Expéditeur (adresse e-mail)]** : adresse e-mail de la marque.
* **[!UICONTROL Expéditeur (nom)]** : le nom de la marque.
* **[!UICONTROL Adresse de réponse (adresse e-mail)]** : adresse e-mail à laquelle le client peut répondre.
* **[!UICONTROL Réponse (nom)]** : nom d’affichage des réponses.
* **[!UICONTROL Erreur (adresse e-mail)]** : adresse e-mail à utiliser en cas d’erreur.

<!--
>[!IMPORTANT]
>
>After having updated the header parameters of the emails, if the name and email address of the sender have not changed in the email created from the template, check the template's advanced settings.
-->

### Paramètres du tracking d&#39;url {#tracking-param}

Dans la section **[!UICONTROL Paramètres de tracking des URL]** , vous pouvez améliorer le tracking des URL en définissant des paramètres supplémentaires pour l’intégration aux outils de Web Analytics tels qu’Adobe Analytics et Google Analytics.

![Capture d’écran affichant les paramètres de tracking d’URL dans l’onglet Paramètres d’en-tête](assets/branding-create6.png)

Cette section contient les champs suivants :

* **[!UICONTROL Paramètres d’URL supplémentaires]** : ajoutez des paramètres en tant que paires clé-valeur, ainsi que leurs conditions d’applicabilité. Chaque nom de paramètre doit être unique et renseigné, et chaque valeur de paramètre doit être complétée. La condition d’applicabilité peut être vide, mais aucune de ces valeurs ne peut inclure de balises JST.

* **[!UICONTROL Liste autorisée de noms de domaine]** : ajoutez des noms de domaine ou des expressions régulières pour correspondre aux URL où des paramètres de suivi seront ajoutés.

**Exemple :** une URL suivie telle que `https://www.luma.com` devient `https://www.luma.com/?age=21&deliveryName=DM101` lorsque les paramètres supplémentaires `age=21` et `deliveryName=DM101` sont configurés pour ce domaine.

## Configurer le branding pour les messages transactionnels {#branding-transactional-config}

>[!IMPORTANT]
>
>Cette section s’applique uniquement aux messages transactionnels (Message Center).
>
>Bien que les fonctionnalités transactionnelles soient disponibles dans l’interface d’utilisation d’Adobe Campaign Web, les étapes de vérification ci-dessous doivent être effectuées dans la console cliente de Campaign v8 (instance de pilotage).

Si vous utilisez la messagerie transactionnelle (Message Center) avec le branding, une configuration supplémentaire est nécessaire.

### Formules de tracking des instances en temps réel

Lorsque le branding est activé sur une instance de pilotage en temps réel (RT), des options de tracking spécifiques sont utilisées pour gérer les formules de tracking. Ces formules sont configurées de manière centralisée sur l’instance de pilotage en temps réel plutôt qu’individuellement sur chaque instance d’exécution en temps réel.

Les options suivantes définissent les formules de tracking utilisées par les diffusions en temps réel :

* **`NmsTracking_RT_ClickFormula`** : indique la formule utilisée pour le suivi des clics sur les instances en temps réel.

* **`NmsTracking_RT_OpenFormula`** : indique la formule utilisée pour le suivi des ouvertures sur les instances en temps réel.

Si votre implémentation nécessite des formules de tracking personnalisées pour les messages transactionnels, utilisez l’option ci-dessous :

* **`Branding_RT_ListXtkOptions_toPublish`** : listez ici les noms des options XTK pour vos formules personnalisées (séparées par des virgules). Cela permet de s’assurer que les diffusions en temps réel peuvent appliquer les formules de tracking personnalisées.
