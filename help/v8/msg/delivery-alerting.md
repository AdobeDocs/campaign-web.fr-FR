---
audience: end-user
title: Alertes de diffusion
description: Découvrez comment utiliser les alertes de diffusion.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 19%

---

# Commencer avec les alertes de diffusion {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Alertes de diffusion"
>abstract="Les alertes de diffusion sont désormais disponibles dans Campaign. Cette fonctionnalité est un système de gestion des alertes qui permet à des groupes d’utilisateurs et utilisatrices de recevoir automatiquement des notifications par e-mail contenant des informations sur leurs exécutions de diffusion."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

Les alertes de diffusion sont un système de gestion des alertes qui permet à des groupes d’utilisateurs et utilisatrices de recevoir automatiquement des notifications par e-mail contenant des informations sur leurs exécutions de diffusion. Les destinataires peuvent surveiller les diffusions en cours traitées par Adobe Campaign et prendre les mesures appropriées en cas de problème.

Les notifications peuvent être personnalisées en fonction de critères d’alerte spécifiques définis via l’interface utilisateur web d’Adobe Campaign.

Pour plus d&#39;informations sur la gestion des diffusions en échec, reportez-vous à la section [Documentation d’Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Contenu des notifications par email {#content}

Les notifications par e-mail comprennent les sections suivantes :

* **Résumé**: affiche le nombre de diffusions répondant aux critères que vous avez définis, avec des libellés et des couleurs pour chaque critère.
* **Détails**: répertorie tous les critères de diffusion définis pour le tableau de bord et les diffusions correspondantes pour chaque critère.

![](assets/alerting-email.png)

## Configurer des alertes de diffusion {#set-up}

Pour vous aider à configurer ces alertes, l&#39;interface utilisateur Web de Campaign vous permet de créer et de gérer :

* **Tableaux de bord des alertes de diffusion**: indiquez les destinataires, définissez les critères des alertes à inclure dans le tableau de bord et accédez à un historique des alertes envoyées. [Découvrez comment utiliser les tableaux de bord](../msg/delivery-alerting-dashboards.md)
* **Critères des alertes de diffusion**: l&#39;interface utilisateur web de Campaign fournit des critères d&#39;alerte prédéfinis (diffusions avec faible débit, diffusions dont la préparation a échoué...) que vous pouvez ajouter à votre tableau de bord. Vous pouvez également créer vos propres critères en fonction de vos besoins. [Découvrez comment utiliser les critères](../msg/delivery-alerting-criteria.md)

Supposons que vous souhaitiez informer les utilisateurs disposant de droits d’administration uniquement des diffusions en échec et des utilisateurs marketing des diffusions présentant un taux de soft bounces élevé. Pour ce faire, créez deux tableaux de bord distincts avec les critères appropriés pour chaque groupe de destinataires.

>[!NOTE]
>
>Pour accéder aux tableaux de bord et aux critères des alertes et les configurer, vous devez disposer des **droits d&#39;administration** ou faire partie de la **Superviseurs de diffusion** groupe de sécurité. Les utilisateurs standard ne peuvent pas accéder aux tableaux de bord dans l’interface Adobe Campaign, mais ils peuvent recevoir des notifications d’alerte. [En savoir plus sur l’accès et les autorisations](../get-started/permissions.md)
