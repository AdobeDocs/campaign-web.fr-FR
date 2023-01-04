---
audience: end-user
title: Envoyer des BAT
description: Documentation de l’application web de Campaign v8
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 28cada1d6b645bd6f0c365528c9302bf4b03ad65
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 100%

---

# Envoyer des BAT {#send-proofs}

>[!NOTE]
>
>Cette documentation est en cours d’élaboration et est fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

L’envoi de BAT vous permet de valider l’e-mail et de vérifier différents éléments tels que des liens, des liens de désinscription, des pages miroir et des images, et de détecter d’éventuelles erreurs.

Vous pouvez envoyer des BAT à deux types de destinataires :

* **Profils/audiences de test** : envoyez des BAT aux adresses de contrôle, qui sont des destinataires supplémentaires de la base qui ne font pas partie de la cible de l’e-mail,

* **Profils de substitution** : envoyez des BAT à une adresse e-mail spécifique à l’aide d’un profil existant. Cela permet de vous mettre à la place de l’un des profils ciblés et d’obtenir une représentation exacte du message que le profil recevra.

## Sélectionner les destinataires des BAT {#recipients}

1. Accédez à l’écran de création de contenu d’e-mail, puis cliquez sur **[!UICONTROL Simuler du contenu]**.

1. Cliquez sur le bouton **[!UICONTROL Test]**, puis utilisez la liste déroulante **[!UICONTROL Mode]** pour sélectionner le type de destinataires qui recevra les BAT :

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Envoyer des BAT à des profils de test

1. Choisissez le mode **[!UICONTROL Utiliser des profils de test]**.

1. Ajoutez les profils de test qui recevront les e-mails de test.

   Vous pouvez également créer une audience pour sélectionner des profils de test en fonction de vos propres critères à l’aide du bouton **[!UICONTROL Ajouter une audience de test]**.

   ![](assets/test-profiles-audience.png)

### Envoyer des BAT aux profils de substitution

1. Sélectionnez le mode **[!UICONTROL Substitution de la cible]**.

1. Ajoutez la ou les adresses e-mail qui recevront les BAT.

   >[!NOTE]
   >
   >Vous pouvez indiquer n’importe quelle adresse e-mail. Vous pouvez ainsi envoyer des BAT à n’importe quel utilisateur ou utilisatrice, même s’il ne s’agit pas d’un utilisateur ou d’une utilisatrice d’Adobe Campaign V8.

1. Pour chaque adresse e-mail, sélectionnez le profil à partir de la cible à utiliser. Vous pouvez également laisser Adobe Campaign sélectionner un profil aléatoire à partir de la cible.

   ![](assets/substitution.png)

Une fois les destinataires du BAT sélectionnés, vous pouvez envoyer l’e-mail de test. [Découvrez comment envoyer des BAT](#send)

>[!NOTE]
>
>Si vous souhaitez envoyer l’e-mail final aux destinataires des BAT, activez l’option **[!UICONTROL Inclure la population test dans la cible principale]**.

## Envoyer les BAT {#send}

Pour envoyer les BAT aux destinataires sélectionné(e)s, cliquez sur **[!UICONTROL Envoyer un e-mail de test]**, puis confirmez l’envoi.

![](assets/send-proof.png)

Une fois les BAT envoyés, vous pouvez accéder aux journaux dédiés à partir du bouton **[!UICONTROL Afficher le journal des e-mails de test]**. Ces journaux permettent d’accéder aux BAT envoyés et aux statistiques relatives à l’envoi du BAT.

![](assets/proof-log.png)

Vous pouvez envoyer autant de BAT que nécessaire jusqu’à ce que le contenu de votre diffusion soit finalisé. Une fois cette opération effectuée, vous pouvez envoyer l’e-mail à la cible principale. [Découvrez comment préparer et envoyer des e-mails](../monitor/prepare-send.md).
