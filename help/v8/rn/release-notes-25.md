---
title: Notes de mise à jour précédentes de l’interface d’utilisation web de Campaign v8
description: Versions de 2025 de l’interface d’utilisation web de Campaign
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: ec994efb6f88b729fe2dc9d7ba118e9ada10be9a
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 100%

---

# Notes de mise à jour 2025 {#2025-release}

Cette page répertorie toutes les modifications et améliorations disponibles dans les **versions de 2025**. Les dernières notes de mise à jour sont disponibles dans [cette page](release-notes.md).

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
<p>Pour plus d’informations sur l’assistant IA, consultez la <a href="../email/generative-lp.md">documentation détaillée</a>.</p>
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
