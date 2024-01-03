---
title: Utiliser des destinataires et des audiences
description: Découvrez comment utiliser les destinataires et les audiences dans le Web de Campaign
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 93%

---

# Utiliser des destinataires et des audiences {#about-recipients}

## Destinataires et audiences {#about}

Dans Adobe Campaign, la population cible d’une diffusion est une audience. Une audience est un ensemble de personnes qui partagent des comportements et/ou des caractéristiques similaires. Cette collection de personnes peut être générée, sélectionnée ou chargée. [comme décrit ci-dessous](#audiences).

Dans la plupart des cas, l’audience est composée de profils stockés sous la forme de [destinataires](#recipients) dans Adobe Campaign. Vous pouvez également travailler avec d’autres mappings de ciblage en modifiant la dimension, tel qu’expliqué [dans cette section](#targeting-dimensions).

## Dimensions de ciblage {#targeting-dimensions}

La dimension de ciblage, c’est-à-dire le mapping de ciblage, est le type de données qu’une opération traite. Il permet de définir la population ciblée : destinataires, bénéficiaires de contrats, opérateurs et opératrices, abonnés et abonnées, etc.

La dimension de ciblage d’un workflow est définie par la première activité **[!UICONTROL Créer une audience]** et est utilisée dans toutes les autres activités jusqu’à la fin du workflow. Si vous effectuez par exemple une requête sur les destinataires de la base de données, la transition sortante contiendra des données de type destinataire et sera transmise à l’activité suivante.

Notez que vous pouvez changer la dimension de ciblage dans un workflow à l’aide d’une activité [Changer une dimension](../workflows/activities/change-dimension.md). Vous pouvez ainsi, par exemple, interroger la base de données sur un tableau spécifique tel que des achats ou des inscriptions, puis changer la dimension de ciblage par Destinataires afin d’envoyer des diffusions aux destinataires correspondants.

Par défaut, les modèles de diffusion par e-mail et SMS ciblent les **[!UICONTROL destinataires]**. Leur dimension de ciblage utilise donc les champs du tableau **nms:recipient**. Pour les notifications push, la dimension de ciblage par défaut est **Applications Abonnés (nms:appSubscriptionRcp)**, qui est liée au tableau des destinataires.

Vous pouvez également utiliser d’autres mappings de ciblage intégrés dans vos workflows et diffusions répertoriés ci-dessous :

| Nom | Utilisation | Schéma |
|---|---|---|
| Destinataires | Diffuser aux destinataires (tableau de destinataires intégré) | nms:recipient |
| Visiteurs | Diffuser aux visiteurs dont les profils ont été collectés par le biais d’une recommandation (marketing viral), par exemple. | mns:visitor |
| Abonnements  | Diffuser aux destinataires abonnés à un service d&#39;information, par exemple une newsletter | nms:subscription |
| Abonnements des visiteurs | Diffuser à des visiteurs abonnés à un service d&#39;information | nms:visitorSub |
| Les opérateurs | Diffuser aux opérateurs Adobe Campaign | nms:operator |
| Fichier externe | Diffuser depuis un fichier contenant les toutes informations nécessaires à la diffusion | Aucun schéma associé, aucune cible renseignée |
| Applications abonnés | Diffuser aux destinataires abonnés à une application | nms:appSubscriptionRcp |

En outre, vous pouvez créer un nouveau mapping de ciblage selon vos besoins. Cette opération est effectuée à partir de la console cliente. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr#new-mapping){target="_blank"}.
