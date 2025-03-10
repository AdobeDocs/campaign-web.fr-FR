---
audience: end-user
title: Gérer la marque
description: Découvrez comment créer et gérer vos directives de marque.
hide: true
hidefromtoc: true
badge: label="Version bêta" type="Informative"
source-git-commit: 4baa86395b3cbd062d641ea53ef337523bc7772d
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 2%

---

# Créer et gérer vos marques {#brands}

>[!AVAILABILITY]
>
>Cette fonctionnalité est disponible en version bêta privée. Elle sera progressivement disponible pour tous les clients dans les prochaines versions.

Les directives sur les marques sont un ensemble complet de règles et de normes qui définissent l&#39;identité visuelle et verbale d&#39;une marque. Ils servent de référence pour assurer une représentation cohérente de la marque sur tous les canaux de marketing et de communication.

Dans [!DNL Adobe Campaign Web], vous pouvez désormais saisir et organiser manuellement vos informations de marque ou charger des documents de directives de marque pour une extraction de données automatique.

## Accéder aux marques {#generative-access}

Pour accéder au menu **[!UICONTROL Marques]** dans [!DNL Adobe Campaign Web], les utilisateurs doivent disposer des profils de produit **[!UICONTROL Administrateur (administrateur)]** et **[!UICONTROL Kit de marque]** pour créer et gérer des marques. Pour un accès en lecture seule, les utilisateurs ont besoin d’un profil de produit [!UICONTROL assistant IA].

[En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++  Découvrez comment attribuer des autorisations liées à la marque

1. Accédez à votre produit Campaign sur la page d’accueil [Admin Console](https://adminconsole.adobe.com/enterprise).

   ![](assets/brands_admin_1.png)

1. Sélectionnez le **[!DNL Product profile]** en fonction du niveau d’autorisations que vous souhaitez accorder à votre utilisateur.

   ![](assets/brands_admin_2.png)

1. Cliquez sur **[!DNL Add users]** pour attribuer le profil de produit sélectionné.

   ![](assets/brands_admin_3.png)

1. Saisissez le nom, le groupe d’utilisateurs ou l’adresse e-mail de votre utilisateur.

1. Cliquez sur **Enregistrer** pour appliquer les modifications.

Les autorisations de tous les utilisateurs et utilisatrices déjà affectés à ce rôle seront automatiquement mises à jour.

+++

## Création de votre marque {#create-brand-kit}

Pour créer et gérer vos directives de marque, procédez comme suit.

Pour créer et gérer vos directives de marque, vous pouvez saisir vous-même les détails ou charger votre document de directives de marque pour que les informations soient extraites automatiquement :


1. Dans le menu **[!UICONTROL Gestion de contenu]**, sélectionnez **[!UICONTROL Marques]**.

1. Dans le menu **[!UICONTROL Marques]**, cliquez sur **[!UICONTROL Créer une marque]**.

   ![](assets/brands_1.png)

1. Saisissez un **[!UICONTROL Nom]** pour votre marque.

1. Effectuez un glisser-déposer ou sélectionnez votre fichier pour charger les directives de votre marque et extraire automatiquement les informations pertinentes sur la marque. Cliquez sur **[!UICONTROL Créer une marque]**.

   Le processus d’extraction des informations commence maintenant. Notez que cette opération peut prendre plusieurs minutes.

   ![](assets/brands_7.png)

1. Vos normes de création visuelle et de contenu sont désormais automatiquement renseignées. Parcourez les différents onglets pour adapter les informations selon vos besoins.

1. Dans l’onglet **[!UICONTROL Style d’écriture]**, cliquez sur ![](assets/do-not-localize/Smock_Add_18_N.svg) pour ajouter une instruction ou une exclusion, ainsi que des exemples.

   ![](assets/brands_2.png)

1. Dans l’onglet **[!UICONTROL Contenu visuel]**, cliquez sur ![](assets/do-not-localize/Smock_Add_18_N.svg) pour ajouter une autre directive ou exclusion.

1. Pour ajouter une image montrant une utilisation correcte, sélectionnez **[!UICONTROL Exemples]** et cliquez sur **[!UICONTROL Sélectionner une image]**. Vous pouvez également ajouter une image montrant une utilisation incorrecte comme exemple d’exclusion.

   ![](assets/brands_3.png)

1. Une fois la configuration effectuée, cliquez sur **[!UICONTROL Enregistrer]** puis **[!UICONTROL Publier]** pour rendre vos directives de marque disponibles dans l’assistant d’IA.

1. Pour apporter des modifications à votre marque publiée, cliquez sur **[!UICONTROL Modifier la marque]**.

   >[!NOTE]
   >
   >Cela crée une copie temporaire en mode d’édition, qui remplace la version active une fois publiée.

   ![](assets/brands_4.png)

1. Dans le tableau de bord **[!UICONTROL Marques]**, ouvrez le menu avancé en cliquant sur l’icône ![](assets/do-not-localize/Smock_More_18_N.svg) pour :

   * Afficher la marque
   * Modifier
   * Dupliquer
   * Publier
   * Dépublier
   * Supprimer

   ![](assets/brands_5.png)

Les directives de votre marque sont désormais accessibles à partir de la liste déroulante **[!UICONTROL Marque]** dans le menu de l’assistant d’IA, ce qui lui permet de générer du contenu et des ressources conformes à vos spécifications. [En savoir plus sur l’assistant IA](../email/generative-gs.md)

![](assets/brands_6.png)
