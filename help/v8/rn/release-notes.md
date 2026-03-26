---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

## Version du 26 mars {#26-3-release}

### Nouvelles fonctionnalités {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Création de schémas (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La fonctionnalité de création de schémas est désormais disponible pour tous les clients (GA). Cette fonctionnalité vous permet de créer et de gérer des schémas directement à partir de l’interface utilisateur web de Campaign. Vous pouvez créer des tables, étendre des schémas existants et créer des formulaires personnalisés. Vous pouvez définir des structures de données personnalisées pour répondre aux besoins spécifiques de votre entreprise sans avoir à accéder à la console cliente.</p>
<p>Pour plus d'informations, consultez la <a href="../administration/schemas.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Thèmes dans Email Designer (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les thèmes offrent une expérience de création d’emails améliorée en vous permettant de définir des styles de thème réutilisables qui correspondent aux directives de votre marque. Vous pouvez désormais utiliser des variables de thème dans des fragments, ce qui garantit une mise en forme cohérente dans vos modèles d’e-mail. Cette fonctionnalité vous permet de créer des e-mails plus rapidement avec des modules prédéfinis qui abstraient des éléments de contenu tels que des titres, des descriptions, des images et des liens, tout en préservant la cohérence de la marque.</p>
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
<p>Choisissez le modèle adapté à vos besoins :</p>
<ul><li> <strong>Adobe model</strong> (optimisé par Firefly Image Model 4) pour la génération immédiate d’images sans configuration supplémentaire</li><li> <strong>Modèle partenaire</strong> (optimisé par Gemini 2.5 Flash) pour des fonctionnalités spécialisées</li><li><strong>Modèles personnalisés</strong> (modèles spécifiques à la marque entraînés sur vos propres ressources) pour une génération sur la marque qui s’aligne précisément sur l’identité, le style et les directives visuelles de votre marque.</li></ul>
<p>Pour plus d'informations, consultez la <a href="../content/generative-models.md">documentation détaillée</a>.</p>
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
<p>L’activité de workflow <strong>Diffusion automatisée</strong> est désormais disponible dans la palette du workflow. Vous pouvez l’utiliser pour créer ou exécuter des actions de diffusion (préparer, envoyer un BAT, préparer et démarrer, etc.) directement dans votre workflow. Sélectionnez une diffusion existante créée en dehors du workflow pour la réutiliser à chaque exécution ou créez une diffusion à partir d'un modèle chaque fois que l'activité s'exécute.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Pour plus d’informations, consultez la documentation <a href="../workflows/activities/automated-delivery.md"> détaillée.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Plusieurs branches de workflow et activité Jointure</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p><strong>Plusieurs branches</strong> sont désormais prises en charge. Au lieu d’utiliser un <strong>Branchement</strong>, vous pouvez cliquer sur <strong>Ajouter une branche</strong> dans la barre d’outils. L’activité <strong>Rendez-vous</strong> a également été améliorée. Il s’agit désormais d’une activité générique <strong>Joindre</strong> qui vous permet de choisir entre les options de jointure ET et OU.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Pour plus d’informations, consultez les pages de documentation <a href="../workflows/orchestrate-activities.md#toolbar">Orchestrer les activités</a> et <a href="../workflows/activities/join.md">Joindre</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#26-3-improvements}

* L’activité de workflow **Démarrer** a été ajoutée pour améliorer la compatibilité avec la console cliente. Cette activité est facultative et n&#39;est pas insérée par défaut dans les nouveaux workflows. Toutefois, il est ajouté automatiquement aux workflows existants.
  [En savoir plus](../workflows/activities/about-activities.md#flow-control)
* Le champ de sélection du fuseau horaire dans les paramètres **Planning** d&#39;une diffusion a été déplacé sous le champ **Date de contact**. [En savoir plus](../msg/create-deliveries.md#gs-schedule)