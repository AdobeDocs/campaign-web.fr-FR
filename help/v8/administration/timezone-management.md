---
title: Gestion des fuseaux horaires
description: Découvrez comment l’interface utilisateur web d’Adobe Campaign affiche les valeurs de date et d’heure en fonction des fuseaux horaires du navigateur, de l’opérateur, du workflow et du serveur.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 4%

---

# Gestion des fuseaux horaires {#timezone-management}

L’interface utilisateur web d’Adobe Campaign affiche toutes les valeurs de date et d’heure en fonction du **fuseau horaire local du navigateur web de l’utilisateur**. Ce comportement peut entraîner des différences lors de la comparaison des horodatages entre l’interface utilisateur web et la console cliente.

Cette section explique les différences attendues entre les fuseaux horaires **UI web**, **console cliente** et **exécution de workflow**.

>[!NOTE]
>
>Aucune donnée stockée sur le serveur n&#39;est modifiée. Seul son affichage dans l’interface change.

## Principaux concepts

* **Fuseau horaire du serveur** : le fuseau horaire du serveur correspond au fuseau horaire configuré sur le système d&#39;exploitation du serveur. Toutes les dates et heures sont stockées en interne en UTC sur le serveur.

* **Comportement de la console cliente** : la console cliente affiche les horodatages à l’aide du **fuseau horaire de l’opérateur**, défini dans les paramètres de l’opérateur. Par défaut, cela correspond au fuseau horaire du **serveur**.

* **Comportement de l’interface utilisateur web** : l’interface utilisateur web affiche la date et l’heure à l’aide du **fuseau horaire local du navigateur**. Lorsque l’utilisateur modifie le fuseau horaire du navigateur ou du système, les valeurs de date et d’heure affichées sont automatiquement mises à jour.

* **Comportement des workflows** : les workflows interprètent les horodatages locaux en fonction du **fuseau horaire configuré du workflow**. S’il n’est pas spécifié, le fuseau horaire du **serveur** est utilisé par défaut.

## Exemple

| Interface | Fuseau horaire utilisé | Exemple d’affichage |
|------------|----------------|-----------------|
| Console cliente | Opérateur (par défaut = serveur) | `2025-10-20 14:00:00` |
| Interface utilisateur web | Fuseau horaire local du navigateur | `2025-10-20 21:00:00` (pour le navigateur en UTC +7) |

Dans cet exemple, les deux interfaces font référence au même horodatage UTC sous-jacent, mais chacune l’affiche avec un fuseau horaire différent.

## Impact

Des différences dans les heures affichées peuvent apparaître dans :

* Champs de profil ou de données contenant des valeurs `datetime`
* Logs de diffusion ou dates de contact
* Exécution des workflows et horodatage des imports

Les données sous-jacentes restent identiques. La différence réside uniquement dans le **rendu**.

>[!NOTE]
>
>Si des utilisateurs de plusieurs régions collaborent sur la même instance, des incohérences apparentes entre les horodatages de l’interface utilisateur web et de la console peuvent se produire.

## Recommandations

Pour aligner les valeurs d’affichage sur les interfaces, vous pouvez :

* Modifiez le **fuseau horaire du navigateur** pour qu’il corresponde au **fuseau horaire de l’opérateur ou du serveur**.
* Lors de l’exportation de données (les exportations utilisent UTC), assurez-vous que les outils de création de rapports convertissent de manière cohérente.
* Lors de la conception de workflows, définissez explicitement le **fuseau horaire du workflow** dans les propriétés d’activité pour une planification et un comportement d’importation prévisibles.
* Signalez aux utilisateurs professionnels que les différences d’horodatage entre les vues de l’interface utilisateur web et de la console cliente sont **normales et attendues**.
