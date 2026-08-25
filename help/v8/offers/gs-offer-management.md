---
audience: end-user
title: Commencer avec la gestion des offres
description: Découvrir comment gérer les offres dans Adobe Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: ht
source-wordcount: 763
ht-degree: 100%

---

# Commencer avec la gestion des offres {#gs-offer-management}

Cette fonctionnalité vous permet d’ajouter des offres personnalisées à vos diffusions et de présenter l’offre la plus pertinente pour chaque profil dans un contexte donné. Les offres peuvent être un simple message de communication ou des promotions sur un ou plusieurs produits. En fonction des règles d’éligibilité et des poids de priorité, le moteur d’offres sélectionne la meilleure proposition à présenter.

L’interface d’utilisation de Campaign Web permet de gérer les offres de bout en bout. Vous pouvez créer et configurer des environnements d’offres, concevoir des emplacements, créer votre catalogue d’offres, définir des règles d’éligibilité, modifier le contenu des offres et publier des offres.

Les offres sont ensuite présentées aux destinataires par le biais de diffusions en fonction de **règles d’éligibilité** et **poids de priorité**, de sorte que la meilleure offre soit sélectionnée pour chaque profil dans un contexte donné.

>[!NOTE]
>
>L’interface d’utilisation de Campaign Web se concentre sur l’utilisation la plus courante de la gestion des offres. Les configurations avancées restent disponibles dans la console cliente Campaign. Consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=fr){target="_blank"}.

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## Principaux concepts {#concepts}

Avant de commencer à utiliser les offres, familiarisez-vous avec les principaux objets concernés.

* **Environnement d’offres** : conteneur contenant un catalogue d’offres et les emplacements correspondants. Il existe deux types d’environnements, l’environnement **Conception**, où vous créez et configurez des offres, et l’environnement en lecture seule **[!UICONTROL En ligne]**, qui contient les objets approuvés et déployés disponibles pour la diffusion. [En savoir plus](offer-environment.md)

* **Emplacement** : définit où et comment une offre est exposée (e-mail, courrier, SMS, web entrant, etc.). L’emplacement répertorie les champs de contenu qui peuvent être utilisés dans l’offre, la fonction de rendu qui crée la représentation de l’offre et les paramètres de stockage qui pilotent le statut de la proposition. [En savoir plus](offer-space.md)

* **Catalogue d’offres et catégories** : les offres sont organisées dans un catalogue hiérarchique de **catégories** et sous-catégories. Chaque catégorie peut partager des règles d’éligibilité, des dates de validité et des **thèmes d’application**. Une catégorie par défaut est proposée dans l’environnement de conception pour recevoir toutes les offres.

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **Offre** : offre individuelle ayant sa propre période d’éligibilité, son filtre cible, son poids et son contenu. Les offres sont approuvées et déployées avant de pouvoir être présentées aux destinataires. [En savoir plus](create-offer.md)

* **Proposition d’offre** : résultat de la présentation d’une offre à un contact dans un emplacement donné (une bannière sur un site web, un e-mail, un SMS, etc.). Le nombre de propositions par diffusion est paramétré lors de la [configuration des offres dans une diffusion](../msg/offers.md).

* **Arbitrage** : principe selon lequel le moteur d’offres classe les offres éligibles par priorité pour sélectionner celles à présenter. L’arbitrage utilise les critères définis sur les catégories, les offres et les offres contextuelles.

## Flux de gestion des offres {#workflow}

Le flux de bout en bout standard dans l’interface d’utilisation de Campaign Web est le suivant :

1. **Vérifier les paramètres de l’environnement d’offres** : vérifiez les paramètres de conception/mappage dynamique, d’éligibilité et de gestion du poids. [En savoir plus](offer-environment.md)

1. **Créer un emplacement** : définissez les champs de contenu, la fonction de rendu et les paramètres avancés correspondant à votre canal. [En savoir plus](offer-space.md)

1. **Créer des offres dans le catalogue** : définissez la période d’éligibilité, le filtre cible, le poids et le contenu de chaque offre. [En savoir plus](create-offer.md)

1. **Approuver et déployer** : soumettez l’offre pour approbation, approuvez son contenu et son éligibilité, puis laissez le processus de déploiement la publier dans l’environnement en ligne. [En savoir plus](create-offer.md#approve-deploy)

1. **Ajouter l’offre à une diffusion** : référencez l’emplacement et les propositions dans votre diffusion e-mail, SMS, push ou courrier. [En savoir plus](../msg/offers.md)

## Accéder aux offres dans l’interface d’utilisation web {#access}

Les offres sont disponibles dans le menu **[!UICONTROL Offres]** situé à gauche. De là, vous pouvez parcourir le catalogue, ouvrir une offre pour la modifier et surveiller son statut d’approbation et de déploiement.

![Copie d’écran affichant le menu Offre.](assets/offers-gs.png){zoomable="yes"}

Les environnements d’offres et les emplacements sont accessibles via l’**[!UICONTROL Explorateur]**, en accédant au dossier correspondant.


## Compléments réservés à la console {#console-complements}

Certaines fonctionnalités d’offre ne sont pas encore disponibles dans l’interface d’utilisation web et doivent toujours être configurées à partir de la console cliente.

* **Simulation d’offres** : module de **Simulation** qui permet de tester la répartition des offres avant leur envoi. Consultez [Simulation d’offres](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html?lang=fr#offer-simulation){target="_blank"}.

* Gestion des **filtres prédéfinis** : règles de filtrage réutilisables pouvant être référencées à partir de n’importe quelle offre. Consultez [Gérer les filtres prédéfinis](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html?lang=fr){target="_blank"}.

* **Suivi des offres** : configuration du suivi des propositions d’offre afin d’alimenter l’historique des propositions. Consultez [Suivre les propositions d’offre](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html?lang=fr){target="_blank"}.

* **Rôles Opérateur** : attribution des droits Chargé d’offres / Chargé de diffusion. Consultez [Opérateurs du module Interaction](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html?lang=fr){target="_blank"}.

* **Bonnes pratiques d’interaction et règles d’arbitrage**. Consultez les [bonnes pratiques relatives aux interactions Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=fr){target="_blank"}.

* **Rapports** : les rapports dédiés sur les offres et les propositions ne sont pas encore disponibles dans l’interface d’utilisation web.