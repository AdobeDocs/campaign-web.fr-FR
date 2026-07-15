---
title: Notes de mise à jour de l’interface d’utilisation de Campaign v8 Web
description: Découvrez les nouvelles fonctionnalités accompagnant la dernière version de l’interface d’utilisation de Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: b8cf1d45b1a69efbe8e055d57b430d0fa04f8494
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 93%

---

# Notes de mise à jour {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notes de mise à jour"
>abstract="Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, les notes de mise à jour de Campaign sont mises à jour plusieurs fois par mois, avec les derniers correctifs, les dernières fonctionnalités et les dernières améliorations. Nous vous recommandons de les vérifier régulièrement."

Les versions de l’interface utilisateur d’Adobe Campaign Web fonctionnent sur un modèle de diffusion continu qui permet une approche plus évolutive et progressive du déploiement des fonctionnalités. Par conséquent, ces notes de mise à jour sont complétées plusieurs fois par mois. Veuillez les vérifier régulièrement.

## Version de juin 2026 {#26-6-release}

_16 juin 2026_

### Améliorations {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* Vous pouvez désormais exporter des données depuis n’importe quel écran de liste, y compris les journaux de suivi. Trouvez votre liste et cliquez simplement sur le bouton d’export. L’export inclut les lignes actuellement chargées et prend en compte les colonnes affichées à l’écran, ainsi que les recherches ou filtres actifs. [En savoir plus](../get-started/list-filters.md)

* Les activités de workflow **Déduplication** et **Fin** prennent désormais en charge plusieurs transitions entrantes. Lorsque plusieurs transitions entrantes sont disponibles, utilisez la section **Ensembles à joindre** dans l&#39;activité
les propriétés de l’activité pour sélectionner les transitions à connecter. En savoir plus dans ces pages : [Déduplication](../workflows/activities/deduplication.md), [Fin](../workflows/activities/end.md)

* Les paramètres avancés sont désormais exposés dans la section **Données d’enrichissement** des activités de workflow **Créer une audience** (type de requête) et **Enrichissement**. Ces paramètres vous permettent d’affiner la manière dont les données d’enrichissement sont créées, notamment le regroupement, la déduplication, la gestion des clés primaires et les données d’événement entrant. [En savoir plus](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
