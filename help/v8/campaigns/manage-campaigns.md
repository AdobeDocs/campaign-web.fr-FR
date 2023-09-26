---
audience: end-user
title: Prise en main des campagnes
description: Découvrez comment commencer avec les campagnes cross-canal.
badge: label="Beta"
source-git-commit: 7a04eb8c5b60b9a2545723fcb6a748c57e9d98e6
workflow-type: ht
source-wordcount: '603'
ht-degree: 100%

---


# Accéder aux campagnes et les gérer{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Planning de la campagne"
>abstract="Définissez ou modifiez le planning de votre campagne."

Pour créer une campagne ou gérer vos campagnes existantes, cliquez sur le menu **[!UICONTROL Campagnes]** dans le volet de navigation de gauche.

## Liste de campagnes {#access-campaigns}

La liste des campagnes comprend deux onglets :

* L’onglet **Parcourir** répertorie toutes les campagnes existantes. Cliquez sur une campagne pour afficher son tableau de bord ou créez une campagne à l’aide du bouton **Créer une campagne**. Consultez cette [section](create-campaigns.md#create-campaigns).

* L’onglet **Modèles** répertorie tous les modèles de campagne disponibles. Vous pouvez afficher un modèle existant ou en créer un nouveau. [En savoir plus](#manage-campaign-templates).

![Liste des campagnes](assets/campaign-list.png)

Par défaut, chaque campagne de la liste affiche des informations sur son statut en cours, sa date de création, la dernière fois qu’elle a été modifiée, etc.

Vous pouvez personnaliser les colonnes affichées en cliquant sur l’icône **Configurer la colonne pour une disposition personnalisée**, située dans le coin supérieur droit de la liste. Vous pouvez ainsi ajouter des informations supplémentaires à la liste. Une barre de recherche et des filtres sont également disponibles pour faciliter la recherche dans la liste. [En savoir plus](../get-started/user-interface.md#list-screens).

Vous pouvez, par exemple, filtrer selon le planning de votre campagne. Ouvrez le panneau de filtrage et accédez à la section **Date de début et de fin** :

![Filtre de campagne](assets/campaign-filter-on-dates.png)

## Tableau de bord de la campagne{#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Liste des diffusions de la campagne"
>abstract="L’onglet **Diffusions** répertorie toutes les diffusions liées à la campagne en cours. Cliquez sur le nom d’une diffusion pour la modifier. Cliquez sur le bouton Créer une diffusion pour ajouter une diffusion à cette campagne."

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

## Utiliser des modèles de campagnes{#manage-campaign-templates}

Les modèles de campagnes contiennent des paramètres préconfigurés qui peuvent être réutilisés pour créer de nouvelles campagnes. Nous mettons à votre disposition un ensemble de modèles intégrés pour vous aider à démarrer. Vous pouvez créer et configurer des modèles d’opération, puis créer des opérations à partir de ces modèles.

Un modèle de campagne peut stocker les informations suivantes :

* **Propriétés** de la campagne et paramètres du **planning**.
* Modèles de workflows.
* Modèles de diffusion.

Pour créer un modèle de campagne, procédez comme suit :

1. Cliquez sur le menu **[!UICONTROL Campagnes]**, accédez à l’onglet **Modèles**, puis cliquez sur le bouton **[!UICONTROL Créer un modèle]**.
1. Sélectionnez le **modèle** à utiliser. Vous pouvez ainsi baser votre nouveau modèle sur un modèle créé précédemment.
1. Attribuez un libellé à votre modèle.
1. Si nécessaire, vous pouvez modifier les **options supplémentaires** suivantes : nom interne, dossier, personnes assignées, description et nature.
1. Définissez le **planning** de votre campagne. Découvrez comment définir le planning de votre campagne dans [cette section](create-campaigns.md#campaign-schedule).
1. Cliquez sur **Créer**.
1. Ajoutez des workflows et des modèles de diffusion à votre campagne.
