---
title: Dimensions de ciblage
description: En savoir plus sur les dimensions de ciblage dans Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 100%

---

# Dimensions de ciblage {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Sélectionner la dimension de ciblage"
>abstract="La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateurs ou opératrices, abonné(e)s, etc. Par défaut, pour les e-mails et les SMS, la cible est sélectionnée à partir du tableau intégré Personnes destinataires. Pour les notifications push, la dimension cible par défaut est Applications des personnes abonnées."

La dimension de ciblage, c’est-à-dire le mapping de ciblage, est le type de données qu’une opération traite. Elle permet de définir la population ciblée : profils, bénéficiaires de contrats, opérateurs et opératrices, abonnées et abonnés, etc.

## Dimensions de ciblage des workflows {#workflow}

La dimension de ciblage d’un workflow est définie par la première activité **[!UICONTROL Créer une audience]** et est utilisée dans toutes les autres activités jusqu’à la fin du workflow. Si vous effectuez par exemple une requête sur les profils de la base de données, la transition sortante contiendra des données de type destinataire et sera transmise à l’activité suivante.

Notez que vous pouvez changer la dimension de ciblage dans un workflow à l’aide d’une activité [Changer une dimension](../workflows/activities/change-dimension.md). Vous pouvez ainsi, par exemple, interroger la base de données sur un tableau spécifique tel que des achats ou des abonnements, puis changer la dimension de ciblage par Destinataires afin d’envoyer des diffusions aux profils correspondants.

Lors de la sélection d’une dimension de ciblage (dans les paramètres du workflow, ou dans des activités telles que **Créer une audience**, **Réconciliation** ou **Changement de dimension**), une sélection des schémas couramment utilisés s’affiche par défaut dans la liste. Pour afficher tous les schémas disponibles, cliquez sur le bouton **[!UICONTROL Afficher tous les schémas]**. La sélection de cette option est enregistrée pour chaque utilisateur ou utilisatrice.

![](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Dimensions de ciblage {#list}

Par défaut, les modèles de diffusion par e-mail et SMS ciblent les profils. Leur dimension de ciblage utilise donc les champs du tableau **nms:recipient**. Pour les notifications push, la dimension de ciblage par défaut est **Applications Abonnés (nms:appSubscriptionRcp)**, qui est liée au tableau des destinataires.

Vous pouvez également utiliser d’autres mappings de ciblage intégrés dans vos workflows et diffusions répertoriés ci-dessous :

| Nom | Utilisation | Schéma |
|---|---|---|
| Destinataires | Diffuser aux profils/ personnesdestinataires (tableau de personnes destinataires intégré). | nms:recipient |
| Visiteurs | Diffuser aux visiteurs dont les profils ont été collectés par le biais d’une recommandation (marketing viral), par exemple. | mns:visitor |
| Abonnements  | Diffuser aux profils abonnés à un service d’information, par exemple à une newsletter. | nms:subscription |
| Abonnements des visiteurs | Diffuser à des visiteurs abonnés à un service d&#39;information | nms:visitorSub |
| Les opérateurs | Diffuser aux opérateurs Adobe Campaign | nms:operator |
| Fichier externe | Diffuser depuis un fichier contenant les toutes informations nécessaires à la diffusion | Aucun schéma associé, aucune cible renseignée |
| Applications abonnés | Diffuser aux profils abonnés à une application. | nms:appSubscriptionRcp |

En outre, vous pouvez créer un nouveau mapping de ciblage selon vos besoins. Cette opération s’effectue uniquement à partir de la console cliente. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr#new-mapping){target="_blank"}.
