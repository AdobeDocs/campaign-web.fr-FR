---
audience: end-user
title: Créer et gérer des emplacements
description: Découvrir comment créer, configurer, déployer et prévisualiser des emplacements dans Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 100%
---
# Créer et gérer des emplacements {#offer-space}

Un **emplacement** définit où et comment une offre est exposée à un contact : le canal qu’elle utilise (e-mail, courrier, SMS, web entrant, etc.), les champs de contenu que l’offre peut utiliser et la manière dont la représentation finale est créée. Un seul environnement peut contenir plusieurs emplacements, un pour chaque point d’exposition.

Un emplacement n’est pas un canal en soi. Il représente un emplacement spécifique où l’offre est affichée sur un canal. Deux bannières sur la même page web correspondent généralement à deux emplacements différents. Pour comprendre le modèle conceptuel complet, consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html?lang=fr){target="_blank"}.

## Créer ou modifier un emplacement{#create-offer-space}

Les emplacements sont stockés dans le dossier d’environnement d’offre. Pour parcourir les emplacements disponibles sur votre plateforme, ouvrez l’**[!UICONTROL Explorateur]**, accédez à l’environnement d’offres et sélectionnez le sous-dossier qui les contient.

![Capture d’écran affichant la liste des emplacements.](assets/offers-space.png){zoomable="yes"}

De là, vous pouvez ouvrir un emplacement existant ou en créer un en cliquant sur **[!UICONTROL Créer un emplacement]**.

![Capture d’écran affichant l’écran Emplacement.](assets/offers-space-1.png){zoomable="yes"}

### Définir les propriétés {#properties}

Cette section vous permet de :

* Saisir le **[!UICONTROL libellé]** de l’emplacement.
* Sélectionner le **[!UICONTROL canal]** correspondant au point d’exposition (e-mail, courrier, SMS, web, etc.).
* Sélectionner **[!UICONTROL Activer le mode unitaire]** si cet emplacement doit également prendre en charge les appels unitaires (temps réel, offre unique) au moteur d’offres, en plus des appels de diffusion en masse.

### Définir les champs de contenu {#content-fields}

Les champs de contenu répertorient les attributs qui peuvent être modifiés au niveau de l’offre et réutilisés par la fonction de rendu. L’ordre dans lequel vous ajoutez les champs dans l’emplacement détermine l’ordre dans lequel ils sont exposés dans la section **[!UICONTROL Contenu]** de l’offre.

Par défaut, le contenu peut contenir les champs suivants : **[!UICONTROL Titre]**, **[!UICONTROL URL de destination]**, **[!UICONTROL URL d’image]**, **[!UICONTROL Contenu HTML]** et **[!UICONTROL Contenu texte]**. Vous pouvez étendre cette liste avec n’importe quel champ personnalisé dont votre rendu a besoin, par exemple un **contenu court**, une **URL suivie** ou tout attribut ajouté par le biais de l’extension de schéma.

Cliquez sur **[!UICONTROL Ajouter un champ de contenu]**, puis sélectionnez l’attribut à exposer dans le schéma d’offre, ou cliquez sur **[!UICONTROL Modifier l’expression]** pour définir une expression personnalisée à la place.

>[!IMPORTANT]
>
>Pour rendre un attribut personnalisé modifiable à partir de la section **[!UICONTROL Contenu]** de l’offre, l’attribut doit également être déclaré dans la section **[!UICONTROL Contenu de l’offre]** du schéma de [!DNL nms:offer]. En savoir plus dans [Utilisation de schémas](../administration/schemas.md).

### Configurer les fonctions de rendu {#rendering}

Les fonctions de rendu créent la représentation finale de l’offre à partir des champs de contenu. Vous pouvez choisir entre le rendu par défaut (qui génère simplement le contenu tel quel) ou une fonction personnalisée qui combine les champs avec HTML, XML ou texte.

Positionnez-vous sur l’onglet **[!UICONTROL Rendu HTML]**, **[!UICONTROL Rendu XML]** ou **[!UICONTROL Rendu de texte]** et sélectionnez **[!UICONTROL Surcharger la fonction de rendu HTML]** pour l’activer.

Utilisez l’éditeur d’expression pour écrire la fonction de rendu. Vous pouvez référencer les champs de contenu définis dans l’espace, les attributs de l’offre et toute fonction à partir de l’[éditeur d’expression](../query/expression-editor.md).

>[!NOTE]
>
>Si aucune fonction de rendu n’est définie, le contenu de l’offre est renvoyé tel quel à l’aide des attributs par défaut. La fonction de rendu XML ne peut être utilisée que lorsque l’option **[!UICONTROL Activer le mode unitaire]** est sélectionnée sur l’emplacement.

### Configurer le stockage et le statut des propositions {#storage}

Cette section vous permet de contrôler la manière dont les propositions générées dans cet espace sont conservées et comment leur statut évolue tout au long de leur cycle de vie :

* **[!UICONTROL Désactiver l’insertion des propositions]** — Empêche les propositions générées par cet emplacement d’être insérées dans la table de stockage des propositions.

* **[!UICONTROL Statut]** sur la proposition — Statut appliqué à la proposition au moment où le moteur d’offres la renvoie (généralement **[!UICONTROL Présentée]** pour les diffusions sortantes).

* **[!UICONTROL Statut]** à l’acceptation — Statut appliqué lorsque la personne destinataire interagit avec l’offre (généralement **[!UICONTROL Acceptée]**).

Les valeurs de statut disponibles correspondent à la liste utilisée par la console cliente. Pour plus d’informations, consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html?lang=fr#offer-proposition-statuses){target="_blank"} dans la documentation de la console.

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### Configurer les paramètres avancés {#advanced}

Cette section permet de définir l’**[!UICONTROL identification de la cible]**. Cliquez sur **[!UICONTROL Ajouter]** et sélectionnez un ou plusieurs attributs **[!UICONTROL Destinataire]** ou cliquez sur **[!UICONTROL Modifier l’expression]** pour définir une expression personnalisée à la place. Ce paramètre est facultatif pour un emplacement de base. Pour des informations de référence et connaître le fonctionnement, consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html?lang=fr){target="_blank"}.

Les emplacements créés sur le **canal web entrant** nécessitent également que le site soit paramétré pour afficher l’offre et appeler le moteur d’offres. Cette intégration est effectuée dans la console cliente. Consultez les sections [Présentation des offres en temps réel](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html?lang=fr){target="_blank"} et [Configuration de l’intégration du moteur d’offres](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html?lang=fr){target="_blank"} dans la documentation de Campaign v8.

## Déployer l’emplacement {#deploy}

Un emplacement doit être déployé avant de pouvoir être utilisé dans une diffusion. Enregistrez votre emplacement, puis cliquez sur **Déployer**. Le statut du déploiement est reflété dans l’emplacement.

![Capture d’écran montrant le déploiement de l’offre.](assets/offers-space-2.png){zoomable="yes"}

## Prévisualiser l’emplacement {#preview}

La fonction de prévisualisation permet de simuler la sélection et le rendu d’une offre pour une cible donnée.

1. Depuis l’emplacement, sélectionnez l’onglet **[!UICONTROL Aperçu]**, en regard de **[!UICONTROL Vue d’ensemble]**.

   ![Capture d’écran affichant l’aperçu de l’offre.](assets/offers-space-3.png){zoomable="yes"}

1. Sélectionnez un profil cible et exécutez l’aperçu. Les offres correspondantes sont renvoyées avec la représentation produite par la fonction de rendu.

>[!NOTE]
>
>Si aucune proposition n’est renvoyée, vérifiez les règles d’éligibilité des offres et la configuration de l’emplacement.

Ensuite, [créez une offre](create-offer.md) dans le catalogue et affectez-la à cet emplacement.
