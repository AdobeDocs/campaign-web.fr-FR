---
audience: end-user
title: Surveiller les logs de diffusion
description: Documentation de l’application web de Campaign v8
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 62%

---

# Surveiller les logs de diffusion {#delivery-logs}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Logs de diffusion"
>abstract="TBC"

Après avoir préparé et envoyé un email, les logs de diffusion vous permettent de vérifier qu&#39;il n&#39;y a pas d&#39;erreur. Ces logs sont accessibles depuis le tableau de bord des messages. Ils indiquent le détail de l&#39;envoi, la cible exclue et les raisons de l&#39;exclusion et fournissent des informations de tracking telles que les ouvertures et les clics.

Pour afficher les logs, accédez au tableau de bord de votre diffusion et cliquez sur le bouton **Journaux** bouton .

Plusieurs onglets sont disponibles :

## Logs

Le **Journaux** contient tous les messages relatifs à la diffusion et aux bons à tirer. Des icônes spécifiques permettent de repérer les erreurs ou avertissements.

Toutes les étapes de validation, les avertissements et les erreurs sont répertoriés. Les icônes colorées indiquent le type de message :

* L’icône grise indique un message informatif.
* L’icône jaune indique une erreur de traitement non critique.
* L’icône rouge indique une erreur critique qui empêche l’envoi de la diffusion.

![](assets/logs.png)

## Diffusions

Le **Diffusions** offre un historique de chaque occurrence de cette diffusion. Y est répertoriée la liste des messages envoyés et leur statut. Il permet de visualiser l&#39;état de la diffusion pour chaque destinataire.

![](assets/logs2.png)

## Exclusions

L’onglet **Logs d’exclusion** liste tous les messages qui ont été exclus de l&#39;envoi à la cible et indique la raison de l&#39;échec de l&#39;envoi.

![](assets/logs3.png)

## Causes d&#39;exclusion

L&#39;onglet **Causes d&#39;exclusion** indique le volume (en nombre de messages) des messages qui ont été exclus de l&#39;envoi à la cible.

![](assets/logs4.png)

## Tracked URLs

L&#39;onglet **URL trackées** regroupe les URL contenues dans le message envoyé, leur type et leur URL source.

![](assets/logs5.png)

## Tracking

Le **Tracking** répertorie l&#39;historique du tracking pour cette diffusion. Cet onglet affiche les données de tracking des messages envoyés, c&#39;est-à-dire toutes les URL qui font l&#39;objet d&#39;un tracking par Adobe Campaign.

>[!NOTE]
>
>Si le tracking n&#39;est pas activé pour une diffusion, cet onglet n&#39;est pas affiché.

![](assets/logs6.png)
