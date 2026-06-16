---
title: Notes de mise à jour précédentes de l’interface d’utilisation web de Campaign v8
description: Versions de l’interface d’utilisation web de Campaign 2026
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 4eae8f0ea3c176a12e040f7406aac699e14a5ba8
workflow-type: tm+mt
source-wordcount: '1204'
ht-degree: 97%

---

# Notes de mise à jour 2026 {#2026-release}

Cette page répertorie toutes les modifications et améliorations disponibles dans les **versions 2026**. Les dernières notes de mise à jour sont disponibles dans [cette page](release-notes.md).

## Version d’avril 2026 {#26-4-release}

_29 avril 2026_

### Amélioration {#26-4-improvement}

La section **Données d’enrichissement** est désormais disponible dans l’activité de workflow **Créer une audience** (type requête). Vous pouvez afficher, ajouter, modifier et supprimer des **données supplémentaires** directement depuis l’interface d’utilisation de Campaign Web. Comme dans l’activité **Enrichissement**, vous pouvez ajouter des attributs d’enrichissement uniques, des liens de collection et des expressions.

[En savoir plus](../workflows/activities/build-audience.md)

## Version de mars 2026 {#26-3-release}

_24 mars 2026_

### Nouvelles fonctionnalités {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Création de schémas (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonctionnalité de création de schémas est désormais disponible pour toutes les clientes et tous les clients (GA). Cette fonctionnalité permet de créer et de gérer des schémas directement à partir de l’interface d’utilisation de Campaign Web. Vous pouvez créer des tables, étendre des schémas existants et créer des formulaires personnalisés. Vous pouvez définir des structures de données personnalisées pour répondre aux besoins spécifiques de votre entreprise, sans avoir à accéder à la console cliente.</p>
<p>Pour plus d'informations, consultez la <a href="../administration/schemas.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Thèmes dans le Concepteur d’e-mail (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les thèmes offrent une expérience de création d’e-mails améliorée en vous permettant de définir des styles de thèmes réutilisables qui correspondent aux directives de votre marque. Vous pouvez désormais utiliser des variables de thème dans des fragments, ce qui garantit une mise en forme cohérente dans vos modèles d’e-mail. Cette fonctionnalité permet de créer des e-mails plus rapidement avec des modules prédéfinis qui résument des éléments de contenu tels que des titres, des descriptions, des images et des liens, tout en préservant la cohérence de la marque.</p>
<p>Remarque : cette fonctionnalité n’est disponible que pour un ensemble d’organisations donné (disponibilité limitée) et sera déployée en disponibilité générale dans une prochaine version.</p>
<p>Pour plus d'informations, consultez la <a href="../email/apply-email-themes.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Intégration de modèles Firefly personnalisés et de modèles de génération d’images tiers</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Activez l’intégration transparente des modèles Firefly standard et personnalisés, ainsi que des modèles d’image tiers approuvés, afin d’offrir une plus grande flexibilité, un meilleur contrôle et un meilleur alignement de la marque lors de la génération d’images.</p>
<p>Choisissez le modèle adapté à vos besoins :</p>
<ul><li> <strong>Modèle Adobe</strong> (optimisé par Firefly Image Model 4) pour la génération immédiate d’images sans configuration supplémentaire</li><li> <strong>Modèle de partenaire</strong> (optimisé par Gemini 2.5 Flash) pour des fonctionnalités spécialisées</li><li><strong>Modèles personnalisés</strong> (modèles spécifiques à la marque entraînés sur vos propres ressources) pour une génération conforme à la marque qui s’aligne précisément sur l’identité, le style et les directives visuelles de votre marque.</li></ul>
<p>Pour plus d’informations, consultez la <a href="../content/generative-models.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Activité de diffusion automatisée</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’activité de workflow <strong>Diffusion automatisée</strong> est désormais disponible dans la palette du workflow. Vous pouvez l’utiliser pour créer ou exécuter des actions de diffusion (préparer, envoyer un BAT, préparer et démarrer, etc.) directement dans votre workflow. Sélectionnez une diffusion existante, créée en dehors du workflow, pour la réutiliser à chaque exécution ou créez une diffusion à partir d'un modèle à chaque fois que l’activité s’exécute.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Pour plus d’informations, consultez la <a href="../workflows/activities/automated-delivery.md">documentation détaillée.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Branches de workflow multiples et activité Jointure</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>Les <strong>branches multiples</strong> sont désormais prises en charge. Au lieu d’utiliser un <strong>branchement</strong>, vous pouvez cliquer sur <strong>Ajouter une branche</strong> dans la barre d’outils. L’activité <strong>Rendez-vous</strong> a également été améliorée. Il s’agit désormais d’une activité <strong>Jointure</strong> générique qui vous permet de choisir entre les options de jointure AND et OR.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Pour plus d’informations, consultez les pages de documentation <a href="../workflows/orchestrate-activities.md#toolbar">Orchestrer les activités</a> et <a href="../workflows/activities/join.md">Jointure</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#26-3-improvements}

* L’activité de workflow **Démarrer** a été ajoutée pour améliorer la compatibilité avec la console cliente. Cette activité est facultative et n’est pas insérée par défaut dans les nouveaux workflows. Toutefois, elle est ajoutée automatiquement aux workflows existants.
  [En savoir plus](../workflows/activities/about-activities.md#flow-control)
* Le champ de sélection du fuseau horaire dans les paramètres **Planifier** d’une diffusion a été déplacé sous le champ **Date de contact**. [En savoir plus](../msg/create-deliveries.md#gs-schedule)

## Version de février 2026 {#26-2-release}

_17 février 2026_

### Nouvelles fonctionnalités {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>Vue Chronologie dans l’inventaire des campagnes</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’inventaire des campagnes comprend désormais une vue Chronologie qui permet de visualiser et de gérer les campagnes au fil du temps : basculer entre la liste et la chronologie, naviguer par semaine, mois ou jour, utiliser le bouton Aujourd’hui pour accéder à la date du jour et ouvrir les détails de la campagne (statut, workflows, diffusions) dans un panneau de droite, avec les mêmes filtres et recherches que la vue Liste.</p>
<p>Pour plus d'informations, consultez la <a href="../campaigns/manage-campaigns.md#timeline">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Création de schémas (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais créer et gérer des schémas directement à partir de l’interface d’utilisation web de Campaign. Cette fonctionnalité permet de créer des tables, d’étendre les schémas existants et de créer des formulaires personnalisés. Vous pouvez définir des structures de données personnalisées pour répondre aux besoins spécifiques de votre entreprise, sans avoir à accéder à la console cliente.</p>
<p>Remarque : cette fonctionnalité n’est disponible que pour un ensemble d’organisations donné (disponibilité limitée) et sera déployée en disponibilité générale dans une prochaine version.</p>
<p>Pour plus d'informations, consultez la <a href="../administration/schemas.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

## Version de janvier 2026 {#26-1-release}

_27 janvier 2026_

### Nouvelles fonctionnalités {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Fonctionnalités de diffusion multilingue (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonctionnalité de diffusion multilingue est désormais disponible pour tous les clients (GA). Cette fonctionnalité vous permet d’envoyer plusieurs messages dans différentes langues dans l’interface utilisateur web d’Adobe Campaign. Vous pouvez choisir la langue par défaut de votre diffusion ainsi que les différentes langues dans lesquelles la diffusion peut être envoyée. Vous pouvez également prévisualiser ces diffusions dans les langues de votre choix. 
<p>Pour plus d'informations, consultez la <a href="../msg/multilingual.md">documentation détaillée</a>.</p>
<p>Les améliorations suivantes ont été apportées aux notifications push multilingues :</p>
<ul>
<li>Vous pouvez désormais remplir rapidement toutes les variantes de langue en chargeant un fichier CSV contenant votre contenu multilingue. <a href="../msg/multilingual.md#csv-upload">En savoir plus</a>
</li>
<li>Les notifications push riches sont désormais prises en charge.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Enrichissement du profil dans les messages transactionnels (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonctionnalité Enrichissement du profil dans les messages transactionnels est désormais disponible pour toutes les clientes et tous les clients (GA). En plus des e-mails, les SMS et les notifications push sont désormais pris en charge. Cette fonctionnalité permet de personnaliser les messages transactionnels en liant des champs de la base de données Adobe Campaign au contenu des messages. Vous pouvez sélectionner des mappings de ciblage, des colonnes d’enrichissement et une clé de réconciliation pour garantir une personnalisation précise en temps réel tout en maintenant vos seuils de performances.</p>
<p>Pour plus d'informations, consultez la <a href="../transactional-messaging/profile-enrichment.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Live Copies et copies de langue d’Adobe Experience Manager</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’intégration de contenu Adobe Experience Manager permet d’accéder à toutes les copies de langue et Live Copies créées dans Adobe Experience Manager directement dans Campaign lors de la création de diffusions. Vous pouvez actualiser le contenu en temps réel pour récupérer les dernières versions d’Adobe Experience Manager. Cette intégration élimine la synchronisation manuelle de contenu entre Adobe Experience Manager et Campaign, ce qui rationalise votre workflow de campagne multilingue.</p>
<p>Pour plus d'informations, consultez la <a href="../integrations/aem-multilingual.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Expériences de contenu - Tests AB</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les expériences de contenu dans Adobe Campaign Web vous permettent de définir plusieurs variantes de diffusion de test A/B afin de mesurer celle qui fonctionne le mieux pour votre audience cible. Vous pouvez faire varier le contenu, l’objet ou l’expéditeur ou expéditrice de la diffusion afin de tester différentes versions et de déterminer la variante produisant les meilleurs résultats. Vous pouvez effectuer des tests AB sur divers éléments d’e-mail tels que l’objet, le nom de l’expéditeur ou de l’expéditrice et le contenu du corps de l’e-mail.</p>
<p>Pour plus d’informations, consultez la <a href="../email/ab-testing.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Activité de diffusion continue</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’activité Diffusion continue permet d’ajouter de nouveaux destinataires à une diffusion existante. Ce type de diffusion évite d’avoir à créer une diffusion à chaque fois, ce qui le rend plus efficace pour les alertes ou notifications à faible volume envoyées selon les besoins. Une diffusion continue crée une instance de diffusion unique. Tous les logs de diffusion (broadLog) et les logs de tracking référencent cette diffusion, ce qui simplifie la surveillance et le reporting.</p>
<p>Pour plus d’informations, consultez la <a href="../workflows/activities/continuous-delivery.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gestion de la validation de campagne</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Le processus de validation permet de coordonner plusieurs parties prenantes et d’assurer un contrôle qualité avant l’envoi des diffusions. Utilisez les validations lorsque votre organisation nécessite la validation de différentes équipes, comme les responsables marketing qui examinent le contenu ou les analystes de données qui valident les audiences cibles.</p>
<p>Pour plus d'informations, consultez la <a href="../campaigns/campaign-approvals.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#26-1-improvements}

* Les rapports dynamiques prennent désormais en charge les notifications push et les SMS. [En savoir plus](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtres prédéfinis - Une nouvelle option de « filtre partagé » permet de mettre un filtre prédéfini à disposition d’autres utilisateurs et utilisatrices de votre organisation. [En savoir plus](../get-started/predefined-filters.md#share-filter)
* Les champs de personnalisation créés dans Adobe Experience Manager, tels que le nom, l’e-mail, la date et l’adresse, sont désormais inclus et disponibles lors de l’utilisation de modèles de contenu.
* L’évaluation de la qualité du contenu recherche désormais les problèmes de lisibilité, de cohésion et d’efficacité, indépendamment des directives de la marque, en identifiant les messages imprécis, les incohérences de ton ou les problèmes structurels. [En savoir plus](../content/brands-score.md)
