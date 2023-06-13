---
audience: end-user
title: Cibler des destinataires à partir d’un fichier
description: Découvrez comment utiliser les destinataires d’un fichier externe pour créer l’audience de vos e-mails.
badge: label="Alpha"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 64%

---

# Chargement d’une audience de courrier électronique à partir d’un fichier {#audience-from-file}

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

Vous pouvez charger des contacts à partir d’un fichier externe. Les profils ne sont pas ajoutés à la base de données, mais tous les champs du fichier d’entrée sont disponibles pour [personnalisation](../personalization/gs-personalization.md). Les formats de fichier pris en charge sont les suivants : texte (TXT) et valeur séparée par des virgules (CSV).

>[!CAUTION]
>
>* Cette fonctionnalité n’est disponible que pour **diffusions email autonomes**. Il ne peut pas être utilisé dans les workflows, ni avec les diffusions SMS ou push.
>
>* Vous ne pouvez pas utiliser les [populations témoins](control-group.md) lors du chargement de la population cible à partir d’un fichier externe.


Pour cibler des profils à partir d&#39;un fichier local directement depuis l&#39;interface de messagerie, procédez comme suit :

1. Ouvrez une diffusion email existante, ou [créer une diffusion email](../email/create-email.md).
1. Dans la fenêtre de création d’une diffusion par e-mail, à partir de la section **Audience**, cliquez sur le bouton **Sélectionner une audience**, puis choisissez l’option **Sélectionner dans un fichier**.

   ![](assets/select-from-file.png)

1. Sélectionnez le fichier local à télécharger. Le format doit s’aligner sur la variable [exemple de fichier](#sample-file).
1. Prévisualisez et vérifiez le mappage des données dans la section centrale de l’écran.
1. Sélectionnez la colonne contenant l’adresse e-mail dans le menu déroulant **Champ d’adresse**. Vous pouvez également sélectionner la colonne de liste bloquée si vous disposez de ces informations dans le fichier d’entrée.
1. Ajustez les paramètres des colonnes et comment formater les données à partir des options disponibles.
1. Cliquez sur **Confirmer** une fois que les paramètres sont corrects.

Lors de la création et de la personnalisation du contenu du message, vous pouvez sélectionner des champs dans le fichier d&#39;entrée du [Éditeur de personnalisation](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## Exemple de fichier {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Exemple de fichier"
>abstract="Formats de fichiers pris en charge : txt, csv. Utilisez la première ligne comme en-tête de colonne."

Les formats pris en charge sont TXT et CSV. La première ligne correspond à l’en-tête de colonne.

Alignez votre format de fichier sur l’exemple de fichier ci-dessous :

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
