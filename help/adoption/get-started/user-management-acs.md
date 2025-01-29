---
title: Migration des utilisateurs et utilisatrices techniques vers Adobe Developer Console
description: Découvrez comment migrer la gestion des accès utilisateur de Campaign Standard vers Campaign V8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: bca2b133968d9392098e9b8b76d65e44d7e84645
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 6%

---

# Gestion des accès des utilisateurs et des utilisatrices de Campaign Standard vers Campaign V8 {#user-management-acs}

Adobe Campaign Standard et Adobe Campaign V8 permettent aux utilisateurs de définir et de gérer des autorisations pour différents utilisateurs/opérateurs. Ces autorisations se composent de droits spécifiques qui accordent aux utilisateurs l’accès à diverses fonctionnalités du produit. Toutefois, les deux produits utilisent des approches et des implémentations distinctes pour gérer l’accès des utilisateurs et utilisatrices.

Les concepts ci-dessous sont utilisés dans Adobe Campaign Standard et Campaign V8 pour gérer l’accès des utilisateurs et utilisatrices :

| Campaign Standard | Campaign V8 |
|---------|----------|
| Utilisateur | Opérateur |
| Rôle | Droit nommé |
| Groupe de sécurité | Groupe D’Opérateurs |
| Organizational unit | Autorisation Dossier |

## Approche de migration du groupe de sécurité vers le groupe d’opérateurs

>[!CAUTION]
>
>Les fonctionnalités de ces rôles/droits nommés peuvent varier dans l’implémentation, ce qui peut entraîner des problèmes d’autorisation (par exemple, élévation des privilèges ou perturbations des fonctionnalités). Nous recommandons aux utilisateurs de passer en revue ces mappages après la transition pour garantir un contrôle d’accès approprié. [En savoir plus sur les autorisations](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

Le tableau ci-dessous décrit l’approche de migration des groupes de rôles utilisateur lors de la transition de Adobe Campaign Standard vers Campaign V8. En Campaign Standard, un **Groupe de sécurité**, appelé **Groupe d’opérateurs** dans Campaign V8, est utilisé pour affecter un ensemble de rôles à un utilisateur. Bien que certains groupes de sécurité/groupes d’opérateurs soient disponibles par défaut, les utilisateurs peuvent créer des groupes ou modifier des groupes existants si nécessaire.

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **Terminologie**  | Groupe de sécurité | Groupe D’Opérateurs |

Dans Adobe Campaign Standard et Campaign V8, les **groupes de sécurité** et **groupes d’opérateurs** sont mappés aux profils de produit dans Admin Console. Si vous souhaitez affecter un **Groupe de sécurité** ou **Groupe d’opérateurs** à un utilisateur, vous pouvez lier le **profil de produit** correspondant dans Admin Console. Cette association est synchronisée lorsque l’utilisateur se connecte. [En savoir plus sur le profil de produit](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Groupe de sécurité Campaign Standard** | **Groupe d’opérateurs Campaign V8** |
|----------|---------|
| Administrateurs | Administrateurs |
| Superviseurs de diffusion | Administrateurs |
| Superviseurs de workflow | Superviseurs de workflow  |

## Approche de migration des rôles utilisateur vers les droits nommés

Dans Adobe Campaign Standard, le terme **rôle utilisateur** est appelé **droit nommé** dans Campaign V8. Le tableau ci-dessous décrit la terminologie utilisée pour **Droits nommés** dans Campaign V8, qui correspond à **Rôles utilisateur** dans Campaign Standard.

| **Rôle d&#39;utilisateur Campaign Standard** | **Droit nommé dans Campaign V8** | **Description**  |
|----------|---------|---------|
| Administration  | Administration  | L’utilisateur disposant du droit d’administration dispose d’un accès complet à l’instance. |
| Modèle de données  | Administration | Droit pour exécuter des publications et créer des ressources personnalisées. Fonctionnalité liée à la création de schémas disponible pour l’administrateur dans Campaign V8.  |
| DéliVRABILITÉ  | Administration  | Droit pour valider les diffusions préalablement analysées.  |
| Exporter | Exporter | Droit pour exporter des données.  |
| Accès aux fichiers  | Accès aux fichiers  | Droit pour valider les diffusions préalablement analysées.  |
| Import générique  | Importer  | Droit pour l&#39;import de données génériques |
| Préparation des diffusions | Préparation des diffusions | Droit pour créer, modifier, préparer et supprimer des diffusions.  |
| Exécution du script SQL | Exécution du script SQL | Droit pour exécuter toute commande SQL directement sur la base de données. |
| Démarrer les diffusions  | Démarrer les diffusions  | Droit pour valider les diffusions préalablement analysées.  |
| Exécution des commandes système | Exécution du programme | Droit pour exécuter des commandes système sur le serveur. |
| Workflow | Workflow | Droit pour gérer l&#39;exécution des workflows, démarrer, arrêter, mettre en pause, etc. |

## Approche de la migration depuis l’entité organisationnelle

Dans Adobe Campaign Standard, l’**organisation uni** t est mappée au modèle de hiérarchie existant **Dossier** dans Campaign V8 afin de conserver un contrôle d’accès similaire. [En savoir plus sur la gestion des dossiers](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **Terminologie**  | Organizational unit | Dossier |

## Approche de migration à partir du programme

Dans Campaign V8, les **programmes** sont représentés sous la forme de **dossiers**. Campaign V8 permet de créer des dossiers et de restreindre leur accès.

En utilisant les **Groupes** et **Droits nommés**, les **Opérateurs** peuvent avoir accès à des **Dossiers** spécifiques dans la hiérarchie de navigation, avec la possibilité d’attribuer des autorisations de lecture, d’écriture et de suppression. [En savoir plus sur la gestion des dossiers](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Un **Programme** étant traité comme un **Dossier** dans Campaign V8, son accès peut être géré de la même manière que n’importe quel autre dossier. Après la migration, les administrateurs de Campaign Standard peuvent suivre les étapes suivantes :

1. Dans l’explorateur, cliquez avec le bouton droit de la souris sur un dossier et sélectionnez **[!UICONTROL Propriétés...]**.
1. Accédez à l’onglet **[!UICONTROL Sécurité]**.
1. Modifiez les autorisations du groupe d’opérateurs en fonction du modèle d’accès souhaité. 

## Mappage du profil de produit pour accéder aux API REST 

Pour accéder aux API transactionnelles à partir de l&#39;instance d&#39;exécution dans Campaign V8, un nouveau **profil de produit** est requis, en plus des profils de produit **Administrateur** et **Message Center**. Ce nouveau **profil de produit** sera ajouté en Campaign Standard aux comptes techniques existants ou précréés.

Après la migration, les utilisateurs du Campaign Standard doivent consulter leurs **mappages de profils de produit** et attribuer le **profil de produit** approprié s’ils ne souhaitent pas lier leurs **comptes techniques** au **profil d’administrateur** de produit. Pour les intégrations futures, il est recommandé d’utiliser l’identifiant client Campaign V8 **Tenant ID** dans l’**URL REST** au lieu de l’ancien Campaign Standard **Tenant ID**.

## Migration de l&#39;accès aux ressources Campaign intégrées pour les opérateurs Campaign Standards

Les opérateurs migrés depuis Campaign Standard disposeront d&#39;un accès en lecture à des ressources intégrées spécifiques dans Campaign V8.

## Groupes et rôles de sécurité non migrés {#non-migrated-groups-roles}

Vous trouverez ci-dessous une liste des rôles de Campaign Standard qui n’ont pas été transférés :

* Compte Relais Par Défaut 

* Notification push Message Center 

Vous trouverez ci-dessous une liste des mappages de groupes de sécurité du Campaign Standard qui n’ont pas fait l’objet d’une transition.

* Agents Message Center

* Agents Push Message Center

* Chargés d&#39;application Adobe Experience Manager

* Compte Relais
