---
product: campaign
title: Journal d’audit
description: Découvrez comment surveiller votre instance à lʼaide du journal dʼaudit Campaign
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 51%

---

# Journal d’audit {#audit-trail}

Dans l’interface utilisateur web d’Adobe Campaign, la fonction **[!UICONTROL Journal d’audit]** offre aux utilisateurs une visibilité complète de toutes les modifications apportées à des entités importantes au sein de votre instance, généralement celles qui ont un impact significatif sur le bon fonctionnement de l’instance.

>[!IMPORTANT]
>
>* L’interface utilisateur web d’Adobe Campaign n’effectue pas l’audit des modifications apportées aux droits des utilisateurs, aux modèles, à la personnalisation ou aux campagnes.
>* Seuls les administrateurs de l’instance peuvent gérer le journal d’audit.

La fonctionnalité **[!UICONTROL Journal d’audit]** enregistre en permanence un journal détaillé des actions et des événements se produisant dans l’instance Adobe Campaign en temps réel. Elle offre une méthode pratique pour accéder à un enregistrement chronologique des données, en traitant des requêtes telles que le statut des workflows, les derniers individus à les modifier ou les activités effectuées par les utilisateurs et utilisatrices au sein de l’instance.

+++ En savoir plus sur les entités disponibles du journal d’audit

* **Journal d’audit du schéma source** : permet de surveiller les activités et les modifications récentes apportées à vos schémas dans la console cliente Campaign V8.

  Pour plus d’informations sur les schémas, consultez la [documentation de Campaign v8](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* Le **Journal d’audit des workflows** permet de suivre les activités et les modifications récentes apportées aux workflows, y compris leurs statuts actuels, telles que :

   * Démarrer
   * Pause
   * Arrêter
   * Redémarrer
   * Nettoyage, qui correspond à l’historique de purge de l’action
   * Simuler, qui correspond à l’action Démarrer en mode simulation.
   * Réveil, qui est égal à action Exécuter les tâches en attente maintenant
   * Arrêt inconditionnel

  Pour plus d’informations sur les workflows, consultez [cette page](../workflows/gs-workflows.md).

* **Journal d’audit des options** : permet de surveiller les activités et les modifications récentes apportées à vos options dans Campaign V8.

  Pour plus d’informations sur les options, consultez [cette page](https://experienceleague.adobe.com/fr/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Journal d’audit des diffusions** : permet de vérifier les activités et les dernières modifications apportées à vos diffusions.

  Pour plus d’informations sur les diffusions, consultez cette [page](../msg/gs-deliveries.md).

* **Compte externe** : permet de vérifier les modifications apportées aux comptes externes dans Campaign V8. Utilisé par des processus techniques tels que des workflows techniques ou des workflows de campagne.

  Pour plus d&#39;informations sur les comptes externes, consultez cette [page](../administration/external-account.md).

* **Mapping de diffusion** : permet de surveiller les activités et les modifications récentes apportées à votre mapping de diffusion dans Campaign V8.

  Pour plus d’informations sur les mappings de diffusion, consultez cette [page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Application web** vous permet de vérifier les modifications apportées aux formulaires web dans Campaign V8, utilisés pour créer des pages avec des champs de saisie et de sélection, et qui peuvent inclure des données de la base de données.

  Pour plus d&#39;informations sur les applications web, consultez cette [page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/content/webapps).

* **Offre** : permet de vérifier les activités et les dernières modifications apportées à vos offres.

  Pour plus d’informations sur les offres, consultez cette [page](../msg/offers.md).

* **Opérateur ou opératrice** : permet de surveiller les activités et les modifications récentes apportées à vos opérateurs et opératrices dans Campaign V8.

  Pour plus d’informations sur les opérateurs et opératrices, consultez cette [page](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Accéder au journal d’audit {#accessing-audit-trail}

Pour accéder au **[!UICONTROL journal d’audit]** de votre instance, procédez comme suit :

1. Dans le menu **[!UICONTROL Administration]**, sélectionnez **[!UICONTROL Journal d’audit]**.

   ![Capture d’écran affichant le menu Administration avec l’option Journal d’audit sélectionnée](assets/audit-trail-1.png)

1. La fenêtre **[!UICONTROL Journal d’audit]** s’ouvre avec la liste de vos entités. L’interface utilisateur web d’Adobe Campaign effectue le contrôle des actions de création, de modification et de suppression des workflows, des options, des diffusions et des schémas.

   Sélectionnez l’une des entités pour en savoir plus sur les dernières modifications.

1. La fenêtre **[!UICONTROL Entité d&#39;audit]** fournit des informations détaillées sur l&#39;entité choisie, telles que :

   * **[!UICONTROL Type]** : workflow, options, diffusions ou schémas.
   * **[!UICONTROL Entité]** : nom interne de vos activités.
   * **[!UICONTROL Modifié par]** : nom d’utilisateur de la dernière personne ayant modifié cette entité.
   * **[!UICONTROL Action]** : dernière action effectuée sur cette entité, qu&#39;elle ait été créée, modifiée ou supprimée.
   * **[!UICONTROL Date de modification]** : date de la dernière action effectuée sur cette entité.

   Le bloc de code fournit davantage d’informations sur ce qui a été modifié dans votre entité.

   ![Capture d’écran affichant la fenêtre Entité d’audit avec des informations détaillées sur les modifications](assets/audit-trail-2.png)