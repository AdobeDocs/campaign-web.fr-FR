---
audience: end-user
title: Ajouter des fragments visuels à vos e-mails
description: Découvrir comment ajouter des fragments visuels à vos e-mails
badge: label="Disponibilité limitée"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 64%

---

# Ajouter des fragments visuels à vos e-mails {#use-visual-fragments}

>[!AVAILABILITY]
>
>Cette fonctionnalité est en disponibilité limitée. Celle-ci est limitée aux clientes et aux clients effectuant la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et ne peut pas être déployée dans un autre environnement.

Vous pouvez utiliser un fragment visuel dans une [diffusion e-mail](../email/get-started-email-designer.md) ou dans un [modèle de contenu](../email/use-email-templates.md). Les étapes sont détaillées ci-dessous. [Découvrez comment créer et gérer des fragments de contenu](fragments.md).

![](assets/fragments.gif)

## Utilisation d’un fragment visuel {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Options des fragments"
>abstract="Ce volet fournit des options relatives au fragment sélectionné. Il vous permet de choisir les appareils sur lesquels vous souhaitez que le fragment s’affiche et d’ouvrir le contenu de ce fragment. Utilisez l’onglet **[!UICONTROL Styles]** pour personnaliser davantage votre fragment. Vous pouvez également rompre l’héritage avec le fragment visuel d’origine."

<!-- pas vu dans l'UI-->

Pour insérer un fragment visuel dans un contenu d’email, procédez comme suit :

1. Ouvrez un contenu d’e-mail ou de modèle à l’aide du [Concepteur d’e-mail](../email/get-started-email-designer.md).

1. Sélectionnez l’icône **[!UICONTROL Fragments]** dans le rail de gauche.

   ![](assets/fragments-in-designer.png)

1. La liste de tous les fragments visuels créés sur le sandbox actuel s’affiche. Vous pouvez ainsi effectuer les actions suivantes :

   * Recherchez un fragment spécifique en commençant à saisir son libellé.
   * Triez les fragments par ordre croissant ou décroissant.
   * Modifiez l’affichage des fragments (mode Carte ou Liste).

   >[!NOTE]
   >
   >Les fragments sont triés par date de création : les fragments récemment ajoutés sont affichés en premier dans la liste.

   Si des fragments visuels ont été modifiés ou ajoutés pendant que vous modifiez votre contenu, cliquez sur l’icône **Actualiser** pour mettre à jour la liste avec les dernières modifications.

1. Faites glisser et déposez tout fragment visuel de la liste dans la zone où vous souhaitez l’insérer. Comme tout autre composant, vous pouvez déplacer le fragment dans votre contenu.

1. Sélectionnez le fragment pour afficher ses options dans le volet de droite.

   ![](assets/fragment-right-pane.png)

   Dans l’onglet **[!UICONTROL Paramètres]** vous pouvez effectuer les actions suivantes :

   * Sélectionner les appareils sur lesquels vous souhaitez que le fragment s’affiche.
   * Cliquer sur le bouton **Modifier le contenu** pour ouvrir le contenu de ce fragment. [En savoir plus](../content/fragments.md#edit-fragments)

     Vous pouvez personnaliser davantage votre fragment à l’aide de l’onglet **[!UICONTROL Styles]**.

1. Si nécessaire, vous pouvez rompre l’héritage avec le fragment visuel d’origine. [En savoir plus](#break-inheritance)

   Vous pouvez également supprimer le fragment de votre contenu ou le dupliquer. Ces actions peuvent être effectuées directement à partir du menu contextuel qui s’affiche au-dessus du fragment.

1. Ajoutez autant de fragments visuels que vous le souhaitez et **[!UICONTROL Enregistrez]** vos modifications.

## Rompre l’héritage {#break-inheritance}

Lorsque vous modifiez un fragment visuel, les modifications sont synchronisées. Elles sont automatiquement propagées à toutes les diffusions e-mail et à tous les modèles de contenu contenant ce fragment.

Lorsqu’ils sont ajoutés à un e-mail ou à un modèle de contenu, les fragments sont synchronisés par défaut.

Vous pouvez toutefois rompre l’héritage du fragment d’origine. Dans ce cas, le contenu du fragment est copié dans la conception actuelle et les modifications ne sont plus synchronisées.

Pour rompre l’héritage, procédez comme suit.

1. Sélectionnez le fragment visuel.

1. Cliquez sur l’icône Déverrouiller dans la barre d’outils contextuelle.

   ![](assets/fragment-break-inheritance.png)

1. Ce fragment devient alors un composant autonome qui n’est plus lié au fragment d’origine. Modifiez-le comme tout autre composant de contenu de votre contenu. [En savoir plus](../email/content-components.md)
