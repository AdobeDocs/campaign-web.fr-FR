---
audience: end-user
title: Valider des messages transactionnels
description: Découvrir comment valider un message transactionnel dans l’interface d’utilisation de Campaign Web
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: bca2b133968d9392098e9b8b76d65e44d7e84645
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 100%

---

# Valider des messages transactionnels

Pendant ou après la création de votre message transactionnel, vous pouvez valider le contenu à l’aide d’un exemple de données.

## Simuler le contenu {#simulate-content}

Pour simuler le contenu de votre message, procédez comme suit :

* Assurez-vous que le chemin de personnalisation dans le contenu de votre message correspond à votre exemple de contexte. Dans l’exemple ci-dessous, pour afficher le prénom du profil de test, nous utilisons le chemin *rtEvent.ctx.basicDetails.firstName*.

  Vous pouvez modifier le contenu du message ou l’exemple de contexte pour les faire correspondre.

  ![](assets/validate-verification.png){zoomable="yes"}

* Cliquez sur le bouton **[!UICONTROL Simuler le contenu]** pour prévisualiser votre message transactionnel avec les données que vous avez saisies dans l’exemple de contexte.

  ![](assets/validate-simulate.png){zoomable="yes"}

  Après avoir vérifié votre contenu, cliquez sur le bouton **[!UICONTROL Fermer]**.

* N’oubliez pas de cliquer sur le bouton **[!UICONTROL Republier]** si vous avez apporté des modifications à votre contenu.

## Envoyer un BAT

Si vous souhaitez tester et expérimenter le message transactionnel tel qu’il serait diffusé via le canal de votre choix (e-mail, SMS ou notification push, par exemple), vous pouvez utiliser la fonctionnalité de BAT.

Dans la [fenêtre de contenu de la simulation](#simulate-content), cliquez sur le bouton **[!UICONTROL Envoyer un BAT]**.

![](assets/transactional-proof.png){zoomable="yes"}

Dans la nouvelle fenêtre qui s’affiche, saisissez l’adresse e-mail (ou le numéro de téléphone, selon le canal) où vous souhaitez recevoir le BAT. Une fois que vous avez saisi l’adresse souhaitée, cliquez sur les boutons **[!UICONTROL Envoyer un BAT]** et **[!UICONTROL Confirmer]**. Cette action vous permet d’envoyer un exemple de votre message transactionnel, en vous assurant que l’ensemble des personnalisations, du contenu dynamique et de la mise en forme s’affichent comme ils le devraient pour vos utilisateurs et utilisatrices finaux.

![](assets/transactional-sendproof.png){zoomable="yes"}

Il s’agit d’une étape essentielle pour identifier les problèmes potentiels avant de publier votre message transactionnel.
