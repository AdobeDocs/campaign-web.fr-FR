---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: ht
source-wordcount: '900'
ht-degree: 100%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont répertoriées sur les pages [2024](release-notes-24.md) et [2025](release-notes-25.md).

## Version de juillet 2025 {#25-7-release}

### Nouvelles fonctionnalités {#25-7-features}

Les fonctionnalités suivantes sont disponibles à compter de la version de juillet.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Prise en charge de CSS personnalisé dans le concepteur d’e-mail</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Lors de la conception de vos e-mails, vous pouvez désormais ajouter votre propre CSS personnalisé directement dans le concepteur d’e-mail. Cette fonctionnalité vous permet d’appliquer un style avancé et spécifique, pour une plus grande flexibilité et un meilleur contrôle de l’aspect de votre contenu.</p>
<p>Pour plus d’informations, consultez la <a href="../email/custom-css.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Marques</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer et personnaliser vos propres marques pour définir clairement votre identité visuelle et verbale dans les communications. Grâce au score d’alignement de la marque, vous pouvez recevoir des commentaires en temps réel sur la manière dont votre contenu reflète le ton, le style et les directives de votre marque, ce qui vous permet de rester constamment en phase avec la marque pour chaque message envoyé.
</p>
<p>Pour plus d’informations, consultez la <a href="../content/brands.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Alertes de diffusion</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonctionnalité Alertes de diffusion est un système de gestion des alertes qui permet à un groupe d’utilisateurs et d’utilisatrices de recevoir automatiquement des notifications contenant des informations sur l’exécution de leurs diffusions.</p>
<p>Pour plus d’informations, consultez la <a href="../msg/delivery-alerting.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>Rapports dynamiques</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais accéder aux rapports dynamiques qui fournissent des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, comme le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. Les rapports dynamiques sont également disponibles pour les diffusions d’e-mails multilingues et les messages transactionnels.</p>
<p>Cette fonctionnalité n’est disponible qu’à la demande. Pour y accéder, contactez votre représentant ou représentante Adobe. Votre serveur doit être mis à niveau vers la version 8.8.1 au minimum. Reportez-vous aux <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr-FR" target="_blank">notes de mise à jour</a> de la console cliente.
<p>Pour plus d’informations, consultez la <a href="../reporting/dynamic-reporting/get-started-reporting.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Branding centralisé</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les administrateurs et administratrices techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. Par exemple : le logo de la marque, le domaine d’URL d’accès aux pages de destination ainsi que les paramètres du tracking des messages. Vous pouvez créer ces marques et les associer à des messages ou à des pages de destination. Cette configuration est gérée dans des modèles. Les options de branding sont désormais disponibles pour tous les canaux, y compris les SMS et le courrier.</p>
<p>Cette fonctionnalité est uniquement disponible à la demande pour les nouvelles implémentations. Pour y accéder, contactez votre représentant ou représentante Adobe. Votre serveur doit être mis à niveau vers la version 8.8.1 au minimum. Reportez-vous aux <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr-FR" target="_blank">notes de mise à jour</a> de la console cliente.
<p>Pour plus d’informations, consultez la <a href="../administration/branding/branding-gs.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

Outre les fonctionnalités répertoriées ci-dessus, cette version comprend également un ensemble de fonctionnalités disponibles dans la console cliente :

* [Nouveau connecteur d’envoi de SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=fr) (environnements FDA)
* [API Rest](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=fr) (à la demande, environnements FDA)

Reportez-vous aux [notes de mise à jour](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr-FR){target="_blank"} de la console cliente.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=fr){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=fr) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=fr) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr){target="_blank"}.

-->

### Améliorations {#25-7-improvements}

* Vous pouvez désormais calculer la population cible directement sur chaque condition et groupe dans le créateur de règles. Cliquez sur le numéro du résultat pour afficher la liste détaillée des enregistrements. [En savoir plus](../query/build-query.md#validate-query)

* Vous pouvez désormais modifier ou supprimer un filtre prédéfini directement à partir du créateur de règles. [En savoir plus](../get-started/predefined-filters.md#manage-predefined-filter)

* Lors de la configuration d’une diffusion par SMS, dans la section **SMS**, vous avez désormais accès aux **Paramètres SMPP facultatifs (TLV)**. Ce paramètre est identique à celui de la console cliente. [En savoir plus](../advanced-settings/delivery-settings.md#sms-tab)

* Vous pouvez désormais activer les notifications en arrière-plan sur iOS à l’aide de la nouvelle option **Contenu disponible**, disponible dans la section **Paramètres avancés** de l’écran d’édition du contenu d’iOS. L’indicateur `content-available:1` est alors ajouté au payload `aps`. Consultez [cette page](../push/content-push.md) pour en savoir plus. Voir également [cette page](../push/rich-push-ios.md)

* Les améliorations suivantes des pages de destination sont désormais disponibles :

   * Vous pouvez désormais référencer une page de destination d’abonnement/de désinscription par défaut lors de la configuration d’un service. Lors de la conception d’un e-mail, si vous définissez un lien vers cette page de destination, les utilisateurs et utilisatrices qui envoient le formulaire de la page de destination sont automatiquement abonnés à ce service ou désinscrits de ce service. [En savoir plus](../audience/manage-services.md#create-service)
   * Une nouvelle option de configuration de page de destination permet aux visiteurs et visiteuses anonymes d’accéder à la page de destination. Si vous désélectionnez cette option, seuls les utilisateurs et les utilisatrices identifiés peuvent accéder au formulaire et l’envoyer. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option de configuration de page de destination permet de stocker des données internes supplémentaires lors de l’envoi de la page de destination. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option permet d’utiliser une page de destination pour plusieurs services, ce qui la rend dynamique. Lors de l’ajout d’un lien vers un e-mail, si vous sélectionnez une page de destination dynamique, vous pouvez sélectionner n’importe quel service. Si vous sélectionnez une page de destination associée à un service spécifique, ce service sera automatiquement utilisé (vous ne pouvez pas en sélectionner un autre). [En savoir plus](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Le contenu conditionnel est désormais pris en charge dans les pages de destination. [En savoir plus](../landing-pages/lp-content.md)
   * Vous pouvez lier une page de destination à un service et envoyer un message de confirmation lorsque des utilisateurs et utilisatrices la valident. [En savoir plus](../landing-pages/lp-content.md#lp-message)
   * Vous pouvez ajouter un captcha pour protéger votre page de destination contre les spams et les abus causés par les robots. Cette action n’implique pas vos clients, car elle ne nécessite aucune interaction de leur part et repose sur les interactions avec votre site. [En savoir plus](../landing-pages/create-lp.md#captcha)
