---
audience: end-user
title: Envoyer des e-mails de test
description: Découvrez comment définir et envoyer des e-mails de test.
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: ht
source-wordcount: '537'
ht-degree: 100%

---

# Envoyer des e-mails de test {#send-proofs}

![](../assets/do-not-localize/badge.png)

L’envoi d’e-mails de test est une étape importante pour valider votre campagne par e-mail et identifier les problèmes potentiels. En envoyant des e-mails de test, vous pouvez vérifier différents éléments tels que des liens, des liens de désinscription, des images et des pages miroir, ainsi que détecter d’éventuelles erreurs.

Vous pouvez envoyer des e-mails de test à deux types de destinataires :

* **Profils de test** : envoyez des e-mails de test aux adresses de contrôle, qui sont des destinataires supplémentaires et fictifs dans la base de données. Ils peuvent être créés à l’aide de la console Adobe Campaign dans le dossier **[!UICONTROL Ressources]** / **[!UICONTROL Gestion de campagne]** / **[!UICONTROL Adresses de contrôle]**.

* **Substitution à partir de la cible principale** : envoyez des e-mails de test à une adresse e-mail spécifique lors de l’emprunt de l’identité d’un profil existant. Vous pouvez ainsi tester l’e-mail comme le feraient les destinataires, ce qui vous donne une représentation exacte du message que le profil reçoit.

## Sélectionner les destinataires du test {#recipients}

1. Accédez à l’écran de simulation du contenu d’e-mail, puis cliquez sur le bouton **[!UICONTROL Test]**.

   ![](assets/test-button.png)

1. Utilisez la liste déroulante **[!UICONTROL Mode]** pour sélectionner le type de destinataires de l’e-mail de test :

   * **Profils de test** : envoyez les e-mails de test aux adresses de contrôle, qui sont des destinataires supplémentaires et fictifs dans la base de données.

   * **Substitution à partir de la cible principale** : envoyez l’e-mail de test à une adresse e-mail spécifique lors de l’emprunt de l’identité d’un profil existant. Vous pouvez ainsi tester l’e-mail comme le feraient les destinataires, ce qui vous donne une représentation exacte du message que le profil recevra.

   ![](assets/test-mode.png)

   >[!NOTE]
   >
   >Par défaut, le mode **[!UICONTROL Profils de test]** est sélectionné. Si vous avez déjà sélectionné des profils pour prévisualiser l’e-mail dans l’écran de simulation du contenu, ces profils sont pré-sélectionnés comme destinataires test. Vous pouvez effacer votre sélection et/ou ajouter des destinataires supplémentaires.

1. Pour envoyer des e-mails de test aux profils de substitution, choisissez le mode **[!UICONTROL Substitution à partir de la cible]**, puis procédez comme suit :

   1. Cliquez sur le bouton **[!UICONTROL Ajouter une adresse]** et indiquez l’adresse e-mail qui reçoit l’e-mail de test.

      Vous pouvez indiquer n’importe quelle adresse e-mail. Vous pouvez ainsi envoyer des e-mails de test à n’importe quel(le) utilisateur (utilisatrice), même s’il ne s’agit pas d’un utilisateur ou d’une utilisatrice d’Adobe Campaign v8.

   1. Sélectionnez le profil de la cible à utiliser pour envoyer l’e-mail de test. Vous pouvez également laisser Adobe Campaign sélectionner un profil aléatoire à partir de la cible.

   1. Confirmez le destinataire et renouvelez l’opération pour ajouter autant d’adresses que nécessaire.

      ![](assets/substitution.png)

1. Une fois les destinataires du test sélectionnés, vous pouvez envoyer l’e-mail de test. [Découvrez comment envoyer des e-mails de test](#send).

   >[!NOTE]
   >
   >Si vous souhaitez envoyer l’e-mail final aux destinataires de l’e-mail de test, activez l’option **[!UICONTROL Inclure la population du test dans la cible principale]**.

## Envoyer l’e-mail de test {#send}

Pour envoyer l’e-mail de test aux destinataires sélectionnés, cliquez sur **[!UICONTROL Envoyer un e-mail de test]**, puis confirmez l’envoi.

![](assets/send-proof.png)

Vous pouvez envoyer autant d’e-mails de test que nécessaire jusqu’à ce que le contenu de votre diffusion soit finalisé. Une fois cette opération effectuée, vous pouvez envoyer l’e-mail à la cible principale. [Découvrez comment préparer et envoyer des e-mails](../monitor/prepare-send.md).

## Accéder aux e-mails de test envoyés {#access-proofs}

Une fois les e-mails de test envoyés, vous pouvez accéder aux journaux dédiés à partir du bouton **[!UICONTROL Afficher le journal des e-mails de test]**.

Ces journaux permettent d’accéder à tous les e-mails de test envoyés pour la diffusion sélectionnée et de visualiser des statistiques spécifiques relatives à leur envoi. [Découvrez comment surveiller les logs de diffusion](../monitor/delivery-logs.md).

![](assets/proof-log.png)

Vous pouvez également accéder aux e-mails de test envoyés à partir de la liste des diffusions, comme pour n’importe quelle diffusion.

![](assets/delivery-list.png)
