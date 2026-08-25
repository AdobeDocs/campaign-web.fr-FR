---
audience: end-user
title: Ajouter une liste modifiable au schéma d’offre
description: Découvrez comment afficher un lien vers une collection personnalisée sous la forme d’une liste modifiable directement dans l’écran des détails de l’offre.
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 043cc60da1938800404964aa7e698f959ef908fd
workflow-type: ht
source-wordcount: 449
ht-degree: 100%

---

# Ajouter une liste modifiable au schéma d’offre {#offer-editable-list}

Lorsque vous [étendez le schéma  [!DNL nms:offer] ](../administration/schemas.md) avec un lien de collection personnalisée, tel qu’un ensemble de segments liés à une offre, vous pouvez l’exposer en tant que liste modifiable directement dans la section **[!UICONTROL Options personnalisées]** de l’offre. Au lieu de gérer les enregistrements associés via un écran distinct, la collection est affichée sous forme de liste dans les détails de l’offre, et vous pouvez créer de nouveaux enregistrements associés directement dans cette liste, via une boîte de dialogue dédiée.

>[!NOTE]
>
>Actuellement, cette fonctionnalité n’est disponible que pour le schéma d’offre.

## Ajouter un champ de lien de collection {#add-field}

1. Étendez le schéma [!DNL nms:offer] avec votre collection personnalisée, puis accédez au menu **[!UICONTROL Schémas]**, ouvrez le schéma **[!UICONTROL Offres marketing]** et cliquez sur **[!UICONTROL Modification de l’écran]**. [En savoir plus](../administration/schemas-browse-access.md#screen-def).

   ![Copie d’écran montrant le bouton de définition d’écran.](assets/offers-editable-list.png){zoomable="yes"}

1. Dans la section **[!UICONTROL Configuration de l’écran des détails]**, cliquez sur l’icône représentant des points de suspension au-dessus du tableau **[!UICONTROL Liste des champs personnalisés]**, puis sélectionnez **[!UICONTROL Sélectionner les attributs]**. [En savoir plus](../administration/schemas-custom-fields.md).

   ![Copie d’écran montrant le bouton de définition d’écran.](assets/offers-editable-list-0.png){zoomable="yes"}

1. Parcourez les attributs et sélectionnez votre lien de collection personnalisée, identifié par son icône de collection.

   ![Copie d’écran affichant le sélecteur d’attributs avec un attribut de lien de collection.](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >Les champs de lien de collection ne peuvent pas être rendus obligatoires et ne prennent pas en charge les sous-attributs. Par défaut, ils occupent deux colonnes du formulaire.

1. Confirmez votre sélection. Le lien de collection est ajouté au tableau **[!UICONTROL Liste des champs personnalisés]** avec pour type **[!UICONTROL collection]**.

   ![Copie d’écran affichant les attributs ajoutés.](assets/offers-editable-list-2.png){zoomable="yes"}

## Configurer la liste modifiable de la collection {#configure-list}

1. Cliquez sur l’icône des points de suspension sur la ligne du champ de collection et choisissez **[!UICONTROL Modifier]** pour ouvrir la boîte de dialogue **[!UICONTROL Paramètres des liens de collection]**.

   ![Copie d’écran affichant le bouton Modifier.](assets/offers-editable-list-3.png){zoomable="yes"}

1. Dans l’onglet **[!UICONTROL Général]**, vous pouvez éventuellement définir une condition **[!UICONTROL Visible si]** ou activer l’option **[!UICONTROL Lecture seule]**.

   ![Copie d’écran affichant l’écran de modification.](assets/offers-editable-list-4.png){zoomable="yes"}

1. Dans l’onglet **[!UICONTROL Configuration de l’écran]**, cliquez sur **[!UICONTROL Sélectionner les attributs]** et sélectionnez les attributs à utiliser lors de l’ajout d’un nouvel élément à la liste, par exemple un nom de segment et un champ personnalisé.

   ![Copie d’écran affichant l’onglet Configuration de l’écran de la boîte de dialogue Paramètres des liens de collection.](assets/offers-editable-list-5.png){zoomable="yes"}

1. Sous l’onglet **[!UICONTROL Disposition]**, conservez ou effacez **[!UICONTROL Étendre sur deux colonnes]**.

1. Cliquez sur **[!UICONTROL Confirmer]**, puis sur **[!UICONTROL Enregistrer]** la définition d’écran.

## Utiliser la liste modifiable dans une offre {#use-list}

1. Dans le menu de gauche, cliquez sur **Offres** et ouvrez une offre. [En savoir plus](create-offer.md#create)

   ![Copie d’écran affichant l’écran d’offre.](assets/offers-editable-list-7.png){zoomable="yes"}

1. Accédez aux propriétés de l’offre. La collection est rendue sous forme de liste dans la section **Options personnalisées**.

   ![Copie d’écran affichant le rendu de liste modifiable dans l’écran des détails de l’offre.](assets/offers-editable-list-6.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Ajouter]** pour afficher les attributs que vous avez configurés, renseignez-les, puis cliquez sur **[!UICONTROL Confirmer]**. Le nouvel élément est ajouté à la liste.

   Vous pouvez ajouter plusieurs éléments à la même liste, et le détail de l’offre peut contenir plusieurs listes modifiables.

1. Cliquez sur **[!UICONTROL Enregistrer]**.

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->