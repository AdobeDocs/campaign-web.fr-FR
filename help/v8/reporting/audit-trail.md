---
product: campaign
title: Journal d’audit
description: Découvrez comment surveiller votre instance à lʼaide du journal dʼaudit Campaign
feature: Audit Trail, Monitoring, Workflows
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 100%

---

# Journal d’audit{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Journal d’audit"
>abstract="La nouvelle fonctionnalité de journal d’audit fournit un enregistrement détaillé et chronologique de toutes les actions et de tous les événements qui ont été réalisés en temps réel sur votre instance Adobe Campaign."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"


Dans l’interface d’utilisation d’Adobe Campaign Web, la fonctionnalité **[!UICONTROL Journal d’audio]** offre aux utilisateurs et utilisatrices une visibilité complète de toutes les modifications apportées à des entités importantes au sein de votre instance, généralement celles qui ont un impact significatif sur le bon fonctionnement de l’instance.

>[!IMPORTANT]
>
>* L’interface d’utilisation d’Adobe Campaign Web ne réalise pas d’audit sur les modifications apportées aux droits des utilisateurs et utilisatrices, aux modèles, aux personnalisations ni aux campagnes.
>* Le Journal d’audit peut uniquement être géré par les administrateurs de l’instance.

La fonctionnalité **[!UICONTROL Journal d’audit]** permet d’enregistrer en temps réel un journal détaillé des actions et événements se produisant dans l’instance Adobe Campaign. Elle offre une méthode pratique d’accès à un enregistrement chronologique des données, en répondant à des requêtes telles que : le statut des workflows, les dernières personnes qui les modifient ou les activités effectuées par les utilisateurs et utilisatrices au sein de l’instance.

+++ En savoir plus sur les entités disponibles du journal d’audit

* **Journal d’audit du schéma source** : permet de surveiller les activités et les modifications récentes apportées à vos schémas dans la console cliente Campaign V8.

  Pour plus d’informations sur les schémas, consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* Le **Journal d’audit des workflows** permet de suivre les activités et les modifications récentes apportées aux workflows, y compris leurs statuts actuels, telles que :

   * Démarrer
   * Pause
   * Arrêter
   * Redémarrer
   * Nettoyer qui correspond à l’action Purge de l’historique
   * Simuler qui correspond à l’action Démarrer en mode simulation
   * Réveiller qui correspond à l’action Traitement anticipé des tâches en attente
   * Arrêt inconditionnel

  Pour plus d’informations sur les workflows, consultez [cette page](../workflows/gs-workflows.md).

* **Journal d’audit des options** : permet de surveiller les activités et les modifications récentes apportées à vos options dans Campaign V8.

  Pour plus d’informations sur les options, consultez [cette page](https://experienceleague.adobe.com/fr/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Journal d’audit des diffusions** : permet de vérifier les activités et les dernières modifications apportées à vos diffusions.

  Pour plus d’informations sur les diffusions, consultez cette [page](../msg/gs-deliveries.md).

* **Compte externe** : permet de vérifier les modifications apportées aux comptes externes dans Campaign V8. Utilisé par des processus techniques tels que des workflows techniques ou des workflows de campagne.

  Pour plus d’informations sur les comptes externes, consultez cette [page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Mapping de diffusion** : permet de surveiller les activités et les modifications récentes apportées à votre mapping de diffusion dans Campaign V8.

  Pour plus d’informations sur les mappings de diffusion, consultez cette [page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Application web** : permet de vérifier les modifications apportées aux formulaires web dans Campaign v8 servant à créer des pages avec des champs de saisie et de sélection et pouvant inclure des données de la base de données.

  Pour plus d’informations sur les applications web, consultez cette [page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/content/webapps).

* **Offre** : permet de vérifier les activités et les dernières modifications apportées à vos offres.

  Pour plus d’informations sur les offres, consultez cette [page](../msg/offers.md).

* **Opérateur ou opératrice** : permet de surveiller les activités et les modifications récentes apportées à vos opérateurs et opératrices dans Campaign V8.

  Pour plus d’informations sur les opérateurs et opératrices, consultez cette [page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Accéder au journal d’audit {#accessing-audit-trail}

Pour accéder au **[!UICONTROL journal d’audit]** de votre instance, procédez comme suit :

1. Sous le menu **[!UICONTROL Administration]**, sélectionnez **[!UICONTROL Journal d’audit]**.

   ![](assets/audit-trail-1.png)

1. La fenêtre **[!UICONTROL Journal d’audit]** s’ouvre avec la liste de vos entités. L’interface d’utilisation d’Adobe Campaign Web réalise l’audit des actions de création, de modification et de suppression pour les workflows, les options, les diffusions et les schémas.

   Sélectionnez l’une des entités pour en savoir plus sur les dernières modifications.

1. La fenêtre **[!UICONTROL Entité d’audit]** vous donne des informations plus détaillées sur l’entité choisie, telles que :

   * **[!UICONTROL Type]** : workflow, options, diffusions ou schémas.
   * **[!UICONTROL Entité]** : nom interne de vos activités.
   * **[!UICONTROL Modifié par]** : nom d’utilisateur de la dernière personne à avoir modifié cette entité.
   * **[!UICONTROL Action]** : dernière action réalisée sur cette entité (création, modification ou suppression).
   * **[!UICONTROL Date de modification]** : date de la dernière action effectuée sur cette entité.

   Ce bloc de code vous donne davantage d’informations sur ce qui a été modifié dans votre entité.

   ![](assets/audit-trail-2.png)

