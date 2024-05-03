---
audience: end-user
title: Utiliser les fragments
description: Découvrez comment utiliser des fragments
hidefromtoc: true
source-git-commit: a882087bc608ea4029e53ed38ecf699e127be065
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 4%

---

# Utiliser les fragments {#fragments}


>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Définition de vos propres fragments"
>abstract="Un fragment est un composant réutilisable pouvant être référencé dans un ou plusieurs emails à l’échelle des campagnes."

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Enregistrement de fragments"
>abstract="Enregistrement de fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Définition de vos propres fragments"
>abstract="Un fragment est un composant réutilisable pouvant être référencé dans un ou plusieurs emails à l’échelle des campagnes."

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Propriétés des fragments"
>abstract="Propriétés des fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Type de fragment"
>abstract="Sélectionnez le type de fragment. Pour l’instant, seuls les fragments visuels pour les emails sont disponibles."

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Définition de vos propres fragments"
>abstract="Un fragment est un composant réutilisable pouvant être référencé dans un ou plusieurs emails à l’échelle des campagnes. Vous pouvez également utiliser des fragments dans vos modèles d’email. Pour l’instant, seuls les fragments visuels sont disponibles."

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Détails des fragments"
>abstract="Détails des fragments"

>[!CONTEXTUALHELP]
>id="acw_create_fragment"
>title="Définition de vos propres fragments"
>abstract="Un fragment est un composant réutilisable pouvant être référencé dans un ou plusieurs emails à l’échelle des campagnes."

Un fragment est un composant réutilisable pouvant être référencé dans un ou plusieurs emails à l’échelle des campagnes. Lors de la modification d’un fragment, chaque contenu qui l’utilise est mis à jour.

Cette fonctionnalité permet de précréer plusieurs blocs de contenu personnalisés qui peuvent être utilisés par les utilisateurs marketing pour assembler rapidement les contenus d’email dans un processus de conception amélioré.

![](assets/fragments.gif)


Pour optimiser l’utilisation des fragments :

* Créez vos propres fragments visuels, comme décrit ci-dessous.
* Utilisez-les autant de fois que nécessaire dans votre contenu, via le Concepteur d&#39;email. Voir [Ajout de fragments visuels à vos emails](../email/use-visual-fragments.md).

## Création d’un fragment visuel {#create-fragments}

Vous pouvez créer des fragments de deux manières différentes :

* Créez un fragment à partir de zéro, à l’aide de la fonction **[!UICONTROL Fragments]** menu dédié. [Voici comment procéder](#create-from-scratch).

* Lors de la conception de contenu, enregistrez une partie de votre contenu en tant que fragment. [Voici comment procéder](#save-as-fragment).

Une fois enregistré, votre fragment peut être utilisé dans un email ou un modèle d’email. Qu’il soit créé à partir de zéro ou d’un contenu existant, vous pouvez désormais utiliser ce fragment lors de la création de tout contenu dans Campaign. Voir [Ajout de fragments visuels](../email/use-visual-fragments.md).

### Créer un fragment à partir de zéro {#create-from-scratch}

Pour créer un fragment à partir de zéro, procédez comme suit.

1. [Accès à la liste des fragments](#access-manage-fragments) par le biais du **[!UICONTROL Gestion de contenu]** > **[!UICONTROL Fragments]** menu de gauche.

   ![](assets/fragments-list.png)

1. Sélectionner **[!UICONTROL Créer un fragment]**.

1. Saisissez le libellé du fragment.

   ![](assets/fragment-create.png)

1. Si nécessaire, vous pouvez définir d’autres options, telles que le nom interne du fragment, son dossier et une description.

   >[!NOTE]
   >
   >Pour l’instant, vous ne pouvez créer que des fragments visuels.

1. Cliquez sur le bouton **Créer** pour configurer le contenu de votre fragment.

1. Le [Concepteur d’e-mail](../email/get-started-email-designer.md) s’affiche. Modifiez votre contenu selon vos besoins, comme vous le feriez pour tout email au sein d’une campagne. Vous pouvez ajouter des images, des liens, des champs de personnalisation et du contenu dynamique.

   ![](assets/fragment-designer.png)

1. Une fois votre fragment prêt, cliquez sur **[!UICONTROL Enregistrer et fermer]**. Il est ajouté à la variable [liste de fragments](#access-manage-fragments).

Ce fragment est maintenant prêt à être utilisé lors de la création d’un [email](../email/get-started-email-designer.md) ou [modèle de contenu](use-email-templates.md) dans Campaign. [Voici comment procéder](../email/use-visual-fragments.md).


### Enregistrement d’un contenu en tant que fragment {#save-as-fragment}

Tout contenu d’email peut être enregistré en tant que fragment en vue d’une réutilisation ultérieure. Lors de la conception d’une [modèle de contenu](use-email-templates.md) ou [email](../email/get-started-email-designer.md) vous pouvez enregistrer une partie de votre contenu en tant que fragment visuel. Pour ce faire, procédez comme suit :

1. Dans le [Concepteur d&#39;email](../email/get-started-email-designer.md), cliquez sur le **Plus** en haut à droite de l’écran.

1. Sélectionner **[!UICONTROL Enregistrer en tant que fragment]** dans le menu déroulant.

   ![](assets/fragment-save-as.png)

1. La variable **[!UICONTROL Enregistrer en tant que fragment]** s’affiche. Sélectionnez ensuite les éléments que vous souhaitez inclure dans votre fragment, notamment les champs de personnalisation et le contenu dynamique.

   >[!CAUTION]
   >
   >Vous ne pouvez sélectionner que les sections adjacentes. Vous ne pouvez pas sélectionner une structure vide ou un autre fragment.

   ![](assets/fragment-save-as-screen.png)

1. Cliquez sur **[!UICONTROL Créer]**. Renseignez le nom du fragment et enregistrez-le.

   ![](assets/fragment-save-confirm.png)

   Ce contenu est désormais un fragment autonome ajouté à la variable [liste de fragments](#manage-fragments)et accessible à partir du menu dédié. Vous pouvez désormais utiliser ce fragment lors de la création d’un [email](../email/get-started-email-designer.md) ou [modèle de contenu](use-email-templates.md) dans Campaign. [Voici comment procéder](../email/use-visual-fragments.md).

>[!NOTE]
>
>Toute modification apportée à ce nouveau fragment n’est pas propagée dans l’email ou le modèle d’origine. De même, lorsque le contenu d’origine est modifié dans cet email ou ce modèle, le nouveau fragment n’est pas modifié.

## Gestion des fragments {#manage-fragments}

Vous pouvez modifier, mettre à jour, dupliquer ou supprimer un fragment de la liste des fragments.

### Modification et mise à jour d’un fragment {#edit-fragments}

Pour modifier un fragment, procédez comme suit.

1. Cliquez sur le nom du fragment à modifier dans la **[!UICONTROL Fragments]** liste.
1. Cliquez sur le bouton **Modifier le contenu** pour ouvrir le contenu de ce fragment.

   ![](assets/fragment-edit-content.png)

1. Effectuez les modifications nécessaires et enregistrez vos modifications.

>[!CAUTION]
>
>Toute modification apportée à un fragment est propagée aux diffusions email ou aux modèles qui l’utilisent.


### Suppression d’un fragment {#delete-fragments}

Pour supprimer un fragment, procédez comme suit :

1. Accédez à la liste des fragments, puis cliquez sur le bouton **[!UICONTROL Autres actions]** en regard du fragment à supprimer.
1. Cliquez sur **Supprimer** et confirmez.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Lors de la suppression d’un fragment de contenu, les diffusions email et les modèles qui l’utilisent sont mis à jour et le fragment est supprimé du contenu de leur message. Vous pouvez interrompre l’héritage si nécessaire. [En savoir plus](use-visual-fragments.md#break-inheritance)
>

### Dupliquer un fragment {#duplicate-fragments}

Vous pouvez facilement dupliquer un fragment pour en créer un nouveau. Pour dupliquer un fragment existant, procédez comme suit :

1. Accédez à la liste des fragments, puis cliquez sur le bouton **[!UICONTROL Autres actions]** en regard du fragment à supprimer.
1. Cliquez sur **Dupliquer** et confirmez.
1. Saisissez le libellé du nouveau fragment et enregistrez vos modifications.

   Le fragment est ajouté à la liste des fragments. Vous pouvez la modifier et la configurer selon vos besoins.
