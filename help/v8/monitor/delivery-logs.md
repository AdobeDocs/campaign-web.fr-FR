---
audience: end-user
title: Surveiller les logs de diffusion
description: Documentation web de Campaign v8
source-git-commit: 4ed89d326acd3b7d5d8f14bec68cceda3c8169fb
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 65%

---

# Surveiller les logs de diffusion {#delivery-logs}

>[!NOTE]
>
>Cette documentation est en cours de construction et fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Logs de diffusion"
>abstract="TBC"

Après avoir préparé et envoyé un email, les logs de diffusion vous permettent de vérifier qu&#39;il n&#39;y a pas d&#39;erreur. Ces logs sont accessibles depuis le tableau de bord des messages. Ils indiquent le détail de l&#39;envoi, la cible exclue et les raisons de l&#39;exclusion et fournissent des informations de tracking telles que les ouvertures et les clics.

Pour afficher les journaux, cliquez sur le bouton **Journaux** bouton .

![](assets/logs.png)

Plusieurs onglets contiennent les informations (si elles existent) relatives aux Envois, aux Exclus, aux Causes d&#39;exclusion, aux Logs de tracking et URL suivies.

**Los** tab

Le **Journaux** contient tous les messages relatifs à la diffusion et aux bons à tirer. Des icônes spécifiques permettent de repérer les erreurs ou avertissements.

Toutes les étapes de validation, les avertissements et les erreurs sont répertoriés. Les icônes colorées indiquent le type de message :

* L’icône grise indique un message informatif.
* L’icône jaune indique une erreur de traitement non critique.
* L’icône rouge indique une erreur critique qui empêche l’envoi de la diffusion.

**Onglet Diffusions**

Le **Diffusions** offre un historique de chaque occurrence de cette diffusion. Y est répertoriée la liste des messages envoyés et leur statut. Il permet de visualiser l&#39;état de la diffusion pour chaque destinataire.

**Exclusions** tab

L’onglet Logs d’exclusion liste tous les messages qui ont été exclus de l&#39;envoi à la cible et indique la raison de l&#39;échec de l&#39;envoi.

**Exclusions appliquées** tab

L&#39;onglet **Causes d&#39;exclusion** indique le volume (en nombre de messages) des messages qui ont été exclus de l&#39;envoi à la cible.

**URL trackées** tab

Le **URL trackées** affichage des onglets

**Onglet Tracking**

L&#39;onglet **Tracking** liste l&#39;historique du tracking pour cette diffusion. Cet onglet affiche les informations de tracking sur les messages envoyés, soit toutes les URL qui ont fait l&#39;objet d&#39;un tracking par Adobe Campaign. Les informations de tracking sont mises à jour toutes les heures.

>[!NOTE]
>
>Si le tracking n&#39;est pas activé pour une diffusion, cet onglet n&#39;est pas affiché.

Les données de tracking sont interprétées dans les rapports de diffusion. Voir cette section.



