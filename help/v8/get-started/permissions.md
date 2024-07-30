---
audience: end-user
title: Gestion des autorisations dans l’interface utilisateur web de Campaign
description: En savoir plus sur les autorisations dans l’interface utilisateur web de Campaign
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 28%

---


# Autorisations {#permissions}

Chaque utilisateur d’Adobe Campaign dispose de ses propres autorisations et restrictions dans l’application.

L&#39;utilisateur peut faire partie d&#39;un groupe d&#39;opérateurs et héritera des permissions du groupe.

En fonction de ses permissions, un opérateur peut :

* l’accès à certaines fonctionnalités
* l’accès à certaines données
* l’accès à certaines actions (création, modification ou suppression)

## Autorisations sur les dossiers {#folder-permissions}

En fonction de vos droits, vous avez la possibilité d’afficher et de gérer les autorisations des dossiers dans les **[!UICONTROL Paramètres du dossier]**.
Voici un exemple sur un dossier de diffusions.

![](assets/folder_settings.png){zoomable="yes"}

Dans la section **[!UICONTROL Sécurité]** des **[!UICONTROL Paramètres du dossier]**, vous pouvez afficher et gérer (ajouter ou supprimer) des opérateurs ou des groupes qui peuvent accéder au dossier.

![](assets/folder_security.png){zoomable="yes"}

Vous pouvez cliquer directement sur les autorisations et les modifier en **[!UICONTROL Autorisé]** ou **[!UICONTROL Refusé]**.

![](assets/folder_security_denied.png){zoomable="yes"}

Si l’option **[!UICONTROL Propager]** est activée, toutes les autorisations définies pour un dossier sont appliquées à tous ses sous-dossiers. Ces autorisations peuvent être surchargées pour chaque sous-dossier.

Si l&#39;option **[!UICONTROL Dossier système]** est cochée, l&#39;accès est autorisé à tous les opérateurs, quelles que soient leurs permissions.

Vous pouvez également [gérer les autorisations sur les dossiers dans la console Adobe Campaign](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/folder-permissions).
Toutes les autorisations de l’interface utilisateur web de Campaign sont synchronisées avec les autorisations de la console cliente Campaign.
