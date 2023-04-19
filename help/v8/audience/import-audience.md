---
audience: end-user
title: Importer des destinataires à partir d’un fichier
description: Découvrez comment importer des destinataires à partir d’un fichier externe.
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f103fe804deccc83638a3e56a03f6e715e68e550
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 96%

---

# Importer des destinataires à partir d’un fichier {#audience-from-file}

Vous pouvez ajouter ou mettre à jour des contacts dans l’interface de diffusion. Il vous suffit de télécharger un fichier texte (TXT) ou un fichier avec des valeurs séparées par des virgules (CSV). Ils seront ensuite ajoutés à la base de données.

>[!NOTE]
>
>Vous pouvez également créer un workflow d’importation pour ajouter ou mettre à jour plusieurs profils.


Pour ajouter des profils à partir d’un fichier local directement dans l’interface, procédez comme suit :

1. Dans la fenêtre de création de la diffusion, cliquez sur le bouton **Sélectionner une audience**, puis sur l’option **Sélectionner dans un fichier**.
1. Sélectionnez le fichier local à télécharger.
1. Définissez les paramètres des colonnes et de format des données. Vous pouvez ignorer une colonne à l’aide du bouton (bascule) **Ignorer la colonne**.
1. Prévisualisez le mappage des données dans la section centrale de l’écran.
1. Cliquez sur **Confirmer** une fois que les paramètres sont corrects.

Lors de la création et de la personnalisation du contenu du message, vous pouvez sélectionner des champs dans le fichier d’entrée de l’éditeur de personnalisation.

## Exemple de fichier {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Exemple de fichier"
>abstract="Formats de fichiers pris en charge : txt, csv, xls. Utiliser la première ligne comme titre des colonnes."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
