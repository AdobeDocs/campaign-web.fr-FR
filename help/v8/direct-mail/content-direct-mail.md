---
audience: end-user
title: Concevoir une diffusion courrier
description: Découvrez comment concevoir votre diffusion courrier avec Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 22%

---

# Concevoir le fichier d’extraction {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Contenu du fichier d’extraction"
>abstract="Cliquez sur le bouton **Modifier le contenu** pour lancer la conception du fichier d’extraction requis par votre fournisseur de services postaux. Vous pouvez ainsi définir les propriétés du fichier, telles que son libellé et son format, et spécifier les colonnes à inclure dans le fichier."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propriétés du fichier"
>abstract="Configurez les propriétés du fichier d’extraction, telles que son nom et son format. Vous pouvez personnaliser le nom du fichier à l’aide des attributs de la base de données de l’éditeur d’expression."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Contenu"
>abstract="Dans cette section, indiquez les colonnes à afficher dans le fichier d’extraction. Une fois cette opération terminée, vous pouvez obtenir un aperçu du fichier d’extraction à l’aide du bouton **Simuler du contenu**."

Pour concevoir le contenu du fichier d&#39;extraction généré par votre diffusion courrier, cliquez sur le bouton **[!UICONTROL Modifier le contenu]** à partir de la page de diffusion, puis configurez les propriétés et le contenu du fichier.

## Configuration des propriétés du fichier d’extraction {#properties}

1. Dans le **[!UICONTROL Nom du fichier]** , indiquez le nom souhaité pour le fichier d’extraction. Vous pouvez personnaliser le nom du fichier à l’aide des attributs de la base de données. Pour ce faire, cliquez sur le bouton **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]** pour ouvrir l’éditeur d’expression. [Découvrez comment personnaliser du contenu](../personalization/personalize.md).

1. Dans le **[!UICONTROL Format du fichier]** , choisissez le format souhaité pour le fichier d’extraction. **Texte**, **Texte contenant des colonnes fixes**, **CSV (Excel)** ou **XML**.

1. Développez l’objet **[!UICONTROL Format d&#39;extraction]** pour accéder aux options spécifiques relatives au format du fichier d&#39;extraction. Les valeurs disponibles dépendent du format sélectionné.

+++ Options de format d’extraction disponibles

   * **[!UICONTROL Utiliser la première ligne comme en-tête de colonne]** (Format Texte/CSV (Excel) : activez cette option pour utiliser la première colonne comme en-tête.
   * **[!UICONTROL Séparateur de colonne]** (Format texte) : spécifiez le caractère à utiliser comme séparateur de colonne dans le fichier d&#39;extraction.
   * **[!UICONTROL Délimiteur de chaîne]** (Format texte) : indiquez comment délimiter les chaînes dans le fichier d’extraction.
   * **[!UICONTROL Fin de ligne]** (Format texte) : indiquez comment délimiter la fin des lignes dans le fichier d&#39;extraction.
   * **[!UICONTROL Encodage]**: choisissez le codage du fichier d&#39;extraction.
   * **[!UICONTROL Format et séparateurs de date]**: indiquez le format des dates dans le fichier d’extraction.
   * **[!UICONTROL Format des nombres]**: indiquez le format des nombres dans le fichier d’extraction.
   * **[!UICONTROL Exporter des libellés plutôt que des valeurs internes des énumérations]**: activez cette option si vous exportez des valeurs d’énumération et souhaitez récupérer les libellés de colonnes plus faciles à comprendre que les identifiants internes.

+++

1. Activez l’option **[!UICONTROL Quantité demandée]** pour limiter le nombre de destinataires de votre diffusion.

   ![](assets/dm-content-details.png){zoomable=&quot;yes&quot;}

## Configuration des colonnes du fichier d&#39;extraction {#content}

Dans le **[!UICONTROL Contenu]** , indiquez les colonnes à afficher dans le fichier d&#39;extraction. Pour ce faire, procédez comme suit :

1. Cliquez sur le bouton **[!UICONTROL Ajouter un attribut]** pour créer une colonne.
1. Sélectionnez l&#39;attribut à afficher dans la colonne puis validez. Une fois la colonne ajoutée, vous pouvez modifier son libellé et modifier l&#39;attribut associé à partir de l&#39;icône d&#39;édition.
1. Répétez ces étapes pour ajouter autant de colonnes que nécessaire à votre fichier d&#39;extraction.
1. Pour trier le fichier d&#39;extraction à l&#39;aide de l&#39;une des colonnes, cliquez sur l&#39;icône dans la **[!UICONTROL Tri]** et sélectionnez la méthode de tri souhaitée.
1. Pour changer la position d&#39;une colonne, utilisez les flèches haut et bas.

![](assets/dm-content-attributes.png)

Vous pouvez maintenant prévisualiser le fichier d&#39;extraction et envoyer la diffusion afin de générer le fichier d&#39;extraction. [Découvrez comment tester et envoyer des messages de courrier](send-direct-mail.md)
