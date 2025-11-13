---
title: Utiliser les schémas
description: Découvrez comment utiliser les schémas.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: ht
source-wordcount: '597'
ht-degree: 100%

---

# Utiliser les schémas {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schémas"
>abstract="**[!DNL Adobe Campaign]** utilise des schémas XML pour définir la structure physique et logique des données dans l’application. Depuis cet écran, vous pouvez afficher tous les schémas existants et accéder aux détails d’un schéma en sélectionnant son nom dans la liste. Des filtres sont disponibles pour aider à affiner la liste, par exemple pour afficher uniquement les schémas modifiables."

## À propos des schémas {#about}

**[!DNL Adobe Campaign]** utilise des schémas XML pour définir la structure physique et logique des données dans l’application. Un schéma est un document XML lié à une table de base de données qui définit les éléments suivants :

* Structure de la table SQL, comprenant le nom de la table, les champs et les relations.
* Structure des données XML, comprenant des éléments, des attributs, une hiérarchie, des types, des valeurs par défaut et des libellés.

Les schémas jouent un rôle essentiel dans ce qui suit :

* Mapping des données d’application avec les tables de la base de données.
* Définition des relations entre les objets de données.
* Spécification de la structure et des propriétés de chaque champ.

Chaque entité d’Adobe Campaign dispose d’un schéma dédié, ce qui permet d’assurer la cohérence des données et leur organisation.

Vous trouverez des informations détaillées sur les schémas dans la [documentation de la console Campaign](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

## Accéder aux schémas dans l’interface d’utilisation web {#access}

Les schémas sont accessibles à partir du menu **[!UICONTROL Administration]** > **[!UICONTROL Schémas]**.

![Écran de liste des schémas affichant les schémas et les filtres disponibles](assets/schemas-list.png)

Depuis cet écran, vous pouvez afficher tous les schémas existants. Des filtres sont disponibles pour aider à affiner la liste, par exemple pour afficher uniquement les schémas modifiables.

Pour ouvrir un schéma, sélectionnez son nom. Une vue de schéma détaillée s’affiche.

![Écran de détails du schéma affichant les propriétés et le contenu du schéma](assets/schema-details.png)

### Vue d’ensemble du schéma {#overview}

L’onglet **[!UICONTROL Vue d’ensemble]** offre une vue générale du schéma :

* La section **[!UICONTROL Propriétés]** affiche des informations clés, telles que le nom du schéma, l’espace de noms et le nom de la table associée.

* La section **[!UICONTROL Définition du schéma]** affiche des détails sur la définition du schéma, comme la clé primaire utilisée pour la réconciliation des données et ses liens avec d’autres tables.

  Cliquez sur le bouton **[!UICONTROL Aperçu du schéma]** pour visualiser les différents champs et liens composant le schéma. Vous pouvez ainsi vérifier la structure complète d’un schéma. Si le schéma a été étendu avec des champs personnalisés, vous pouvez visualiser toutes ses extensions.

* La section **[!UICONTROL Contenu]** affiche le contenu XML du schéma, ce qui vous permet de basculer entre la source et la syntaxe générée.

### Données de schéma {#data}

L’onglet **[!UICONTROL Données]** fournit des informations sur les données du schéma.

![Onglet Données de schéma présentant la structure et les attributs des données](assets/schemas-data.png)

## Configurer la définition d’écran {#screen-definition}

### Modifier des champs personnalisés {#fields}

Les champs personnalisés sont des attributs supplémentaires ajoutés aux schémas prêts à l’emploi via la console Adobe Campaign. Ils vous permettent de personnaliser les schémas en incluant de nouveaux attributs en fonction des besoins de votre entreprise.

Les champs personnalisés peuvent être affichés sur différents écrans, comme les détails de profil dans l’interface web de Campaign. Vous pouvez contrôler quels champs sont visibles et la manière dont ils apparaissent dans l’interface. Pour ce faire, cliquez sur le bouton **[!UICONTROL Édition d’écran]** dans le menu **[!UICONTROL Schémas]**.

![Écran de champs personnalisés affichant les attributs modifiables](assets/schemas-custom.png)

Cliquez sur **[!UICONTROL Aperçu]** pour afficher les champs personnalisés dans un exemple d’écran.

Pour plus d’informations sur la modification des champs personnalisés dans un schéma, reportez-vous à la section [Configurer des champs personnalisés](../administration/custom-fields.md).

### Ajouter des listes de collection {#collection-lists}

La section **Liste des listes personnalisées** vous permet de définir des liens de collection, tels que les achats. Les données associées sont alors affichées sur les écrans des profils via un onglet dédié.

>[!NOTE]
>
>Actuellement, cette fonctionnalité n’est disponible que pour le schéma Destinataires.

1. Pour ajouter une liste de collections à l’interface, cliquez sur le bouton représentant des points de suspension et choisissez **Sélectionner des listes personnalisées**.

   ![Création de listes de collection](assets/schemas-collection1.png)

1. Sélectionnez l’une des listes personnalisées disponibles, par exemple les achats, puis cliquez sur **Confirmer**.

   ![Création de listes de collections](assets/schemas-collection2.png)

1. Accédez au menu **Profils** et filtrez les profils qui ont effectué des achats.

   ![Création de listes de collections](assets/schemas-collection3.png)

1. Cliquez sur un profil. Vous remarquerez que le nouvel onglet s’affiche. Vous pouvez ajouter d’autres colonnes si nécessaire.

   ![Création de listes de collections](assets/schemas-collection4.png)
