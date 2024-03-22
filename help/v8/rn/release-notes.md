---
title: Dernières notes de mise à jour
description: Découvrir les nouvelles fonctionnalités de l’interface utilisateur web de Campaign
source-git-commit: 5b0e59e8bb7e4a8ee3ce648c4af7dd9e41be7a81
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 9%

---

# Notes de mise à jour {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Nouveautés"
>abstract="Les versions de l’interface utilisateur Web d’Adobe Campaign fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Les notes de mise à jour sont mises à jour plusieurs fois par mois. **La version de mars est maintenant en ligne**, y compris le canal Courrier, la nouvelle activité de workflow Modifier la source de données et d’autres améliorations."


<!--Last update: **March 19, 2024**-->

Les versions de l’interface utilisateur Web d’Adobe Campaign fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont mises à jour plusieurs fois par mois. Veuillez les vérifier régulièrement.

>[!AVAILABILITY]
>
>Cette version est disponible pour tous les utilisateurs qui démarrent [Version de Campaign (console) v8.6](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr). En savoir plus sur les versions et mises à niveau de la console cliente Adobe Campaign dans [Documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=fr){target="_blank"}.

## Notes de mise à jour de mars {#24-3-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Publipostage direct"
>abstract="Le canal Courrier est désormais disponible pour les workflows et les diffusions autonomes. Utilisez le canal Courrier hors ligne pour créer, personnaliser et générer un fichier d’extraction, et partagez-le avec vos opérateurs de services postaux afin d’envoyer du courrier à vos clients."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes" text="Voir les notes de mise à jour"

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Modifier la source de données"
>abstract="Utilisez la nouvelle activité de ciblage de workflow Modifier la source de données pour modifier la source de données utilisée par la table de travail de votre workflow. Cette activité offre davantage de flexibilité en vous permettant de gérer les données dans vos différentes bases de données et d’améliorer les performances."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes" text="Voir les notes de mise à jour"


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
