---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 62294ce1809caee8af770b376aad97bac71c942c
workflow-type: ht
source-wordcount: '688'
ht-degree: 100%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont dans [2024](release-notes-24.md) et [2025](release-notes-25.md).

## Mises à jour de juillet 2025 {#25-7-updates}

>[!AVAILABILITY]
>
>Pour bénéficier de ces mises à jour, votre serveur doit être mis à niveau vers la version 8.8.1 au minimum. Reportez-vous aux [notes de mise à jour](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr){target="_blank"} de la console cliente.

Publiées précédemment en disponibilité limitée, les fonctionnalités suivantes sont désormais disponibles dans tous les environnements (disponibilité générale) :

* **Création de diffusions multilingues** : vous pouvez désormais envoyer plusieurs diffusions par e-mail dans différentes langues dans l’interface d’utilisation d’Adobe Campaign Web. La fonction Diffusion multilingue permet de choisir la langue par défaut de votre diffusion ainsi que les différentes langues dans lesquelles la diffusion peut être envoyée. Vous pouvez également prévisualiser ces diffusions dans les langues de votre choix. [En savoir plus](../email/edit-content.md#multilingual-delivery).

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=fr){target="_blank"}
-->

* **Alertes de diffusion** : la fonctionnalité Alertes de diffusion est un système de gestion des alertes qui permet à un groupe d’utilisateurs et d’utilisatrices de recevoir automatiquement des notifications contenant des informations sur l’exécution de leurs diffusions. [En savoir plus](../msg/delivery-alerting.md)

* **Améliorations des pages de destination** : les améliorations suivantes ont été apportées aux pages de destination :

   * Vous pouvez désormais référencer une page de destination d’abonnement/de désinscription par défaut lors de la configuration d’un service. Lors de la conception d’un e-mail, si vous définissez un lien vers cette page de destination, les utilisateurs et utilisatrices qui envoient le formulaire de la page de destination sont automatiquement abonnés à ce service ou désinscrits de ce service. [En savoir plus](../audience/manage-services.md#create-service)
   * Une nouvelle option de configuration de page de destination permet aux visiteurs et visiteuses anonymes d’accéder à la page de destination. Si vous désélectionnez cette option, seuls les utilisateurs et les utilisatrices identifiés peuvent accéder au formulaire et l’envoyer. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option de configuration de page de destination permet de stocker des données internes supplémentaires lors de l’envoi de la page de destination. [En savoir plus](../landing-pages/create-lp.md#create-landing-page)
   * Une nouvelle option permet d’utiliser une page de destination pour plusieurs services, ce qui la rend dynamique. Lors de l’ajout d’un lien vers un e-mail, si vous sélectionnez une page de destination dynamique, vous pouvez sélectionner n’importe quel service. Si vous sélectionnez une page de destination associée à un service spécifique, ce service sera automatiquement utilisé (vous ne pouvez pas en sélectionner un autre). [En savoir plus](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Le contenu conditionnel est désormais pris en charge dans les pages de destination. [En savoir plus](../landing-pages/lp-content.md)
   * Vous pouvez lier une page de destination à un service et envoyer un message de confirmation lorsque des utilisateurs et utilisatrices la valident. [En savoir plus](../landing-pages/lp-content.md#lp-message)
   * Vous pouvez ajouter un captcha pour protéger votre page de destination contre les spams et les abus causés par les robots. Cette action n’implique pas vos clients, car elle ne nécessite aucune interaction de leur part et repose sur les interactions avec votre site. [En savoir plus](../landing-pages/create-lp.md#captcha)

Publiées précédemment en disponibilité limitée, les fonctionnalités suivantes sont désormais disponibles **à la demande** :

* **Rapports dynamiques** : vous pouvez désormais accéder aux rapports dynamiques qui fournissent des rapports entièrement personnalisables en temps réel pour mesurer l’impact de vos activités marketing. Ils offrent la possibilité d’accéder aux données de profil, ce qui permet l’analyse démographique par dimensions de profil, comme le genre, la ville et l’âge, en plus des données de campagne par e-mail fonctionnelles comme les ouvertures et les clics. Les rapports dynamiques sont également disponibles pour les diffusions d’e-mails multilingues et les messages transactionnels. [En savoir plus](../reporting/dynamic-reporting/get-started-reporting.md)

* **Branding centralisé** : les administrateurs et administratrices techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. Par exemple : le logo de la marque, le domaine d’URL d’accès aux pages de destination ainsi que les paramètres du tracking des messages. Vous pouvez créer ces marques et les associer à des messages ou à des pages de destination. Cette configuration est gérée dans des modèles. Les options de branding sont désormais disponibles pour tous les canaux, y compris les SMS et le courrier. [En savoir plus](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Cette fonctionnalité est uniquement disponible pour les nouvelles implémentations.

Outre les fonctionnalités répertoriées ci-dessus, cette version comprend également un ensemble de fonctionnalités disponibles dans la console cliente :

* [Nouveau connecteur d’envoi de SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=fr).
* [API REST](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=fr)

Reportez-vous aux [notes de mise à jour](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=fr){target="_blank"} de la console cliente.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=fr){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/fr/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->