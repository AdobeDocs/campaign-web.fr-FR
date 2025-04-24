---
audience: end-user
title: Gestion des autorisations dans l’interface utilisateur web de Campaign
description: En savoir plus sur les autorisations dans l’interface utilisateur web de Campaign
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '239'
ht-degree: 100%

---

# Autorisations {#permissions}

Chaque utilisateur et utilisatrice d’Adobe Campaign dispose de ses propres autorisations et restrictions dans l’application. L’utilisateur ou l’utilisatrice peut appartenir à un groupe d’opérateurs et d’opératrices et hériter des autorisations du groupe.

En fonction de ses autorisations, l’opérateur ou l’opératrice peut :

* Accéder à certaines fonctionnalités
* Accéder à certaines données
* Accéder à certaines actions (création, modification ou suppression)

La procédure détaillée de configuration des autorisations dans Adobe Campaign est disponible dans la [documentation Adobe Campaign v8 (console)](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Autorisations sur les dossiers {#folder-permissions}

En fonction de vos droits, vous pouvez afficher et gérer les autorisations sur les dossiers dans les **[!UICONTROL paramètres des dossiers]**.

Voici un exemple de dossier de diffusion :

![Exemple de paramètres de dossier dans Adobe Campaign](assets/folder_settings.png){zoomable="yes"}

Dans la section **[!UICONTROL Sécurité]** des **[!UICONTROL Paramètres du dossier]**, vous pouvez afficher et gérer (ajouter ou supprimer) des opérateurs ou opératrices ou des groupes qui peuvent accéder au dossier.

![Exemple de paramètres de sécurité des dossiers dans Adobe Campaign](assets/folder_security.png){zoomable="yes"}

Vous pouvez cliquer directement sur les autorisations et les définir sur **[!UICONTROL Autorisé]** ou **[!UICONTROL Refusé]**.

![Exemple d’autorisations refusées dans les paramètres de sécurité des dossiers](assets/folder_security_denied.png){zoomable="yes"}

Si l’option **[!UICONTROL Propager]** est activée, toutes les autorisations définies pour un dossier sont appliquées à tous ses sous-dossiers. Ces autorisations peuvent être remplacées pour chaque sous-dossier.

Si l’option **[!UICONTROL Dossier système]** est activée, l’accès est autorisé à tous les opérateurs et opératrices, quelles que soient leurs autorisations.

Vous pouvez également [gérer les autorisations sur les dossiers dans la console Adobe Campaign](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Toutes les autorisations de l’interface d’utilisation de Campaign Web sont synchronisées avec celles de la console cliente Campaign.