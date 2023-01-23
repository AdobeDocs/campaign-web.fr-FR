---
title: Personnaliser votre contenu dans Campaign
description: Découvrez comment personnaliser votre contenu dans l’interface utilisateur web d’Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 51bd6f405ad151e2264d69c57ffe5e1783077203
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 23%

---

# Personnaliser le contenu{#add-personalization}

![](../assets/do-not-localize/badge.png)

Vous pouvez personnaliser le contenu du message en procédant comme suit :

* Insérer dynamique **champs de personnalisation**

   Les champs de personnalisation sont utilisés pour la personnalisation de premier niveau de vos messages. Vous pouvez sélectionner n’importe quel champ disponible dans la base de données dans l’éditeur de personnalisation. Pour une diffusion, vous pouvez sélectionner n&#39;importe quel champ associé au destinataire, au message ou à la diffusion. Ces attributs de personnalisation peuvent être insérés dans la ligne d’objet ou dans le corps de vos messages.

   ![](assets/perso-subject-line.png)

   La syntaxe suivante insère la ville du destinataire dans votre contenu : &lt;%= recipient.location.city %>.

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
1. Cliquez sur **Confirmer** pour valider. Les attributs de personnalisation sont ajoutés à l’objet.

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

Pour ajouter un bloc de contenu à votre email, procédez de la même manière et sélectionnez un bloc de contenu à partir de la dernière icône :

![](assets/perso-insert-block.png)

Une fois inséré, le bloc de contenu est ajouté au contenu de l&#39;email, comme illustré ci-dessous. Il est automatiquement adapté au profil du destinataire lors de la génération de la personnalisation, à l’étape de préparation de la diffusion.

![](assets/perso-content-block-in-email.png)


Les blocs de contenu intégrés sont les suivants :
* **[!UICONTROL Activé par Adobe Campaign]** : insère le logo &quot;Activé par Adobe Campaign&quot;.
* **[!UICONTROL Fonction de formatage d&#39;un nom propre]** : génère la fonction JavaScript **[!UICONTROL toSmartCase]** qui convertit la première lettre de chaque mot en majuscule.
* **[!UICONTROL Salutations]** : insère des salutations avec le nom du destinataire. Par exemple : &quot;Bonjour John Doe,&quot;.
* **[!UICONTROL Insertion du logo]** : insère un logo défini dans les paramètres de l’instance.
* **[!UICONTROL Lien vers la page miroir]** : insère un lien vers la page miroir : « Si vous ne parvenez pas à voir correctement ce message, cliquez ici ».
* **[!UICONTROL URL de page miroir]** : insère l&#39;URL de page miroir qui permet aux concepteurs de diffusion de vérifier le lien.
* **[!UICONTROL URL d’acceptation des offres en mode unitaire]** : insère une URL permettant de définir une offre sur **[!UICONTROL Acceptée]**.
* **[!UICONTROL URL de la page d’enregistrement]** : insère une URL d’abonnement.
* **[!UICONTROL Lien d&#39;inscription]** : insère un lien d&#39;inscription. Ce lien est défini dans les paramètres de l&#39;instance. Le contenu par défaut est le suivant : &quot;Pour vous inscrire, cliquez ici.&quot;
* **[!UICONTROL Lien d&#39;inscription (avec parrain)]** : insère un lien d&#39;inscription permettant d&#39;identifier le visiteur et la diffusion. Ce lien est défini dans les paramètres de l&#39;instance.
* **[!UICONTROL Confirmation de votre inscription]** : insère un lien permettant de confirmer l&#39;inscription.
* **[!UICONTROL Liens de partage sur les réseaux sociaux]** : insère des boutons permettant au destinataire de partager un lien vers le contenu de la page miroir.
* **[!UICONTROL Style des emails de contenu]** et **[!UICONTROL Style de notification]** : génèrent un code permettant de formater un email avec les styles HTML par défaut.
* **[!UICONTROL Lien de désinscription]** : insère un lien permettant de se désabonner de toutes les diffusions (liste bloquée). Le contenu associé par défaut est : &quot;Vous recevez ce message car vous avez été en contact avec ***nom de votre organisation*** ou un affilié. Pour ne plus recevoir de messages de ***nom de votre organisation*** cliquez ici.&quot;


## Personnalisation des liens dans vos emails {#personalize-links}

Pour personnaliser une **link**:

1. Sélectionnez un bloc de texte ou une image.
1. Dans la barre d’outils contextuelle, sélectionnez **Lien d’insertion**.

   ![](assets/perso-link.png)

1. Saisissez le libellé du lien et utilisez la méthode **Lien d’insertion** pour personnaliser le lien.

   ![](assets/perso-link-insert-icon.png)

1. Utilisez l’éditeur de personnalisation pour définir et personnaliser le lien, puis validez.

   ![](assets/perso-link-edit.png)


## Personnaliser vos offres {#personalize-offers}

Vous pouvez également accéder à l’éditeur de personnalisation lorsque vous ajoutez du contenu de type texte aux représentations de vos offres. En savoir plus dans [cette section](../content/offers.md).
