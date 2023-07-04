---
audience: end-user
title: Prise en main des campagnes
description: Découvrez comment commencer avec les campagnes cross-canal.
badge: label="Alpha"
source-git-commit: c9954ce69e50e1c8db2532be3292f71ff20f9f74
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Accéder aux campagnes et les gérer{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Planning de la campagne"
>abstract="Définissez ou modifiez le planning de votre campagne."

Pour créer une campagne ou gérer vos campagnes existantes, cliquez sur le menu **[!UICONTROL Campagnes]** dans le volet de navigation de gauche.

## La liste des campagnes{#access-campaigns}

La liste des campagnes comprend deux onglets :

* L’onglet **Parcourir** répertorie toutes les campagnes existantes. Cliquez sur une campagne pour afficher son tableau de bord ou créez une campagne à l’aide du bouton **Créer une campagne**. Consultez cette [section](create-campaigns.md#create-campaigns).

* L’onglet **Modèles** répertorie tous les modèles de campagne disponibles. Les modèles de campagne sont préconfigurés afin de pouvoir être réutilisés lors de la création de campagnes. Ils sont créés à partir de la console cliente. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=fr)

![Liste des campagnes](assets/campaign-list.png)

Par défaut, chaque campagne de la liste affiche des informations sur son statut en cours, sa date de création, la dernière fois qu’elle a été modifiée, etc.

Vous pouvez personnaliser les colonnes affichées en cliquant sur l’icône **Configurer la colonne pour une disposition personnalisée**, située dans le coin supérieur droit de la liste. Vous pouvez ainsi ajouter des informations supplémentaires à la liste. Une barre de recherche et des filtres sont également disponibles pour faciliter la recherche dans la liste. [En savoir plus](../get-started/user-interface.md#list-screens).

Vous pouvez, par exemple, filtrer selon le planning de votre campagne. Ouvrez le panneau de filtrage et accédez à la section **Date de début et de fin** :

![Filtre de campagne](assets/campaign-filter-on-dates.png)

## Le tableau de bord de la campagne{#campaign-dashboard}

Sous l’onglet **Parcourir** de la liste des campagnes, cliquez sur une campagne pour afficher ses détails.

![Tableau de bord de la campagne](assets/campaign-dashboard.png)

Le statut et le planning de la campagne sont affichés en haut de l’écran. L’icône **Configurer les paramètres de campagne** permet de modifier les propriétés de la campagne précédemment définies. Trois boutons permettent d’afficher les logs, de créer des rapports, de dupliquer ou de supprimer la campagne. Consultez cette [section](create-campaigns.md#create-campaigns).

Deux onglets sont disponibles :

* L’onglet **Workflows** dresse la liste des workflows liés à la campagne. Cet onglet permet également de créer un workflow au sein de la campagne. Consultez cette [section](create-campaigns.md#create-campaigns)..

* L’onglet **Diffusions** répertorie toutes les diffusions liées à la campagne en cours. Vous pouvez également créer une diffusion au sein de la campagne. Consultez cette [section](create-campaigns.md#create-campaigns).

## Dupliquer et supprimer une campagne

Vous pouvez dupliquer ou supprimer une campagne :

* dans la liste des campagnes, cliquez sur le bouton représentant des points de suspension puis sélectionnez **Dupliquer** ou **Supprimer** ;
* dans la campagne elle-même, cliquez sur le bouton **Plus** puis sélectionnez **Dupliquer** ou **Supprimer**.

>[!NOTE]
>
>L’onglet **Diffusions** affiche toutes les diffusions liées à la campagne. Cependant, les diffusions créées dans un workflow ne peuvent pas être supprimées depuis cet endroit. Pour supprimer une diffusion créée dans le cadre d’un workflow, vous devez supprimer l’activité de diffusion du workflow. [En savoir plus](../msg/gs-messages.md#delivery-delete).
