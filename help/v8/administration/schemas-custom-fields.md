---
title: Modifier des champs personnalisés
description: Découvrez comment configurer des champs personnalisés et leur visibilité dans l’interface.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 53%

---

# Modifier des champs personnalisés {#fields}

Les champs personnalisés sont des attributs supplémentaires ajoutés aux schémas prêts à l’emploi via la console Adobe Campaign. Ils vous permettent de personnaliser les schémas en incluant de nouveaux attributs en fonction des besoins de votre entreprise.

Les champs personnalisés peuvent être affichés sur différents écrans, comme les détails du profil dans l’interface. Vous pouvez contrôler quels champs sont visibles et comment ils apparaissent dans l’interface.

Pour plus d&#39;informations sur l&#39;écran de définition d&#39;écran et sur la façon d&#39;y accéder, consultez la section [Accéder à la définition d&#39;écran](schemas-browse-access.md#screen-def).

Pour ajouter des champs personnalisés à la liste :

1. Accédez au menu **[!UICONTROL Schémas]** et recherchez les schémas modifiables à l’aide des filtres.

1. Sélectionnez le nom du schéma dans la liste pour l’ouvrir et cliquez sur le bouton **[!UICONTROL Modification de l’écran]** dans la vue des détails du schéma pour accéder à la définition d’écran.

1. Cliquez sur l’icône représentant des points de suspension au-dessus du tableau **[!UICONTROL Liste de champs personnalisés]** et choisissez **[!UICONTROL Sélectionner des attributs]** pour sélectionner un ou plusieurs champs personnalisés à afficher dans l’interface.
   ![Écran de champs personnalisés affichant les attributs modifiables](assets/schemas-custom5.png)
1. Sélectionnez les champs personnalisés à ajouter et confirmez-les.

   ![Écran de champs personnalisés affichant les attributs modifiables](assets/schemas-custom2.png)

   >[!NOTE]
   >
   > Vous pouvez également sélectionner **[!UICONTROL Remplir automatiquement la liste des champs personnalisés]** pour ajouter tous les champs personnalisés définis pour le schéma à l’interface.

Une fois les champs personnalisés ajoutés, vous pouvez les prévisualiser, les réorganiser, les rendre obligatoires, modifier leurs paramètres ou les organiser en sous-sections.

## Configurer les paramètres de champ {#field-settings}

Pour configurer des paramètres spécifiques à chaque champ personnalisé, cliquez sur l’icône représentant des points de suspension sur une ligne de champ de la liste et sélectionnez **[!UICONTROL Modifier]**.

![&#x200B; Boîte de dialogue Paramètres des attributs &#x200B;](assets/schemas-attribute-settings.png)

Les paramètres disponibles sont les suivants :

* **[!UICONTROL Attribut]** : nom du champ personnalisé (lecture seule).
* **[!UICONTROL Libellé (personnalisé)]** : libellé à afficher dans l’interface. Si aucun libellé n’est renseigné, le libellé défini dans le schéma s’affiche.
* **[!UICONTROL Visible si]** : définissez une condition à l’aide d’une expression xtk qui contrôle quand le champ doit être affiché. Par exemple, masquer le champ si un autre champ est vide.
* **[!UICONTROL Obligatoire]** : permet au champ d’être obligatoire dans l’interface.
* **[!UICONTROL Lecture seule]** : permet au champ d’être en lecture seule dans l’interface. Les utilisateurs et les utilisatrices ne pourront pas modifier la valeur du champ.
* **[!UICONTROL Paramètres de filtrage]** (pour les champs de type lien) : utilisez le concepteur de requête pour spécifier les règles d’affichage d’un champ personnalisé de type lien. Par exemple, limitez les valeurs d’une liste en fonction de l’entrée d’un autre champ.

  +++Afficher l’exemple

  Vous pouvez également référencer dans vos conditions une valeur saisie dans d’autres champs à l’aide de la syntaxe `$(<field-name>)`. Cela vous permet de référencer la valeur actuelle d’un champ telle qu’elle a été saisie dans le formulaire, même si elle n’a pas encore été enregistrée dans la base de données.

  Dans l’exemple ci-dessous, la condition vérifie si la valeur du champ @ref correspond à la valeur saisie dans le champ @refCom. En revanche, utiliser `@refCom` au lieu de `$(@refCom)` référencerait la valeur du champ @ref telle qu’elle existe dans la base de données.

  ![Capture d’écran illustrant un exemple de paramètres de filtre pour les champs personnalisés](assets/custom-fields-ref.png)

  +++

* **[!UICONTROL Étendre sur deux colonnes]** : par défaut, les champs personnalisés s’affichent dans l’interface sur deux colonnes. Activez cette option pour afficher le champ personnalisé sur toute la largeur de l’écran au lieu de deux colonnes.

## Prévisualiser les champs personnalisés {#preview}

Cliquez sur **[!UICONTROL Aperçu]** pour afficher les champs personnalisés dans un exemple d’écran. Vous pouvez ainsi voir comment les champs apparaîtront dans l’interface, y compris les champs marqués comme obligatoires.

![Aperçu des champs personnalisés](assets/schemas-custom4.png)

## Organisation des champs dans les sous-sections {#separator}

Vous pouvez ajouter des séparateurs pour regrouper les champs personnalisés dans l’interface afin d’en améliorer la lisibilité. Pour ce faire, procédez comme suit :

1. Cliquez sur l’icône représentant des points de suspension au-dessus du tableau **[!UICONTROL Liste de champs personnalisés]** et choisissez **[!UICONTROL Ajouter un séparateur]**.

1. Une nouvelle ligne représentant le séparateur est ajoutée à la liste. Cliquez sur l’icône représentant des points de suspension sur la ligne de séparation et choisissez **[!UICONTROL Modifier]**.

1. Saisissez un **[!UICONTROL Libellé]** pour le séparateur et (facultatif) définissez une condition **[!UICONTROL Visible si]** pour contrôler l’affichage du séparateur.

   ![Boîte de dialogue Propriétés du séparateur](assets/schemas-custom3.png)

1. Utilisez les flèches haut et bas pour déplacer le séparateur vers l’emplacement souhaité. Les champs répertoriés sous le séparateur seront regroupés sous celui-ci.

   Dans cet exemple, les champs « Interested Collections » et « Brand » sont regroupés dans une sous-section « Collection ».

   | Configuration des champs personnalisés | Rendu dans l’interface |
   |  ---  |  ---  |
   | ![Capture d’écran affichant la configuration d’un séparateur](assets/custom-fields-separator.png){zoomable="yes"} | ![Capture d’écran affichant le rendu d’une sous-section dans l’interface](assets/custom-fields-section.png){zoomable="yes"} |
