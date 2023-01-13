---
title: Personnaliser votre contenu dans Campaign
description: Découvrez comment personnaliser votre contenu dans l’interface utilisateur web d’Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 2d23b04b81ab625de0936fdf058f6ac8bd1017c3
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 7%

---

# Personnaliser le contenu{#add-personalization}

![](../assets/do-not-localize/badge.png)

Vous pouvez personnaliser le contenu du message en procédant comme suit :

* Insérer dynamique **champs de personnalisation**

   Les champs de personnalisation sont utilisés pour la personnalisation de premier niveau de vos messages. Vous pouvez sélectionner n’importe quel champ disponible dans la base de données dans l’éditeur de personnalisation. Pour une diffusion, vous pouvez sélectionner n&#39;importe quel champ associé au destinataire, au message ou à la diffusion. Ces attributs de personnalisation peuvent être insérés dans la ligne d’objet ou le corps de vos messages.

   ![](assets/perso-subject-line.png)

   La syntaxe ci-dessus insère la ville du destinataire dans votre contenu : &lt;%= recipient.location.city %>.

* Insertion de données prédéfinies **blocs de contenu**

   Campaign est fourni avec un ensemble de blocs de personnalisation qui contiennent un rendu spécifique que vous pouvez insérer dans vos diffusions. Vous pouvez par exemple ajouter un logo, un message de salutations ou un lien vers la page miroir du message. Les blocs de contenu sont disponibles à partir d’une entrée dédiée dans l’éditeur de personnalisation.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personnaliser l&#39;objet de l&#39;email {#personalize-subject-line}

Pour ajouter de la personnalisation dans le **[!UICONTROL Objet]** du message, procédez comme suit :

1. Cliquez sur le bouton **Ouvrir la boîte de dialogue de personnalisation** à droite de la **Objet** champ .
1. Saisissez l’objet du contenu et sélectionnez les attributs de personnalisation à ajouter.
1. Cliquez sur Confirmer pour valider. Les attributs de personnalisation sont ajoutés à l’objet.

![](assets/perso-subject.png)

## Personnaliser le contenu de votre email {#personalize-emails}

Pour personnaliser le contenu de l&#39;email, ouvrez le message dans le Concepteur d&#39;email et :

1. Cliquez à l’intérieur d’un bloc de texte.
1. Dans la barre d’outils contextuelle, sélectionnez **Ajouter une personnalisation**.

   ![](assets/perso-add-to-content.png)

1. Insérez le nom du destinataire dans l&#39;éditeur de personnalisation et validez.

   ![](assets/perso-add-name.png)

   L&#39;attribut de personnalisation est ajouté au contenu de l&#39;email.

   Vous pouvez simuler le contenu pour vérifier le rendu. [En savoir plus](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## Personnalisation des liens dans vos emails {#personalize-links}

Pour personnaliser une **link**:

1. Sélectionnez un bloc de texte ou une image.
1. Dans la barre d’outils contextuelle, sélectionnez **Ajouter une personnalisation**.

   ![](assets/perso-link.png)

1. Utilisez l&#39;éditeur de personnalisation pour définir et personnaliser le lien.

## Personnaliser vos offres {#personalize-offers}

Vous pouvez également accéder à l’éditeur de personnalisation lorsque vous ajoutez du contenu de type texte aux représentations de vos offres.
