---
audience: end-user
title: Surveiller les logs de diffusion
description: Découvrez comment surveiller les logs de diffusion.
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 100%

---

# Surveiller les logs de diffusion {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Logs de diffusion"
>abstract="Les logs de diffusion affichent le détail de l’envoi. Ils indiquent le détail de l’envoi, la cible exclue et les raisons de l’exclusion et fournissent des informations de tracking telles que les ouvertures et les clics."

Une fois la diffusion préparée et lorsque vous avez cliqué sur le bouton **Envoyer**, accédez aux logs de diffusion pour vérifier les avertissements, les erreurs, le statut, les exclusions et les données de tracking. Vous pouvez accéder à ces logs depuis le tableau de bord des messages. Ils indiquent le détail de l’envoi, la cible exclue et les raisons de l’exclusion et fournissent des informations de tracking telles que les ouvertures et les clics.

Pour afficher les logs, accédez au tableau de bord de votre diffusion et cliquez sur le bouton **Logs**.

Les onglets suivants sont disponibles :

* [Logs](#logs-tab)
* [Diffusions](#deliveries-tab)
* [Exclusions](#exclusion-tab)
* [Causes d’exclusion](#exclusion-causes)
* [URL trackées](#tracked-urls)
* [Tracking](#tracking)

## Logs {#logs-tab}

L’onglet **Logs** contient tous les messages relatifs à la diffusion et aux bons à tirer (BAT). Des icônes spécifiques permettent de repérer les erreurs ou avertissements.

Toutes les étapes de validation, les avertissements et les erreurs sont répertoriés. Les icônes colorées indiquent le type de message :

* L’icône grise indique un message informatif.
* L’icône jaune indique une erreur de traitement non critique.
* L’icône rouge indique une erreur critique qui empêche l’envoi de la diffusion. Les erreurs critiques doivent être corrigées pour que la diffusion soit envoyée.

![ Onglet Logs affichant les étapes de validation, les avertissements et les erreurs avec des icônes colorées indiquant les types de messages.](assets/logs.png){zoomable="yes"}

## Diffusions {#deliveries-tab}

L&#39;onglet **Envois** propose un historique des occurrences de cette diffusion. Y est répertoriée la liste des messages envoyés et leur statut. Il permet de visualiser l&#39;état de la diffusion pour chaque destinataire.

![ L’onglet Diffusions affichant l&#39;historique des messages envoyés et leur statut.](assets/logs2.png){zoomable="yes"}

## Exclusions {#exclusion-tab}

L’onglet **Logs d’exclusion** répertorie tous les messages qui ont été exclus de la cible et indique la raison de l’échec de l’envoi.

![Onglet Exclusions répertoriant les messages exclus et les raisons des échecs d’envoi.](assets/logs3.png){zoomable="yes"}

## Causes d’exclusion {#exclusion-causes-tab}

L’onglet **Causes des exclusions** affiche, pour chaque cause possible, le nombre de messages qui ont été exclus de la cible.

![Onglet Causes d’exclusion indiquant le nombre de messages exclus pour chaque cause.](assets/logs4.png){zoomable="yes"}

## URL suivies {#tracked-urls-tab}

L’onglet **URL trackées** regroupe les URL contenues dans les messages envoyés, y compris leur type et leur source.

![Onglet URL trackées affichant les URL contenues dans les messages envoyés, leurs types et leurs sources.](assets/logs5.png){zoomable="yes"}

## Tracking {#tracking-tab}

L’onglet **Tracking** liste l&#39;historique du tracking pour cette diffusion. Cet onglet affiche les données de tracking sur les messages envoyés, notamment toutes les URL qui ont fait l’objet d’un tracking par Adobe Campaign.

![Onglet Tracking affichant l’historique du tracking et les données des messages envoyés.](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>Si le tracking n’est pas activé pour une diffusion, cet onglet n’est pas affiché.