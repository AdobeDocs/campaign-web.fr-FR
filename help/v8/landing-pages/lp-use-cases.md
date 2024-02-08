---
solution: Journey Optimizer
product: journey optimizer
title: Cas d’utilisation de l’URL de la page de destination
description: Découvrir les cas d’utilisation les plus courants pour les pages de destination dans Journey Optimizer
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: destination, page de destination, cas d’utilisation
exl-id: 8c00d783-54a3-45d9-bd8f-4dc58804d922
source-git-commit: 601cc62c5640069ce9e6ee4830f924c610e0915f
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 30%

---

# Comment utiliser une landing page {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copier l’URL avec précaution"
>abstract="Pour tester ou exploiter pleinement votre landing page, vous ne pouvez pas copier-coller ce lien directement dans un navigateur web ou dans vos diffusions. Utilisez plutôt la variable **Simulation du contenu** pour le tester, et suivez les étapes décrites dans la documentation pour utiliser correctement votre landing page."

Pour utiliser correctement votre landing page, vous devez la référencer en tant que lien dans une diffusion à l&#39;aide de l&#39;option dédiée.

>[!CAUTION]
>
>Pour exploiter pleinement votre landing page, vous ne pouvez pas copier-coller le lien affiché dans le tableau de bord des diffusions publiées directement dans vos diffusions ou dans une page web.

Dans le [!DNL Adobe Campaign Web] dans l’interface, quatre modèles d’usine vous permettent de mettre en oeuvre différents cas d’utilisation. Toutefois, les principales étapes restent les mêmes et sont présentées ci-après.

1. [Créer une landing page](create-lp.md#create-landing-page) et sélectionnez le modèle de votre choix, en fonction de votre cas d’utilisation :

   * [Acquisition](#lp-acquisition)
   * [Abonnement](#lp-subscription)
   * [Désabonnement](#lp-unsubscription)
   * [Liste bloquée](#lp-denylist)

1. Définissez les propriétés et les paramètres de la landing page.

   ![](assets/lp-uc-properties.png)

1. Selon votre cas, sélectionnez la variable **[!UICONTROL Acquisition]**, **[!UICONTROL Abonnement]**, **[!UICONTROL Désabonnement]** ou **[!UICONTROL Liste bloquée]** page.

1. Le contenu de la page s’affiche. Sélectionnez la partie correspondant au formulaire de landing page.

   ![](assets/lp-uc-form.png)

1. Effectuez autant de mises à jour des libellés et des champs de landing page que nécessaire. Modifiez le reste de votre contenu comme vous le souhaitez, enregistrez vos modifications et fermez-les.

1. Suivez les étapes détaillées ci-dessous pour chaque cas d’utilisation.

1. Modifiez la variable **[!UICONTROL Confirmation]** si nécessaire, ainsi que la variable **[!UICONTROL Erreur]** et **[!UICONTROL Expiration]** pages. Il sera affiché à vos destinataires une fois qu&#39;ils auront envoyé le formulaire d&#39;inscription.

   ![](assets/lp-uc-confirmation-page.png)

1. Test et [publier](create-lp.md#publish-landing-page) votre landing page.

1. Créez un [email](../email/create-email.md) pour diriger le trafic vers la landing page.

1. [Insérez un lien](../email/message-tracking.md#insert-links) dans le contenu de votre message. Sélectionner **[!UICONTROL Landing page]** comme la propriété **[!UICONTROL Type de lien]** et sélectionnez la variable [landing page](create-lp.md#configure-primary-page) que vous avez créé.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Pour pouvoir envoyer votre message, vérifiez que la page de destination sélectionnée n’a pas encore expiré. Découvrez comment mettre à jour la date d’expiration [dans cette section](create-lp.md#create-landing-page).

Une fois qu&#39;ils ont reçu l&#39;email, si vos destinataires cliquent sur le lien vers la landing page et envoient le formulaire de landing page, ils sont redirigés vers la page de confirmation et toute autre action définie dans votre landing page est appliquée (par exemple, les utilisateurs seront abonnés à votre service, ou vous ne recevrez plus de communications de votre part).

Vous trouverez ci-dessous quelques exemples d’utilisation des pages de destination [!DNL Adobe Campaign] pour que vos clientes et clients s’abonnent à certaines ou toutes vos communications, ou s’en désabonnent.

## Acquisition de profils {#lp-acquisition}

1. [Créer une landing page](create-lp.md#create-landing-page). Sélectionnez la variable **[!UICONTROL Acquisition]** modèle.

1. Définissez les propriétés et les paramètres de la landing page.

   ![](assets/lp-uc-properties.png)

1. Sélectionnez la variable **[!UICONTROL Acquisition]** pour modifier son contenu.

1. Le contenu de la page s’affiche. Sélectionnez la partie correspondant au formulaire de landing page.

## Abonnement à un service {#lp-subscription}

Un des cas d’utilisation les plus courants consiste à inviter vos clientes et vos clients à [s’abonner à un service](../audience/manage-services.md) (comme une newsletter ou un événement) via une page de destination. Suivez les étapes ci-dessous.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Créez tout d&#39;abord un modèle de confirmation pour les utilisateurs qui s&#39;abonnent à votre événement, afin que vous puissiez le sélectionner facilement lors de la création du service. [En savoir plus](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png)

1. Créez un service d’abonnement qui stockera les utilisateurs enregistrés dans votre événement. [Découvrez comment créer un service](../audience/manage-services.md)

1. Sélectionnez le modèle que vous avez créé comme email de confirmation que les utilisateurs recevront lors de leur inscription.

   ![](assets/lp-uc-subscription-service.png)

1. [Créer une landing page](create-lp.md#create-landing-page) pour permettre aux destinataires de s&#39;inscrire à votre événement. Sélectionnez la variable **[!UICONTROL Abonnement]** modèle.

   <!--![](assets/lp-uc-subscription-template.png)-->

1. Définissez les propriétés et les paramètres de la landing page.

   <!--![](assets/lp-uc-properties.png)-->

1. Sélectionnez la variable **[!UICONTROL Abonnement]** pour modifier son contenu.

   ![](assets/lp-uc-subscription-page-edit.png)

1. Le contenu de la page s’affiche. Sélectionnez la partie correspondant au formulaire de landing page et développez l&#39;objet **[!UICONTROL Case à cocher 1]** .

   Dans le **[!UICONTROL Abonnements et services]** , sélectionnez le service que vous avez créé pour votre événement. Laissez le champ **[!UICONTROL S’abonner si coché]** activée.

   ![](assets/lp-uc-subscription-checkbox-1.png)

1. Vous pouvez ajouter une case à cocher supplémentaire pour proposer un abonnement à votre newsletter, par exemple.

<!--

1. You can also update the profiles who register for your event for the email channel. Expand the **[!UICONTROL Call to action]** section and select Additional updates.

    ![](assets/lp-uc-subscription-call-to-action.png)-->

1. Effectuez autant de mises à jour des libellés et des champs de landing page que nécessaire. Modifiez le reste de votre contenu comme vous le souhaitez, enregistrez vos modifications et fermez-les.

1. Modifiez la variable **[!UICONTROL Confirmation]** si nécessaire, ainsi que la variable **[!UICONTROL Erreur]** et **[!UICONTROL Expiration]** pages. Il sera affiché à vos destinataires une fois qu&#39;ils auront envoyé le formulaire d&#39;inscription.

   ![](assets/lp-uc-confirmation-page.png)

1. Test et [publier](create-lp.md#publish-landing-page) votre landing page.

1. Créez un **Email** pour diriger le trafic vers la landing page d’inscription. Concevez le courrier électronique pour annoncer que l’enregistrement est désormais ouvert pour votre événement.

1. [Insérez un lien](../email/message-tracking.md#insert-links) dans le contenu de votre message. Sélectionnez **[!UICONTROL Page de destination]** comme **[!UICONTROL Type de lien]** et sélectionnez la [page de destination](create-lp.md#configure-primary-page) que vous avez créée pour l’inscription.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Pour pouvoir envoyer votre message, vérifiez que la page de destination sélectionnée n’a pas encore expiré. Découvrez comment mettre à jour la date d’expiration [dans cette section](create-lp.md#create-landing-page).

A la réception de l&#39;email, si vos destinataires cliquent sur le lien vers la landing page et envoient le formulaire de landing page, ils seront redirigés vers la page de confirmation et ils seront ajoutés à la liste d&#39;inscription.

## Désabonnement {#lp-unsubscription}

1. [Créer une landing page](create-lp.md#create-landing-page). Sélectionnez la variable **[!UICONTROL Désabonnement]** modèle.

1. Définissez les propriétés et les paramètres de la landing page.

1. Sélectionnez la variable **[!UICONTROL Désabonnement]** pour modifier son contenu.

1. Le contenu de la page s’affiche. Sélectionnez la partie correspondant au formulaire de landing page.

## Configuration des landing pages de désinscription {#lp-denylist}

Donner aux personnes destinataires la capacité de se désabonner des communications d’une marque est une obligation légale. En savoir plus sur la législation applicable dans la [documentation Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/privacy/regulations/overview.html?lang=fr#regulations){target="_blank"}.

Par conséquent, vous devez toujours inclure un **lien de désabonnement** dans chaque e-mail envoyé aux personnes destinataires :

* Lorsque vous cliquez sur ce lien, les personnes destinataires sont redirigées vers une page de destination comprenant un bouton pour confirmer leur désinscription.
* Lorsque vous cliquez sur le bouton de désinscription, les données de profil sont mises à jour avec ces informations.

Vous pouvez configurer une **[!UICONTROL Liste bloquée]** landing page qui permettra aux utilisateurs de se désinscrire de toutes les diffusions.

Pour permettre aux utilisateurs de se désinscrire de toutes les diffusions, vous devez créer et publier un **[!UICONTROL Liste bloquée]** landing page.

Lorsqu&#39;un utilisateur clique sur le lien de la landing page, l&#39;option **[!UICONTROL Ne plus contacter (tous canaux)]** du profil est automatiquement sélectionnée.

![](assets/blocklisting_allchannels.png)

définir une **[!UICONTROL Exclusion]** et choisissez de mettre à jour **[!UICONTROL Canal (email)]**: le profil qui coche la zone d’exclusion sur votre page d’entrée sera exclu de toutes vos communications.

Une fois le message reçu, si une personne destinataire clique sur le lien de désabonnement dans l’e-mail, votre page de destination s’affiche.

![](assets/lp_opt-out-submit-form.png)

Si la personne destinataire coche la case et envoie le formulaire :

* La personne destinataire qui se désabonne est redirigée vers l’écran du message de confirmation.

* Les données de profil sont mises à jour et le profil ne recevra aucune communication de votre marque, sauf s’il s’abonne à nouveau.

Pour vérifier que le choix du profil correspondant a été mis à jour, accédez à Profils et sélectionnez le profil.







