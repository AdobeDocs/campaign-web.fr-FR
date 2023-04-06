---
title: Personnaliser votre contenu dans Campaign
description: Découvrez comment personnaliser votre contenu dans l’interface utilisateur web d’Adobe Campaign.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positif"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 99%

---


# Personnaliser votre contenu{#add-personalization}

Vous pouvez personnaliser le contenu du message en procédant comme suit :

* Insérer des **champs de personnalisation** dynamiques.

   Les champs de personnalisation sont utilisés pour la personnalisation de premier niveau de vos messages. Vous pouvez sélectionner n’importe quel champ disponible dans la base de données de l’éditeur de personnalisation. Pour une diffusion, vous pouvez sélectionner n’importe quel champ associé au ou à la destinataire, au message ou à la diffusion. Ces attributs de personnalisation peuvent être insérés dans l’objet ou dans le corps de vos messages.

   ![](assets/perso-subject-line.png)

   La syntaxe suivante insère la ville du ou de la destinataire dans votre contenu : &lt;%= recipient.location.city %>.

* Insérer des **blocs de contenu** prédéfinis

   Campaign est fourni avec un ensemble de blocs de personnalisation qui contiennent un rendu spécifique que vous pouvez insérer dans vos diffusions. Vous pouvez par exemple ajouter un logo, un message de salutation ou un lien vers la page miroir du message. Les blocs de contenu sont disponibles à partir d’une entrée dédiée dans l’éditeur de personnalisation.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personnaliser l’objet de l’e-mail {#personalize-subject-line}

Pour ajouter de la personnalisation dans le champ **[!UICONTROL Objet]** du message, procédez comme suit :

1. Cliquez sur l’icône **Ouvrir la boîte de dialogue de personnalisation** à droite du champ **Objet**.
1. Saisissez le contenu de l’objet et sélectionnez les attributs de personnalisation à ajouter.
1. Cliquez sur **Confirmer** pour valider. Les attributs de personnalisation sont ajoutés à l’objet.

![](assets/perso-subject.png)

## Personnaliser le contenu de vos e-mails {#personalize-emails}

Pour personnaliser le contenu des e-mails, ouvrez le message dans le concepteur d’e-mail et :

1. Cliquez à l’intérieur d’un bloc de texte.
1. Dans la barre d’outils contextuelle, sélectionnez **Ajouter une personnalisation**.

   ![](assets/perso-add-to-content.png)

1. Insérez le nom du ou de la destinataire dans l’éditeur de personnalisation et confirmez.

   ![](assets/perso-add-name.png)

   L’attribut de personnalisation est ajouté au contenu de l’e-mail.

   Vous pouvez simuler le contenu pour vérifier le rendu. [En savoir plus](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

Pour ajouter un bloc de contenu à votre e-mail, procédez de la même manière et sélectionnez un bloc de contenu à partir de la dernière icône :

![](assets/perso-insert-block.png)

Une fois inséré, le bloc de contenu est ajouté au contenu de l’e-mail, comme illustré ci-dessous. Il est automatiquement adapté au profil du ou de la destinataire lors de la génération de la personnalisation, à l’étape de préparation de la diffusion.

![](assets/perso-content-block-in-email.png)


Les blocs de contenu intégrés sont les suivants :

* **[!UICONTROL Enabled by Adobe Campaign]** : insère le logo « Enabled by Adobe Campaign ».
* **[!UICONTROL Fonction de formatage d’un nom propre]** : génère la fonction JavaScript **[!UICONTROL toSmartCase]** qui convertit la première lettre de chaque mot en majuscule.
* **[!UICONTROL Salutations]** : permet d’insérer des salutations avec le nom complet du ou de la destinataire, suivi d’une virgule. Exemple : « Bonjour Pierre Martin, ».
* **[!UICONTROL Insertion du logo]** : insère un logo défini dans les paramètres de l’instance.
* **[!UICONTROL Lien vers la page miroir]** : insère un lien vers la [page miroir](../content/mirror-page.md). Le format par défaut est : « Si vous ne parvenez pas à voir correctement ce message, cliquez ici »
* **[!UICONTROL URL de page miroir]** : insère l’URL de page miroir qui permet aux concepteurs et conceptrices de diffusion de vérifier le lien.
* **[!UICONTROL URL d’acceptation d’une offre en mode unitaire]** : insère une URL permettant de définir une offre comme étant **[!UICONTROL Acceptée]**. (Ce bloc est disponible si le module Interaction est activé).
* **[!UICONTROL Confirmation de votre inscription]** : insère un lien permettant de confirmer l’abonnement.
* **[!UICONTROL Lien d’inscription]** : insère un lien d’abonnement. Ce lien est défini dans les paramètres de l’instance. Le contenu par défaut est le suivant : « Pour vous inscrire, cliquez ici. ».
* **[!UICONTROL Lien d’inscription (avec parrain)]** : insère un lien d’abonnement permettant d’identifier le visiteur ou la visiteuse et la diffusion. Ce lien est défini dans les paramètres de l’instance.
* **[!UICONTROL URL de la page d’inscription]** : insère une URL d’abonnement.
* **[!UICONTROL Style des e-mails de contenu]** et **[!UICONTROL Style de notification]** : permettent de générer un code qui formate l’e-mail avec les styles HTML par défaut.
* **[!UICONTROL Lien de désinscription]** : insère un lien permettant de se désabonner de toutes les diffusions (liste bloquée). Le contenu associé par défaut est : « Vous recevez ce message car vous avez été en contact avec ***nom de votre organisation*** ou une entité associée. Pour ne plus recevoir de messages de ***nom de votre organisation***, cliquez ici. »



## Personnaliser les liens dans vos e-mails {#personalize-links}

Pour personnaliser un **lien** :

1. Sélectionnez un bloc de texte ou une image.
1. Dans la barre d’outils contextuelle, sélectionnez **Insérer un lien**.

   ![](assets/perso-link.png)

1. Saisissez le libellé du lien et utilisez le bouton **Insérer un lien** pour personnaliser le lien.

   ![](assets/perso-link-insert-icon.png)

1. Utilisez l’éditeur de personnalisation pour définir et personnaliser le lien, puis confirmez.

   ![](assets/perso-link-edit.png)


## Personnaliser vos offres {#personalize-offers}

Vous pouvez également accéder à l’éditeur de personnalisation lorsque vous ajoutez du contenu de type texte aux représentations de vos offres. En savoir plus dans [cette section](../content/offers.md).
