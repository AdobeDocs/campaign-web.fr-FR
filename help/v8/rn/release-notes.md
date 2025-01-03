---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont répertoriées [sur cette page](release-notes-24.md).

## Version d’octobre 2024 {#24-10-release}

**Date de publication** : 29 octobre 2024

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version d’octobre.

### Fonctionnalités

<table>
<thead>
<tr>
<th><strong>Comptes externes</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Vous pouvez désormais configurer et gérer des comptes externes directement via l’interface d’utilisation d’Adobe Campaign Web. Cette nouvelle fonctionnalité facilite la configuration de différents types de comptes externes, tels que les e-mails rejetés (POP3) ou les instances d’exécution.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Messages transactionnels</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Les messages transactionnels (Message Center) sont désormais disponibles dans l’interface d’utilisation de Campaign Web. Ce module complémentaire est conçu pour les messages de déclenchement qui sont générés à partir d’événements déclenchés depuis des systèmes d’information et qui peuvent correspondre aux éléments suivants : facture, confirmation de commande, confirmation d’expédition, changement de mot de passe, notification d’indisponibilité d’un produit, relevé de compte, création d’un compte sur un site web, etc.</p>
<p>Pour plus d’informations, consultez la <a href="../transactional-messaging/transactional.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Améliorations

* **Activités de workflows** : vous pouvez désormais déplacer une activité et tous ses nœuds enfant d’une transition vers une autre au sein d’un workflow. Un bouton **Déplacer** dédié est disponible dans le volet des propriétés de l’activité pour effectuer cette opération. [En savoir plus](../workflows/orchestrate-activities.md#move)

* **Activité d’enrichissement de workflow**

   * Vous pouvez désormais définir un Alias et un Libellé lors de la création d’un champ dans l’activité **Enrichissement**. [En savoir plus](../workflows/activities/enrichment.md#collection-settings)
   * Vous pouvez désormais ajouter des offres pour chaque profil dans l’activité **Enrichissement**. [En savoir plus](../workflows/activities/enrichment.md##add-offers)

* **Répartition des valeurs** : lorsque vous accédez à la liste des champs à personnaliser, vous pouvez désormais vérifier comment les valeurs sont distribuées pour chaque champ. Une fenêtre contextuelle dédiée indique le nombre et le pourcentage pour chaque valeur. [En savoir plus](../query/build-query.md#distribution-values-query)

* **Version et informations sur le système** : vous pouvez désormais accéder aux détails sur les versions de votre instance, à la fois pour la console cliente et l’interface d’utilisation web. Cette nouvelle section répertorie également tous les packages intégrés installés dans votre environnement. [En savoir plus](../get-started/user-interface.md#user-interface-about)

* **Listes** : vous pouvez désormais facilement réorganiser les valeurs d’une liste. [En savoir plus](../get-started/work-with-folders.md)

* **Diffusion** : les variables de diffusion sont désormais accessibles à partir des champs de personnalisation. [En savoir plus](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)