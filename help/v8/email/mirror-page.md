---
audience: end-user
title: Ajouter un lien vers la page miroir
description: Découvrez comment ajouter et gérer le lien vers la page miroir.
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 29%

---

# Page miroir {#mirror-page}

La page miroir est une version en ligne de votre e-mail. Il est recommandé d’ajouter un lien vers la page miroir dans le cadre du marketing par e-mail. Les utilisateurs peuvent accéder à la page miroir d’un e-mail, par exemple, s’ils rencontrent des problèmes de rendu ou si des images sont endommagées lors de leur affichage dans leur boîte de réception. Il est également recommandé de fournir une version en ligne pour des raisons d’accessibilité ou pour encourager le partage sur les réseaux sociaux.

La page miroir générée par Adobe Campaign comprend toutes les données de personnalisation.

![Exemple de lien miroir dans un email](assets/mirror-page-link.png){width="600" align="left"}

## Ajouter un lien vers la page miroir {#link-to-mirror-page}

Dans Adobe Campaign, insérez un lien vers la page miroir dans le contenu de l’e-mail à l’aide du **bloc de personnalisation** dédié. Le bloc de personnalisation intégré **Lien vers la page miroir** insère le code suivant dans le contenu de votre e-mail : `<%@ include view='MirrorPage' %>`.

Pour ajouter un lien vers une page miroir dans l’e-mail, procédez comme suit :

1. Sélectionnez un élément (texte ou image), puis cliquez sur **[!UICONTROL Insérer un lien]** dans la barre d’outils contextuelle.

   ![ Barre d’outils contextuelle affichant l’option Insérer un lien ](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Sélectionnez l’icône **[!UICONTROL Ajouter une personnalisation]** pour accéder au menu de personnalisation.

   Menu Personalization ![dans Adobe Campaign](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Dans le menu **[!UICONTROL Fragments]**, sélectionnez **[!UICONTROL URL de la page miroir]**, puis cliquez sur **[!UICONTROL Ajouter]**. [Découvrez comment utiliser les fragments d’expression.](../content/use-expression-fragments.md)

   ![Option URL de page miroir dans le menu Fragments](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

La page miroir est automatiquement créée.

Lorsque l’e-mail est envoyé, les destinataires qui cliquent sur le lien de la page miroir voient le contenu de l’e-mail affiché dans leur navigateur web par défaut.

Par défaut, la période de conservation d’une page miroir est de **60 jours**. Passé ce délai, la page miroir n’est plus disponible.

>[!CAUTION]
>
>* Les liens de la page miroir sont générés automatiquement et ne peuvent pas être modifiés. Ils incluent toutes les données personnalisées chiffrées requises pour générer l’e-mail original. L’utilisation d’attributs personnalisés dotés de valeurs élevées peut générer de longues URL de page miroir, ce qui peut empêcher le lien de fonctionner dans les navigateurs web appliquant une longueur d’URL maximale.
>
>* Dans le BAT envoyé aux profils de test, le lien vers la page miroir n’est pas actif. Il n’est activé que dans les messages finaux.

## Génération de la page miroir {#mirror-page-generation}

Par défaut, Adobe Campaign génère automatiquement la page miroir si le contenu de l’e-mail n’est pas vide et contient un lien vers la page miroir (également appelé Lien miroir).

Contrôler le mode de génération de la page miroir de l’e-mail via les options disponibles dans les propriétés de la diffusion. [En savoir plus](../advanced-settings/delivery-settings.md#mirror)