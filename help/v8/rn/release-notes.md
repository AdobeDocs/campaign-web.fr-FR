---
title: Dernières notes de mise à jour
description: Découvrir les nouvelles fonctionnalités de l’interface utilisateur web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 99%

---

# Notes de mise à jour {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Nouveautés"
>abstract="Les versions de l’interface utilisateur web d’Adobe Campaign fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Les notes de mise à jour sont complétées plusieurs fois par mois. **La version de mars est maintenant en ligne**. Elle contient le canal Courrier, la nouvelle activité de workflow Modifier la source de données et d’autres améliorations encore."


<!--Last update: **March 19, 2024**-->

Les versions de l’interface utilisateur web d’Adobe Campaign fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

>[!AVAILABILITY]
>
>Cette version est disponible pour l’ensemble des utilisateurs et utilisatrices à partir de la [version 8.6 de Campaign (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr). Apprenez-en davantage sur les versions et les mises à niveau de la console cliente d’Adobe Campaign dans la [documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=fr){target="_blank"}.

## Notes de mise à jour de mars {#24-3-release}

**Date de publication** : 19-20 mars 2024

### Canal Courrier {#24-3-dm}

Le canal **Courrier** est désormais disponible pour une utilisation dans les workflows et en tant que diffusions autonomes. Le canal Courrier est un canal hors ligne qui vous permet de créer, personnaliser et générer des fichiers d’extraction, et de les partager avec vos fournisseurs de services postaux pour envoyer du courrier à votre clientèle. [En savoir plus](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Nouvelle activité de workflow Modifier la source de données {#24-3-change-data-source}

L’activité de ciblage **Modifier la source de données** permet de modifier la source de données de la table de travail d’un workflow. Cette activité offre davantage de flexibilité en vous permettant de gérer les données dans vos différentes bases de données et d’améliorer les performances. [En savoir plus](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Amélioration de l’activité de workflow Partage {#24-3-split}

Vous pouvez désormais utiliser l’option **Générer tous les sous-ensembles dans le même tableau** de l’activité de workflow **Partage** pour regrouper tous les sous-ensembles dans une seule transition de sortie. [En savoir plus](../workflows/activities/split.md)

### Concepteur de requête {#24-3-query-modeler}

* Le concepteur de requête est désormais disponible dans le concepteur d’e-mail. Il vous permet de créer des conditions lors de la création de contenu conditionnel. [En savoir plus](../personalization/conditions.md)
* Les valeurs prédéfinies sont désormais disponibles pour les attributs de type date lors de la création d’une condition personnalisée. [En savoir plus](../query/build-query.md)
* Les opérateurs ne peuvent plus être ajoutés sur une nouvelle transition du diagramme. Ils ne peuvent être ajoutés que sur une transition existante avant le filtrage des composants visant à les regrouper. [En savoir plus](../query/build-query.md)
