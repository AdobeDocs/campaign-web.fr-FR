---
audience: end-user
title: Cibler des destinataires à partir d’un fichier
description: Découvrez comment utiliser les destinataires d’un fichier externe pour créer l’audience de vos e-mails.
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 100%

---

# Charger une audience d’e-mail à partir d’un fichier {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Sélection de fichier"
>abstract="Sélectionnez le fichier local à télécharger. Les formats pris en charge sont TXT et CSV. Alignez votre format de fichier sur l’exemple de fichier ci-dessous."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Définition des colonnes"
>abstract="Vérifiez le format des colonnes à insérer à partir de votre fichier local."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Paramètres de formatage"
>abstract="Vérifiez les paramètres de formatage de votre fichier."

Vous pouvez charger des contacts à partir d’un fichier externe. Les profils ne sont pas ajoutés à la base de données, mais tous les champs du fichier d’entrée peuvent être [personnalisés](../personalization/gs-personalization.md). Les formats de fichier pris en charge sont les suivants : texte (TXT) et valeur séparée par des virgules (CSV).

>[!CAUTION]
>
>* Cette fonctionnalité est réservée aux **diffusions e-mail autonomes**. Elle ne peut être utilisée dans les workflows et les diffusions SMS ou Notification push.
>
>* Vous ne pouvez pas utiliser les [populations témoins](control-group.md) lors du chargement de la population cible à partir d’un fichier externe.


Pour cibler des profils à partir d’un fichier local directement dans l’interface e-mail, procédez comme suit :

1. ouvrez une diffusion e-mail existante ou [créez une diffusion e-mail](../email/create-email.md).
1. Dans la fenêtre de création d’une diffusion par e-mail, à partir de la section **Audience**, cliquez sur le bouton **Sélectionner une audience**, puis choisissez l’option **Sélectionner dans un fichier**.

   ![](assets/select-from-file.png)

1. Sélectionnez le fichier local à télécharger. Le format doit correspondre à celui de l’[exemple de fichier](#sample-file).
1. Prévisualisez et vérifiez le mappage des données dans la section centrale de l’écran.
1. Sélectionnez la colonne contenant l’adresse e-mail dans le menu déroulant **Champ d’adresse**. Vous pouvez également sélectionner la colonne de liste bloquée si vous disposez de ces informations dans le fichier d’entrée.
1. Ajustez les paramètres des colonnes et comment formater les données à partir des options disponibles.
1. Cliquez sur **Confirmer** une fois que les paramètres sont corrects.

Lors de la création et de la personnalisation du contenu du message, vous pouvez sélectionner des champs dans le fichier d’entrée de l’[éditeur de personnalisation](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## Exemple de fichier {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Exemple de fichier"
>abstract="Formats de fichiers pris en charge : txt, csv. Utilisez la première ligne comme en-tête de colonne."

Les formats pris en charge sont TXT et CSV. La première ligne correspond à l’en-tête de colonne.

Choisissez le même format de fichier que celui de l’exemple de fichier ci-dessous :

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
