---
audience: end-user
title: Ajouter un lien vers la page miroir
description: Découvrez comment ajouter et gérer le lien vers la page miroir.
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 00a612513bcb649d23b2c5b4d5ed05b06a6a80ef
workflow-type: ht
source-wordcount: '390'
ht-degree: 100%

---

# Page miroir {#mirror-page}

La page miroir est une version en ligne de votre e-mail. L’ajout d’un lien vers la page miroir constitue une bonne pratique en matière de marketing par e-mail. Les utilisateurs et utilisatrices consultent la page miroir d’un e-mail en cas de problème d’affichage des images dans leur boîte de réception ou lorsque ces dernières sont endommagées. Il est également recommandé de fournir une version en ligne pour des raisons d’accessibilité ou pour faciliter le partage sur les réseaux sociaux.

La page miroir générée par Adobe Campaign contient toutes les données de personnalisation.

![exemple de lien miroir](assets/mirror-page-link.png){width="600" align="left"}

## Ajouter un lien vers la page miroir{#link-to-mirror-page}

Dans Adobe Campaign, vous pouvez insérer un lien vers la page miroir dans le contenu de l’e-mail à l’aide du **bloc de personnalisation** dédié. Le bloc de personnalisation intégré **Lien vers la page miroir** insère le code suivant dans le contenu de votre e-mail : `<%@ include view='MirrorPage' %>`.

Pour ajouter un lien vers une page miroir dans l’e-mail, procédez comme suit :

1. Sélectionnez un élément (texte ou image) et cliquez sur **[!UICONTROL Insérer un lien]** dans la barre d’outils contextuelle.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Sélectionnez l’icône **[!UICONTROL Ajouter une personnalisation]** pour accéder au menu de personnalisation.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Dans le menu **[!UICONTROL Fragments]**, sélectionnez **[!UICONTROL URL de la page miroir]** et cliquez sur **[!UICONTROL Ajouter]**. [Découvrez comment utiliser les fragments d’expression.](../content/use-expression-fragments.md)

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

La page miroir est automatiquement créée.

Une fois l’e-mail envoyé, lorsque les destinataires cliquent sur le lien de la page miroir, le contenu de l’e-mail s’affiche dans leur navigateur web par défaut.

Par défaut, la période de conservation d’une page miroir est de **60 jours**. Une fois ce délai écoulé, la page miroir n’est plus disponible.

>[!CAUTION]
>
>* Les liens de pages miroir sont générés automatiquement et ne peuvent pas être modifiés. Ils contiennent toutes les données personnalisées chiffrées requises pour générer l’e-mail original. Par conséquent, l’utilisation d’attributs personnalisés avec des valeurs élevées peut générer de longues URL de pages miroir. Cela peut empêcher le lien de fonctionner dans les navigateurs web qui imposent des limites de longueur d’URL.
>
>* Dans le BAT envoyé aux profils de test, le lien vers la page miroir est inactif. Il n’est activé que dans les messages finaux.


## Génération de la page miroir {#mirror-page-generation}

Par défaut, la page miroir est automatiquement générée par Adobe Campaign si le contenu de l’e-mail n’est pas vide et s’il comporte un lien vers la page miroir (ou lien miroir).

Vous pouvez choisir le mode de génération de la page miroir de l’e-mail. Plusieurs options s’offrent à vous dans les propriétés de la diffusion. [En savoir plus](../advanced-settings/delivery-settings.md#mirror)
