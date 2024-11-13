---
audience: end-user
title: Utiliser un groupe de recouvrements
description: Découvrez comment utiliser un groupe de recouvrements pour votre diffusion dans l’interface d’utilisation de Campaign Web.
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: ht
source-wordcount: '397'
ht-degree: 100%

---

# Utiliser un groupe de recouvrements {#trap-group}

Un **[!UICONTROL groupe de recouvrements]** (également appelé **[!UICONTROL liste de contrôle]**) est utilisé pour inclure des adresses spécifiques dans vos diffusions afin de surveiller et vérifier le processus de distribution en ciblant les profils qui ne correspondent pas aux critères de ciblage définis. Ainsi, les destinataires qui n’entrent pas dans le cadre de la diffusion peuvent la recevoir, comme tout autre destinataire cible.

Un **[!UICONTROL groupe de recouvrements]** est un groupe **[!UICONTROL d’adresses de contrôle]**, appelé **[!UICONTROL Profil de test]** sur l’interface utilisateur web de Campaign.

## Pourquoi utiliser un groupe de recouvrements ? {#why-trap-group}

Vous pouvez utiliser un **[!UICONTROL groupe de recouvrements]** dans les cas suivants :

1. **En tant qu’épreuve** : chaque personne membre du **[!UICONTROL Groupe de recouvrements]** recevra la diffusion comme si elle faisait partie de l’audience.

1. **Pour protéger votre liste de publipostage** : en recevant ce que l’audience recevra, chaque **[!UICONTROL profil de test]** du **[!UICONTROL groupe de recouvrements]** sera informé si la liste de publipostage est utilisée par un tiers.

>[!NOTE]
>
>Outre [l’envoi d’épreuves lors de la création de la diffusion](../email/create-email.md#preview-test) et depuis [la population témoin](control-group.md), l’ajout d’un groupe de recouvrements est un bon moyen de tester votre audience.

## À propos des groupes de recouvrements {#about-trap-group}

Les profils de test sont automatiquement exclus des rapports sur les statistiques de diffusions suivants : **Clics**, **Ouvertures**, **Désinscriptions**. Les rapports ne portent que sur l’audience réelle.

Pour une diffusion par e-mail, seule l’adresse e-mail est nécessaire pour le **[!UICONTROL groupe de recouvrements]**, la personnalisation des autres champs sera renseignée de manière aléatoire par Campaign.

## Ajouter un groupe de recouvrements à une diffusion {#trap-group-in-delivery}

Pour configurer un **[!UICONTROL groupe de recouvrements]**, accédez aux paramètres **[!UICONTROL Audience]** de votre diffusion. Vous disposez de 2 options :

* [Sélectionner des profils de test](#select-test-profile)
* [Créer une condition](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Sélectionner des profils de test {#select-test-profiles}

Lorsque vous choisissez **Sélectionner les profils de test**, vous pouvez utiliser le bouton **Ajouter un ou plusieurs profils de test** comme illustré ci-dessous :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Lorsque vous cliquez sur le bouton, vous avez accès aux profils de test que vous pouvez ajouter à votre **[!UICONTROL groupe de recouvrements]**. Sélectionnez ceux que vous souhaitez utiliser.

Vous pouvez également créer de nouveaux profils de test. [En savoir plus](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Lorsque vous confirmez vos profils de test, vérifiez que vous disposez du nombre correct sous **[!UICONTROL Groupe de recouvrements]**.

![](assets/trap-check.png){zoomable="yes"}

### Créer une condition {#create-condition}

Avec l’option **[!UICONTROL Créer une condition]**, vous pouvez créer une requête pour définir les profils de test que vous souhaitez utiliser :

![](assets/trap-create-condition.png){zoomable="yes"}

Votre requête s’affiche sous **[!UICONTROL Groupe de recouvrements]**.

![](assets/trap-custom.png){zoomable="yes"}

## Créer un profil de test {#create-seed}

Vous pouvez créer un **[!UICONTROL profil de test]** depuis le dossier **[!UICONTROL Explorateur]** > **[!UICONTROL Ressources]** > **[!UICONTROL Gestion de campagnes]** > **[!UICONTROL Membres de contrôle]**

![](assets/trap-create.png){zoomable="yes"}

Configurez tous les paramètres de votre **[!UICONTROL profil de test]** comme pour n’importe quel profil :

![](assets/trap-create-contact.png){zoomable="yes"}
