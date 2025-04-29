---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 589d78737a498ffe91cb49a6f689f4104b244d0b
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 34%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

Les modifications et améliorations disponibles avec les versions précédentes sont répertoriées dans les versions [2024](release-notes-24.md) et [2025](release-notes-25.md).

## Version d’avril 2025 {#25-4-release}

**Date de publication** : mercredi 29 avril 2025


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
<p>Le canal centre d’appel est désormais disponible dans l’interface utilisateur web de Campaign. Ce canal fait référence à une méthode de communication utilisée pour gérer et suivre les communications ou interactions gérées par un centre d’appels (généralement des appels téléphoniques passés par des agents à des clients ou des prospects).</p>
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
<p>Un nouveau créateur de règles est désormais disponible pour vous aider à définir des conditions complexes dans une interface utilisateur améliorée. Vous pouvez passer de l’ancien au nouveau créateur de règles selon vos besoins.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Pour plus d’informations, consultez la <a href="../query/query-modeler-overview.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Création de compte externe</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>En tant qu’administrateur Campaign, vous pouvez désormais configurer de nouvelles connexions avec des systèmes externes à partir de l’interface utilisateur web de Campaign.
Vous pouvez également afficher, mettre à jour et gérer les comptes externes existants.</p>
<p>Pour plus d’informations, consultez la <a href="../administration/external-account.md">documentation détaillée</a>.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#25-4-improvements}

**Améliorations générales de l’interface**

* Les options Description du champ, Ajouter aux favoris et Distribution des valeurs pour les attributs de schéma sont désormais plus visibles dans l’interface utilisateur. Pour plus d’informations, consultez la [documentation détaillée](../get-started/attributes.md).
* Dans l’interface d’, la date et l’heure s’affichent désormais en fonction de la langue principale définie dans les préférences d’Experience League. Cette amélioration n’est disponible que pour plusieurs langues. Pour consulter la liste complète des langues prises en charge, reportez-vous à la [documentation détaillée](https://experienceleague.adobe.com/en/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Éditeur d’email** : pour améliorer l’accessibilité dans l’interface utilisateur web de Campaign, deux nouveaux champs sont désormais disponibles dans le Designer d’email : ils correspondent à l’élément `title` et l’attribut lang dans l’élément `html` du contenu de votre email. Vous pouvez définir ces paramètres en plus du champ Pré-titre , dans la section Corps de l’e-mail.

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schémas**

* Vous pouvez désormais modifier le schéma temporaire d’une liste à partir de l’interface utilisateur web de Campaign. Pour plus d’informations, consultez la [documentation détaillée](../audience/manage-audience.md).
* Vous pouvez désormais prévisualiser les champs personnalisés d’un schéma dans un exemple d’écran. Pour plus d’informations, consultez la [documentation détaillée](../administration/custom-fields.md#add).
* Vous pouvez désormais déplacer des champs personnalisés dans la liste à l’aide du glisser-déposer. Pour plus d’informations, consultez la [documentation détaillée](../administration/custom-fields.md#add).


### Nouvelles fonctionnalités en disponibilité limitée {#25-4-features-la}

>[!AVAILABILITY]
>
>Les fonctionnalités suivantes sont en disponibilité limitée. Ils sont limités aux clients effectuant la migration de **de Adobe Campaign Standard vers Adobe Campaign v8** et ne peuvent pas être déployés dans d’autres environnements. Ils nécessitent une mise à niveau du serveur Campaign vers la version 8.7.4.
>
>Consultez les pages de documentation suivantes : [Transition de Campaign Standard vers Campaign v8](../rn/acs-migration.md) et [Fonctionnalités pour les utilisateurs et les utilisatrices de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=fr).

* **Création de diffusions multilingues** - Vous pouvez désormais envoyer plusieurs diffusions e-mail dans différentes langues dans l’interface utilisateur web d’Adobe Campaign. La fonction Diffusion multilingue permet de choisir la langue par défaut de votre diffusion ainsi que les différentes langues dans lesquelles la diffusion peut être envoyée. Vous pouvez également prévisualiser ces diffusions dans les langues de votre choix. Pour plus d’informations, consultez la [documentation détaillée](../email/edit-content.md).

* **Rapports dynamiques pour le multilinguisme** - Les rapports dynamiques sont désormais disponibles pour les diffusions par e-mail multilingues. Pour plus d’informations, consultez la [documentation détaillée](../reporting/global-reports.md).

* **Prise en charge de l’API REST SMS (LA)** - L’API REST de messagerie transactionnelle est désormais disponible pour le canal SMS. Lorsque le payload contient à la fois un e-mail et un téléphone mobile, vous pouvez utiliser le champ « wishedChannel » pour spécifier le canal. S’il n’est pas fourni, l’e-mail est utilisé par défaut, sauf si wishedChannel demande explicitement un SMS. Pour plus d’informations, consultez la [documentation détaillée](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

