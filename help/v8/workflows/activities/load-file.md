---
audience: end-user
title: Utiliser l’activité de workflow Chargement de fichier
description: Découvrez comment utiliser l’activité de workflow Chargement de fichier.
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 86%

---

# Chargement de fichier {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Activité Chargement de fichier"
>abstract="L’activité **Chargement de fichier** est une activité de **Data Management**. Elle vous permet d’utiliser les données stockées dans un fichier externe."

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

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Fichier cible pour l’activité Chargement de fichier"
>abstract="Fichier cible pour l’activité Chargement de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Remappage de valeurs pour l’activité Chargement de fichier"
>abstract="Remappage de valeurs pour l’activité Chargement de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Load File Commande"
>abstract="Autoriser une commande arbitraire pour le prétraitement est un problème de sécurité. Désactivez l’option de sécurité XtkSecurity_Disable_Preproc pour forcer l’utilisation d’une liste prédéfinie de commandes."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Supprimer le fichier après l&#39;import"
>abstract="TBC"

L’activité **Chargement de fichier** est une activité de **Data Management**. Utilisez-la lorsque vous travaillez avec des profils et des données stockés dans un fichier externe. Les profils et les données ne sont pas ajoutés à la base de données, mais tous les champs du fichier d’entrée sont disponibles pour la [personnalisation](../../personalization/gs-personalization.md) ou la mise à jour des profils ou des tables.

>[!NOTE]
>Les formats de fichier pris en charge sont les suivants : texte (TXT) et valeur séparée par des virgules (CSV).

Combinée avec l’activité [Réconciliation](reconciliation.md), elle permet de lier des données non identifiées à des ressources existantes. L’activité **Chargement de fichier** peut par exemple être placée après une activité de **Réconciliation** si vous importez des données non standard dans la base de données.

## Configurer l’activité Chargement de fichier {#load-configuration}

Pour configurer l’activité **Chargement de fichier**, procédez comme suit :

1. Placez une activité **Chargement de fichier** dans votre workflow. Cliquez sur le bouton **Sélectionner à partir du fichier**.

1. Sélectionnez le fichier local à utiliser. Le format doit correspondre à celui de l’[exemple de fichier](../../audience/file-audience.md#sample-file).

1. Prévisualisez et vérifiez le mappage des données dans la section centrale de l’écran.

   ![](../assets/load-file.png)

1. Utilisez la section **Colonnes** dans le volet de gauche pour ajuster le type et la largeur des données pour chaque colonne.

1. Dans la section **Formatage**, située sous la configuration des colonnes, indiquez le format du fichier externe pour vous assurer que les données sont correctement importées.

1. Cliquez sur **Confirmer** une fois que les paramètres sont corrects.

## Exemple{#load-example}

Un exemple de chargement de fichier externe est disponible avec l’activité **Réconciliation** dans [cette section](reconciliation.md#reconciliation-example).
