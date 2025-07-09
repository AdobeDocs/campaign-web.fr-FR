---
title: Prise en main des rapports dynamiques
description: En savoir plus sur le contrat d’utilisation des rapports dynamiques
level: Beginner
audience: end-user
exl-id: 9fcef466-f306-480e-b42e-d18daa8bcf06
source-git-commit: fb5bcde9c087f73bfe5724463fe280c1e494ef1f
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 64%

---

# Accord sur l&#39;utilisation des rapports dynamiques {#pii-agreement}

L’accord sur l’utilisation des rapports dynamiques fonctionne comme un consentement pop-up pour le traitement des données. Par défaut, seuls les utilisateurs auxquels sont affectés des droits d&#39;administration peuvent afficher et accepter ou refuser cet accord.

Pour accéder au contrat d’utilisation des rapports dynamiques, sélectionnez **[!UICONTROL Outils]** > **[!UICONTROL Avancé]** > **[!UICONTROL Assistant de déploiement]**.

![](assets/pii-agreement.png)

Trois options sont disponibles :

* **[!UICONTROL Me demander ultérieurement]** : tant que vous n’avez pas accepté ou refusé le contrat, les dimensions de profil n’apparaîtront pas dans vos rapports et les informations d’identification personnelles de vos clients ne seront pas collectées ni envoyées.
* **[!UICONTROL Accepter]** : lorsque vous acceptez les termes de cet accord, vous autorisez Adobe Campaign à collecter les PII de vos clients et à les transférer au centre de données ou de reporting.
* **[!UICONTROL Refuser]** : lorsque vous refusez les termes de l&#39;accord, les dimensions de profil ne s&#39;affichent pas dans vos rapports et les PII de vos clients ne sont pas collectées ni envoyées. Notez que dans ce cas, externalID sera toujours collecté et utilisé pour identifier les utilisateurs finaux.

Le tableau ci-dessous indique ce qui se passe après l&#39;acceptation de cet accord selon votre zone géographique.

|  | Rapports dynamiques | Connecteur Microsoft Dynamics 365 |
|---|---|---|
| Amériques et Asie-Pacifique | **Fonctionnalité disponible**. <br>Toutes les informations de profil prêtes à l’emploi (c’est-à-dire la ville, le pays/la région, l’État, le sexe et les segments en fonction de l’âge) et personnalisées transmises au centre de reporting des États-Unis. | **Fonctionnalité disponible**. <br>Tous les champs de profil personnalisés et d&#39;usine, ainsi que les champs d&#39;événement Adobe Campaign, sont traités dans le centre de données des États-Unis. |
| EMEA (Europe, Moyen-Orient et Afrique) | **Fonctionnalité disponible**. <br>Toutes les informations de profil prêtes à l’emploi (c’est-à-dire la ville, le pays/la région, l’État, le sexe et les segments en fonction de l’âge) et personnalisées transmises au centre de reporting EMEA. | **Fonctionnalité disponible.** <br>Tous les champs de profil personnalisés et d&#39;usine, ainsi que les champs d&#39;événement Adobe Campaign, sont traités dans le centre de données EMEA. Les <br>**[!UICONTROL données de contrôle ]**qui contiennent les données d&#39;enregistrement Adobe I/O et les identifiants des événements utilisateur des clients sont envoyés et stockés dans le centre de données des Etats-Unis. |

Le tableau ci-dessous indique ce qui se passe après le refus de cet accord selon votre zone géographique. Notez que même si vous refusez cet accord, le reporting sur les diffusions et l&#39;intégration de Microsoft Dynamics 365 sera toujours disponible.

| Zone géographique | Rapports dynamiques | Connecteur Microsoft Dynamics 365 |
|---|---|---|
| Amériques et Asie-Pacifique | **Fonctionnalité disponible**. <br> Aucune information de profil personnalisée et d&#39;usine n&#39;est transmise au centre de reporting des Etats-Unis, à l&#39;exception d&#39;ExternalID. | **Fonctionnalité disponible**. <br>Aucun champ de profil personnalisé et d&#39;usine n&#39;est envoyé au centre de données des Etats-Unis, à l&#39;exception des champs Identifiant externe et Identifiant du destinataire. <br>Tous les champs d’événement Adobe Campaign sont traités dans le centre de données des États-Unis, à l’exception de l’ID de page miroir. |
| EMEA (Europe, Moyen-Orient et Afrique) | **Fonctionnalité disponible**. <br>Aucune information de profil personnalisée et d&#39;usine n&#39;est transmise au centre de reporting EMEA, à l&#39;exception d&#39;ExternalID. | **Fonctionnalité disponible.** <br>Aucun champ de profil personnalisé et d&#39;usine n&#39;est envoyé au centre de données EMEA, à l&#39;exception des champs Identifiant externe et Identifiant du destinataire. <br>Tous les champs d’événement Adobe Campaign sont traités dans le centre de données EMEA, à l’exception de l’ID de page miroir. |

Ce choix n&#39;est pas définitif, vous pouvez toujours le modifier en sélectionnant l&#39;option **[!UICONTROL realtimeReporting_collectPII]** dans **[!UICONTROL Administration]** > **[!UICONTROL Platform]** > **[!UICONTROL Options]**.

La valeur peut être modifiée à tout moment. La valeur 1 correspond à **[!UICONTROL Me demander plus tard]**, 2 à **[!UICONTROL Refuser]** et 3 à **[!UICONTROL Accepter]**.
