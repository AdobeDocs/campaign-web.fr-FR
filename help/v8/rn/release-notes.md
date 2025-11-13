---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ca1a437f8a8a25c0a15b9148e9c73271795f16c7
workflow-type: ht
source-wordcount: '506'
ht-degree: 100%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont répertoriées sur les pages [2024](release-notes-24.md) et [2025](release-notes-25.md).

## Version d’octobre 2025 {#25-10-updates}

_3 novembre 2025_

<table>
<thead>
<tr>
<th><strong>Fonctionnalités multilingues pour les messages transactionnels, les notifications push et les SMS (disponibilité limitée)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais envoyer plusieurs messages transactionnels, notifications push et SMS dans différentes langues dans l’interface d’utilisation d’Adobe Campaign Web. La fonction Diffusion multilingue permet de choisir la langue par défaut de votre diffusion ainsi que les différentes langues dans lesquelles la diffusion peut être envoyée. Vous pouvez également prévisualiser ces diffusions dans les langues que vous avez choisies.</p>
<p>Remarque : cette fonctionnalité n’est disponible que pour un ensemble d’organisations donné (disponibilité limitée) et sera déployée en disponibilité générale dans une prochaine version.</p>
<p>Pour plus d’informations, consultez la <a href="../msg/multilingual.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>Enrichissement des profils dans les messages transactionnels (disponibilité limitée)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Cette fonctionnalité vous permet de personnaliser les messages transactionnels en liant des champs de la base de données Adobe Campaign au contenu des messages. Vous pouvez sélectionner des mappings de ciblage, des colonnes d’enrichissement et une clé de réconciliation pour garantir une personnalisation précise en temps réel tout en maintenant vos seuils de performances.</p>
<p>Remarque : cette fonctionnalité n’est disponible que pour un ensemble d’organisations donné (disponibilité limitée) et sera déployée en disponibilité générale dans une prochaine version. Cette fonctionnalité n’est actuellement disponible que pour les e-mails.</p>
<p>Pour plus d’informations, consultez la <a href="../transactional-messaging/profile-enrichment.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Intégration d’Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Pour améliorer l’efficacité du marketing et maintenir la cohérence de la marque, vous pouvez désormais intégrer les expériences GenStudio for Performance Marketing à Campaign de manière transparente. Vous pouvez ainsi tirer parti de la création de contenu basée sur l’IA de GenStudio tout en bénéficiant des fonctionnalités d’orchestration avancées de Campaign.<p>
<p>Pour plus d’informations, consultez la <a href="../integrations/genstudio.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Prise en charge du mode sombre dans le Concepteur d’e-mail</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Le Concepteur d’e-mail offre désormais la possibilité de passer en mode sombre, dans lequel vous pouvez en outre définir des paramètres personnalisés spécifiques. Notez que le rendu final dépend du client de messagerie de la personne destinataire et que certains clients de messagerie ne prennent pas en charge le mode sombre.</p>
<p>Pour plus d’informations, consultez la <a href="../email/dark-mode.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Améliorations {#25-10-improvements}

* Dans les diffusions créées dans la console cliente, la section **Audience** indique désormais si une condition dynamique a été définie pour les cibles des BAT. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* Vous pouvez désormais basculer entre le nouveau créateur de règles et l’ancien lors de la configuration d’une condition à l’aide de la fonctionnalité de contenu conditionnel du Concepteur d’e-mail. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* Vous pouvez désormais sélectionner des liens de collection, tels que des achats, dans la définition de l’écran du schéma Destinataires. Les données associées sont alors affichées sur les écrans des profils via un onglet dédié. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* En tant qu’administrateur ou administratrice Campaign, vous pouvez désormais configurer des connexions vers Salesforce CRM et Microsoft Dynamics.
  [En savoir plus](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

