---
audience: end-user
title: Importer le contenu des e-mails
description: Découvrez comment importer le contenu des e-mails.
exl-id: ef9c8e6f-f422-404e-9ebb-a89d1bd45e7f
badge: label="Disponibilité limitée"
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 100%

---

# Importer le contenu des e-mails {#existing-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_import_content"
>title="Utiliser un contenu d’e-mail existant"
>abstract="Le concepteur d’e-mail permet d’importer du contenu HTML existant. Ce contenu peut être un fichier HTML avec une feuille de style incorporée ou un dossier ZIP contenant le fichier HTML, la feuille de style (CSS) et les images."

Vous pouvez importer du contenu HTML existant dans le concepteur d’e-mail. Ce contenu peut être :

* Un **fichier HTML** avec une feuille de style incorporée,
* Un **dossier ZIP** contenant le fichier HTML, la feuille de style (CSS) et les images.

  >[!NOTE]
  >
  >La structure du fichier ZIP est libre. Toutefois, les références doivent être relatives et adaptées à l’arborescence du dossier ZIP.

Pour importer un fichier contenant du contenu HTML, procédez comme suit :

1. Sur la page d’accueil du [concepteur d’e-mail](get-started-email-designer.md), sélectionnez **[!UICONTROL Importer du contenu HTML]**.

   ![](assets/html-import.png)

1. Faites glisser et déposez le fichier HTML ou ZIP contenant le contenu HTML, puis cliquez sur **[!UICONTROL Importer]**.

1. Le contenu HTML chargé passe en **[!UICONTROL Mode de compatibilité]**.

   Ce mode permet uniquement de personnaliser votre texte, d’ajouter des liens ou d’inclure des ressources à votre contenu.

   ![](assets/html-imported.png)

1. Pour pouvoir exploiter les composants de contenu du concepteur d’e-mail, accédez à l’onglet **[!UICONTROL Convertisseur HTML]** et cliquez sur **[!UICONTROL Convertir]**.

   ![](assets/html-imported-2.png)

   >[!NOTE]
   >
   > L’utilisation d’une balise `<table>` comme premier calque d’un fichier HTML peut entraîner une perte de style, y compris des paramètres d’arrière-plan et de largeur de la balise de calque supérieure.

1. Vous pouvez désormais personnaliser votre fichier importé selon vos besoins à l’aide des fonctionnalités du concepteur d’e-mail. [En savoir plus](content-components.md).

