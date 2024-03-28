---
title: Dernières notes de mise à jour
description: Découvrir les nouvelles fonctionnalités de l’interface utilisateur web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 30%

---

# Notes de mise à jour {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Nouveautés"
>abstract="Les mises à jour de l’interface utilisateur web d’Adobe Campaign fonctionnent sur un modèle de diffusion continue qui permet une approche plus évolutive et plus progressive du déploiement des fonctionnalités. Ces notes de mise à jour sont modifiées plusieurs fois par mois. **La version de mars est maintenant en ligne**, y compris le canal Courrier, la nouvelle activité de workflow Modifier la source de données et d’autres améliorations encore."


<!--Last update: **March 19, 2024**-->

Les mises à jour de l’interface utilisateur web d’Adobe Campaign fonctionnent sur un modèle de diffusion continue qui permet une approche plus évolutive et plus progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont mises à jour plusieurs fois par mois. Veuillez les vérifier régulièrement.

>[!AVAILABILITY]
>
>Cette version est disponible pour tous les utilisateurs qui démarrent [Version de Campaign (console) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr). En savoir plus sur les versions et mises à niveau de la console cliente Adobe Campaign dans [Documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=fr){target="_blank"}.

## Notes de mise à jour de mars {#24-3-release}

**Date de publication**: 19-20 mars 2024

### Canal courrier {#24-3-dm}

**Canal Courrier** est désormais disponible pour une utilisation dans les workflows et en tant que diffusions autonomes. Le canal Courrier est un canal off-line qui vous permet de créer, personnaliser et générer des fichiers d’extraction, et de les partager avec vos fournisseurs de services postaux pour envoyer du courrier à vos clients. [En savoir plus](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Activité de workflow Modifier la source de données {#24-3-change-data-source}

La variable **Modification de la source de données** l&#39;activité de ciblage permet de modifier la source de données utilisée par la table de travail de votre workflow. Cette activité offre davantage de flexibilité en vous permettant de gérer les données dans vos différentes bases de données et d’améliorer les performances. [En savoir plus](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Amélioration de l’activité de workflow de partage {#24-3-split}

Vous pouvez désormais utiliser la variable **Générer tous les sous-ensembles dans la même table** dans le **Partage** activité de workflow pour regrouper tous les sous-ensembles dans une seule transition de sortie. [En savoir plus](../workflows/activities/split.md)

### Concepteur de requête {#24-3-query-modeler}

* Le modèle de requête est désormais disponible dans le Concepteur d’email. Il vous permet de créer des conditions lors de la création de contenu conditionnel. [En savoir plus](../personalization/conditions.md)
* Les valeurs prédéfinies sont désormais disponibles pour les attributs de type date lors de la création d’une condition personnalisée. [En savoir plus](../query/build-query.md)
* Les opérateurs ne peuvent plus être ajoutés sur une nouvelle transition du diagramme. Ils ne peuvent être ajoutés que sur une transition existante avant de filtrer les composants pour les regrouper. [En savoir plus](../query/build-query.md)
