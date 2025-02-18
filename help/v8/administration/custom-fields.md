---
title: Champs personnalisés
description: Découvrez comment configurer des champs personnalisés et leur visibilité dans l’interface.
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 5%

---


# Configurer des champs personnalisés {#custom-fields}

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields"
>title="Modifier les détails personnalisés"
>abstract="Tous les champs personnalisés affichés dans l’interface pour le schéma sélectionné s’affichent. Vous pouvez modifier leur ordre d’affichage dans l’interface à l’aide des flèches vers le haut et vers le bas, et regrouper les champs en sous-sections en ajoutant des séparateurs. Pour supprimer un champ personnalisé ou modifier des paramètres tels que les conditions de visibilité, cliquez sur le bouton représentant des points de suspension."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_general"
>title="Général"
>abstract="Définissez les paramètres généraux du champ personnalisé. Si aucun libellé n’est fourni, le libellé défini dans le schéma s’affiche. Utilisez le champ **Visible si** pour définir une condition à l’aide d’une expression xtk qui contrôle l’affichage du champ. Vous pouvez également marquer le champ comme obligatoire ou en lecture seule dans l’interface."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_link"
>title="Propriétés du lien"
>abstract="Utilisez le requêteur pour spécifier les règles d&#39;affichage d&#39;un champ personnalisé de type lien. Par exemple, restreignez les valeurs de liste en fonction de l’entrée d’un autre champ."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_layout"
>title="Disposition"
>abstract="Par défaut, les champs personnalisés s’affichent dans l’interface en deux colonnes. Activez cette option pour afficher le champ personnalisé sur toute la largeur de l’écran au lieu de deux colonnes."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_separatorproperties"
>title="Propriétés du séparateur"
>abstract="Indiquez le nom à afficher dans l’interface de la sous-section."

<!-- NOT USED IN THE UI?-->
>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings"
>title="Paramètres des attributs"
>abstract="Paramètres des attributs"

Les champs personnalisés sont des attributs supplémentaires ajoutés aux schémas d’usine par le biais de la console Adobe Campaign. Ils vous permettent de personnaliser les schémas en incluant de nouveaux attributs en fonction des besoins de votre entreprise. Découvrez comment étendre un schéma dans la documentation d’[Adobe Campaign v8 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=fr){target="_blank"}.

Les champs personnalisés peuvent être affichés dans différents écrans, comme les détails du profil dans l’interface Web de Campaign. Les administrateurs peuvent contrôler les champs visibles et la manière dont ils apparaissent. Ces modifications s&#39;appliquent à tous les utilisateurs de Campaign.

>[!NOTE]
>
>Vous devez disposer de droits d’administrateur pour gérer les champs personnalisés.

Les champs personnalisés sont disponibles pour les schémas suivants :

* Campagnes (nms)
* Plans (nms)
* Programmes (nms)
* Personnes destinataires (nms)
* Adresses de contrôle (nms)
* Diffusions (nms)

## Ajouter des champs personnalisés à l’interface {#add}

Pour afficher des champs personnalisés dans l’interface, procédez comme suit :

1. Accédez au menu **[!UICONTROL Schémas]** dans le volet de navigation de gauche et recherchez le schéma souhaité.

   Utilisez le filtre **[!UICONTROL Modifiable]** dans le volet Filtres pour identifier rapidement les schémas comportant des champs personnalisés.

   ![](assets/custom-fields-open.png)

1. Sélectionnez le nom du schéma dans la liste pour l’ouvrir. Une vue de schéma détaillée affiche [En savoir plus sur les détails du schéma](../administration/schemas.md). Cliquez sur le bouton **[!UICONTROL Modifier les détails personnalisés]** pour accéder aux champs personnalisés. Dans cet exemple, nous allons ajouter des champs pour le schéma **[!UICONTROL Destinataires]**.

   ![](assets/custom-fields-edit.png)

1. La liste des champs personnalisés affichée dans l’interface pour le schéma s’affiche. Ici, le champ « ID CRM » est visible dans l’écran des détails des profils et a été marqué comme obligatoire.

   | Configuration des champs personnalisés | Rendu dans l’interface |
   |  ---  |  ---  |
   | ![](assets/custom-fields-detail.png){zoomable="yes"} | ![](assets/custom-fields-detail-crm.png){zoomable="yes"} |

1. Pour ajouter un champ personnalisé à l’interface , cliquez sur le bouton représentant des points de suspension et choisissez l’une des options suivantes :

   * **[!UICONTROL Sélectionner des champs personnalisés]** : sélectionnez un ou plusieurs champs personnalisés à afficher dans l’interface.
   * **[!UICONTROL Remplir automatiquement la liste des champs personnalisés]** : ajoutez à l&#39;interface tous les champs personnalisés définis pour le schéma.

   ![](assets/custom-fields-add.png)

1. Une fois les champs personnalisés ajoutés, vous pouvez :

   * **Réorganiser les champs** : utilisez les flèches haut et bas.
   * **Rendre les champs obligatoires** : cochez la case **Obligatoire**.
   * **Modifier les paramètres des champs** : cliquez sur le bouton représentant des points de suspension et choisissez **[!UICONTROL Modifier]**. [En savoir plus](#settings)
   * **Supprimer les champs** : cliquez sur le bouton représentant des points de suspension et choisissez **[!UICONTROL Supprimer]**.
   * **Organiser les champs en sous-sections dans l’interface** : cliquez sur le bouton représentant des points de suspension à côté des flèches haut et bas et choisissez **[!UICONTROL Ajouter un séparateur]**. [En savoir plus](#separator)

## Configuration des paramètres de champs personnalisés {#settings}

Pour configurer des paramètres spécifiques à chaque champ personnalisé, cliquez sur le bouton représentant des points de suspension en regard du champ souhaité, puis sélectionnez **[!UICONTROL Modifier]**.

![](assets/custom-fields-settings.png)

Les paramètres disponibles sont les suivants :

* **[!UICONTROL Attribut]** : nom du champ personnalisé.
* **[!UICONTROL Libellé (personnalisé)]** : libellé à afficher dans l’interface. Si aucun libellé n’est fourni, le libellé défini dans le schéma s’affiche.
* **[!UICONTROL Visible si]** : définissez une condition à l’aide d’une expression xtk qui contrôle l’affichage du champ. Par exemple, masquez ce champ si un autre champ est vide.
* **[!UICONTROL Obligatoire]** : rendez le champ obligatoire dans l’interface.
* **[!UICONTROL Lecture seule]** : permet au champ d’être en lecture seule dans l’interface. Les utilisateurs ne pourront pas modifier la valeur du champ.
* **[!UICONTROL Paramètres de filtrage]** (pour les champs de type lien) : utilisez le modéliseur de requête pour spécifier les règles d’affichage d’un champ personnalisé de type lien. Par exemple, restreignez les valeurs de liste en fonction de l’entrée d’un autre champ.

  Vous pouvez également référencer la valeur saisie dans d’autres champs de vos conditions à l’aide de la syntaxe `$(<field-name>)`. Vous pouvez ainsi référencer la valeur actuelle d’un champ telle qu’elle a été saisie dans le formulaire, même s’il n’a pas encore été enregistré dans la base de données.

  Dans l’exemple ci-dessous, la condition vérifie si la valeur du champ @ref correspond à la valeur saisie dans le champ @refCom . En revanche, l’utilisation de `@refCom` au lieu de `$(@refCom)` référencerait la valeur du champ de @ref tel qu’il existe dans la base de données.

  +++Afficher l’exemple

  ![](assets/custom-fields-ref.png)

+++

* **[!UICONTROL S’étendre sur deux colonnes]** : par défaut, les champs personnalisés s’affichent dans l’interface en deux colonnes. Activez cette option pour afficher le champ personnalisé sur toute la largeur de l’écran au lieu de deux colonnes.

## Organisation des champs personnalisés dans des sous-sections {#separator}

L’interface utilisateur web de Campaign vous permet d’ajouter des séparateurs afin de regrouper les champs personnalisés dans l’interface pour une meilleure lisibilité. Pour ce faire, procédez comme suit :

1. Cliquez sur le bouton représentant des points de suspension à côté des flèches haut et bas et sélectionnez **[!UICONTROL Ajouter un séparateur]**.

1. Une nouvelle ligne représentant le séparateur est ajoutée à la liste. Cliquez sur le bouton représentant des points de suspension et choisissez **[!UICONTROL Modifier]** pour nommer la sous-section.

1. Utilisez les flèches vers le haut et vers le bas pour déplacer le séparateur vers l’emplacement souhaité. Les champs répertoriés sous le séparateur seront regroupés sous celui-ci.

   Dans cet exemple, les champs « Collections intéressées » et « Marque » sont regroupés dans une sous-section « Collection ».

   | Configuration des champs personnalisés | Rendu dans l’interface |
   |  ---  |  ---  |
   | ![](assets/custom-fields-separator.png){zoomable="yes"} | ![](assets/custom-fields-section.png){zoomable="yes"} |
