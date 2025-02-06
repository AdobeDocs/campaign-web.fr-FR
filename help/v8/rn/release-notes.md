---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 4ece6d0a766682d65fb4a3f9135b667f558cb51c
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 83%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont répertoriées [sur cette page](release-notes-24.md).

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
<p>Vous pouvez désormais définir des diffusions externes et des modèles de diffusion externe dans l’interface web de Campaign. Dans ce mode, les messages sont compilés dans un fichier de sortie, qui peut être partagé avec votre fournisseur externe. Par défaut, le mode de diffusion externe est utilisé pour le canal courrier.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Pour plus d’informations, consultez la <a href="../msg/send-external-deliveries.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in the Adobe Campaign web interface. A typology is a collection of typology rules that help control, filter, and prioritize deliveries. Typologies ensure that your deliveries always contain required elements (such as an unsubscribe link or subject line) and apply filtering rules to exclude specific groups from your target audience (such as unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

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
<th><strong>Génération de pages de destination avec l’accélérateur de contenu de l’assistant d’IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’accélérateur de contenu de l’assistant d’IA est désormais disponible avec vos diffusions de page de destination, ce qui vous permet de générer du texte, des images ou des mises en page complètes.</p>
<p>Pour plus d’informations sur l’accélérateur de contenu de l’assistant AI, consultez la <a href="../email/generative-lp.md">documentation détaillée</a>.</p>
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

* Comptes externes : le nouveau type **[!UICONTROL Routage]** peut être sélectionné lors de la création d’un compte externe. Il permet de configurer un compte externe spécifique à utiliser dans vos diffusions externes. [En savoir plus](../administration/external-account.md#routing)