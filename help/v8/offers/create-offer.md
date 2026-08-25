---
audience: end-user
title: Créer et publier une offre
description: Découvrir comment créer, configurer, approuver et déployer une offre dans Campaign Web
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7bd09b83112efb99c90884b7da21a5e9a5c76b6c
workflow-type: ht
source-wordcount: 1057
ht-degree: 100%

---

# Créer et publier une offre {#create-offer}

Une **offre** est une proposition individuelle avec sa propre période d’éligibilité, son filtre cible, son poids et son contenu. Les offres sont organisées dans le catalogue d’offres au travers de **catégories** et sont présentées aux destinataires par le biais d’un **emplacement**.

Avant de créer une offre, assurez-vous que l’environnement des offres est configuré et qu’au moins un emplacement est publié. Pour en savoir plus, consultez les sections [Configurer un environnement d’offres](offer-environment.md) et [Créer et gérer des emplacements](offer-space.md).

## Accéder au catalogue d’offres {#access}

Pour parcourir et créer des offres, sélectionnez **[!UICONTROL Offres]** dans le rail de navigation de gauche. La liste affiche les offres existantes. Utilisez le champ de recherche, le sélecteur de dossiers ou le [concepteur de requête](../query/query-modeler-overview.md) pour filtrer la liste.

![Copie d’écran affichant le catalogue d’offres.](assets/offers-offer.png){zoomable="yes"}

Cliquez sur le nom d’une offre pour l’ouvrir en vue de la modifier ou utilisez les trois points en regard pour la **[!UICONTROL Dupliquer]** ou la **[!UICONTROL Supprimer]**.

## Créer une offre {#create}

Pour créer une offre :

1. Dans la liste des offres, cliquez sur **[!UICONTROL Créer une offre]**.

1. Sélectionnez le **[!UICONTROL modèle]** à partir duquel créer l’offre (par exemple, une offre vierge ou un modèle d’offre anonyme).

   ![Copie d’écran montrant la création d’une offre.](assets/offers-offer-1.png){zoomable="yes"}

1. Saisissez un **[!UICONTROL Libellé]** et, éventuellement, affectez l’offre à un opérateur ou une opératrice à l’aide de l’option **[!UICONTROL Affecté à]** et/ou saisissez un **[!UICONTROL code d’offre]**.

1. Développez **[!UICONTROL Options supplémentaires]** pour modifier le **[!UICONTROL nom interne]** généré automatiquement, sélectionner la **[!UICONTROL catégorie]** dans laquelle l’offre est stockée ou ajouter une description. Cette étape est facultative.

1. Développez **[!UICONTROL Approbations]** pour affecter des approbateurs et approbatrices aux groupes **[!UICONTROL Approbation de l’éligibilité]** et **[!UICONTROL Approbation du contenu]**. Cette étape est facultative.

1. Développez **[!UICONTROL Options personnalisées]** pour remplir les champs supplémentaires que votre organisation a ajoutés au schéma d’offre. Les champs affichés dans cette section varient d’une instance Campaign à l’autre. Cette étape est facultative.

1. Cliquez sur **[!UICONTROL Créer]**. L’écran complet des paramètres s’affiche.

   ![Copie d’écran affichant l’écran Paramètres des offres.](assets/offers-offer-2.png){zoomable="yes"}

### Définir l’éligibilité {#eligibility}

Cette section vous permet de contrôler quand et à qui l’offre peut être présentée. Les options disponibles sont les suivantes :

* **[!UICONTROL Planning]** : définissez les dates de début et de fin entre lesquelles l’offre peut être présentée.

  >[!NOTE]
  >
  >Les périodes d’éligibilité qui se chevauchent avec la catégorie parent sont prises en compte : même si le planning propre à l’offre est plus large, l’offre n’est présentée que lorsque sa catégorie parent est aussi éligible.

* **[!UICONTROL Filtres sur la cible]** : cliquez sur **[!UICONTROL Créer un filtre]** pour ouvrir le créateur de règles et restreindre l’offre à une audience spécifique. Laissez le filtre vide pour rendre l’offre éligible à l’audience entière de l’environnement. Pour réutiliser un **filtre prédéfini** déclaré au niveau de la plateforme, reportez-vous à la documentation de [Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html?lang=fr){target="_blank"}. Les filtres prédéfinis sont créés à partir de la console cliente.

* **[!UICONTROL Gestion du poids de l’offre]** : cliquez sur **[!UICONTROL Afficher le poids de l’offre]**, puis **[!UICONTROL Ajouter un poids]** pour influencer la priorité de l’offre lorsque plusieurs offres sont éligibles en même temps. Chaque poids comporte une date de début, une date de fin et un filtre facultatif.

>[!NOTE]
>
>Le moteur d’offres trie les offres éligibles par poids décroissant et renvoie en premier les propositions les plus pondérées. La logique de sélection, appelée **arbitrage**, prend également en compte les règles d’éligibilité et les poids configurés sur la catégorie parent et sur l’environnement. Pour en savoir plus sur le principe d’arbitrage, consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=fr){target="_blank"}.

### Définir le contenu {#content}

Depuis l’offre, sélectionnez l’onglet **[!UICONTROL Contenu]**. Cet onglet définit les valeurs qui seront exposées par la fonction de rendu.

1. Renseignez les attributs prêts à l’emploi : **[!UICONTROL Titre]**, **[!UICONTROL URL de destination]**, **[!UICONTROL URL d’image]** et tout attribut personnalisé déclaré dans le schéma d’offre.

1. Utilisez l’[éditeur d’expression](../query/expression-editor.md) pour personnaliser les valeurs avec des données de profil, des attributs d’offre ou des champs de proposition.

1. Pour les payloads HTML et texte, cliquez sur **[!UICONTROL Modifier le contenu]** pour ouvrir l’éditeur de contenu. Vous pouvez concevoir le contenu à partir de zéro, coder votre propre HTML ou importer du contenu HTML existant, en partant éventuellement d’un modèle.

>[!IMPORTANT]
>
>Les attributs disponibles dans la section **[!UICONTROL Contenu]** dépendent du schéma [!DNL nms:offer]. Pour exposer des attributs personnalisés, étendez le schéma et sélectionnez-les dans la section **[!UICONTROL Contenu de l’offre]**. Pour en savoir plus, consultez [Utiliser des schémas](../administration/schemas.md).

## Prévisualiser l’offre {#preview}

Vous pouvez prévisualiser l’offre avant de l’envoyer.

1. Dans l’offre, sélectionnez l’onglet **[!UICONTROL Prévisualisation]** en regard de **[!UICONTROL Vue d’ensemble]**.

   ![Capture d’écran affichant l’aperçu de l’offre.](assets/offers-offer-3.png){zoomable="yes"}

1. Sélectionnez un profil cible et, le cas échéant, l’emplacement sur lequel la prévisualisation doit être exécutée.

   La fonction de rendu définie sur l’emplacement est appliquée au contenu de l’offre, et la représentation résultante s’affiche.

>[!NOTE]
>
>Si la prévisualisation renvoie une erreur ou aucun contenu, vérifiez la fonction de rendu de l’emplacement, les règles d’éligibilité de l’offre et assurez-vous que tous les champs de contenu obligatoires sont remplis.

## Approuver et déployer l’offre {#approve-deploy}

Les offres ne sont pas immédiatement disponibles dans les diffusions : elles passent par un cycle d’approbation et de déploiement.

1. Dans la vue d’ensemble de l’offre, cliquez sur **[!UICONTROL Approbation]**.

   ![Copie d’écran affichant l’approbation de l’offre.](assets/offers-offer-4.png){zoomable="yes"}

1. Approuvez l’**[!UICONTROL Éligibilité]** et le **[!UICONTROL Contenu]**. Le contenu peut être approuvé par emplacement, vous pouvez donc l’approuver pour un emplacement tout en laissant les autres en attente.

1. Une fois les deux approbations accordées, cliquez sur **[!UICONTROL Déployer]** pour publier l’offre dans l’environnement en ligne.

1. Actualisez la vue de l’offre pour confirmer que la représentation **[!UICONTROL en ligne]** est à jour.

<!--
>[!NOTE]
>
>Once deployed, the design offer's status resets to **[!UICONTROL Being edited]** — its normal draft status, not a sign that someone is actively editing it. This just means the design offer is ready to accept further changes, which would then need to go through a new approval and deployment cycle. The live representation itself remains untouched until that happens.
-->

>[!CAUTION]
>
>L’approbation de l’éligibilité et du contenu d’une offre sont deux actions distinctes. Une offre peut être partiellement approuvée (contenu uniquement, par exemple) et rester indisponible pour la diffusion jusqu’à ce que l’approbation de l’éligibilité soit également accordée.

## Surveiller le tableau de bord des offres {#dashboard}

L’onglet **[!UICONTROL Vue d’ensemble]** de l’offre résume le statut de l’offre dans les cartes **[!UICONTROL Propriétés]**, **[!UICONTROL Contenu]** et **[!UICONTROL Éligibilité]**, avec une icône en forme de crayon sur chacune d’elles pour revenir au mode édition. Une carte **[!UICONTROL Représentation]** répertorie chaque emplacement auquel l’offre est liée, ainsi que son statut de conception actuel.

![Copie d’écran affichant le tableau de bord des offres.](assets/offers-offer-5.png){zoomable="yes"}

Cliquez sur **[!UICONTROL Journaux]** pour accéder aux journaux de déploiement, ou sur le menu **···** (**[!UICONTROL Plus]**) pour **[!UICONTROL Dupliquer]** ou **[!UICONTROL Supprimer]** l’offre.

Une fois qu’une offre est active, la modification de n’importe quel paramètre fait revenir l’offre de conception à un état modifiable. La représentation en ligne reste inchangée jusqu’au cycle suivant d’approbation et de déploiement.

## Utiliser l’offre dans une diffusion {#use-in-delivery}

Lorsque l’offre est en ligne, elle peut être sélectionnée dans n’importe quelle diffusion qui cible l’emplacement correspondant. Découvrez comment configurer des offres dans une diffusion dans [Ajouter des offres à vos messages](../msg/offers.md).

Pour l’intégration complète des diffusions sortantes, notamment la manière dont l’appel au moteur est créé et dont le suivi est appliqué aux liens des offres, consultez la [documentation de Campaign v8 sur les offres dans les diffusions sortantes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-send-offers.html?lang=fr){target="_blank"}.

