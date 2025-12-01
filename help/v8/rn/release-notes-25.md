---
title: Notes de mise à jour précédentes de l’interface d’utilisation web de Campaign v8
description: Versions de 2025 de l’interface d’utilisation web de Campaign
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '2667'
ht-degree: 100%

---

# Notes de mise à jour 2025 {#2025-release}

Cette page répertorie toutes les modifications et améliorations disponibles dans les **versions de 2025**. Les dernières notes de mise à jour sont disponibles dans [cette page](release-notes.md).

## Version de septembre 2025 {#25-9-release}

_23 septembre 2025_

Les fonctionnalités suivantes sont disponibles à compter de la version de septembre.

<table>
<thead>
<tr>
<th><strong>Canal personnalisé pour les diffusions API</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais, directement à partir de l’interface d’utilisation d’Adobe Campaign Web, orchestrer et exécuter des diffusions basées sur des canaux d’API personnalisés. Ces diffusions peuvent être autonomes ou faire partie d’un workflow. La configuration du canal d’API personnalisé est effectuée dans la console.</p>
<p>Pour plus d’informations, consultez la <a href="../call-center/gs-custom-channel.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Création d’un compte externe</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>En tant qu’administrateur ou administratrice Campaign, vous pouvez désormais configurer de nouvelles connexions avec des systèmes externes à partir de l’interface d’utilisation de Campaign Web. Vous pouvez également afficher, mettre à jour et gérer les comptes externes existants.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/create-external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Verrouillage du contenu des e-mails</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign permet désormais de verrouiller du contenu dans les modèles d’e-mail, en verrouillant soit l’ensemble du modèle, soit des structures et composants spécifiques. Cela vous permet d’éviter les modifications ou suppressions involontaires, de mieux contrôler la personnalisation des modèles et d’améliorer l’efficacité et la fiabilité de vos campagnes par e-mail.</p>
<p>Pour plus d’informations, consultez la <a href="../content/content-locking.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### Améliorations {#25-9-improvements}

* Un ensemble de nouveaux opérateurs a été ajouté lors de la configuration d’une condition à l’aide de la fonctionnalité de contenu conditionnel du Concepteur d’e-mail.
* La dimension de filtrage est désormais disponible dans l’activité de workflow **Créer une audience**. Pour l’afficher ou la modifier, cliquez sur l’icône en regard de la dimension de ciblage. [En savoir plus](../workflows/activities/build-audience.md#build-audience-configuration).
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

## Version d’août 2025 {#25-8-release}

Cette version inclut une série de correctifs, notamment :

* Le processus de duplication des profils a été amélioré pour correspondre au comportement de la console cliente, assurant ainsi une expérience cohérente sur les deux interfaces. Cela corrige un problème qui pouvait empêcher la création des profils dupliqués.

* L’option **[!UICONTROL E-mail Cci]**, dans l’écran de configuration de la diffusion, fonctionne désormais avec Momentum (MTA amélioré). Cette fonctionnalité n’était auparavant disponible que dans la console cliente.

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
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">release notes</a>.
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
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}

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

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

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

## Version du 25 juin {#25-6-release}

### Améliorations {#25-6-improvements}

* Le rapport Résumé de diffusion est désormais disponible pour les canaux Centre d’appel et Personnalisé. [En savoir plus](../reporting/direct-mail.md)

* Lors de la configuration d’une diffusion par SMS, vous avez désormais accès aux paramètres des SMS spécifiques. Il s’agit des mêmes paramètres que dans la console cliente. [En savoir plus](../advanced-settings/delivery-settings.md#sms-tab)

* Vos dossiers favoris s’affichent désormais dans la partie supérieure du panneau de gauche de la page Explorateur, ce qui les rend plus accessibles. [En savoir plus](../get-started/work-with-folders.md#favorite-folders)

* Le créateur de règles prend désormais en charge le glisser-déposer, ce qui vous permet de réorganiser plus efficacement les composants de votre requête. [En savoir plus](../query/build-query.md#drag-and-drop)

* La « condition humaine » dans le créateur de règles a été améliorée. Il s’agit de la version écrite en langage clair de vos règles, affichée en bas de l’écran :

   * Les attributs sont maintenant mis en surbrillance et le schéma associé s’affiche.
   * Vous pouvez cliquer sur ces éléments pour afficher des informations plus détaillées.
   * Vous pouvez désormais copier la condition humaine à l’aide du bouton correspondant.

* L’accès aux dossiers « Workflows techniques » et « Objets créés automatiquement » est désormais restreint afin de les empêcher d’être consultés. [En savoir plus](../get-started/work-with-folders.md#about-folders)

## Version de mai 2025 {#25-5-release}

Les fonctionnalités suivantes sont disponibles pour tous les utilisateurs et utilisatrices à compter de la version de mai.

<table>
<thead>
<tr>
<th><strong>Score d’alignement sur la marque (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonction Score d’alignement sur la marque fournit des commentaires clairs directement dans le concepteur d’e-mail, ce qui vous permet de voir si votre contenu correspond au ton, au style et aux règles de votre marque. Cette fonctionnalité est disponible en version Beta.</p>
<p>Pour plus d’informations, consultez la <a href="../content/brands-score.md">documentation détaillée</a>.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Canal personnalisé pour les diffusions externes</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais orchestrer et exécuter des diffusions directement à partir de l’UI Web d’Adobe Campaign,en fonction de canaux externes personnalisés. Ces diffusions peuvent être autonomes ou faire partie d’un workflow. La création du canal externe personnalisé intégré à un tiers est effectuée dans la console.</p>
<p>Remarque : la création de rapports n’est pas disponible dans l’UI Web pour le canal personnalisé. Vous devez parcourir la console cliente pour accéder aux rapports.</p>
<p>Pour plus d’informations, consultez la <a href="../call-center/gs-custom-channel.md">documentation détaillée</a>.</p>
<img src="assets/do-not-localize/custom-channel.gif">
</td>
</tr>
</tbody>
</table>

### Améliorations {#25-5-improvements}

L’écran de création des règles de typologie a été mis à jour afin de faciliter la sélection du type de règle.

## Version d’avril 2025 {#25-4-release}

**Date de publication** : 29 avril 2025

### Nouvelles fonctionnalités {#25-4-features}

Les fonctionnalités suivantes sont disponibles pour tous les utilisateurs et utilisatrices à compter de la version d’avril.

<table>
<thead>
<tr>
<th><strong>Canal centre d’appel</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Le canal centre d’appel est désormais disponible dans l’interface d’utilisation de Campaign Web. Ce canal fait référence à une méthode de communication utilisée pour gérer et suivre les communications ou interactions gérées par un centre d’appel (généralement des appels téléphoniques passés par des agentes et agents à des clientes et clients ou à des prospects).</p>
<p>Remarque : la création de rapports n’est pas disponible dans l’UI Web pour le canal du centre d’appel. Vous devez parcourir la console cliente pour accéder aux rapports.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Pour plus d’informations, consultez la <a href="../call-center/gs-call-center.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Nouveau créateur de règles</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Un nouveau créateur de règles est désormais disponible pour vous aider à définir des conditions complexes dans une interface d’utilisation améliorée. Vous pouvez passer de l’ancien au nouveau créateur de règles selon vos besoins.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Pour plus d’informations, consultez la <a href="../query/query-modeler-overview.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Création d’un compte externe</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>En tant qu’administrateur ou administratrice Campaign, vous pouvez désormais configurer de nouvelles connexions avec des systèmes externes à partir de l’interface d’utilisation de Campaign Web.
Vous pouvez également afficher, mettre à jour et gérer les comptes externes existants.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#25-4-improvements}

**Améliorations générales de l’interface**

* Les options Description du champ, Ajouter aux favoris et Distribution des valeurs pour les attributs de schéma sont désormais plus visibles dans l’interface d’utilisation. Pour plus d’informations, consultez la [documentation détaillée](../get-started/attributes.md).
* Dans l’interface d’utilisation, la date et l’heure s’affichent désormais en fonction de la langue principale définie dans les préférences d’Experience League. Cette fonctionnalité est uniquement disponible pour plusieurs langues. Pour consulter la liste complète des langues prises en charge, reportez-vous à la [documentation détaillée](https://experienceleague.adobe.com/fr/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Éditeur d’e-mails** : pour améliorer l’accessibilité dans l’interface d’utilisation de Campaign Web, deux nouveaux champs sont désormais disponibles dans le concepteur d’e-mail : ils correspondent à l’élément `title` et l’attribut lang dans l’élément `html` du contenu de votre e-mail. Vous pouvez définir ces paramètres en plus du champ Pré-en-tête, dans la section Corps de l’e-mail. Pour plus d’informations, consultez la [documentation détaillée](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schémas**

* Vous pouvez désormais modifier le schéma temporaire d’une liste à partir de l’interface d’utilisation de Campaign Web. Pour plus d’informations, consultez la [documentation détaillée](../audience/manage-audience.md).
* Vous pouvez désormais prévisualiser les champs personnalisés d’un schéma dans un exemple d’écran. Pour plus d’informations, consultez la [documentation détaillée](../administration/custom-fields.md#add).
* Vous pouvez désormais déplacer des champs personnalisés dans la liste à l’aide du glisser-déposer. Pour plus d’informations, consultez la [documentation détaillée](../administration/custom-fields.md#add).


### Nouvelles fonctionnalités en disponibilité limitée {#25-4-features-la}

>[!AVAILABILITY]
>
>Les fonctionnalités suivantes sont en disponibilité limitée. Elles sont limitées aux clientes et clients effectuant la migration **d’Adobe Campaign Standard à Adobe Campaign v8** et ne peuvent pas être déployées dans un autre environnement. Elles nécessitent une mise à niveau du serveur Campaign vers la version 8.7.4.
>
>Consultez les pages de documentation suivantes : [Transition de Campaign Standard vers Campaign v8](../rn/acs-migration.md) et [Fonctionnalités pour les utilisateurs et les utilisatrices de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr).

* **Création de diffusions multilingues** : vous pouvez désormais envoyer plusieurs diffusions par e-mail dans différentes langues dans l’interface d’utilisation d’Adobe Campaign Web. La fonction Diffusion multilingue permet de choisir la langue par défaut de votre diffusion ainsi que les différentes langues dans lesquelles la diffusion peut être envoyée. Vous pouvez également prévisualiser ces diffusions dans les langues de votre choix. Pour plus d’informations, consultez la [documentation détaillée](../email/edit-content.md).

* **Rapports dynamiques pour le multilinguisme** : les rapports dynamiques sont désormais disponibles pour les diffusions par e-mail multilingues. Pour plus d’informations, consultez la [documentation détaillée](../reporting/global-reports.md).

* **Prise en charge de l’API REST SMS (disponibilité limitée)** : l’API REST de messagerie transactionnelle est désormais disponible pour le canal SMS. Lorsque le payload contient à la fois un e-mail et un téléphone mobile, vous pouvez utiliser le champ « wishedChannel » pour spécifier le canal. S’il n’est pas fourni, l’e-mail est utilisé par défaut, sauf si wishedChannel demande explicitement un SMS. Pour plus d’informations, consultez la [documentation détaillée](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=fr){target=_blank}.

## Version de février 2025 {#25-2-release}

**Date de publication** : 18 février 2025

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version de février.

### Fonctionnalités {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Créer des règles métier (règles de typologie)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer des typologies et des règles de typologie dans l’interface d’utilisation web d’Adobe Campaign. Les typologies permettent de contrôler, de filtrer et de hiérarchiser l’envoi des diffusions. Les typologies permettent de confirmer que les diffusions contiennent toujours certains composants obligatoires (comme un lien de désabonnement ou un objet) ou des règles de filtrage pour exclure des groupes de votre audience (tels que les personnes désabonnées, la concurrence, et la clientèle ne faisant pas partie du programme de fidélité).</p>
<img src="assets/do-not-localize/typology.gif">
<p>Pour plus d’informations, consultez la <a href="../administration/typologies.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Mappings de ciblage</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer des mappings de ciblage dans l’interface d’utilisation web de Campaign. Les mappings de ciblage définissent la manière dont différents canaux de diffusion (e-mails, SMS, notifications push) sont liés aux champs de données d’un schéma. Le mapping de ciblage vous permet de définir l’audience ciblée : profils, bénéficiaires de contrats, opérateurs et opératrices, personnes abonnées, prospects, etc.</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>Pour plus d’informations, consultez la <a href="../administration/target-mappings.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Détails du schéma</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais accéder aux détails d’un schéma en sélectionnant son nom dans la liste. La modification des champs personnalisés est désormais accessible à partir du bouton <b>Modifier les champs personnalisés</b> disponible dans les détails du schéma.</p>
<img src="assets/do-not-localize/schemas.gif">
<p>Pour plus d’informations, consultez la <a href="../administration/schemas.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

## Version de janvier 2025 {#25-1-release}

**Date de publication** : 5 février 2025

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version de janvier.

### Fonctionnalités {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Créer et utiliser des fragments visuels</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les fragments visuels sont des blocs visuels prédéfinis que vous pouvez réutiliser dans plusieurs diffusions e-mail ou dans des modèles de contenu. Cette fonctionnalité est désormais disponible pour les clientes et clients utilisant la version 8.6.4 du serveur et les versions ultérieures.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>Pour plus d’informations, consultez la <a href="../content/use-visual-fragments.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Utiliser un système tiers pour envoyer des diffusions</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais définir des diffusions externes et des modèles de diffusion externe dans l’interface web de Campaign. Avec ce mode, les messages sont compilés dans un fichier de sortie qui peut être partagé avec votre fournisseur externe. Par défaut, le mode de diffusion externe est utilisé pour le canal courrier.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Pour plus d’informations, consultez la <a href="../msg/send-external-deliveries.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gérer vos énumérations</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer des énumérations directement via l’interface d’utilisation web d’Adobe Campaign. Une énumération est une liste de valeurs proposées par le système pour renseigner les champs. Utilisez des énumérations pour normaliser les valeurs de ces champs, faciliter la saisie de données ou les utiliser dans des requêtes.</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>Pour plus d’informations, consultez la <a href="../administration/enumerations.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Créer des options personnalisées</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais accéder aux options techniques de l’interface d’utilisation web d’Adobe Campaign et créer vos propres options personnalisées en fonction de vos besoins. Cela s’avère particulièrement utile lorsque vous travaillez avec des activités de workflow de code JavaScript pour stocker des données intermédiaires.</p>
<img src="assets/do-not-localize/options.gif">
<p>Pour plus d’informations, consultez la <a href="../administration/options.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Définir et appeler des codes JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer des codes JavaScript dans l’interface d’utilisation web d’Adobe Campaign. Vous pouvez ainsi créer des fonctions réutilisables qui peuvent être utilisées dans les workflows, à la manière d’une bibliothèque.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>Pour plus d’informations, consultez la <a href="../administration/javascript-codes.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Génération de page de destination avec l’assistant IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’assistant IA est désormais disponible avec vos diffusions de page de destination, ce qui vous permet de générer du texte, des images ou des mises en page complètes.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Pour plus d’informations sur l’assistant IA, consultez la <a href="../content/generative-full-content.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>


### Améliorations {#25-1-improvements}

* Personnalisez l’affichage des champs personnalisés dans l’interface :

   * Vous pouvez désormais sélectionner d’autres champs personnalisés à afficher dans l’interface.
   * Vous pouvez désormais définir des règles pour l’affichage des champs personnalisés de type lien, par exemple en limitant les valeurs de liste en fonction de l’entrée d’un autre champ.
   * Vous pouvez désormais organiser les champs dans l’interface avec plus de flexibilité : les champs peuvent s’étendre sur une seule colonne ou être regroupés en sous-sections pour une meilleure organisation.
   * Vous pouvez désormais définir des champs spécifiques en lecture seule.

* Filtres récents et favoris : pour réutiliser rapidement des attributs fréquemment utilisés, vous pouvez désormais les ajouter aux favoris. Cela permet de s’assurer qu’ils sont facilement accessibles pour les tâches futures. Outre les favoris, vous pouvez également afficher et utiliser les derniers attributs sélectionnés.

* Comptes externes : le nouveau type **[!UICONTROL Routage]** peut être sélectionné lors de la création d’un compte externe. Il permet de configurer un compte externe spécifique à utiliser dans vos diffusions externes. [En savoir plus](../administration/external-account.md#routing)
