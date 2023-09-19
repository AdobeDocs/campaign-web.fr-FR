---
audience: end-user
title: Gestion des autorisations dans Campaign web
description: En savoir plus sur les autorisations dans Campaign web v8
badge: label="Beta"
source-git-commit: 5e2af07f54fae9b0d64d173388be14639e6aaaa2
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 42%

---


# Accès et autorisations {#access-and-permissions}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="Autorisation requise"
>abstract="Votre administrateur doit vous accorder l’autorisation avant de pouvoir créer cet objet."


>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="Cette audience est en lecture seule"
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier cette audience. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."


>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="Ce service est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier ce service. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."


>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Cette campagne est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier cette campagne. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="Cette diffusion est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier cette diffusion. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="Ce workflow est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier ce workflow. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Ce workflow est en lecture seule."
>abstract="Vous ne pouvez pas modifier ce workflow en raison d’un canevas non pris en charge ou incompatible."

Le contrôle d’accès peut restreindre l’accès aux objets et données des listes principales, telles que les diffusions, les destinataires ou les workflows. Ces restrictions s’appliquent également dans la variable **Explorateur** arborescence de navigation. En outre, vous avez besoin d’autorisations pour créer, supprimer, dupliquer et modifier des objets à partir de l’interface utilisateur.

Le contrôle d’accès est géré dans la console cliente Campaign. Toutes les autorisations de Campaign web sont synchronisées avec celles de la console cliente Campaign. Seuls les administrateurs ou les administratrices de Campaign peuvent définir et modifier les autorisations utilisateur. En savoir plus sur les autorisations utilisateur dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=fr){target="_blank"}.

Lorsque vous naviguez dans l&#39;interface utilisateur Web de Campaign, vous pouvez accéder aux données, aux objets et aux fonctionnalités en fonction de vos permissions. Par exemple, si vous ne disposez pas des autorisations d’accès à un dossier, vous ne pouvez pas l’afficher. Vos autorisations ont également une incidence sur la gestion des objets et des données. Sans autorisation d’écriture pour un dossier spécifique, vous ne pouvez pas créer de diffusion dans ce dossier, même si vous pouvez l’afficher dans l’interface utilisateur.

## Affichage des autorisations {#view-permissions}

Dans la **Explorateur**, vous pouvez parcourir les autorisations pour chaque dossier. Ces permissions sont définies dans la console cliente et sont utilisées pour organiser et contrôler l&#39;accès aux données de Campaign.

Pour afficher les autorisations d’un dossier, procédez comme suit :

1. Dans la **Explorateur** dans le menu de navigation de gauche, sélectionnez un dossier.
1. Cliquez sur les trois points dans le coin supérieur droit et sélectionnez **Autorisations de dossier**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. Vérifiez les détails dans l’écran, comme ci-dessous :

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   Un groupe, ou un opérateur, peut disposer des autorisations de lecture, d’écriture et/ou de suppression sur les données stockées dans le dossier sélectionné.

   Si la variable **Propager** est activée, toutes les autorisations définies pour un dossier sont appliquées à tous ses sous-dossiers. Ces autorisations peuvent être surchargées pour chaque sous-dossier.

   Si la variable **Dossier système** est activée, l’accès est autorisé à tous les opérateurs, quelles que soient leurs permissions.

En savoir plus sur les autorisations de dossiers dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## Utilisation de dossiers {#folders}

Vous pouvez créer, renommer, réorganiser et déplacer des dossiers pour organiser vos composants et vos données. Vous pouvez également supprimer des dossiers à partir du même menu.

>[!CAUTION]
>
>Lors de la suppression d’un dossier, toutes les données stockées dans le dossier sont également supprimées.

Pour créer un dossier, procédez comme suit :

1. Dans la **Explorateur** dans le menu de navigation de gauche, sélectionnez un dossier.
1. Cliquez sur les trois points dans le coin supérieur droit et choisissez **Créer un sous-dossier**.
1. Saisissez le nom du dossier et enregistrez-le.

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   Le dossier est ajouté en tant que sous-dossier du dossier actif. Accédez à ce nouveau dossier pour y créer des composants directement. Vous pouvez également créer un composant à partir de n’importe quel dossier, puis l’enregistrer dans ce nouveau dossier, à partir de l’événement **Options supplémentaires** des propriétés, comme illustré ci-dessous pour une diffusion :

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}

