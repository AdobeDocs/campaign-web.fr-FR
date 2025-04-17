---
audience: end-user
title: Gérer la marque
description: Découvrir comment créer et gérer vos directives de marque
hide: true
hidefromtoc: true
badge: label="Version bêta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 40%

---

# Créer et gérer vos marques {#brands}

>[!AVAILABILITY]
>
>Cette fonctionnalité est publiée sous la forme d’une version Private Beta. Elle sera progressivement disponible pour tous les clients dans les prochaines versions.

Les directives de marque sont un ensemble complet de règles et de normes qui définissent l’identité visuelle et verbale d’une marque. Elles servent de référence pour homogénéiser la représentation de la marque sur tous les canaux de marketing et de communication.

Dans [!DNL Adobe Campaign Web], les utilisateurs peuvent saisir et organiser manuellement des informations sur la marque ou charger des documents de directives sur la marque pour une extraction automatique des données.

## Accéder aux marques {#generative-access}

Pour accéder au menu **[!UICONTROL Marques]** dans [!DNL Adobe Campaign Web], les utilisateurs doivent disposer des profils de produit **[!UICONTROL Administrateur (administrateur)]** et **[!UICONTROL Kit de marque]** pour créer et gérer des marques. Pour un accès en lecture seule, les utilisateurs ont besoin du profil de produit [!UICONTROL assistant IA].

[En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Découvrez comment attribuer des autorisations liées à la marque

1. Accédez à votre produit Campaign sur la page d’accueil [Admin Console](https://adminconsole.adobe.com/enterprise).

   ![Page d’accueil Admin Console montrant l’accès au produit Campaign](assets/brands_admin_1.png)

1. Sélectionnez le **[!DNL Product profile]** en fonction du niveau d’autorisations que vous souhaitez accorder à votre utilisateur.

   ![Sélection du profil de produit dans Admin Console](assets/brands_admin_2.png)

1. Cliquez sur **[!DNL Add users]** pour attribuer le profil de produit sélectionné.

   ![Option Ajouter des utilisateurs dans Admin Console](assets/brands_admin_3.png)

1. Saisissez le nom, le groupe d’utilisateurs ou l’adresse e-mail de votre utilisateur.

1. Cliquez sur **Enregistrer** pour appliquer les changements.

Les utilisateurs et utilisatrices déjà affectés à ce rôle voient leurs autorisations automatiquement mises à jour.

+++

## Créer votre marque {#create-brand-kit}

Pour créer et configurer vos directives de marque, suivez les étapes indiquées ci-dessous.

Les utilisateurs peuvent saisir les détails manuellement ou charger un document de directives de marque pour extraire automatiquement les informations :

1. Dans le menu **[!UICONTROL Gestion de contenu]**, sélectionnez **[!UICONTROL Marques]**.

1. Dans le menu **[!UICONTROL Marques]**, cliquez sur **[!UICONTROL Créer une marque]**.

   ![Menu Marques avec l’option Créer une marque](assets/brands_1.png)

1. Saisissez le **[!UICONTROL nom]** de votre marque.

1. Effectuez un glisser-déposer ou sélectionnez votre fichier pour charger vos directives de marque et extraire automatiquement les informations de marque pertinentes. Cliquez sur **[!UICONTROL Créer une marque]**.

   Le processus d’extraction des informations commence. Notez que cette opération peut prendre plusieurs minutes.

   ![Chargement de fichier pour l’extraction des directives de la marque](assets/brands_7.png)

1. Vos normes de création visuelle et de contenu sont automatiquement renseignées. Parcourez les différents onglets pour adapter les informations selon vos besoins.

1. Dans l’onglet **[!UICONTROL Style d’écriture]**, cliquez sur ![Ajouter une icône](assets/do-not-localize/Smock_Add_18_N.svg) pour ajouter une instruction ou une exclusion, ainsi que des exemples.

   ![Onglet Style d’écriture avec l’option Ajouter une règle](assets/brands_2.png)

1. Dans l’onglet **[!UICONTROL Contenu visuel]**, cliquez sur ![Ajouter une icône](assets/do-not-localize/Smock_Add_18_N.svg) pour ajouter une autre directive ou exclusion.

1. Pour ajouter une image présentant une utilisation correcte, sélectionnez **[!UICONTROL Exemples]** et cliquez sur **[!UICONTROL Sélectionner une image]**. Vous pouvez également ajouter une image montrant une utilisation incorrecte comme exemple d’action à ne pas faire.

   ![Onglet Contenu visuel avec des exemples d’options d’image](assets/brands_3.png)

1. Une fois la configuration effectuée, cliquez sur **[!UICONTROL Enregistrer]**, puis sur **[!UICONTROL Publier]** pour mettre à disposition vos directives de marque dans l’assistant IA.

1. Pour modifier la marque publiée, cliquez sur **[!UICONTROL Modifier la marque]**.

   >[!NOTE]
   >
   >Cela crée une copie temporaire en mode d’édition, qui remplace la version active une fois publiée.

   ![Option Modifier la marque dans le menu Marques](assets/brands_4.png)

1. Dans le tableau de bord **[!UICONTROL Marques]**, ouvrez le menu avancé en cliquant sur l’icône ![Plus d’options](assets/do-not-localize/Smock_More_18_N.svg) pour :

   * Afficher la marque
   * Modifier
   * Dupliquer
   * Publier
   * Dépublier
   * Supprimer

   ![Options de menu avancées dans le tableau de bord Marques](assets/brands_5.png)

Vos directives de marque sont désormais accessibles à partir du menu déroulant **[!UICONTROL Marque]** dans le menu de l’assistant d’IA. Cela permet à l’assistant d’IA de générer du contenu et des ressources alignés sur vos spécifications. [En savoir plus sur l’assistant IA](../email/generative-gs.md)

![Menu assistant AI avec liste déroulante Marque](assets/brands_6.png)