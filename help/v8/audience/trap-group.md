---
audience: end-user
title: Utilisation d’un groupe de type piège
hide: true
hidefromtoc: true
description: Découvrez comment utiliser un groupe de pièges pour votre diffusion dans l'interface utilisateur web de Campaign
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 3%

---

# Utilisez une **[!UICONTROL groupe de pièges]** {#trap-group}

A **[!UICONTROL groupe de pièges]** est utilisé pour cibler les destinataires qui ne correspondent pas aux critères de ciblage définis. Ainsi, les destinataires qui ne sont pas compris dans la portée de la diffusion peuvent recevoir la diffusion, comme le ferait tout autre destinataire cible.
A **[!UICONTROL groupe de pièges]** est un groupe de **[!UICONTROL adresses de contrôle]**.

## Pourquoi utiliser **[!UICONTROL groupe de pièges]**

Vous pouvez utiliser **[!UICONTROL groupe de pièges]** :

1. **Comme preuve** : chaque membre du **[!UICONTROL Groupe de pièges]** recevra la diffusion comme si elle faisait partie de l’audience.


1. **Pour protéger votre liste de messagerie** : en recevant ce que l’audience recevra, chaque **[!UICONTROL adresse de contrôle]** de **[!UICONTROL Groupe de pièges]** sera remarqué si la liste de distribution est utilisée par un tiers.

## A propos **[!UICONTROL Groupe de pièges]**

Les adresses de contrôle sont automatiquement exclues des rapports sur les statistiques de diffusion suivantes : **Clics**, **Ouvertures**, **Désabonnements**. Les rapports ne portent que sur le public réel.

Pour une diffusion par email, seule l’adresse email est nécessaire pour la variable **[!UICONTROL Groupe de pièges]**, la personnalisation des autres champs sera renseignée de manière aléatoire par Campaign.

## Configuration d’une **[!UICONTROL Groupe de pièges]** dans la diffusion

Pour configurer une **[!UICONTROL Groupe de pièges]**, accédez au **[!UICONTROL Audience]** des paramètres de votre diffusion. Vous disposez de 2 options :
- [Sélectionner des profils de test](#select-test-profile)
- [Créer une condition](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Sélectionner des profils de test {#select-test-profiles}

Lorsque vous sélectionnez &quot;Sélectionner les profils de test&quot;, la fenêtre ci-dessous vous invite à **[!UICONTROL Ajouter un ou plusieurs profils de test]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Lorsque vous cliquez sur le bouton, vous avez accès aux adresses de contrôle que vous pouvez ajouter à votre **[!UICONTROL groupe de pièges]**. Cochez ceux que vous souhaitez utiliser.
Vous pouvez créer de nouvelles adresses de contrôle. [En savoir plus](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Lorsque vous confirmez vos adresses de piège, vérifiez que vous disposez du nombre correct sous **[!UICONTROL Groupe de pièges]**.

![](assets/trap-check.png){zoomable="yes"}

### Créer une condition {#create-condition}

Avec la variable **[!UICONTROL Création d’une condition]** vous obtiendrez alors une nouvelle fenêtre dans laquelle vous pourrez personnaliser une requête afin de définir les adresses de contrôle à utiliser :

![](assets/trap-create-condition.png){zoomable="yes"}

Votre requête s’affiche sous **[!UICONTROL Groupe de pièges]**.

![](assets/trap-custom.png){zoomable="yes"}

## Comment créer une nouvelle **[!UICONTROL adresse de contrôle]** {#create-seed}

Vous pouvez créer une **[!UICONTROL adresse de contrôle]** in **[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Membres de l’adresse de contrôle]**

![](assets/trap-create.png){zoomable="yes"}

Vous pouvez renseigner tous les détails sur votre membre de contrôle comme s’il s’agissait d’un profil d’audience :

![](assets/trap-create-contact.png){zoomable="yes"}