---
audience: end-user
title: Envoyer des offres
description: Envoyer des offres
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: 4faf949f061f62accc80b5e11f99318c18f59d2e
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 99%

---

# Envoyer des offres {#offers-content}

![](../assets/do-not-localize/badge.png)

Adobe Campaign v8 Web vous permet d’envoyer les offres qui ont été créées dans la console à l’aide du module **[!UICONTROL Interaction]** avec les e-mails. Pour plus d’informations sur Interaction et la gestion d’un catalogue d’offres dans la console, consultez la [documentation de Campaign V8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=fr){target="_blank"}.

Les étapes clés pour envoyer des offres avec un e-mail sont les suivantes :

1. [Configurer les offres à proposer](#configure),
1. [Insérer les offres dans l’e-mail](#insert).

## Configurer les offres à proposer {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Paramètres des offres"
>abstract="Configurez les offres qui doivent être proposées aux destinataires."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Paramètres avancés des offres"
>abstract="Configurez les options avancées sur les offres."

1. Pour sélectionner les offres à proposer dans l’e-mail, cliquez sur le bouton **[!UICONTROL Offres]** sur l’écran de modification du contenu de l’e-mail.

   ![](assets/setup-offers.png)

1. Configurez les offres qui doivent être proposées aux destinataires. Sélectionnez d’abord l’**[!UICONTROL emplacement]** correspondant à votre environnement d’offres.

   ![](assets/create-content-offers.png)

1. Pour affiner le choix des offres du moteur, sélectionnez une **[!UICONTROL Catégorie d’offres]** spécifique dans laquelle les offres sont triées.

   Si vous ne sélectionnez aucune catégorie, toutes les offres contenues dans l’environnement sont prises en compte par le moteur d’offres, sauf si vous sélectionnez un **[!UICONTROL Thème d’offre]**.

   >[!NOTE]
   >
   >Les thèmes sont des mots-clés définis en amont dans les catégories. Ils servent de filtre et permettent ainsi d’affiner le nombre d’offres à présenter en les sélectionnant dans un ensemble de catégories.

1. Utilisez le champ **[!UICONTROL Propositions]** pour indiquer le nombre d’offres à insérer dans l’e-mail.

1. Sélectionnez l’option **[!UICONTROL Exclure les destinataires non éligibles]**, si nécessaire.

   Cette option permet d’activer ou désactiver l’exclusion des destinataires pour lesquels il n’y a pas assez d’offres éligibles.

   * Si vous activez cette option, les destinataires qui n’ont pas suffisamment de propositions sont exclus de la diffusion.
   * Si vous désactivez cette option, ces destinataires ne sont pas exclus, mais ils ne peuvent pas avoir le nombre de propositions demandé.

1. Si nécessaire, sélectionnez l’option **[!UICONTROL Masquer tout si aucune offre n’est sélectionnée]**.

   Cette option vous permet de choisir le mode de traitement du message au cas où l’une des propositions n’existerait pas.

   * Si vous activez cette option, la représentation de la proposition manquante ne s’affiche pas et aucun contenu n’apparaît dans le message pour cette proposition.
   * Si vous désactivez cette option, le message est annulé lors de l’envoi et les destinataires ne peuvent plus recevoir de messages.

Une fois que vous avez configuré les offres à proposer, vous pouvez les insérer dans l’e-mail à l’aide de l’éditeur d’expression. [Découvrez comment insérer des offres dans l’e-mail](#insert).

## Insérer des offres dans l’e-mail {#insert}

Vous pouvez ajouter des offres à l’e-mail à l’aide de l’éditeur d’expression. Vous pouvez les insérer de l’une des manières suivantes :

* dans l’objet de l’e-mail,
* dans le corps de l’e-mail en autorisant la personnalisation dans n’importe quel composant de contenu. [Découvrez comment ajouter des composants de contenu](content-components.md).

>[!NOTE]
>
>Avant d’insérer une offre, vérifiez que vous avez [configuré les offres à proposer avec l’e-mail](#configure).

Pour insérer une offre à l’aide de l’éditeur d’expression, procédez comme suit :

1. Ouvrez l’éditeur d’expression, puis sélectionnez le menu **[!UICONTROL Propositions]**.

   Les propositions disponibles s’affichent dans la liste. Vous définissez le nombre de propositions lors de la configuration des offres à proposer.

   ![](assets/offer-insertion.png)

1. Ajoutez les propositions dans l’objet ou le corps de l’e-mail à l’aide des champs de personnalisation, des fonctions de rendu ou des attributs d’offre disponibles pour chaque proposition.

   ![](assets/offer-inserted.png)
