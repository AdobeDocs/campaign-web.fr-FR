---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 73553f19c6e88256f0e9f38479bdfc292a3221f8
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

## Version du 26 septembre {#26-9-release}

_2 septembre 2026_

### Nouvelles fonctionnalités {#26-9-features}

<table>
<thead>
<tr>
<th><strong>Canal LINE</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign prend désormais en charge le canal <strong>LINE</strong>, une application de messagerie instantanée populaire. Créez et envoyez des messages LINE à l'aide de contenu texte, image ou vidéo, dans des diffusions autonomes ou dans des workflows, aux côtés de vos autres canaux. <a href="../line/get-started-line.md">En savoir plus</a></p>
</td>
</tr>
</tbody>
</table>

### Améliorations {#26-9-improvements}

* **Accès à la navigation latérale** : les administrateurs peuvent désormais masquer des entrées de menu spécifiques de la navigation latérale. [En savoir plus](../administration/schemas-browse-access.md#screen-def)
* **Types de validation supplémentaires** : vous pouvez désormais exiger des validations de budget et de début de diffusion pour les diffusions de Campaign, en plus des validations de contenu et de cible. [En savoir plus](../campaigns/campaign-approvals.md#configure-approvals)
* **Ciblage des SMS basé sur les visiteurs** : le mapping de ciblage des visiteurs est désormais disponible pour les diffusions SMS. [En savoir plus](../sms/create-sms.md)
* **Bouton d’annulation du workflow** : un nouveau bouton **Annuler** permet d’annuler les modifications non enregistrées dans un workflow. [En savoir plus](../workflows/orchestrate-activities.md#save-cancel)
* **Déduplication avec plusieurs valeurs** : l’option **Suivant une liste de valeurs** prend désormais en charge plusieurs attributs. [En savoir plus](../workflows/activities/deduplication.md#deduplication-configuration)
* **Mapping de ciblage mobile** : vous pouvez désormais créer des mappings de ciblage pour les cibles des applications mobiles. [En savoir plus](../administration/target-mappings.md#create-mapping)
* **Enrichissement de base de données externe** : vous pouvez désormais enrichir les données d&#39;une base de données externe dans l&#39;activité **Enrichissement** ou **Créer une audience**. [En savoir plus](../workflows/activities/enrichment.md#external-data)
* **Réconciliation des audiences de fichiers** : vous pouvez désormais choisir d’importer des destinataires dans la base de données lors du ciblage d’une audience à partir d’un fichier. [En savoir plus](../audience/file-audience.md#upload)
* **Jointures directes sur les collections** : lors de la sélection d’un attribut directement à partir d’une collection, vous pouvez désormais choisir la manière dont la condition est créée : à l’aide de l’option par défaut recommandée, d’une fonction d’agrégat ou d’une jointure directe avancée. [En savoir plus](../query/build-query.md#links)

