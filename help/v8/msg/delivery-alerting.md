---
audience: end-user
title: Alertes de diffusion
description: Découvrez comment utiliser les alertes de diffusion.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 39dcf11797339ee9800da6c5a32b1a1c3470529a
workflow-type: ht
source-wordcount: '342'
ht-degree: 100%

---

# Commencer avec les alertes de diffusion {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Alertes de diffusion"
>abstract="Les alertes de diffusion sont désormais disponibles dans Campaign. Cette fonctionnalité est un système de gestion des alertes qui permet à des groupes d’utilisateurs et utilisatrices de recevoir automatiquement des notifications par e-mail contenant des informations sur leurs exécutions de diffusion."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

Les alertes de diffusion sont un système de gestion des alertes qui permet à des groupes d’utilisateurs et d’utilisatrices de recevoir automatiquement des notifications par e-mail contenant des informations sur l’exécution de leurs diffusions. Les personnes destinataires peuvent surveiller les diffusions en cours traitées par Adobe Campaign et prendre les mesures appropriées en cas de problème.

Les notifications peuvent être personnalisées en fonction de critères d’alertes spécifiques définis via l’interface d’utilisation web d’Adobe Campaign.

Pour plus d’informations sur la gestion des diffusions en échec, reportez-vous à la [documentation d’Adobe Campaign v8 (console)](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}.

## Table des matières des notifications par e-mail {#content}

Les notifications par e-mail comprennent les sections suivantes :

* **Résumé** : affiche le nombre de diffusions répondant aux critères que vous avez définis, avec des libellés et des couleurs pour chaque critère.
* **Détails** : répertorie tous les critères de diffusion définis pour le tableau de bord et les diffusions correspondantes pour chaque critère.

![](assets/alerting-email.png)

## Configurer des alertes de diffusion {#set-up}

Pour vous aider à configurer ces alertes, l’interface d’utilisation de Campaign Web vous permet de créer et de gérer les éléments suivants :

* **Tableaux de bord des alertes de diffusion** : indiquez les personnes destinataires, définissez les critères des alertes à inclure dans le tableau de bord et accédez à un historique des alertes envoyées. [Découvrir comment utiliser les tableaux de bord](../msg/delivery-alerting-dashboards.md)
* **Critères des alertes de diffusion** : l’interface d’utilisation de Campaign Web fournit des critères des alertes prédéfinis (diffusions avec faible débit, diffusions dont la préparation a échoué...) que vous pouvez ajouter à votre tableau de bord. Vous pouvez également créer vos propres critères en fonction de vos besoins. [Découvrir comment utiliser les critères](../msg/delivery-alerting-criteria.md)

Supposons que vous souhaitiez informer les utilisateurs et utilisatrices disposant de droits d’administration uniquement des diffusions en échec et les utilisateurs et utilisatrices marketing des diffusions présentant un taux d’erreurs de rebonds temporaires élevé. Pour ce faire, créez deux tableaux de bord distincts avec les critères appropriés pour chaque groupe de personnes destinataires.

>[!NOTE]
>
>Pour accéder aux tableaux de bord ainsi qu’aux critères des alertes et les configurer, vous devez disposer de **droits d’administration** ou figurer dans le groupe de sécurité **Superviseurs et superviseuses de diffusion**. Les utilisateurs et utilisatrices standard ne peuvent pas accéder aux tableaux de bord dans l’interface Adobe Campaign, mais ils peuvent recevoir des notifications d’alertes. [En savoir plus sur l’accès et les autorisations](../get-started/permissions.md)
