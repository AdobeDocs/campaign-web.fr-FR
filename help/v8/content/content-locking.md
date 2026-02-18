---
audience: end-user
product: Campaign
title: Verrouiller du contenu dans les modèles de contenu d’e-mail
description: Découvrez comment verrouiller du contenu dans vos modèles de contenu d’e-mail Adobe Campaign.
feature: Templates
topic: Content Management
role: User
level: Beginner, Intermediate
exl-id: 2835c114-0878-4c41-9071-165d71840941
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 100%

---

# Verrouiller du contenu dans les modèles d’e-mail {#lock-content-email-templates}

>[!CONTEXTUALHELP]
>id="ajo_locking_governance"
>title="Gouvernance"
>abstract="Activez la gouvernance pour verrouiller le contenu dans le modèle, en verrouillant soit l’ensemble du modèle, soit des structures et composants spécifiques. Cela vous permet d’éviter les modifications ou suppressions involontaires, de mieux contrôler la personnalisation des modèles et d’améliorer l’efficacité et la fiabilité de vos campagnes par e-mail."

>[!CONTEXTUALHELP]
>id="ajo_locking_mode"
>title="Mode"
>abstract="Sélectionnez le mode de verrouillage souhaité pour le modèle. Le **Verrouillage du contenu** vous permet de verrouiller des sections spécifiques de contenu dans le modèle. La **Lecture seule** vous permet de verrouiller l’intégralité du contenu du modèle, empêchant toute modification."

>[!CONTEXTUALHELP]
>id="ajo_locking_content_addition"
>title="Activer l’ajout de contenu"
>abstract="Activez cette option pour définir plus précisément comment les personnes peuvent interagir avec le modèle. Sélectionnez **Autoriser l’ajout de structures et de contenu** pour permettre aux utilisateurs et aux utilisatrices d’insérer de nouvelles structures entre celles déjà en place et d’ajouter des composants ou fragments de contenu dans les structures modifiables. **Autoriser l’ajout de contenu uniquement** permet aux utilisateurs et aux utilisatrices d’ajouter des composants ou fragments de contenu dans des structures modifiables, sans possibilité d’ajouter ou de dupliquer des structures."

>[!CONTEXTUALHELP]
>id="ajo_email_locking_activated"
>title="Gouvernance activée"
>abstract="Le verrouillage de contenu est activé et empêche les modifications."

>[!CONTEXTUALHELP]
>id="ajo_email_locking_read_only"
>title="Lecture seule"
>abstract="Ce contenu est en lecture seule et ne peut pas être modifié."

Adobe Campaign permet de verrouiller du contenu dans les modèles d’e-mail, en verrouillant soit l’ensemble du modèle, soit des structures et composants spécifiques. Cela permet d’éviter les modifications ou suppressions involontaires, de mieux contrôler la personnalisation des modèles et d’améliorer l’efficacité et la fiabilité de vos campagnes par e-mail.
<!--
>[!IMPORTANT]
>
>Content locking is an editor-level feature for authors and does not guarantee the content will remain unedited when imported or created through API.-->

Le verrouillage de contenu peut être appliqué au niveau de la **structure** ou au niveau du **composant**. Vous trouverez ci-dessous les principales règles qui s’appliquent au niveau de la structure et du composant lors du verrouillage de contenu dans votre modèle :

* Lorsqu’une structure est verrouillée :

   * Tout le contenu de cette structure est également verrouillé par défaut.
   * Aucun contenu ne peut être ajouté à la structure.
   * Par défaut, vous ne pouvez pas supprimer la structure. Vous pouvez contourner cette restriction en activant l’option « Autoriser la suppression ».
   * Les composants de contenu individuels de la structure verrouillée peuvent être définis comme modifiables.

* Lorsqu’une structure est modifiable (structure non verrouillée) :

   * Les composants de contenu individuels peuvent être verrouillés dans cette structure.
   * Par défaut, vous ne pouvez pas supprimer un composant s’il est verrouillé ou si l’option « Verrouillage de contenu modifiable uniquement » est sélectionnée. Vous pouvez contourner cette restriction en activant l’option « Autoriser la suppression ».

>[!AVAILABILITY]
>
>Les personnes autorisées à créer des modèles de contenu peuvent activer le verrouillage de contenu.

<!--
➡️ [Discover this feature in video](#video)-->

## Verrouiller un modèle d’e-mail {#define}

### Activer le verrouillage de contenu {#enable}

Vous pouvez activer le verrouillage de contenu pour un modèle d’e-mail directement dans le Concepteur d’e-mail, que vous créiez un nouveau modèle ou en modifiiez un existant. Procédez comme suit :

1. Ouvrez ou créez un modèle d’e-mail et accédez à l’écran d’édition de contenu dans le [Concepteur d’e-mail](../email/get-started-email-designer.md).

1. Dans le volet **[!UICONTROL Corps]** à droite, activez l’option **[!UICONTROL Gouvernance]**.

1. Dans la liste déroulante **[!UICONTROL Mode]**, sélectionnez le mode de verrouillage souhaité pour le modèle :

   * **[!UICONTROL Verrouillage de contenu]** : verrouillez des sections spécifiques de contenu dans le modèle. Par défaut, toutes les structures et tous les composants deviennent modifiables. Vous pouvez ensuite choisir de verrouiller certains éléments individuels.
   * **[!UICONTROL Lecture seule]** : verrouillez l’intégralité du contenu du modèle et empêchez toute modification.

   ![](assets/template-lock-enable.png)

1. Si vous avez sélectionné le mode **[!UICONTROL Verrouillage de contenu]**, vous pouvez définir plus en détail la manière dont les utilisateurs et utilisatrices peuvent interagir avec le modèle. Activez l’option **[!UICONTROL Activer l’ajout de contenu]**, puis choisissez l’une des options suivantes :

   * **[!UICONTROL Autoriser l’ajout de structures et de contenu]** : les utilisateurs et les utilisatrices peuvent insérer de nouvelles structures entre celles déjà en place et ajouter des composants ou fragments de contenu dans les structures modifiables.

   * **[!UICONTROL Autoriser l’ajout de contenu uniquement]** : les utilisateurs et les utilisatrices peuvent ajouter des composants ou fragments de contenu dans des structures modifiables, sans possibilité d’ajouter ou de dupliquer des structures.

1. Après avoir sélectionné le mode de verrouillage, vous pouvez définir les structures et/ou composants à verrouiller si vous avez sélectionné le mode **[!UICONTROL Verrouillage de contenu]** :

   * [Découvrir comment verrouiller des structures](#lock-structures)
   * [Découvrir comment verrouiller des composants](#lock-components)

   Si vous avez choisi le mode **[!UICONTROL Lecture seule]**, finalisez et enregistrez votre modèle comme vous le faites habituellement.

Vous pouvez régler les paramètres de **[!UICONTROL gouvernance]** à tout moment lors de la conception de votre modèle en sélectionnant le corps du modèle. Pour ce faire, cliquez sur le lien **[!UICONTROL Corps]** dans le rail de navigation situé en haut du volet droit.

![](assets/template-lock-body.png)

### Verrouiller des structures {#lock-structures}

>[!CONTEXTUALHELP]
>id="ajo_locking_structure"
>title="Verrouillage du contenu dans la structure"
>abstract="Pour verrouiller la structure dans le modèle, sélectionnez **Verrouillé** dans la liste déroulante **Type de verrouillage**. Par défaut, les utilisateurs et les utilisatrices ne peuvent pas supprimer les structures verrouillées. Vous pouvez contourner cette restriction en activant l’option **[!UICONTROL Autoriser la suppression]**."

Pour verrouiller une structure dans votre modèle :

1. Sélectionnez la structure à verrouiller.

1. Dans la liste déroulante **[!UICONTROL Type de verrouillage]**, choisissez **[!UICONTROL Verrouillé]**.

   ![](assets/template-lock-structure.png)

   >[!NOTE]
   >
   >Par défaut, les utilisateurs et les utilisatrices ne peuvent pas supprimer les structures verrouillées. Vous pouvez contourner cette restriction en activant l’option **[!UICONTROL Autoriser la suppression]**.

Une fois qu’une structure est verrouillée, aucun autre composant ou fragment de contenu ne peut être dupliqué ou ajouté à l’intérieur de celle-ci. Tous les composants d’une structure verrouillée sont également verrouillés par défaut. Pour rendre un composant modifiable dans une structure verrouillée :

1. Sélectionnez le composant à déverrouiller.

1. Activez l’option **[!UICONTROL Utiliser un verrouillage spécifique]**.

1. Dans la liste déroulante **[!UICONTROL Type de verrouillage]**, choisissez **[!UICONTROL Modifiable]**. Pour autoriser la modification du contenu lors du verrouillage des styles, sélectionnez **[!UICONTROL Contenu modifiable uniquement]**. [Découvrir comment verrouiller des composants](#lock-components)

   ![](assets/template-lock-editable-component.png)

### Verrouiller des composants {#lock-components}

>[!CONTEXTUALHELP]
>id="ajo_locking_component"
>title="Utiliser un verrouillage spécifique dans le composant"
>abstract="Pour verrouiller le composant dans le modèle, activez l’option **Utiliser le verrouillage spécifique**. Dans la liste déroulante **[!UICONTROL Type de verrouillage]**, sélectionnez l’option de verrouillage souhaitée : **Verrouillage de contenu modifiable uniquement** permet de verrouiller les styles du composant tout en autorisant la modification du contenu, tandis que **Verrouillé** verrouille entièrement le contenu et les styles du composant."

Pour verrouiller un composant spécifique dans une structure :

1. Sélectionnez le composant et activez l’option **[!UICONTROL Utiliser un verrouillage spécifique]** dans le volet de droite.

1. Dans la liste déroulante **[!UICONTROL Type de verrouillage]**, sélectionnez l’option de verrouillage de votre choix :

   ![](assets/template-lock-component.png)

   * **[!UICONTROL Contenu modifiable uniquement]** : verrouillez les styles du composant, mais autorisez la modification du contenu.
   * **[!UICONTROL Verrouillé]** : verrouillez entièrement le contenu et les styles du composant.

   >[!NOTE]
   >
   >Le type de verrouillage **[!UICONTROL modifiable]** permet aux utilisateurs et aux utilisatrices de modifier un composant, même dans une structure verrouillée. [Découvrir comment verrouiller des structures](#lock-structures)

1. Par défaut, les utilisateurs et les utilisatrices ne peuvent pas supprimer des composants verrouillés. Vous pouvez activer la suppression en activant l’option **[!UICONTROL Autoriser la suppression]**.

### Identifier du contenu verrouillé {#identify}

Pour identifier facilement les structures et les composants verrouillés dans votre modèle, utilisez l’**[!UICONTROL arborescence de navigation]** située dans le menu de gauche. Ce menu donne un aperçu visuel de tous les éléments du modèle, en mettant en évidence les éléments verrouillés avec une icône de verrou et les éléments modifiables avec une icône en forme de crayon.

Dans l’exemple ci-dessous, la gouvernance est activée pour le corps du modèle. La *structure 2* est verrouillée et le *composant 1* est modifiable, tandis que la *structure 3* est entièrement verrouillée.

![](assets/template-lock-navigation.png)

## Utilisation de modèles avec du contenu verrouillé {#use}

>[!CONTEXTUALHELP]
>id="ajo_email_editable_areas"
>title="Mise en surbrillance des zones modifiables"
>abstract="Selon le type de verrouillage appliqué au modèle, vous pouvez effectuer différentes actions sur les structures et composants du modèle. Pour identifier rapidement toutes les zones modifiables dans le modèle, activez l’option **[!UICONTROL Mettre en surbrillance les zones modifiables]**."

Lors de l’utilisation d’un modèle avec du contenu verrouillé, un message s’affiche dans le volet de droite.

Selon le type de verrouillage appliqué au modèle, vous pouvez effectuer différentes actions sur les structures et composants du modèle. Pour identifier rapidement toutes les zones modifiables dans le modèle, activez l’option **[!UICONTROL Mettre en surbrillance les zones modifiables]**.

Par exemple, dans le modèle ci-dessous, toutes les zones sont modifiables, à l’exception de l’image supérieure qui a été verrouillée, ce qui signifie que vous ne pouvez pas la modifier ni la supprimer.

![](assets/template-lock-highlight.png)

Vous trouverez des informations détaillées sur les différents types de verrouillage pouvant être appliqués dans les sections suivantes :

* [Verrouiller des structures](#lock-structures)
* [Verrouiller des composants](#lock-components)

Voici quelques exemples de modifications d’e-mail et des configurations de verrouillage de contenu associées qui ont été configurées :

| Type de verrouillage du contenu | Configuration du modèle | Modification d’e-mail |
| ------- | ------- | ------- |
| Modèle de contenu en lecture seule | ![](assets/locking-sample-read-only-conf.png){zoomable="yes"} | ![](assets/locking-sample-read-only.png){zoomable="yes"} |
| L’intégralité du contenu est modifiable, mais les utilisateurs et les utilisatrices ne peuvent pas ajouter de structure ni de composant. | ![](assets/locking-sample-no-addition-conf.png){zoomable="yes"} | ![](assets/locking-sample-no-addition.png){zoomable="yes"} |
| Structure verrouillée ne pouvant pas être supprimée. | ![](assets/locking-sample-structure-locked-conf.png){zoomable="yes"} | ![](assets/locking-sample-structure-locked.png){zoomable="yes"} |
| Composant avec styles verrouillés. Les utilisateurs et les utilisatrices peuvent uniquement modifier le contenu. | ![](assets/locking-sample-content-only-conf.png){zoomable="yes"} | ![](assets/locking-sample-content-only.png){zoomable="yes"} |
| Composant modifiable dans une structure verrouillée. | ![](assets/locking-sample-editable-component-conf.png){zoomable="yes"} | ![](assets/locking-sample-editable-component.png){zoomable="yes"} |

<!--
TO REPLACE WITH VIDEO FOR CAMPAIGN IF/WHEN CREATED

## How-to video {#video}

Learn how to lock content in email templates.

>[!VIDEO](https://video.tv.adobe.com/v/3451591?quality=12)-->
