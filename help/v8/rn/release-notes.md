---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: a1b1a40be4d2004181f03bba5c43d0302d6f2c47
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 95%

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
<th><strong>Accélérateur de contenu de l’assistant IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Une fois que vous avez conçu et personnalisé votre message, passez au niveau supérieur avec l’accélérateur de contenu de l’assistant d’IA dans Adobe Campaign Web. Cet outil puissant vous permet d’optimiser l’impact de votre contenu en générant un éventail de textes attirants, de grands titres et d’images visuellement attrayantes.</p>
<p>Plongez dans une expérience pratique avec la <a href="https://experienceleague.adobe.com/fr/apps/journey-optimizer/ai-assistant-content-accelerator">prévisualisation de notre fonctionnalité en direct</a>, conçue pour explorer ses capacités en avant-première et comprendre pleinement ses possibilités.</a></p>
<p>Pour plus d’informations, consultez la <a href="../email/generative-gs.md">documentation détaillée</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Date de disponibilité : 12 septembre</p>
</td>
</tr>
</tbody>
</table>

## Notes de mise à jour d’août {#24-8-release}

**Date de publication** : 3 septembre 2024

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version d’août.

* **Répartition des valeurs** : lorsque vous accédez à la liste des champs à personnaliser, vous pouvez désormais vérifier comment les valeurs sont distribuées pour chaque champ. Une fenêtre contextuelle dédiée indique le nombre et le pourcentage pour chaque valeur. [En savoir plus](../query/build-query.md#distribution-values-query)

* **Paramètres SMTP** : les paramètres SMTP sont désormais disponibles dans les paramètres de diffusion par e-mail. [En savoir plus](../advanced-settings/delivery-settings.md#smtp)

* **Variables globales**  : vous pouvez désormais définir des variables globales pour définir des valeurs pour vos diffusions. [En savoir plus](../advanced-settings/delivery-settings.md#variables-delivery)

### Nouvelles fonctionnalités en disponibilité limitée {#acs-24-8}

>[!AVAILABILITY]
>
>Les fonctionnalités suivantes sont en disponibilité limitée. Celles-ci sont limitées aux clientes et clients qui effectuent la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et elles ne peuvent pas être déployées dans un autre environnement.
>
>Consultez les pages de documentation suivantes : [Transition de Campaign Standard vers Campaign v8](../rn/acs-migration.md) et [Fonctionnalités pour les utilisateurs et les utilisatrices de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr){target="_blank"}.

* **Branding du publipostage direct** : les administrateurs et administratrices techniques peuvent désormais définir une ou plusieurs marques afin de centraliser les paramètres qui affectent l’identité d’une marque. Par exemple : le logo de la marque, le domaine d’URL d’accès aux pages de destination ainsi que les paramètres du tracking des messages. Vous pouvez à présent créer ces marques et les associer à des messages ou à des pages de destination. Cette configuration est gérée dans des modèles. [En savoir plus](https://experienceleague.adobe.com/fr/docs/experience-cloud/campaign/branding/branding-assign)

* **Abonnements avec les pages de destination** : vous pouvez désormais lier une page de destination à un service, et envoyer un message de confirmation lorsque des utilisateurs ou utilisatrices la valident. [En savoir plus](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragments visuels** : vous pouvez désormais archiver des fragments de contenu visuel. [En savoir plus](../content/create-fragment.md#archive)

* **Captcha dans les pages de destination** : vous pouvez désormais ajouter un captcha pour protéger votre page de destination contre le spam et les abus causés par les robots. Cette action n’implique pas vos clients, car elle ne nécessite aucune interaction de leur part et repose sur les interactions avec votre site. [En savoir plus](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
