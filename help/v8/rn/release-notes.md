---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 100%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont répertoriées sur les pages [2024](release-notes-24.md) et [2025](release-notes-25.md).

## Mises à jour d’octobre 2025 {#25-9-updates}

_9 octobre 2025_

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

