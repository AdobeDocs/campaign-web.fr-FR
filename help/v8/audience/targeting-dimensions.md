---
title: Dimensions de ciblage
description: En savoir plus sur les dimensions de ciblage dans Adobe Campaign Web
badge: label="Disponibilité limitée"
source-git-commit: 2770ddc3d0253d40c4432f71d2b192570e632a8e
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 61%

---

# Dimensions de ciblage {#targeting-dimensions}

La dimension de ciblage, c’est-à-dire le mapping de ciblage, est le type de données qu’une opération traite. Il permet de définir la population ciblée : profils, bénéficiaires de contrats, opérateurs, abonnés, etc.

## Dimension de ciblage des workflows {#workflow}

La dimension de ciblage d’un workflow est définie par la première activité **[!UICONTROL Créer une audience]** et est utilisée dans toutes les autres activités jusqu’à la fin du workflow. Par exemple, si vous effectuez une requête sur les profils de la base, la transition sortante contiendra des données de type &#39;recipient&#39; et sera transmise à l&#39;activité suivante.

Notez que vous pouvez changer la dimension de ciblage dans un workflow à l’aide d’une activité [Changer une dimension](../workflows/activities/change-dimension.md). Vous pouvez ainsi, par exemple, interroger la base de données sur une table spécifique telle que des achats ou des abonnements, puis modifier la dimension de ciblage en Destinataires afin d&#39;envoyer des diffusions aux profils correspondants.

Lors de la sélection d’une dimension de ciblage (dans les paramètres du workflow, ou dans des activités telles que **Créer une audience**, **Réconciliation** ou **Changement de dimension**), une sélection de schémas couramment utilisés s’affiche par défaut dans la liste. Pour afficher tous les schémas disponibles, activez l’option **[!UICONTROL Afficher tous les schémas]** bouton . La sélection de l’option est enregistrée pour chaque utilisateur.

![](assets/targeting-dimension-show-all.png)

## Dimensions de ciblage {#list}

Par défaut, les modèles de diffusion email et SMS ciblent les profils. Leur dimension de ciblage utilise donc les champs du tableau **nms:recipient**. Pour les notifications push, la dimension de ciblage par défaut est **Applications Abonnés (nms:appSubscriptionRcp)**, qui est liée au tableau des destinataires.

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
