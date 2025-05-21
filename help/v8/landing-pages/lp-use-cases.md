---
solution: Campaign, Campaign v8 Web User Interface
title: Cas d’utilisation de page de destination
description: Découvrir les cas d’utilisation les plus courants pour les pages de destination dans l’interface utilisateur web de Campaign
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: destination, page de destination, cas d’utilisation
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: a9ce4fd103c4af8f47ba887031e8d6d53e8d5f0b
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 100%

---

# Comment utiliser une page de destination {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copier l’URL avec précaution"
>abstract="Pour tester ou tirer pleinement profit de votre page de destination, vous ne pouvez pas copier-coller ce lien directement dans un navigateur web ou dans vos diffusions. Utilisez plutôt la fonction **Simuler le contenu** pour la tester, et suivez les étapes décrites dans la documentation pour utiliser correctement votre page de destination."

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="Copier l’URL avec précaution"
>abstract="Lors de la création d’une page de destination, quatre modèles prêts à l’emploi permettent de mettre en œuvre différents cas pratiques : ajouter ou mettre à jour un profil dans la base de données Campaign, abonner des clientes et clients à un service, les désabonner d’un service ou exclure des utilisateurs et utilisatrices."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html?lang=fr#create-landing-page" text="Créer une page de destination"

Pour utiliser correctement votre page de destination, référencez-la en tant que lien dans un message à l’aide de l’option dédiée. Vous ne pouvez pas copier-coller le lien affiché dans le tableau de bord des diffusions publiées directement dans vos diffusions ou dans une page web. Utilisez plutôt la fonctionnalité **Simuler le contenu** pour le tester.

Dans l’interface [!DNL Adobe Campaign Web], quatre modèles prêts à l’emploi vous permettent de mettre en œuvre différents cas d’utilisation. Toutefois, les étapes principales restent les mêmes et sont décrites ci-dessous.

1. [Créez une page de destination](create-lp.md#create-landing-page) et sélectionnez le modèle de votre choix, en fonction de votre cas d’utilisation.

1. Définissez les propriétés et les paramètres de la page de destination.

   ![Capture d’écran montrant l’interface des propriétés et des paramètres de la page de destination.](assets/lp-uc-properties.png){zoomable="yes"}

1. Selon votre cas, sélectionnez la page **[!UICONTROL Acquisition]**, **[!UICONTROL Abonnement]**, **[!UICONTROL Désabonnement]** ou **[!UICONTROL Liste bloquée]**.

1. Le contenu de la page s’affiche. Sélectionnez la partie correspondant au formulaire de page de destination.

   ![Capture d’écran montrant l’interface des formulaires de page de destination.](assets/lp-uc-form.png){zoomable="yes"}

1. Modifiez votre contenu en fonction du modèle sélectionné :

   * [Acquisition](#lp-acquisition)
   * [Abonnement](#lp-subscription)
   * [Désabonnement](#lp-unsubscription)
   * [Liste bloquée](#lp-denylist)

1. Modifiez le reste de votre contenu selon vos besoins, enregistrez vos modifications et fermez.

1. Modifiez la page **[!UICONTROL Confirmation]** si nécessaire, ainsi que les pages **[!UICONTROL Erreur]** et **[!UICONTROL Expiration]**. La page **[!UICONTROL Confirmation]** s’affichera pour vos personnes destinataires une fois le formulaire envoyé.

   ![Capture d’écran montrant l’interface de la page de confirmation.](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. [Testez](create-lp.md#test-landing-page) et [publiez](create-lp.md#publish-landing-page) votre page de destination.

1. Créez une diffusion [e-mail](../email/create-email.md) pour diriger le trafic vers la page de destination.

1. [Insérez un lien](../email/message-tracking.md#insert-links) dans le contenu de votre message. Sélectionnez **[!UICONTROL Page de destination]** comme **[!UICONTROL Type de lien]** et sélectionnez la page de destination que vous avez créée.

   ![Capture d’écran montrant l’interface d’insertion de liens d’e-mail.](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >Pour pouvoir envoyer votre message, vérifiez que la page de destination sélectionnée n’a pas encore expiré. [En savoir plus](create-lp.md#create-landing-page)

Une fois qu’elles ont reçu l’e-mail, si vos personnes destinataires cliquent sur le lien vers la page de destination et envoient le formulaire :

* Elles seront redirigées vers la page de confirmation.
* Toute autre action définie dans votre page de destination sera appliquée. Par exemple, soit les utilisateurs et utilisatrices seront abonnés à votre service, soit ils ne recevront plus de communications de votre part.

Vous trouverez ci-dessous quelques exemples d’utilisation des pages de destination [!DNL Adobe Campaign] dans les différents cas d’utilisation possibles.

## Acquisition de profils {#lp-acquisition}

Le premier modèle vous permet d’ajouter ou de mettre à jour un profil dans la base de données Campaign.

1. Lors de la [création de votre page de destination](create-lp.md#create-landing-page), sélectionnez le modèle **[!UICONTROL Acquisition]**.

1. Dans les propriétés de la page de destination, sélectionnez l’option **[!UICONTROL Préremplir avec les données référencées dans le formulaire]** afin de précharger les informations existantes du profil et d’éviter de créer des doublons.

1. Sélectionnez la page **[!UICONTROL Acquisition]** pour modifier son contenu.

1. Modifiez les champs de texte selon les besoins, en fonction des informations que vous souhaitez rassembler sur vos profils.

1. Ajoutez une case à cocher invitant vos clientes et clients à s’abonner à votre service de newsletter. [Découvrir comment créer un service](../audience/manage-services.md)

   ![Capture d’écran montrant l’interface de la page d’acquisition avec une case à cocher d’abonnement à la newsletter.](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. Ajustez votre contenu selon vos besoins et enregistrez vos modifications.

1. Vérifiez et [publiez](create-lp.md#publish-landing-page) votre page de destination.

1. Créez un [e-mail](../email/create-email.md) et [ajoutez un lien](../email/message-tracking.md#insert-links) à votre page de destination.

Une fois l’e-mail reçu, si vos personnes destinataires cliquent sur le lien vers la page de destination et envoient le formulaire, leur profil sera ajouté à la base de données Campaign ou mis à jour avec les informations fournies.

![Capture d’écran montrant un profil mis à jour dans la base de données Campaign.](assets/lp-uc-profile-updated.png){zoomable="yes"}

En cas d’abonnement à votre newsletter, le service correspondant leur sera proposé.

![Capture d’écran montrant une confirmation d’abonnement à la newsletter.](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## Abonnement à un service {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Définir la page de destination d’abonnement"
>abstract="Une page d’abonnement permet à vos clientes et clients de s’abonner à un service."

Un des cas d’utilisation les plus courants consiste à inviter vos clientes et clients à [s’abonner à un service](../audience/manage-services.md) (comme une newsletter ou un événement) via une page de destination. Suivez les étapes ci-dessous.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Créez un modèle de confirmation pour les utilisateurs et utilisatrices qui s’abonnent à votre événement, afin que vous puissiez le sélectionner facilement lors de la création du service. [En savoir plus](../audience/manage-services.md#create-confirmation-message)

   ![Capture d’écran montrant l’interface du modèle d’e-mail de confirmation.](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. Créez un service d’abonnement qui stockera les personnes enregistrées dans votre événement. [Découvrir comment créer un service](../audience/manage-services.md)

1. Sélectionnez le modèle que vous avez créé comme e-mail de confirmation que les personnes recevront lors de leur inscription.

   ![Capture d’écran montrant l’interface du service d’abonnement.](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. [Créez une page de destination](create-lp.md#create-landing-page) pour permettre aux personnes destinataires de s’inscrire à votre événement. Sélectionnez le modèle **[!UICONTROL Abonnement]**.

1. Sélectionnez la page **[!UICONTROL Abonnement]** pour modifier son contenu.

1. Le contenu de la page s’affiche. Sélectionnez la partie correspondant au formulaire la de page de destination et développez la section **[!UICONTROL Case à cocher 1]**.

1. Dans le champ **[!UICONTROL Abonnements et services]**, sélectionnez le service que vous avez créé pour votre événement. Laissez l’option **[!UICONTROL S’abonner à si cette option est cochée]** activée.

   ![Capture d’écran montrant l’interface de la case à cocher d’abonnement.](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Ajustez votre contenu selon vos besoins et enregistrez vos modifications.

1. Révisez et [publiez](create-lp.md#publish-landing-page) votre page de destination.

1. Créez un [e-mail](../email/create-email.md) et [ajoutez un lien](../email/message-tracking.md#insert-links) pour diriger le trafic vers la page de destination de l’enregistrement.

1. Concevez l’e-mail pour annoncer que l’inscription à votre événement est maintenant ouverte.

Une fois l’e-mail reçu, si vos personnes destinataires cliquent sur le lien vers la page de destination et envoient le formulaire, elles sont redirigées vers la page de confirmation et sont ajoutées à la liste d’abonnements.

## Désabonnement {#lp-unsubscription}

Vous pouvez permettre à vos clientes et clients de se désabonner d’un service à l’aide d’une page de destination.

1. Créez un modèle de confirmation pour les utilisateurs et utilisatrices qui se désabonnent de votre service, afin que vous puissiez le sélectionner facilement lors de la création du service. [En savoir plus](../audience/manage-services.md#create-confirmation-message)

1. Dans votre [service d’abonnement](../audience/manage-services.md), sélectionnez le modèle que vous avez créé comme e-mail de confirmation que les utilisateurs et utilisatrices recevront lors de leur désinscription.

1. [Créez une page de destination](create-lp.md#create-landing-page). Sélectionnez le modèle **[!UICONTROL Désinscription]**.

1. Sélectionnez la page **[!UICONTROL Désinscription]** pour modifier son contenu.

1. Le contenu de la page s’affiche. Sélectionnez la partie correspondant au formulaire de page de destination.

1. Ajoutez une section **[!UICONTROL Case à cocher]**, sélectionnez le service et choisissez l’option **[!UICONTROL Se désabonner si cette case est cochée]**.

   ![Capture d’écran montrant l’interface de la case à cocher de désabonnement.](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. Développez la section **[!UICONTROL Appel à l’action]** et sélectionnez l’option **[!UICONTROL Mises à jour supplémentaires]**. Sélectionnez le service et cochez l’option **[!UICONTROL Se désabonner]**.

   ![Capture d’écran montrant l’interface d’appel à l’action pour le désabonnement.](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. Ajustez votre contenu selon vos besoins et enregistrez vos modifications.

1. Prévisualisez et [publiez](create-lp.md#publish-landing-page) votre page de destination.

1. Créez un [e-mail](../email/create-email.md) et [ajoutez un lien](../email/message-tracking.md#insert-links) à la page de destination.

Une fois l’e-mail reçu, si vos personnes destinataires cliquent sur le lien vers la page de destination et soumettent le formulaire, elles seront redirigées vers la page de confirmation de désinscription et sont ajoutées au service d’inscription.

## Liste bloquée {#lp-denylist}

Donner aux personnes destinataires la capacité de se désabonner des communications d’une marque est une obligation légale. Par conséquent, vous devez toujours inclure un **lien de désabonnement** dans chaque e-mail envoyé aux personnes destinataires. Lorsque vous cliquez sur ce lien, les personnes destinataires sont redirigées vers une page de destination comprenant un bouton pour confirmer leur désinscription.

Vous pouvez configurer une page de destination **[!UICONTROL Liste bloquée]**, qui permettra aux utilisateurs et utilisatrices de se désinscrire de toutes les diffusions.

1. Au cours de la [création de votre page de destination](create-lp.md#create-landing-page), sélectionnez le modèle **[!UICONTROL Liste bloquée]**.

1. Sélectionnez la page **[!UICONTROL Liste bloquée]** pour modifier son contenu.

1. Développez la section **[!UICONTROL Appel à l’action]** et sélectionnez l’option **[!UICONTROL Mises à jour supplémentaires]**.

1. Dans la liste déroulante correspondante, sélectionnez **[!UICONTROL Canal (e-mail)]** pour permettre aux personnes destinataires de ne pas recevoir de communications par e-mail uniquement. Vous pouvez également sélectionner **[!UICONTROL Tous les canaux]** pour les exclure des communications sur tous les canaux.

   ![Capture d’écran montrant l’interface de la liste de blocage](assets/lp-uc-denylist.png){zoomable="yes"}

1. Ajustez votre contenu selon vos besoins et enregistrez vos modifications.

1. Vérifiez et [publiez](create-lp.md#publish-landing-page) votre page de destination.

1. Créez un [e-mail](../email/create-email.md) et [ajoutez un lien](../email/message-tracking.md#insert-links) à votre page de destination afin de permettre aux utilisateurs et aux utilisatrices de se désinscrire des communications.

Une fois l’e-mail reçu, si vos personnes destinataires cliquent sur le lien vers la page de destination et soumettent le formulaire, elles seront redirigées vers la page de confirmation de liste bloquée et leur profil sera mis à jour avec les informations qu’elles ont fournies.

Pour vérifier que le choix du profil correspondant a été mis à jour, accédez au menu **[!UICONTROL Profils]** et sélectionnez le profil concerné.

Par exemple, si vous choisissez de mettre à jour l’option **[!UICONTROL Canal (e-mail)]** dans votre page de destination, l’option **[!UICONTROL Ne plus contacter par e-mail]** est cochée.

![Capture d’écran montrant un profil dont les préférences de liste de blocage ont été mises à jour.](assets/lp-uc-denylist-profile.png){zoomable="yes"}

Ce profil ne recevra pas de communications par e-mail de votre marque, sauf en cas de nouvel abonnement.