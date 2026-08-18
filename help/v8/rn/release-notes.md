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
source-git-commit: d6b9b9c9905d840e65ac0aa267a665997c6e6b16
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 33%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

>[!NOTE]
>
>Une documentation détaillée sur les fonctionnalités et améliorations ci-dessous sera ajoutée progressivement au cours des prochains jours.

## Version du 26 août {#26-8-release}

_18 août 2026_

### Nouvelles fonctionnalités {#26-8-features}

<table>
<thead>
<tr>
<th><strong>Activité de workflow d’approbation</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>L’activité de workflow <strong>Validation</strong>, auparavant uniquement disponible dans la console cliente, est désormais disponible dans l’interface utilisateur web de Campaign. Affectez la tâche à un groupe ou à un opérateur individuel, personnalisez le titre et le message de la notification, puis définissez les réponses possibles (par exemple Oui/Non) comme des branches de sortie.</p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#26-8-improvements}

* **Suivi des ouvertures** : vous pouvez désormais activer ou désactiver le suivi des ouvertures directement depuis l’interface utilisateur web de Campaign. Cela vous aide à vous conformer aux réglementations en matière de protection des données.
* **Vue Liste des programmes** : les programmes sont désormais répertoriés dans une vue dédiée, comme les campagnes, les diffusions et les workflows. Vous pouvez parcourir les programmes existants et en créer de nouveaux directement à partir de cette vue.
* **Configuration de schéma personnalisé** : dans la section **Données d’action**, vous pouvez désormais interdire l’action **Dupliquer** sur les enregistrements d’un schéma personnalisé.
  <!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->
* **Filtres personnalisés** : dans l’éditeur de schémas, les filtres personnalisés prennent désormais en charge les conditions de filtrage sur les liens directs et vous pouvez remplacer le libellé par défaut de tout attribut à l’aide du nouveau **Paramètres de filtre personnalisé**.
* **Validation du schéma** : vous pouvez désormais valider la structure d’un schéma directement à partir de l’éditeur de schémas, à l’aide du nouveau bouton **Valider**.
* **Sécurité des dossiers** : l&#39;option **Renommer** est désormais disponible pour un dossier lorsque l&#39;utilisateur dispose du droit d&#39;accès **Insérer** ou **Modifier**.
  <!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
