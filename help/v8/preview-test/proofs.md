---
audience: end-user
title: Envoyer des BAT
description: Découvrez comment définir et envoyer des messages de BAT
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 045025367a826eece052367be557e47aaf37dc99
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 77%

---

# Envoyer des BAT {#send-proofs}

![](../assets/do-not-localize/badge.png)

L&#39;envoi d&#39;emails de test vous permet de valider votre email et de vérifier différents éléments tels que des liens, des liens d&#39;opt-out et des pages miroir, des images et de détecter d&#39;éventuelles erreurs.

Vous pouvez envoyer des BAT à deux types de destinataires :

* **Profils de test**: envoyer des BAT aux adresses de contrôle, qui sont des destinataires supplémentaires et fictifs dans la base,
* **Profils de substitution** : envoyez des BAT à une adresse e-mail spécifique à l’aide d’un profil existant. Cela permet de vous mettre à la place de l’un des profils ciblés et d’obtenir une représentation exacte du message que le profil recevra.

## Sélectionner les destinataires des BAT {#recipients}

1. Accédez à l’écran de création de contenu d’e-mail, puis cliquez sur **[!UICONTROL Simuler du contenu]**.

1. Cliquez sur le bouton **[!UICONTROL Test]**, puis utilisez la liste déroulante **[!UICONTROL Mode]** pour sélectionner le type de destinataires qui recevra les BAT :

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Envoyer des BAT à des profils de test

1. Choisissez le mode **[!UICONTROL Utiliser des profils de test]**.

1. Ajoutez les profils de test qui recevront les e-mails de test.

   <!--FOR BETA: You can also build an audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.-->

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

Vous pouvez envoyer autant de BAT que nécessaire jusqu’à ce que le contenu de votre diffusion soit finalisé. Une fois cette opération effectuée, vous pouvez envoyer l’e-mail à la cible principale. [Découvrez comment préparer et envoyer des e-mails](../monitor/prepare-send.md).

## Accès aux BAT envoyés {#access-proofs}

Une fois les BAT envoyés, vous pouvez accéder aux journaux dédiés à partir du bouton **[!UICONTROL Afficher le journal des e-mails de test]**. Ces logs permettent d&#39;accéder à tous les BAT envoyés pour la diffusion sélectionnée et de visualiser des statistiques spécifiques relatives à leur envoi.

![](assets/proof-log.png)

Vous pouvez également accéder aux BAT à partir de la liste des diffusions, comme n&#39;importe quelle diffusion.

![](assets/delivery-list.png)
