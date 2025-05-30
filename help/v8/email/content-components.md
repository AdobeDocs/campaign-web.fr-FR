---
audience: end-user
title: Utiliser les composants de contenu du concepteur d’e-mail
description: Découvrez comment utiliser des composants de contenu dans vos emails.
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: ht
source-wordcount: '1389'
ht-degree: 100%

---

# Utiliser les composants de contenu {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="À propos des contenus"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’un email."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="À propos des contenus"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’une page de destination."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="À propos des contenus"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’un fragment de contenu."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="À propos des contenus"
>abstract="Les composants de contenu sont des espaces réservés de contenu vides que vous pouvez utiliser pour créer la disposition d’un modèle."

Lorsque vous créez le contenu de votre e-mail, les composants de **[!UICONTROL contenu]** vous permettent de personnaliser votre e-mail à l’aide des composants bruts et vides que vous pouvez utiliser une fois placés dans un e-mail.

Vous pouvez ajouter autant de **[!UICONTROL contenus]** que nécessaire dans une **[!UICONTROL structure]**, ce qui permet de définir la disposition de votre e-mail.

## Ajouter des composants de contenu {#add-content-components}

Pour ajouter des composants de contenu à votre e-mail et les ajuster selon vos besoins, suivez les étapes ci-dessous.

1. Dans le concepteur d’e-mail, utilisez un [contenu existant](existing-content.md) ou faites glisser et déposez une **[!UICONTROL structure]** dans votre contenu vide pour définir la disposition de votre e-mail. [Voici comment procéder](create-email-content.md).

1. Faites glisser et déposez le **[!UICONTROL contenu]** de votre choix dans les structures appropriées.

   ![Capture d’écran montrant comment faire glisser et déposer des composants de contenu dans des structures dans le concepteur d’e-mail.](assets/email_designer_add_content_components.png){zoomable="yes"}

   >[!NOTE]
   >
   >Vous pouvez ajouter plusieurs composants dans une seule structure et dans chaque colonne d’une structure.

1. Ajustez les options de chaque composant en utilisant l’onglet **[!UICONTROL Paramètres]** contextuels. Par exemple, choisissez de ne l’afficher que sur les ordinateurs de bureau ou les appareils mobiles, ou les deux. Vous pouvez également gérer les options de lien à partir de cet onglet. [En savoir plus sur la gestion des liens](message-tracking.md)

1. Ajustez les attributs de style de chaque composant à l’aide de l’onglet **[!UICONTROL Style]**. Par exemple, vous pouvez changer le style de texte, la marge intérieure ou la marge de chaque composant. [En savoir plus sur l’alignement et la marge intérieure](alignment-and-padding.md).

   ![Capture d’écran montrant l’onglet Paramètres pour les composants de contenu dans le concepteur d’e-mail.](assets/email_designer_content_components_settings.png){zoomable="yes"}

1. Dans le menu avancé de votre **[!UICONTROL Contenu]** dans le volet de droite, supprimez ou dupliquez facilement n’importe quel composant de contenu, si nécessaire.

## Conteneur {#container}

Vous pouvez ajouter un conteneur simple à l’intérieur duquel vous ajouterez un autre composant de contenu. Vous pouvez ainsi appliquer un style spécifique au conteneur, qui est différent du composant utilisé à l’intérieur.

Par exemple, ajoutez un composant **[!UICONTROL Conteneur]**, puis ajoutez un composant [Bouton](#button) à l’intérieur de ce conteneur. Utilisez un arrière-plan spécifique pour le conteneur et un autre pour le bouton.

![Capture d’écran montrant comment ajouter un composant de conteneur dans le concepteur d’e-mail.](assets/email_designer_container_component.png){zoomable="yes"}

## Bouton {#buttons}

Utilisez le composant **[!UICONTROL Bouton]** pour insérer un ou plusieurs boutons dans votre e-mail et rediriger votre audience d’e-mail vers une autre page.

1. À partir de la liste **[!UICONTROL Contenu]**, faites glisser et déposez le composant de **[!UICONTROL bouton]** dans un composant de **[!UICONTROL structure]**.

   ![Capture d’écran montrant comment faire glisser et déposer un composant Bouton dans le concepteur d’e-mail.](assets/email_designer_13.png){zoomable="yes"}

1. Cliquez sur le bouton que vous venez d’ajouter pour personnaliser le texte et accéder aux onglets **[!UICONTROL Paramètres]** et **[!UICONTROL Styles]**.

   ![Capture d’écran montrant l’onglet Paramètres pour les composants Bouton dans le concepteur d’e-mail.](assets/email_designer_14.png){zoomable="yes"}

1. Depuis l’onglet **[!UICONTROL Paramètres]**, dans le champ **[!UICONTROL URL]**, ajoutez l’URL vers laquelle vous souhaitez rediriger lors d’un clic sur le bouton.

1. Choisissez l’affichage du contenu à l’aide de la liste déroulante **[!UICONTROL Cible]** :

   * **[!UICONTROL Aucune]** : ouvre le lien dans le même cadre que celui sur lequel l’utilisateur ou l’utilisatricea cliqué (par défaut).
   * **[!UICONTROL Vierge]** : ouvre le lien dans une nouvelle fenêtre ou un nouvel onglet.
   * **[!UICONTROL Auto]** : ouvre le lien dans le même cadre que celui sur lequel l’utilisateur ou l’utilisatrice a cliqué.
   * **[!UICONTROL Parent]** : ouvre le lien dans le cadre parent.
   * **[!UICONTROL Haut]** : ouvre le lien dans le corps complet de la fenêtre.

   ![Capture d’écran montrant les options cibles des composants Bouton dans le concepteur d’e-mail.](assets/email_designer_15.png){zoomable="yes"}

1. Personnalisez davantage votre bouton en modifiant les attributs de style, tels que **[!UICONTROL Bordure]**, **[!UICONTROL Taille]**, **[!UICONTROL Marge]**, etc., à partir de l’onglet **[!UICONTROL Styles]**.

## Texte {#text}

Utilisez le composant **[!UICONTROL Texte]** pour insérer du texte dans votre e-mail et ajuster le style (bordure, taille, marge intérieure, etc.) à l’aide des onglets **[!UICONTROL Paramètres]** et **[!UICONTROL Styles]**.

1. Dans le menu **[!UICONTROL Contenu]**, faites glisser et déposez du **[!UICONTROL texte]** dans un composant de **[!UICONTROL structure]**.

   ![Capture d’écran montrant comment faire glisser et déposer un composant de texte dans le concepteur d’e-mail.](assets/email_designer_11.png){zoomable="yes"}

1. Cliquez sur le composant que vous venez d’ajouter pour personnaliser le texte et accéder aux onglets **[!UICONTROL Paramètres]** et **[!UICONTROL Styles]**.

1. Modifiez votre texte avec les options suivantes disponibles dans la barre d’outils contextuelle :

   ![Capture d’écran affichant la barre d’outils d’édition de texte dans le Concepteur d’e-mail.](assets/email_designer_27.png){zoomable="yes"}

   * **[!UICONTROL Modifier le style de texte]** : appliquez le style gras, italique, souligné ou barré à votre texte.
   * **Modifier l’alignement** : sélectionnez l’alignement gauche, droite, centré ou justifié pour votre texte.
   * **[!UICONTROL Créer une liste]** : ajoutez une liste à puces ou à nombres à votre texte.
   * **[!UICONTROL Définir un titre]** : ajoutez jusqu’à six niveaux de titre à votre texte.
   * **Taille de police** : sélectionnez la taille de police de votre texte en pixels.
   * **[!UICONTROL Modifier l’image]** : ajoutez une image ou une ressource à votre composant de texte.
   * **[!UICONTROL Afficher le code source]** : affichez le code source de votre texte. Impossible d’effectuer une modification.
   * **[!UICONTROL Dupliquer]** : ajoutez une copie de votre composant de texte.
   * **[!UICONTROL Supprimer]** : supprimez le composant de texte sélectionné de votre e-mail.
   * **[!UICONTROL Ajouter une personnalisation]** : ajoutez des champs de personnalisation pour personnaliser le contenu des données de vos profils.
   * **[!UICONTROL Activer le contenu conditionnel]** : ajoutez du contenu conditionnel pour adapter le contenu du composant aux profils ciblés.

1. Ajustez les autres attributs de style, tels que la couleur du texte, la famille de polices, la bordure, la marge intérieure, la marge, et d’autres éléments à partir de l’onglet **[!UICONTROL Styles]**.

   ![Capture d’écran affichant l’onglet des styles pour les composants de texte dans le Concepteur d’e-mail.](assets/email_designer_12.png){zoomable="yes"}

## Diviseur {#divider}

Utilisez le composant **[!UICONTROL Diviseur]** pour insérer une ligne de séparation afin d’organiser la disposition et le contenu de l’e-mail.

Vous pouvez ajuster les attributs de style, tels que la couleur, le style et la hauteur des lignes depuis l’onglet **[!UICONTROL Styles]**.

![Capture d’écran affichant comment ajouter un composant diviseur dans le Concepteur d’e-mail.](assets/email_designer_16.png){zoomable="yes"}

## HTML {#HTML}

Utilisez le composant **[!UICONTROL HTML]** pour copier-coller les différentes parties de votre code HTML existant. Vous pouvez ainsi créer des composants HTML modulaires autonomes afin de réutiliser du contenu externe.

1. À partir des **[!UICONTROL Composants]**, faites glisser et déposez le composant **[!UICONTROL HTML]** dans une **[!UICONTROL structure]**.

   ![Capture d’écran affichant la manière de faire glisser et déposer un composant HTML dans le Concepteur d’e-mail.](assets/email_designer_22.png){zoomable="yes"}

1. Cliquez sur le composant que vous venez d’ajouter, puis sélectionnez **[!UICONTROL Afficher le code source]** dans la barre d’outils contextuelle pour ajouter votre code HTML.

   ![Capture d’écran affichant l’option de code source pour les composants HTML dans le Concepteur d’e-mail.](assets/email_designer_23.png){zoomable="yes"}

>[!NOTE]
>
>Pour rendre un contenu externe compatible avec le Concepteur d’e-mail, Adobe recommande de [créer un message en partant de zéro](create-email-content.md) et de copier le contenu de l’e-mail existant dans des composants.

## Image {#image}

>[!IMPORTANT]
>
>L’accès au menu Assets est limité aux personnes disposant d’une licence Adobe Experience Manager as a Cloud Service active. Si vous ne possédez pas cette licence, le menu Assets ne sera pas disponible.

Utilisez le composant **[!UICONTROL Image]** pour insérer un fichier image de votre ordinateur dans l’e-mail.

1. Dans le menu **[!UICONTROL Contenu]**, faites glisser et déposez **[!UICONTROL Image]** dans un composant de **[!UICONTROL structure]**.

   ![Capture d’écran affichant la façon de faire glisser et déposer un composant d’image dans le Concepteur d’e-mail.](assets/email_designer_9.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Parcourir]** pour choisir un fichier image parmi vos ressources. Vous pouvez également choisir d’**[!UICONTROL importer votre contenu multimédia]**.

   Pour en savoir plus sur le chargement et l’ajout de ressources dans Adobe Experience Manager, reportez-vous à la [documentation d’Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html?lang=fr).

   ![Capture d’écran affichant l’option de navigation pour les composants d’image dans le Concepteur d’e-mail.](assets/email_designer_28.png){zoomable="yes"}

1. Parcourez vos dossiers pour localiser la ressource spécifique dont vous avez besoin ou utilisez la barre de recherche pour la chercher efficacement.

   Une fois que vous avez trouvé la ressource recherchée, cliquez sur **[!UICONTROL Sélectionner]**.

   ![Capture d’écran affichant le processus de sélection de ressources dans le Concepteur d’e-mail.](assets/email_designer_29.png){zoomable="yes"}

1. Cliquez sur le composant que vous venez d’ajouter et configurez les propriétés de l’image à l’aide de l’onglet **[!UICONTROL Paramètres]** :

   * Le **[!UICONTROL Titre de l’image]** permet de définir un titre pour l’image.
   * **[!UICONTROL Texte alternatif]** permet de définir la légende associée à votre image. Cela correspond à l’attribut HTML alternatif.

   ![Capture d’écran affichant l’onglet Paramètres pour les composants d’image dans le Concepteur d’e-mail.](assets/email_designer_10.png){zoomable="yes"}

1. Ajoutez un lien pour rediriger votre audience vers un autre contenu. [En savoir plus](message-tracking.md)

1. Ajustez d’autres attributs de style, tels que la marge, la bordure et autres à l’aide de l’onglet **[!UICONTROL Styles]**.

## Social {#social}

Utilisez le composant **[!UICONTROL Social]** pour insérer des liens vers des pages de réseaux sociaux dans le contenu de l’e-mail.

1. À partir du menu **[!UICONTROL Composants]**, faites glisser et déposez le composant **[!UICONTROL Social]** dans un composant de **[!UICONTROL structure]**.

1. Cliquez sur le composant que vous venez d’ajouter.

1. Dans le champ **[!UICONTROL Social]** de l’onglet **[!UICONTROL Paramètres]**, sélectionnez les médias sociaux à ajouter ou à supprimer.

   ![Capture d’écran affichant l’onglet Paramètres pour les composants sociaux dans le Concepteur d’e-mail.](assets/email_designer_20.png){zoomable="yes"}

1. Sélectionnez la taille des icônes dans le champ **[!UICONTROL Taille des images]**.

1. Cliquez sur chaque icône de réseau social pour configurer l’**[!UICONTROL URL]** vers laquelle votre audience est redirigée.

   ![Capture d’écran affichant la configuration de l’URL pour les icônes de médias sociaux dans le Concepteur d’e-mail.](assets/email_designer_21.png){zoomable="yes"}

1. Modifiez les icônes de chaque média social si nécessaire dans le champ **[!UICONTROL Source]**.

1. Ajustez d’autres attributs de style, tels que le style, la marge, la bordure et d’autres depuis l’onglet **[!UICONTROL Styles]**.