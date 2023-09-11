---
title: Créer et utiliser des filtres prédéfinis
description: Découvrez comment créer et gérer des filtres prédéfinis dans l’interface utilisateur web d’Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
source-git-commit: 5c7d60b3f59de2a5176a55d9556a3f1c6d2a7651
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 3%

---

# Utilisation de filtres prédéfinis {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Gestion des filtres prédéfinis"
>abstract="Le web de Campaign vous offre désormais une interface conviviale pour gérer et personnaliser facilement des filtres prédéfinis en fonction de vos besoins spécifiques. Créez une fois et enregistrez pour une utilisation ultérieure."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Filtres prédéfinis"
>abstract="Le web de Campaign vous offre désormais une interface conviviale pour gérer et personnaliser facilement des filtres prédéfinis en fonction de vos besoins spécifiques. Créez une fois et enregistrez pour une utilisation ultérieure."

Les filtres prédéfinis sont des filtres personnalisés qui sont créés et enregistrés afin d’être disponibles pour une utilisation ultérieure. Ils peuvent être utilisés comme raccourcis lors d’opérations de filtrage avec le créateur de règles, par exemple lors du filtrage d’une liste de données ou de la création de l’audience d’une diffusion.

Vous pouvez utiliser des filtres intégrés existants pour accéder à un sous-ensemble spécifique de vos données, ou créer vos propres filtres prédéfinis et les enregistrer.


## Créer un filtre prédéfini {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Créer un filtre prédéfini"
>abstract="Saisissez un libellé pour le filtre prédéfini et sélectionnez le tableau auquel il s&#39;applique. Ouvrez les options supplémentaires pour ajouter une description et définir ce filtre comme favori. Utilisez ensuite le bouton &quot;Créer une règle&quot; pour définir les conditions de filtrage."

Lors de la création d’un filtre à l’aide du créateur de règles, vous pouvez l’enregistrer pour une utilisation ultérieure. Lorsqu’il est enregistré en tant que filtre personnalisé, il peut être utilisé ultérieurement. Vous pouvez également créer et modifier un filtre prédéfini à partir du menu dédié dans le volet de navigation de gauche.

![](assets/predefined-filters-menu.png)

Pour enregistrer un filtre personnalisé dans le créateur de règles, procédez comme suit :

1. Ouvrez le créateur de règles et définissez vos conditions de filtrage. Dans l&#39;exemple ci-dessous, vous filtrez les destinataires qui vivent à Madrid.
1. Cliquez sur le bouton **Sélectionner ou enregistrer un filtre** et sélectionnez **Enregistrer en tant que filtre**.

   ![](assets/predefined-filters-save.png)

1. Sélectionner **Créer un nouveau filtre**, puis saisissez un nom et une description pour ce filtre.

   ![](assets/predefined-filters-save-filter.png)

1. (facultatif) Activez la variable **Enregistrer en tant que favori** si vous souhaitez voir ce filtre prédéfini dans vos favoris.


   Lorsqu’un filtre est enregistré comme favori, il est disponible pour tous les utilisateurs de la variable **Filtres favoris** de la liste de création de filtre, comme illustré ci-dessous :

   ![](assets/predefined-filters-favorite.png)


1. Cliquez sur **Confirmer** pour sauvegarder vos changements.

Votre filtre personnalisé est désormais disponible dans la **Filtres prédéfinis** Liste et accessible à tous les utilisateurs de Campaign.

Vous pouvez également créer un filtre à partir du **Filtres prédéfinis** dans le menu de gauche. Pour ce faire, suivez les étapes ci-après :

1. Parcourez les **Filtres prédéfinis** dans le menu de gauche.
1. Cliquez sur le bouton **Créer un filtre** bouton .
1. Saisissez le nom du filtre et, dans la **Type de document** , sélectionnez le schéma auquel il s’applique. Le schéma par défaut est : `Recipients(nms)`.
1. Définissez la règle pour le filtre. Par exemple, les profils de plus de 30 ans.

   ![](assets/filter-30+.png)

1. Enregistrez vos modifications. Le filtre est ajouté à la liste des filtres prédéfinis.

## Utiliser un filtre prédéfini {#use-predefined-filter}

Les filtres prédéfinis sont disponibles lors de la définition des propriétés de règle. Pour accéder aux filtres prédéfinis, choisissez la **Sélectionner un filtre personnalisé** dans la liste déroulante du créateur de règles.

Vous pouvez ensuite accéder à la liste complète des filtres prédéfinis disponibles pour le contexte actuel.

Vous pouvez également utiliser les raccourcis de filtrage disponibles dans la **Filtres favoris** de la liste déroulante.


Par exemple, pour créer une audience à partir d’un filtre prédéfini, procédez comme suit :

1. Parcourez les **Audiences** dans le menu de gauche.
1. Cliquez sur le bouton **Création d’une audience** bouton .
1. Saisissez le nom de l’audience, puis cliquez sur le bouton **Création d’une audience** bouton .
1. Sélectionnez la variable **Requête** activité, puis, dans le volet de droite, cliquez sur **Créer une audience** bouton .

   ![](assets//build-audience-from-filter.png)

1. Dans la **Bouton Sélectionner ou enregistrer un filtre**, choisissez la variable **Sélectionner un filtre personnalisé** .

   ![](assets/build-audience-select-custom-filter.png)

1. Accédez au filtre prédéfini à utiliser pour créer l’audience, sélectionnez-la et confirmez-la.

   ![](assets/build-audience-filter-list.png)

1. Vérifiez les propriétés de la règle pour ce filtre et confirmez.

   ![](assets/build-audience-check.png)

   Le filtre est désormais utilisé comme requête dans la variable **Requête** activité.

   ![](assets/build-audience-confirm.png)

1. Enregistrez vos modifications et cliquez sur le bouton **Début** pour créer l’audience et la rendre disponible dans la liste des audiences.

## Gestion des filtres prédéfinis {#manage-predefined-filter}

Les filtres prédéfinis sont tous regroupés dans l’entrée dédiée du menu de navigation de gauche.

Dans cette liste, vous pouvez créer un nouveau filtre, comme décrit ci-dessus, et :

* modifier un filtre existant, puis modifier ses règles et ses propriétés ;
* dupliquer un filtre prédéfini
* suppression d’un filtre prédéfini

## Filtres prédéfinis intégrés {#ootb-predefined-filter}

Campaign est fourni avec un ensemble de filtres prédéfinis, créés à partir de la console cliente. Ces filtres peuvent être utilisés pour définir vos audiences et règles. Ils ne doivent pas être modifiés.
