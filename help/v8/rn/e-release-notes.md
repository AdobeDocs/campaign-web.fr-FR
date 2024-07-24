---
title: Notes de mise à jour de l’interface d’utilisation web de Campaign v8
description: Découvrez les nouvelles fonctionnalités accompagnant la version suivante de l’interface d’utilisation de Campaign Web.
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: f8bdb15151774b33a0bcf16e86347dae6ab417a2
workflow-type: ht
source-wordcount: '401'
ht-degree: 100%

---

# Notes de mise à jour anticipées {#e-release}

L’interface d’utilisation d’Adobe Campaign Web fournit continuellement de nouvelles fonctionnalités, des améliorations des fonctionnalités existantes et des correctifs. Toutes les modifications sont consolidées à la fin de chaque mois dans les [notes de mise à jour](release-notes.md).

**Les notes de mise à jour anticipées ci-dessous peuvent être modifiées sans préavis jusqu’à la date de publication.**. Les liens, les écrans et la documentation mise à jour sont publiés dans les [notes de mise à jour](release-notes.md), à la date de publication.

## Notes de mise à jour de juillet {#24-7-release}

**Date de publication** : 30-31 juillet 2024

Les fonctionnalités et améliorations suivantes sont disponibles à compter de la version de juillet.

### Fragments de contenu {#24-7-1}

Vous pouvez désormais créer et utiliser des fragments de contenu. Un fragment de contenu est un composant réutilisable pouvant être référencé dans un ou plusieurs messages. Lors de la modification d’un fragment, chaque contenu qui l’utilise est mis à jour. Cette fonctionnalité permet de précréer plusieurs blocs de contenu personnalisés destinés aux utilisateurs et utilisatrices marketing et permettant d’assembler rapidement les contenus de messages dans un processus de conception amélioré.

Deux types de fragments sont disponibles :

* Les **fragments d’expression** sont des expressions prédéfinies disponibles à partir d’une entrée dédiée dans l’éditeur d’expression.
* Les **fragments visuels** sont des blocs visuels prédéfinis que vous pouvez réutiliser dans plusieurs diffusions e-mail ou dans des modèles de contenu. [En savoir plus](../email/fragments.md)

  >[!AVAILABILITY]
  >
  >Les **fragments visuels** sont en disponibilité limitée (LA). Cette fonctionnalité est limitée aux clientes et clients qui effectuent la migration **d’Adobe Campaign Standard vers Adobe Campaign v8** et ne peut pas être déployée dans un autre environnement.

### Listes de contrôle {#24-7-2}

Une liste de contrôle, autrement dit, un **groupe de recouvrements**, est une liste d’adresses de contrôle. Elle est utilisée pour inclure des adresses spécifiques dans vos diffusions, puis pour cibler des profils qui ne correspondent pas aux critères de ciblage définis. Ainsi, les personnes destinataires qui ne font pas partie de l’audience de la diffusion peuvent la recevoir, comme toute autre personne destinataire cible. Vous pouvez utiliser des adresses de contrôle lors de l’envoi d’épreuves ou pour protéger votre liste de publipostage.

### Modèles de notifications push enrichies {#24-7-3}

Vous pouvez désormais envoyer des notifications push enrichies. La notification push enrichie est une forme améliorée de notification mobile qui va au-delà des messages texte simples en incorporant des éléments multimédias tels que des images, des boutons interactifs ou d’autres contenus multimédias enrichis. Avec cette version, un ensemble de modèles pour les notifications push enrichies est désormais disponible pour vos applications iOS et Android.

>[!AVAILABILITY]
>
>Cette fonctionnalité nécessite une mise à jour de Campaign vers la version 8.6.3 ou 8.7.2. En savoir plus dans les [Notes de mise à jour de la console cliente Campaign v8](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/releases/release-notes)

### Améliorations {#improvements-24-7}

**Gestion des dossiers** : vous pouvez désormais gérer les autorisations et les restrictions sur les dossiers.
