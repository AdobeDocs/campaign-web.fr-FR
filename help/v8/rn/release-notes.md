---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 36d2b7a67ef087d628151199a223ceee54f84180
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 31%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont répertoriées sur les pages [2024](release-notes-24.md) et [2025](release-notes-25.md).

## Version du 26 janvier {#26-1-release}

_27 janvier 2026_

### Nouvelles fonctionnalités {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Fonctionnalités de diffusion multilingue (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonctionnalité de diffusion multilingue est désormais disponible pour tous les clients (GA). Cette fonctionnalité vous permet d’envoyer plusieurs messages dans différentes langues dans l’interface utilisateur web d’Adobe Campaign. Vous pouvez choisir la langue par défaut de votre diffusion ainsi que les différentes langues dans lesquelles la diffusion peut être envoyée. Vous pouvez également prévisualiser ces diffusions dans les langues que vous avez choisies. 
<p>Pour plus d'informations, consultez la <a href="../msg/multilingual.md">documentation détaillée</a>.</p>
<p>Les améliorations suivantes ont été apportées aux notifications push multilingues :</p>
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
<th><strong>Enrichissement du profil dans les messages transactionnels (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonctionnalité Enrichissement du profil dans les messages transactionnels est désormais disponible pour tous les clients (GA). Outre les e-mails, les SMS et les notifications push sont désormais pris en charge. Cette fonctionnalité vous permet de personnaliser les messages transactionnels en liant les champs de la base de données Adobe Campaign au contenu du message. Vous pouvez sélectionner des mappings de ciblage, des colonnes d’enrichissement et une clé de réconciliation pour garantir une personnalisation précise en temps réel tout en maintenant vos seuils de performances.</p>
<p>Pour plus d'informations, consultez la <a href="../transactional-messaging/profile-enrichment.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Live Copies et copies de langue de Adobe Experience Manager</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’intégration de contenu Adobe Experience Manager vous permet d’accéder à toutes les copies de langue et Live Copies créées dans Adobe Experience Manager directement dans Campaign lors de la création de diffusions. Vous pouvez actualiser le contenu en temps réel pour récupérer les dernières versions de Adobe Experience Manager. Cette intégration élimine la synchronisation manuelle de contenu entre Adobe Experience Manager et Campaign, rationalisant ainsi votre workflow de campagne multilingue.</p>
<p>Pour plus d'informations, consultez la <a href="../integrations/aem-multilingual.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Expériences de contenu - Tests A/B</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les expériences de contenu dans Adobe Campaign Web vous permettent de définir plusieurs variantes de diffusion de test A/B afin de mesurer celle qui fonctionne le mieux pour votre audience cible. Vous pouvez varier le contenu, l’objet ou l’expéditeur de la diffusion afin de tester différentes versions et de déterminer la variante produisant les meilleurs résultats. Vous pouvez effectuer des tests A/B sur divers éléments d’e-mail tels que l’objet, le nom de l’expéditeur et le contenu du corps de l’e-mail.</p>
<p>Pour plus d'informations, consultez la <a href="../email/ab-testing.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Activité de diffusion au fil de l'eau</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L'activité Diffusion au fil de l'eau permet d'ajouter de nouveaux destinataires à une diffusion existante. Ce type de diffusion évite d’avoir à créer une diffusion à chaque fois, ce qui le rend plus efficace pour les alertes de faible volume ou les notifications envoyées selon les besoins. Une diffusion au fil de l’eau crée une instance de diffusion unique. Tous les logs de diffusion (broadLog) et les logs de tracking référencent cette diffusion, simplifiant la surveillance et le reporting.</p>
<p>Pour plus d'informations, consultez la <a href="../workflows/activities/continuous-delivery.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gestion de la validation des campagnes</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Le processus de validation permet de coordonner plusieurs parties prenantes et d’assurer un contrôle qualité avant l’envoi des diffusions. Utilisez les validations lorsque votre organisation nécessite la validation de différentes équipes, telles que les responsables marketing qui examinent le contenu ou les analystes de données qui valident les audiences cibles.</p>
<p>Pour plus d'informations, consultez la <a href="../campaigns/campaign-approvals.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#26-1-improvements}

* Les rapports dynamiques prennent désormais en charge les notifications push et les SMS. [En savoir plus](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtres prédéfinis - Une nouvelle option de « filtre partagé » vous permet de rendre un filtre prédéfini disponible pour d’autres utilisateurs de votre organisation. [En savoir plus](../get-started/predefined-filters.md#share-filter)
* Les champs de personnalisation créés dans Adobe Experience Manager, tels que le nom, l’e-mail, la date et l’adresse, sont désormais inclus et disponibles lors de l’utilisation de modèles de contenu.
* L’évaluation de la qualité du contenu recherche désormais les problèmes de lisibilité, de cohésion et d’efficacité indépendamment des directives de la marque, en identifiant les messages imprécis, le ton incohérent ou les lacunes structurelles. [En savoir plus](../content/brands-score.md)
