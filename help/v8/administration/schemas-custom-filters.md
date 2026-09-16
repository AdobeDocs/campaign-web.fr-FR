---
title: Ajouter des filtres personnalisés
description: Découvrez comment ajouter des filtres personnalisés en tant que champs d’accès rapide dans le volet Filtres d’une vue Liste.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 100%
---
# Ajouter des filtres personnalisés {#custom-filters}

La section **[!UICONTROL Configuration de la liste d’inventaire]** > **[!UICONTROL Filtres personnalisés]** vous permet de choisir les attributs qui s’affichent en tant que champs d’accès rapide dans le volet [Filtres](../query/filter.md) de la vue Liste d’un schéma, au-dessus du créateur de règles de **[!UICONTROL Filtres avancés]**.

Pour plus d’informations sur l’écran de définition d’écran et la façon d’y accéder, consultez la section [Accéder à la définition d’écran](schemas-browse-access.md#screen-def).

## Ajouter des filtres personnalisés {#add}

1. Accédez au menu **[!UICONTROL Schémas]** et recherchez les schémas modifiables à l’aide des filtres.

1. Sélectionnez le nom du schéma dans la liste pour l’ouvrir et cliquez sur le bouton **[!UICONTROL Modification d’écran]** dans la vue des détails du schéma pour accéder à la définition d’écran.

1. Accédez à la section **[!UICONTROL Configuration de la liste d’inventaire]**, cliquez sur l’icône représentant des points de suspension au-dessus du tableau **[!UICONTROL Filtres personnalisés]**, puis sélectionnez **[!UICONTROL Sélectionner les attributs]**.

   ![Sélection des filtres personnalisés](assets/schemas-custom-filters1.png)

1. Sélectionnez un ou plusieurs attributs et confirmez.

   Vous pouvez sélectionner les éléments suivants :

   * Un attribut direct du schéma, par exemple un code ou une catégorie.
   * Un attribut de lien, par exemple une marque liée à un produit. Dans ce cas, le filtre utilise un sélecteur de recherche limité au schéma lié.
   * Un sous-attribut d’un lien, par exemple le nom complet d’un dossier lié ou l’adresse e-mail d’une personne destinataire liée.

   ![Sélecteur d’attributs affichant les attributs directs et les sous-attributs de lien](assets/schemas-custom-filters2.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**. Vous pouvez réorganiser les filtres personnalisés à l’aide des flèches vers le haut et vers le bas ou en les faisant glisser. Pour supprimer un filtre, cliquez sur l’icône des points de suspension sur sa ligne et sélectionnez **[!UICONTROL Supprimer]**.

1. Accédez à la liste des enregistrements de ce schéma et ouvrez le volet Filtres. Les attributs que vous avez sélectionnés s’affichent sous la forme de **[!UICONTROL Filtres personnalisés]**, au-dessus du créateur de règles de **[!UICONTROL Filtres avancés]**.

   ![Filtres personnalisés affichés dans le volet Filtres](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >Un filtre personnalisé basé sur un attribut de date ou de date et d’heure s’affiche sous la forme d’un sélecteur de période.

1. Saisissez ou sélectionnez une valeur dans l’un des filtres personnalisés pour affiner la liste.

## Limiter les valeurs d’un filtre personnalisé de type lien {#settings}

Dans le cas d’un filtre personnalisé basé sur un attribut de lien, vous pouvez limiter les valeurs disponibles dans le sélecteur.

>[!NOTE]
>
>L’option **[!UICONTROL Modifier]** décrite ci-dessous n’est disponible que pour les filtres personnalisés basés sur un attribut de lien. Les filtres personnalisés basés sur d’autres types d’attributs peuvent uniquement être réorganisés ou supprimés.

1. Sur la ligne d’un filtre personnalisé de type lien, cliquez sur l’icône des points de suspension et sélectionnez **[!UICONTROL Modifier]**.

   ![Option d’édition sur un filtre personnalisé de type lien](assets/schemas-custom-filters4.png)

1. Dans l’onglet **[!UICONTROL Paramètres de filtre]**, cliquez sur **[!UICONTROL Modifier le filtre]** et utilisez le concepteur de requête pour définir une condition qui limite les valeurs disponibles dans le sélecteur. Par exemple, limitez un filtre de diffusion aux diffusions utilisant le canal e-mail.

   ![Onglet Paramètres de filtre dans la boîte de dialogue Paramètres du lien](assets/schemas-custom-filters5.png)

1. Validez vos modifications.
