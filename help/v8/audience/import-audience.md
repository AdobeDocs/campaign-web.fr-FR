---
audience: end-user
title: Cibler les destinataires à partir d’un fichier
description: Découvrez comment utiliser les destinataires d’un fichier externe pour créer votre audience de courrier électronique
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a6c85aeed30726532ab6060fec5cb4b5e398d9ec
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 37%

---

# Cibler les destinataires à partir d’un fichier {#audience-from-file}

Vous pouvez transférer des contacts depuis un fichier externe. Cette fonctionnalité est uniquement disponible pour les diffusions email. Les formats pris en charge sont les suivants : fichier texte (TXT) ou fichier de valeurs séparées par des virgules (CSV). Ils seront ensuite ajoutés à la base de données.

>[!NOTE]
>
>Vous pouvez créer un workflow d&#39;import pour ajouter ou mettre à jour plusieurs profils.  En savoir plus


Pour cibler des profils à partir d’un fichier local directement à partir de l’interface, procédez comme suit :

1. Dans la fenêtre de création d&#39;une diffusion email, cliquez sur le bouton **Sélection de l’audience** et sélectionnez l’option **Sélectionner dans le fichier** .

   ![](assets/select-from-file.png)

1. Sélectionnez le fichier local à télécharger.
1. Prévisualisez le mappage des données dans la section centrale de l’écran.
1. Sélectionnez la colonne contenant l&#39;adresse email parmi les **Champ d’adresse** menu déroulant.
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
