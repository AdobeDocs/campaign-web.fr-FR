---
title: Notes de mise à jour précédentes de l’interface d’utilisation web de Campaign v8
description: Versions de 2025 de l’interface d’utilisation web de Campaign
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: d70409846dbe950e3e4e475be6866fb5ed9799de
workflow-type: ht
source-wordcount: '1438'
ht-degree: 100%

---

# Notes de mise à jour 2025 {#2025-release}

Cette page répertorie toutes les modifications et améliorations disponibles dans les **versions de 2025**. Les dernières notes de mise à jour sont disponibles dans [cette page](release-notes.md).

## Version de mai 2025 {#25-5-release}

Les fonctionnalités suivantes sont disponibles pour tous les utilisateurs et utilisatrices à compter de la version de mai.

<table>
<thead>
<tr>
<th><strong>Score d’alignement sur la marque (version bêta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonction Score d’alignement sur la marque fournit des commentaires clairs directement dans le concepteur d’e-mail, ce qui vous permet de voir si votre contenu correspond au ton, au style et aux règles de votre marque. Cette fonctionnalité est disponible en version bêta.</p>
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

* **Prise en charge de l’API REST SMS (disponibilité limitée)** : l’API REST de messagerie transactionnelle est désormais disponible pour le canal SMS. Lorsque le payload contient à la fois un e-mail et un téléphone mobile, vous pouvez utiliser le champ « wishedChannel » pour spécifier le canal. S’il n’est pas fourni, l’e-mail est utilisé par défaut, sauf si wishedChannel demande explicitement un SMS. Pour plus d’informations, consultez la [documentation détaillée](https://experienceleague.adobe.com/fr/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

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
