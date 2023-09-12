---
audience: end-user
title: Création d'audiences
description: Découvrez comment créer des audiences dans Adobe Campaign Web
badge: label="Beta"
source-git-commit: ba449ee0b5a4b41db8efbbabeb37ce7cd7cc3720
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 4%

---


# Création d&#39;audiences {#create-audiences}

menu audiences

peut les créer et les cibler dans des diffusions ou des campagnes autonomes ;

## Créer votre première audience {#create}

1. Audience > menu
1. Créer une audience
1. Propriétés : libellé et options supplémentaires
1. Canevas de workflow avec activité de création d’audience
1. Modifier l’activité, modifier le flux de workflow en fonction de ses besoins
1. démarrer le workflow (ajouter des activités de ciblage uniquement ? Aucune activité de canal ?) = Crée l&#39;audience et le workflow

## Surveillance et gestion de vos audiences {#monitor}

Dans l&#39;audience créée, le tableau de bord avec deux onglets :
* vue d&#39;ensemble : propriétés + état du workflow et nombre de destinataires dans cette audience en cliquant sur calculer + , vous pouvez accéder au workflow et le modifier à partir de là
* data : affichez les profils de données d’une partie de l’audience. Vous pouvez ajouter de nouvelles colonnes si nécessaire. Voir données enrichies

liste d’audiences : duplication, suppression

**questions :**

Workflow en &quot;mode audience&quot; => envoi des activités de canal non disponibles

* sur l’instance d’évaluation : nous pouvons supprimer la dernière activité qsave et ajouter plutôt une activité de canal
* comment reconnaître un workflow en mode &quot;audience&quot; ?
