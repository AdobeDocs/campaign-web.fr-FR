---
title: Gestion des fuseaux horaires
description: Découvrez comment l’interface d’utilisation d’Adobe Campaign Web affiche les valeurs de date et d’heure en fonction du fuseau horaire du navigateur, de l’opérateur ou de l’opératrice, du workflow et du serveur.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 100%

---

# Gestion des fuseaux horaires {#timezone-management}

L’interface d’utilisation d’Adobe Campaign Web affiche toutes les valeurs de date et d’heure en fonction du **fuseau horaire local du navigateur web de l’utilisateur ou de l’utilisatrice**. Ce comportement peut faire apparaître des différences entre les dates et heures de l’interface d’utilisation web et de la console cliente.

Cette section explique les différences attendues entre les fuseaux horaires de l’**interface d’utilisation web**, de la **console cliente** et de l’**exécution des workflows**.

>[!NOTE]
>
>Aucune donnée stockée sur le serveur n’est modifiée. Seul l’affichage dans l’interface change.

## Principaux concepts

* **Fuseau horaire du serveur** : le fuseau horaire du serveur correspond au fuseau horaire configuré sur le système d’exploitation du serveur. Toutes les dates et heures sont stockées en interne en UTC sur le serveur.

* **Comportement de la console cliente** : la console cliente affiche les dates et heures selon le **fuseau horaire de l’opérateur ou de l’opératrice**, défini dans les paramètres de l’opérateur ou de l’opératrice. Cela correspond par défaut au **fuseau horaire du serveur**.

* **Comportement de l’interface d’utilisation web** : l’interface d’utilisation web affiche les dates et heures selon le **fuseau horaire local du navigateur**. Si le fuseau horaire du navigateur ou du système est modifié, les valeurs de date et d’heure affichées sont automatiquement mises à jour.

* **Comportement des workflows** : les workflows interprètent les dates et heures locales en fonction du **fuseau horaire configuré des workflows**. S’il n’est pas spécifié, le **fuseau horaire du serveur** est utilisé par défaut.

## Exemple

| Interface | Fuseau horaire utilisé | Exemple d’affichage |
|------------|----------------|-----------------|
| Console cliente | Opérateur ou opératrice (par défaut : serveur) | `2025-10-20 14:00:00` |
| Interface utilisateur web | Fuseau horaire local du navigateur | `2025-10-20 21:00:00` (pour le navigateur en UTC +7) |

Dans cet exemple, les deux interfaces utilisent les mêmes dates et heures UTC sous-jacentes, mais chacune les affiche selon un fuseau horaire différent.

## Impact

Des différences dans les heures affichées peuvent apparaître dans :

* les champs de profil ou de données contenant des valeurs `datetime` ;
* les logs de diffusion ou dates de contact ;
* l’exécution des workflows et les dates et heures des imports.

Les données sous-jacentes restent les mêmes. La différence réside uniquement dans le **rendu**.

>[!NOTE]
>
>Si des utilisateurs et utilisatrices de différentes régions collaborent sur la même instance, des différences entre les dates et heures de l’interface d’utilisation web et de la console peuvent apparaître.

## Recommandations

Pour harmoniser les valeurs affichées sur les différentes interfaces, vous pouvez :

* modifier le **fuseau horaire du navigateur** pour qu’il corresponde au **fuseau horaire de l’opérateur ou de l’opératrice, ou du serveur**.
* Lors de l’export de données (les exports utilisent UTC), vérifiez que la conversion dans les outils de création de rapports est cohérente.
* Lors de la conception de workflows, définissez explicitement le **fuseau horaire du workflow** dans les propriétés de l’activité afin de garantir une planification et un import prévisibles.
* Informez les personnes professionnelles que les différences de date et heure entre les affichages de l’interface d’utilisation web et de la console cliente sont **normales et attendues**.
