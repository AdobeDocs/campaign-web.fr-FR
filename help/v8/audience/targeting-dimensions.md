---
title: Dimensions de ciblage
description: En savoir plus sur les dimensions de ciblage dans Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 29%

---

# Dimensions de ciblage {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Sélectionner la dimension de ciblage"
>abstract="La dimension de ciblage permet de définir la population ciblée par l’opération : destinataires, bénéficiaires d’un contrat, opérateur ou opératrice, abonnées et abonnés, etc. Par défaut, pour les e-mails et les SMS, la cible est sélectionnée à partir du tableau intégré Personnes destinataires. Pour les notifications push, la dimension cible par défaut est Applications des personnes abonnées."

La dimension de ciblage, également appelée mappage de ciblage, correspond au type de données géré par une opération. Il définit la population ciblée, telle que les profils, les bénéficiaires d’un contrat, les opérateurs ou les abonnés.

## Dimensions de ciblage des workflows {#workflow}

La dimension de ciblage d’un workflow est définie par la première activité **[!UICONTROL Créer une audience]** et est utilisée dans toutes les activités suivantes jusqu’à la fin du workflow. Par exemple, lors de l&#39;interrogation de profils à partir de la base de données, la transition sortante contient des données de type &#39;destinataire&#39;, qui sont transmises à l&#39;activité suivante.

Basculez la dimension de ciblage dans un workflow à l’aide d’une [activité Modifier la dimension](../workflows/activities/change-dimension.md). Cela permet d’interroger la base de données sur une table spécifique, telle que des achats ou des abonnements, puis de modifier la dimension de ciblage en Destinataires pour envoyer des diffusions aux profils correspondants.

Lors de la sélection d’une dimension de ciblage (dans les paramètres du workflow ou dans des activités telles que **Créer une audience**, **Réconciliation** ou **Modifier la dimension**), une liste des schémas couramment utilisés s’affiche par défaut. Pour afficher tous les schémas disponibles, activez/désactivez le bouton **[!UICONTROL Afficher tous les schémas]**. La sélection de cette option est enregistrée pour chaque utilisateur ou utilisatrice.

![Capture d’écran montrant l’interface de la dimension de ciblage avec le bouton « Afficher tous les schémas » activé.](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Dimensions de ciblage {#list}

Par défaut, les modèles de diffusion par e-mail et SMS ciblent les profils. Leur dimension cible utilise les champs du tableau **nms:recipient**. Pour les notifications push, la dimension de ciblage par défaut est **Applications Abonnés (nms:appSubscriptionRcp)**, qui est liée au tableau des destinataires.

Utilisez d&#39;autres mappings de ciblage intégrés dans les workflows et les diffusions, comme indiqué ci-dessous :

| Nom | Utiliser pour diffuser à | Schéma |
|-----------------------|-------------------------------------------------------|-------------------------|
| Destinataires | Profils/destinataires (table des destinataires intégrée) | nms:recipient |
| Visiteurs | Visiteurs et visiteuses dont les profils ont été collectés par le biais d’une recommandation (marketing viral pour ex) | mns:visitor |
| Abonnements  | Les profils abonnés à un service d’information tel qu’une newsletter | nms:subscription |
| Abonnements des visiteurs | Visiteurs abonnés à un service d&#39;information | nms:visitorSub |
| Opérateurs | Opérateurs Adobe Campaign | nms:operator |
| Fichier externe | Diffusion via un fichier contenant toutes les informations nécessaires | Aucun schéma associé, aucune cible renseignée |
| Applications abonnés | Profils abonnés à une application | nms:appSubscriptionRcp |

En outre, créez de nouveaux mappings de ciblage en fonction de besoins spécifiques. Effectuez cette opération à partir de la console cliente uniquement. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr#new-mapping){target="_blank"}.