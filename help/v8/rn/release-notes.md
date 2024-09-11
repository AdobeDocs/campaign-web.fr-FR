---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 166623c699aa1c91b2d4e7530f5b2ea1b54507b4
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 59%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

## Mises à jour de septembre {#9-2024}

<table>
<thead>
<tr>
<th><strong>Assistant d’IA - Accélérateur de contenu</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Une fois que vous avez conçu et personnalisé votre message, redirigez-le vers le niveau supérieur avec l’assistant d’IA dans Adobe Campaign Web for Content Acceleration. Cet outil puissant vous permet d’optimiser l’impact de votre contenu en générant un éventail de texte engageant, de titres principaux et d’images visuellement attrayantes.</p>
<p>Découvrez une expérience pratique avec <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">notre aperçu des fonctionnalités en direct</a>, conçu pour vous permettre d’explorer directement ses fonctionnalités et de comprendre pleinement ses fonctionnalités.</a>.</p>
<p>Pour plus d’informations, consultez la <a href="../email/generative-gs.md">documentation détaillée</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
</td>
</tr>
</tbody>
</table>

## Notes de mise à jour d’août {#24-8-release}

**Date de publication** : 3 septembre 2024

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version d’août.

* **Répartition des valeurs** : lorsque vous accédez à la liste des champs à personnaliser, vous pouvez désormais vérifier comment les valeurs sont distribuées pour chaque champ. Une fenêtre contextuelle dédiée affiche le nombre et le pourcentage de chaque valeur. [En savoir plus](../query/build-query.md#distribution-values-query)

* **Paramètres SMTP** - Les paramètres SMTP sont désormais disponibles dans les paramètres de diffusion email. [En savoir plus](../advanced-settings/delivery-settings.md#smtp)

* **Variables globales** - Vous pouvez désormais définir des variables globales pour définir des valeurs pour vos diffusions. [En savoir plus](../advanced-settings/delivery-settings.md#variables-delivery)

### Nouvelles fonctionnalités en disponibilité limitée {#acs-24-8}

>[!AVAILABILITY]
>
>Les fonctionnalités suivantes sont en disponibilité limitée. Celles-ci sont limitées aux clientes et clients qui effectuent la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et elles ne peuvent pas être déployées dans un autre environnement.
>
>Reportez-vous aux pages de documentation suivantes : [transition Campaign Standard vers Campaign v8](../rn/acs-migration.md) et [Fonctionnalités pour les utilisateurs Campaign Standards](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr){target="_blank"}.

* **Branding du publipostage direct** : les administrateurs et administratrices techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. Par exemple : le logo de la marque, le domaine d’URL d’accès aux pages de destination ainsi que les paramètres du tracking des messages. Vous pouvez à présent créer ces marques et les associer à des messages ou à des pages de destination. Cette configuration est gérée dans des modèles. [En savoir plus](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Abonnements avec landing pages** - Vous pouvez désormais lier une landing page à un service et envoyer un message de confirmation lorsque les utilisateurs la valident. [En savoir plus](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragments visuels** - Vous pouvez désormais archiver des fragments de contenu visuel. [En savoir plus](../content/create-fragment.md#archive)

* **Captcha dans les landing pages** - Vous pouvez maintenant ajouter des captcha pour protéger votre landing page des spams et des abus causés par les robots. Il ne présente pas d’intrusion par rapport à vos clients, car il ne nécessite aucune interaction de leur part et repose sur les interactions avec votre site. [En savoir plus](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
