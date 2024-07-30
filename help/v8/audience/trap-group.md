---
audience: end-user
title: Utiliser un groupe de recouvrements
description: Découvrez comment utiliser un groupe de recouvrements pour votre diffusion dans l’interface d’utilisation de Campaign Web.
source-git-commit: 39dcf11797339ee9800da6c5a32b1a1c3470529a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 29%

---

# Utiliser un groupe de recouvrements {#trap-group}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Groupe de recouvrements"
>abstract="Vous pouvez utiliser un groupe de pièges pour inclure des adresses spécifiques dans vos diffusions afin de surveiller et vérifier le processus de distribution en ciblant les profils qui ne correspondent pas aux critères de ciblage définis."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

Un **[!UICONTROL groupe de pièges]** (également appelé **[!UICONTROL liste de contrôle]**) est utilisé pour inclure des adresses spécifiques dans vos diffusions afin de surveiller et vérifier le processus de distribution en ciblant les profils qui ne correspondent pas aux critères de cible définis. Ainsi, les destinataires qui n’entrent pas dans le cadre de la diffusion peuvent la recevoir, comme tout autre destinataire cible.

Un **[!UICONTROL groupe de pièges]** est un groupe **[!UICONTROL d’adresses de contrôle]**, appelé **[!UICONTROL Profil de test]** sur l’interface utilisateur web de Campaign.

## Pourquoi utiliser un groupe de pièges {#why-trap-group}

Vous pouvez utiliser **[!UICONTROL trap group]** :

1. **En tant que BAT** : chaque membre du **[!UICONTROL groupe Piège]** recevra la diffusion comme s’il faisait partie de l’audience.

1. **Pour protéger votre liste de distribution** : en recevant ce que l’audience recevra, chaque **[!UICONTROL profil de test]** du **[!UICONTROL groupe de pièges]** sera remarqué si la liste de distribution est utilisée par un tiers.

>[!NOTE]
>
>Outre [l&#39;envoi de BAT lors de la création de la diffusion](../email/create-email.md#preview-test) et depuis [la population témoin](control-group.md), l&#39;ajout d&#39;un groupe de type piège est un bon moyen de tester votre audience.

## À propos des groupes de pièges {#about-trap-group}

Les profils de test sont automatiquement exclus des rapports sur les statistiques de diffusions suivants : **Clics**, **Ouvertures**, **Désinscriptions**. Les rapports ne portent que sur l’audience réelle.

Pour une diffusion par e-mail, seule l’adresse e-mail est nécessaire pour le **[!UICONTROL groupe de recouvrements]**, la personnalisation des autres champs sera renseignée de manière aléatoire par Campaign.

## Ajout d’un groupe Piège dans une diffusion {#trap-group-in-delivery}

Pour configurer un **[!UICONTROL groupe de recouvrements]**, accédez aux paramètres **[!UICONTROL Audience]** de votre diffusion. Vous disposez de 2 options :

* [Sélectionner des profils de test](#select-test-profile)
* [Créer une condition](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Sélectionner des profils de test {#select-test-profiles}

Lorsque vous choisissez **Sélectionner les profils de test**, vous pouvez utiliser le bouton **Ajouter un ou plusieurs profils de test** comme illustré ci-dessous :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Lorsque vous cliquez sur le bouton, vous avez accès aux profils de test que vous pouvez ajouter à votre **[!UICONTROL groupe de pièges]**. Sélectionnez ceux que vous souhaitez utiliser.

Vous pouvez également créer de nouveaux profils de test. [En savoir plus](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Lorsque vous confirmez vos profils de test, vérifiez que vous avez le nombre correct sous **[!UICONTROL Groupe de pièges]**.

![](assets/trap-check.png){zoomable="yes"}

### Créer une condition {#create-condition}

Avec l’option **[!UICONTROL Créer une condition]** , vous pouvez créer une requête pour définir les profils de test que vous souhaitez utiliser :

![](assets/trap-create-condition.png){zoomable="yes"}

Votre requête est affichée sous **[!UICONTROL Groupe de pièges]**.

![](assets/trap-custom.png){zoomable="yes"}

## Création d’un profil de test {#create-seed}

Vous pouvez créer un **[!UICONTROL profil de test]** à partir du dossier **[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Membres de l&#39;adresse]**.

![](assets/trap-create.png){zoomable="yes"}

Configurez tous les paramètres de votre **[!UICONTROL profil de test]** comme pour n’importe quel profil :

![](assets/trap-create-contact.png){zoomable="yes"}