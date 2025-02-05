---
title: Utiliser les codes JavaScript
description: Découvrez comment utiliser les codes JavaScript.
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---


# Utiliser les codes JavaScript {#javascript-codes}

<!-- JavaScript codes -->

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_list"
>title="Codes JavaScript"
>abstract="Codes JavaScript"

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_create"
>title="Créer du code JavaScript"
>abstract="Créer du code JavaScript"

## À propos des codes JavaScript {#about}

Les codes JavaScript vous permettent de créer des fonctions réutilisables qui peuvent être utilisées dans l’ensemble des workflows, comme une bibliothèque. Ces fonctions sont stockées dans le menu **[!UICONTROL Administration]** > **[!UICONTROL Codes JavaScript]** dans le volet de navigation de gauche.

![](assets/javascript-list.png)

À partir de la liste des codes JavaScript, vous pouvez :

* **Dupliquer ou supprimer un code** : cliquez sur le bouton représentant des points de suspension et sélectionnez l’action souhaitée.
* **Modifier un code** : cliquez sur le nom d’un code pour ouvrir ses propriétés. Apportez vos modifications et enregistrez-les.
* **Créer un nouveau code JavaScript** : cliquez sur le bouton **[!UICONTROL Créer un code JavaScript]**.

>[!NOTE]
>
>Bien que l’emplacement du menu Codes JavaScript diffère entre la console Adobe Campaign et l’interface utilisateur web, la liste est identique et fonctionne comme un miroir.

## Création d’un code JavaScript {#create}

Pour créer un code JavaScript, procédez comme suit :

1. Accédez au menu **[!UICONTROL Codes JavaScript]** et cliquez sur le bouton **[!UICONTROL Créer un code JavaScript]**.

1. Définissez les propriétés du code :

   * **[!UICONTROL Espace de noms]** : spécifiez l’espace de noms pertinent pour vos ressources personnalisées. Par défaut, l’espace de noms est « cus », mais il peut varier en fonction de votre implémentation.
   * **[!UICONTROL Name]** : identifiant unique à utiliser pour référencer le code.
   * **[!UICONTROL Libellé]** : libellé descriptif à afficher dans la liste des codes JavaScript.

   ![](assets/javascript-create.png)

   >[!NOTE]
   >
   >Une fois créés, les champs **[!UICONTROL Espace de noms]** et **[!UICONTROL Nom]** ne peuvent pas être modifiés. Pour apporter des modifications, dupliquez le code et mettez-le à jour si nécessaire.
   >
   >Dans la console Campaign, le nom de code JavaScript s’affiche sous la forme d’une concaténation de ces deux champs.

1. Cliquez sur le bouton **[!UICONTROL Créer un code]** pour définir le code JavaScript. Le volet de gauche propose deux menus qui vous permettent d&#39;utiliser des fonctions prédéfinies liées à des conditions et à la mise en forme des dates.

   ![](assets/javascript-code.png)

1. Cliquez sur **[!UICONTROL Confirmer]** pour enregistrer votre code.

1. Lorsque votre code JavaScript est prêt, cliquez sur **[!UICONTROL Créer]**.  Le code JavaScript peut désormais être utilisé dans tous les workflows.

## Utiliser un code JavaScript d’un workflow {#workflow}

### Chargement des bibliothèques de code JavaScript {#library}

Vous pouvez référencer des codes JavaScript dans les workflows afin d’éviter de réécrire du code pour des tâches répétitives. Pour utiliser ces codes, vous devez d’abord charger la bibliothèque correspondante dans le script d’initialisation du workflow. Cela vous permet de charger toutes les bibliothèques contenant les fonctions que vous souhaitez utiliser dans votre workflow une fois.

Pour charger une bibliothèque, procédez comme suit :

1. Ouvrez un workflow et cliquez sur le bouton **[!UICONTROL Paramètres]**.
1. Accédez à la section **[!UICONTROL Script d’initialisation]** et cliquez sur **[!UICONTROL Créer un code]**.

   ![](assets/javascript-initialization.png)

1. Utilisez la syntaxe ci-dessous dans le code pour charger une bibliothèque :

   ```
   loadLibrary("/<namespace>/<name>")
   ```

   * Remplacez `<namespace>` par l’espace de noms spécifié lors de la création du code JavaScript.
   * Remplacez `<name>` par le nom du code JavaScript.

1. Cliquez sur **[!UICONTROL Confirmer]** et enregistrez les paramètres.

### Fonctions de référence dans les workflows {#reference}

Une fois la bibliothèque JavaScript chargée, vous pouvez référencer les fonctions définies dans le code JavaScript directement dans le workflow, généralement à l’aide d’une activité **[!UICONTROL Code JavaScript]**.

![](assets/javascript-function.png)
