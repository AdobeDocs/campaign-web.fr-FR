---
audience: end-user
title: Gérer la marque
description: Découvrir comment créer et gérer vos directives de marque
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 96%

---

# Créer et gérer vos marques {#brands}

Les directives de marque sont un ensemble complet de règles et de normes qui définissent l’identité visuelle et verbale d’une marque. Elles servent de référence pour homogénéiser la représentation de la marque sur tous les canaux de marketing et de communication.

Dans [!DNL Adobe Campaign Web], les utilisateurs et utilisatrices peuvent saisir et organiser manuellement les informations de marque ou charger des documents de directives de marque pour une extraction de données automatique.

## Accéder aux marques {#generative-access}

Pour accéder au menu **[!UICONTROL Marques]** dans [!DNL Adobe Campaign Web], les utilisateurs et utilisatrices doivent disposer de profils de produit **[!UICONTROL Administration (admin)]** et **[!UICONTROL Kit de marque]** pour créer et gérer des marques. Pour un accès en lecture seule, les utilisateurs et utilisatrices ont besoin d’un profil de produit [!UICONTROL Assistant IA]. [En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Découvrir comment attribuer des autorisations liées à la marque

1. Accédez à votre produit Campaign sur la page d’accueil [Admin Console](https://adminconsole.adobe.com/enterprise).

   ![Page d’accueil Admin Console montrant l’accès au produit Campaign](assets/brands_admin_1.png)

1. Sélectionnez le **[!DNL Product profile]** en fonction du niveau d’autorisations que vous souhaitez accorder à la personne.

   ![Sélection du profil de produit dans Admin Console](assets/brands_admin_2.png)

1. Cliquez sur **[!DNL Add users]** pour attribuer le profil de produit sélectionné.

   ![Option Ajouter des utilisateurs et des utilisatrices dans Admin Console](assets/brands_admin_3.png)

1. Saisissez le nom de la personne, le groupe d’utilisateurs et d’utilisatrices ou l’adresse e-mail.

1. Cliquez sur **Enregistrer** pour appliquer les changements.

Les personnes déjà affectées à ce rôle voient leurs autorisations automatiquement mises à jour.

+++

## Créer votre marque {#create-brand-kit}

Pour créer et configurer vos directives de marque, suivez les étapes indiquées ci-dessous.

Les utilisateurs et utilisatrices peuvent saisir les détails manuellement ou charger un document de directives de marque pour extraire automatiquement les informations :

1. Dans le menu **[!UICONTROL Marques]**, cliquez sur **[!UICONTROL Créer une marque]**.

   ![Menu Marques avec l’option Créer une marque](assets/brands-1.png)

1. Saisissez le **[!UICONTROL nom]** de votre marque.

1. Effectuez un glisser-déposer ou sélectionnez votre fichier pour charger vos directives de marque et extraire automatiquement les informations pertinentes. Cliquez sur **[!UICONTROL Créer une marque]**.

   Le processus d’extraction des informations commence alors. Notez que cette opération peut prendre plusieurs minutes.

   ![Chargement de fichier pour l’extraction des directives de la marque](assets/brands-2.png)

1. Vos normes de création visuelle et de contenu sont désormais automatiquement renseignées. Parcourez les différents onglets pour adapter les informations selon vos besoins. [En savoir plus](#personalize)

1. Dans le menu avancé de chaque section ou catégorie, vous pouvez ajouter des références pour extraire automatiquement les informations de marque pertinentes.

   Pour supprimer du contenu existant, utilisez les options **[!UICONTROL Effacer la section]** ou **[!UICONTROL Effacer la catégorie]**.

   ![](assets/brands-15.png)

1. Une fois la configuration effectuée, cliquez sur **[!UICONTROL Enregistrer]**, puis sur **[!UICONTROL Publier]** pour mettre à disposition vos directives de marque dans l’assistant IA.

1. Pour apporter des modifications à votre marque publiée, cliquez sur **[!UICONTROL Modifier la marque]**.

   >[!NOTE]
   >
   >Cela crée une copie temporaire en mode d’édition, qui remplace la version active une fois publiée.

   ![Option Modifier la marque dans le menu Marques](assets/brands-8.png)

1. Dans le tableau de bord **[!UICONTROL Marques]**, ouvrez le menu avancé en cliquant sur l’icône ![](assets/do-not-localize/Smock_More_18_N.svg) pour effectuer les actions suivantes :

   * Afficher la marque
   * Modifier
   * Marquer comme marque par défaut
   * Dupliquer
   * Publier
   * Dépublier
   * Supprimer

   ![Options de menu avancées dans le tableau de bord Marques](assets/brands-6.png)

Vos directives de marque sont désormais accessibles à partir du menu déroulant **[!UICONTROL Marque]** dans le menu de l’assistant IA. Cela permet à l’assistant IA de générer du contenu et des ressources alignés sur vos spécifications. [En savoir plus sur l’assistant IA](../content/generative-gs.md)

Vous pouvez également utiliser les directives de votre marque pour évaluer la qualité de votre contenu et l’alignement de votre marque. [En savoir plus sur la validation de la qualité du contenu](brands-score.md#validate-quality)

![Menu de l’assistant IA avec la liste déroulante Marque](assets/brands_6.png)

### Définir une marque par défaut {#default-brand}

Vous pouvez désigner une marque par défaut à appliquer automatiquement lors de la génération du contenu et du calcul des scores d’alignement pendant la création de campagne.

Pour définir une marque par défaut, accédez au tableau de bord **[!UICONTROL Marques]**. Ouvrez le menu avancé en cliquant sur l’icône ![](assets/do-not-localize/Smock_More_18_N.svg) et sélectionnez **[!UICONTROL Marquer comme marque par défaut]**.

![Options de menu avancées dans le tableau de bord Marques](assets/brands-6.png)

