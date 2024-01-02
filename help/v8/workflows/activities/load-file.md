---
audience: end-user
title: Utilisation de l’activité de workflow Chargement de fichier
description: Découvrez comment utiliser l’activité de workflow Chargement de fichier
badge: label="Disponibilité limitée"
source-git-commit: 6068e3695ebed22a94a75b9aded59d1e5fb6b47a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 40%

---

# Chargement de fichier  {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Activité Chargement de fichier"
>abstract="La variable **Chargement de fichier** est une activité **Gestion des données** activité. Utilisez cette activité pour travailler avec des profils stockés dans un fichier externe."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Exemple de fichier"
>abstract="Exemple de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nom du fichier"
>abstract="Nom du fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Base de données cible"
>abstract="Base de données cible"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Gestion des rejets pour l’activité Chargement de fichier"
>abstract="Gestion des rejets pour l’activité Chargement de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Transition sortante de la gestion des rejets"
>abstract="Transition sortante de la gestion des rejets"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Transition sortante de la gestion des rejets (pour les rejets)"
>abstract="Transition sortante de la gestion des rejets (pour les rejets)"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Mise en forme de l’activité Chargement de fichier"
>abstract="Mise en forme de l’activité Chargement de fichier"


La variable **Chargement de fichier** est une activité **Gestion des données** activité. Utilisez cette activité pour travailler avec des profils stockés dans un fichier externe. Les profils ne sont pas ajoutés à la base de données, mais tous les champs du fichier d’entrée sont disponibles pour [personnalisation](../../personalization/gs-personalization.md)ou pour mettre à jour des profils.


>[!NOTE]
>Les formats de fichier pris en charge sont les suivants : texte (TXT) et valeur séparée par des virgules (CSV).


Cette activité peut être utilisée avec une [Réconciliation](reconciliation.md) pour lier des données non identifiées à des ressources existantes. Par exemple, la variable **Chargement de fichier** peut être placée avant une activité **Réconciliation** si vous importez des données non standard dans la base de données.


## Configuration de l’activité Chargement de fichier {#load-configuration}

Pour configurer la variable **Chargement de fichier** activité :


1. Faites glisser et déposez un **Chargement de fichier** dans votre workflow. Cliquez sur le bouton **Sélectionner dans le fichier** bouton .
1. Sélectionnez le fichier local à utiliser. Le format doit être aligné avec la variable [exemple de fichier](../../audience/file-audience.md#sample-file).
1. Prévisualisez et vérifiez le mappage des données dans la section centrale de l’écran.
1. Ajustez les paramètres des colonnes et comment formater les données à partir des options disponibles.
1. Cliquez sur **Confirmer** une fois que les paramètres sont corrects.

## Exemple{#load-example}

Un exemple de chargement de fichier externe est disponible avec la fonction **Réconciliation** activité dans [cette section](reconciliation.md#example).