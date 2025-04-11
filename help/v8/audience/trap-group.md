---
audience: end-user
title: Utiliser un groupe de recouvrements
description: Découvrez comment utiliser un groupe de recouvrements pour votre diffusion dans l’interface d’utilisation de Campaign Web.
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 35%

---

# Utiliser un groupe de recouvrements {#trap-group}

Un **[!UICONTROL groupe de recouvrements]** (également appelé **[!UICONTROL liste de contrôle]**) est utilisé pour inclure des adresses spécifiques dans vos diffusions afin de surveiller et vérifier le processus de distribution en ciblant les profils qui ne correspondent pas aux critères de ciblage définis. Ainsi, les destinataires qui ne sont pas dans le cadre de la diffusion peuvent la recevoir, comme n’importe quel autre destinataire cible.

Un **[!UICONTROL groupe de pièges]** est un groupe d’**[!UICONTROL adresses de contrôle]**, nommé **[!UICONTROL Profil de test]** dans l’interface utilisateur web de Campaign.

## Pourquoi utiliser un groupe de recouvrements ? {#why-trap-group}

Vous pouvez utiliser un **[!UICONTROL groupe de pièges]** :

1. **Comme un bon à tirer** : chaque membre du groupe **[!UICONTROL piège]** reçoit la diffusion comme s’il faisait partie de l’audience.

1. **Pour protéger votre liste de diffusion** : en recevant ce que l’audience recevra, chaque **[!UICONTROL profil de test]** du groupe **[!UICONTROL piège]** sera remarqué si la liste de diffusion est utilisée par un tiers.

>[!NOTE]
>
>Outre [l’envoi d’épreuves lors de la création de la diffusion](../email/create-email.md#preview-test) et depuis [la population témoin](control-group.md), l’ajout d’un groupe de recouvrements est un bon moyen de tester votre audience.

## À propos des groupes de recouvrements {#about-trap-group}

Les profils de test sont automatiquement exclus des rapports sur les statistiques de diffusions suivants : **Clics**, **Ouvertures**, **Désinscriptions**. Les rapports se concentrent uniquement sur l’audience réelle.

Pour une diffusion par e-mail, seule l’adresse e-mail est requise pour le **[!UICONTROL groupe de pièges]**. La personnalisation des autres champs est renseignée de manière aléatoire par Campaign.

## Ajouter un groupe de recouvrements à une diffusion {#trap-group-in-delivery}

Pour configurer un **[!UICONTROL groupe d’interruptions]**, accédez aux paramètres **[!UICONTROL Audience]** de votre diffusion. Deux options s’offrent à vous :

* [Sélectionner des profils de test](#select-test-profiles)
* [Créer une condition](#create-condition)

[Capture d’écran de l’interface des paramètres du groupe de pièges](assets/trap-group.png){zoomable="yes"}

### Sélectionner des profils de test {#select-test-profiles}

Lorsque vous choisissez **Sélectionner des profils de test**, utilisez le bouton **Ajouter un ou plusieurs profils de test** comme illustré ci-dessous :

[Capture d’écran du bouton Ajouter un profil de test](assets/trap-no-test-profile.png){zoomable="yes"}

Lorsque vous cliquez sur le bouton, vous pouvez accéder aux profils de test à ajouter à votre **[!UICONTROL groupe de pièges]**. Sélectionnez ceux que vous souhaitez utiliser.

Vous pouvez également créer de nouveaux profils de test. [En savoir plus](#create-seed)

[Capture d’écran de l’interface des profils de test](assets/trap-select-test-profiles.png){zoomable="yes"}

Après avoir confirmé vos profils de test, vérifiez que le nombre correct apparaît sous **[!UICONTROL Groupe de pièges]**.

[Capture d’écran de confirmation du groupe de pièges](assets/trap-check.png){zoomable="yes"}

### Créer une condition {#create-condition}

Avec l’option **[!UICONTROL Créer une condition]**, créez une requête pour définir les profils de test à utiliser :

[Capture d’écran de l’interface Créer une condition](assets/trap-create-condition.png){zoomable="yes"}

Votre requête s’affiche sous **[!UICONTROL Groupe de recouvrements]**.

[Capture d’écran d’affichage des requêtes de groupe de pièges](assets/trap-custom.png){zoomable="yes"}

## Créer un profil de test {#create-seed}

Vous pouvez créer un nouveau **[!UICONTROL profil de test]** à partir du dossier **[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Gestion de campagne]** > **[!UICONTROL Membres de contrôle]**.

[Création d’une capture d’écran de navigation du profil de test](assets/trap-create.png){zoomable="yes"}

Configurez tous les paramètres de votre **[!UICONTROL profil de test]** comme vous le feriez pour n’importe quel profil :

[Capture d’écran de la configuration du profil de test](assets/trap-create-contact.png){zoomable="yes"}