---
audience: end-user
title: Cibler les destinataires à partir d’un fichier
description: Découvrez comment utiliser les destinataires d’un fichier externe pour créer votre audience de courrier électronique
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 7893f3132689446db388613ad5ec033ca5f26bf5
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 23%

---

# Cibler les destinataires à partir d’un fichier {#audience-from-file}

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

Vous pouvez transférer des contacts depuis un fichier externe. Cette fonctionnalité n’est disponible que pour les diffusions email. Les formats de fichiers pris en charge sont les suivants : texte (TXT) et valeur séparée par des virgules (CSV). Les profils ne sont pas ajoutés à la base de données, mais tous les champs du fichier d’entrée peuvent être personnalisés.

>[!NOTE]
>
>Vous pouvez créer un workflow d&#39;import pour ajouter ou mettre à jour plusieurs profils dans la base de données. En savoir plus


Pour cibler des profils à partir d’un fichier local directement à partir de l’interface, procédez comme suit :

1. Dans la fenêtre de création d&#39;une diffusion email, à partir du **Audience** , cliquez sur le bouton **Sélection de l’audience** et choisissez la méthode **Sélectionner dans le fichier** .

   ![](assets/select-from-file.png)

1. Sélectionnez le fichier local à télécharger.
1. Prévisualisez et vérifiez le mappage des données dans la section centrale de l’écran.
1. Sélectionnez la colonne contenant l&#39;adresse email parmi les **Champ d’adresse** menu déroulant. Vous pouvez également sélectionner la colonne liste bloquée si vous disposez de ces informations dans le fichier d’entrée.
1. Ajustez les paramètres des colonnes et comment formater les données à partir des options disponibles.
1. Cliquez sur **Confirmer** une fois que les paramètres sont corrects.

Lors de la création et de la personnalisation du contenu du message, vous pouvez sélectionner des champs dans le fichier d’entrée de l’éditeur de personnalisation.

![](assets/select-external-perso.png)

## Exemple de fichier {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Exemple de fichier"
>abstract="Formats de fichiers pris en charge : txt, csv. Utiliser la première ligne comme en-tête de colonne."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
