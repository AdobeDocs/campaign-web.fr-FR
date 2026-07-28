---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 23%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

## Version du 26 juillet {#26-7-release}

_28 juillet 2026_

### Nouvelles fonctionnalités {#26-7-features}

<table>
<thead>
<tr>
<th><strong>Gestion des offres</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais gérer les offres de bout en bout directement à partir de l’interface utilisateur web de Campaign. Configurez les environnements d'offres et les emplacements, créez votre catalogue d'offres et vos catégories, créez des offres avec des règles d'éligibilité et des poids de priorité, puis validez et déployez-les pour les utiliser dans vos diffusions. Les configurations avancées restent disponibles dans la console cliente.</p>
<p>Pour plus d'informations, consultez la <a href="../offers/gs-offer-management.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Paramétrage des marques</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les administrateurs techniques peuvent désormais créer et configurer des marques directement à partir de l’interface utilisateur web de Campaign, sans utiliser la console cliente. Tous les paramètres de marque, notamment l’identité, le sous-domaine et les protocoles, les paramètres d’en-tête des e-mails et les paramètres de tracking des URL, sont désormais disponibles dans l’interface utilisateur web.</p>
<p>Pour plus d'informations, consultez la <a href="../administration/branding/branding-configure.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Ressources publiques dans le Designer Email</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Lors de l’ajout d’images à vos e-mails, vous pouvez désormais sélectionner <strong>ressources publiques</strong>. Vous pouvez ainsi choisir une image déjà disponible sur votre instance Adobe Campaign, telle qu’un fichier précédemment importé dans le Designer de messagerie ou une ressource publique téléchargée à partir de la console cliente.</p>
<p>Pour plus d'informations, consultez la <a href="../email/content-components.md#image">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Activité de workflow Chargement (SGBD)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’activité <strong> Chargement (SGBD)</strong> est désormais disponible dans l’interface utilisateur web de Campaign. Utilisez cette activité pour charger des données directement à partir d’une base de données relationnelle externe dans votre workflow. Les données extraites sont disponibles dans l’ensemble du workflow et peuvent être utilisées à des fins de ciblage, d’enrichissement ou de traitement des données ultérieur.</p>
<p>Pour plus d'informations, consultez la <a href="../workflows/activities/data-loading-rdbms.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Pages dynamiques JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les pages Dynamic JavaScript (JSSP) vous permettent de créer des pages côté serveur, qui génèrent du contenu dynamique lors d’un accès via une URL, tel que des API personnalisées, des exports ou une logique d’application web. Vous pouvez désormais créer, modifier, dupliquer et supprimer ces pages directement depuis l’interface utilisateur web de Campaign.</p>
<p>Pour plus d'informations, consultez la <a href="../administration/dynamic-javascript-pages.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#26-7-improvements}

* Les améliorations suivantes ont été apportées à **configuration de schéma personnalisé** :
  * La nouvelle section **Données d’action** vous permet de restreindre les actions disponibles sur les enregistrements d’un schéma personnalisé, quelles que soient les règles de sécurité configurées sur des dossiers individuels. [En savoir plus](../administration/schemas-action-data.md)
  * Des **filtres personnalisés** ont été ajoutés dans la section **Configuration de la liste d’inventaire**. Ils vous permettent de choisir les attributs qui s’affichent en tant que champs d’accès rapide dans le volet Filtres de la vue Liste. [En savoir plus](../administration/schemas-custom-filters.md)

* Les améliorations suivantes ont été apportées aux **workflows** :
  * La suppression d’une activité de workflow est désormais plus flexible : lorsque l’activité comporte d’autres activités, vous pouvez choisir de toutes les supprimer, de ne supprimer que l’activité sélectionnée ou de la supprimer tout en conservant ses activités suivantes dans une nouvelle branche. [En savoir plus](../workflows/orchestrate-activities.md#delete-activity)
  * Vous pouvez désormais déconnecter une transition entre deux activités de workflow sans supprimer l’une ou l’autre. Vous pouvez ainsi réorganiser un diagramme de workflow, par exemple pour mettre temporairement de côté un groupe d’activités que vous souhaitez conserver, sans avoir à les supprimer et à les recréer. [En savoir plus](../workflows/orchestrate-activities.md#disconnect-transition)
  * Des barres de défilement horizontales et verticales s’affichent désormais autour de la zone de travail des workflows. Vous pouvez ainsi parcourir les workflows volumineux en faisant glisser directement la souris sur la zone à afficher. [En savoir plus](../workflows/orchestrate-activities.md)
  * Lors de l’enregistrement ou du démarrage/redémarrage d’un workflow, un avertissement s’affiche désormais si un autre utilisateur ou une autre utilisatrice a modifié le workflow dans l’interface utilisateur web ou la console cliente depuis que vous l’avez ouvert. Vous pouvez choisir de remplacer les autres modifications par les vôtres, de recharger le workflow pour obtenir la dernière version ou d’annuler.

* **Adresse e-mail de l’expéditeur** : vous pouvez désormais restreindre le champ **E-mail de l’expéditeur** de vos diffusions à une liste prédéfinie d’adresses, à l’aide de l’option **NmsDelivery_senderAddressMask**. [En savoir plus](../administration/options.md#restrict-sender-address)
* Amélioration des **messages d’erreur de connexion** : lorsqu’une tentative de connexion échoue, l’interface utilisateur web affiche désormais un message d’erreur plus spécifique dans plusieurs cas (par exemple, si aucune zone de sécurité n’est affectée à l’utilisateur ou si son adresse IP est restreinte).
