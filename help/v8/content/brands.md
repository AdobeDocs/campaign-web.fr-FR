---
audience: end-user
title: Gérer la marque
description: Découvrir comment créer et gérer vos directives de marque
badge: label="Version bêta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: 61078f86bcd433b1bc3a995489f283eb709b3687
workflow-type: tm+mt
source-wordcount: '1275'
ht-degree: 17%

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

1. Une fois la configuration effectuée, cliquez sur **[!UICONTROL Enregistrer]** puis **[!UICONTROL Publier]** pour rendre votre ligne directrice de marque disponible dans l’assistant AI.

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

Vos directives de marque sont désormais accessibles à partir de la liste déroulante **[!UICONTROL Marque]** dans le menu de l’assistant AI. Cela permet à l’assistant AI de générer du contenu et des ressources alignés sur vos spécifications. [En savoir plus sur l’assistant AI](../email/generative-gs.md)

![Menu assistant AI avec liste déroulante Marque](assets/brands_6.png)

### Définir une marque par défaut {#default-brand}

Vous pouvez désigner une marque par défaut à appliquer automatiquement lors de la génération du contenu et du calcul des scores d’alignement lors de la création de la campagne.

Pour définir une marque par défaut, accédez au tableau de bord **[!UICONTROL Marques]**. Ouvrez le menu avancé en cliquant sur l’icône ![](assets/do-not-localize/Smock_More_18_N.svg) et sélectionnez **[!UICONTROL Marquer comme marque par défaut]**.

![Options de menu avancées dans le tableau de bord Marques](assets/brands-6.png)

## Personnaliser votre marque {#personalize}

### À propos de la marque {#about-brand}

Utilisez l’onglet **[!UICONTROL À propos de la marque]** pour établir l’identité principale de votre marque en décrivant son objectif, sa personnalité, son slogan et d’autres attributs déterminants.

1. Commencez par renseigner les informations fondamentales de votre marque dans la catégorie **[!UICONTROL Détails clés]** :

   * **[!UICONTROL Nom du kit de marque]** : saisissez le nom du kit de marque.

   * **[!UICONTROL Quand l’utiliser]** : spécifiez les scénarios ou les contextes où ce kit de marque doit être appliqué.

   * **[!UICONTROL Nom de la marque]** : saisissez le nom officiel de la marque.

   * **[!UICONTROL Description de la marque]** : donnez un aperçu de ce que représente cette marque.

   * **[!UICONTROL Ligne de balise par défaut]** : ajoutez la ligne de balise principale associée à la marque.

     ![Catégorie Détails clés](assets/brands-about-1.png)

1. Dans la catégorie **[!UICONTROL Principes directeurs]**, clarifiez l’orientation et la philosophie de base de votre marque :

   * **[!UICONTROL Mission]** : détaillez l’objectif de votre marque.

   * **[!UICONTROL Vision]** : Décrivez votre objectif à long terme ou l’état futur souhaité.

   * **[!UICONTROL Positionnement sur le marché]** : Expliquez comment votre marque est positionnée sur le marché.

   ![Catégorie des principes directeurs](assets/brands-about-2.png)

1. Dans la catégorie **[!UICONTROL Valeurs de marque principales]**, cliquez sur ![Texte secondaire de l’image de plongée](assets/do-not-localize/Smock_Add_18_N.svg "Icône Ajouter") pour ajouter les valeurs de base de la marque et renseigner les détails :

   * **[!UICONTROL Valeur]** : attribuez un nom à une valeur de marque principale.

   * **[!UICONTROL Description]** : expliquez ce que cette valeur signifie pour votre marque.

   * **[!UICONTROL Comportements]** : Décrivez les actions ou attitudes qui reflètent cette valeur dans la pratique.

   * **[!UICONTROL Manifestations]** : donnez des exemples de la manière dont cette valeur est exprimée dans le branding réel.

     ![](assets/brands-12.png)

1. Si nécessaire, cliquez sur l’icône ![Texte secondaire de l’image de plongée](assets/do-not-localize/Smock_Edit_18_N.svg "Modifier")pour mettre à jour ou supprimer l’une des valeurs de votre marque principale.

   ![Modifier la valeur](assets/brands-10.png)

Vous pouvez désormais personnaliser davantage votre marque ou [publier votre marque](#create-brand-kit).

### Style d&#39;écriture {#writing-style}

La section **[!UICONTROL Style d’écriture]** décrit les normes d’écriture de contenu et explique en détail comment la langue, le formatage et la structure doivent être utilisés pour garantir la clarté, la cohérence et l’homogénéité de l’ensemble des ressources.

+++ Catégorie et exemples disponibles

<table>
  <thead>
    <tr>
      <th>Catégorie</th>
      <th>Sous-catégorie</th>
      <th>Exemple de directives</th>
      <th>Exemple d’exclusions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="4">Normes de création de contenu</td>
      <td>Normes de message de marque</td>
      <td>Mettez l’accent sur l’innovation et le message client.</td>
      <td>Ne promettez pas outre mesure les fonctionnalités du produit.</td>
    </tr>
    <tr>
      <td>Utilisation des balises</td>
      <td>Placez le slogan sous le logo sur toutes les ressources de marketing numérique.</td>
      <td>Ne modifiez ou ne traduisez pas le slogan.</td>
    </tr>
    <tr>
      <td>Messagerie principale</td>
      <td>Insistez sur l'énoncé des principaux avantages, comme l'amélioration de la productivité.</td>
      <td>N’utilisez pas de propositions de valeur non liées.</td>
    </tr>
    <tr>
      <td>Normes de dénomination</td>
      <td>Utilisez des noms simples et descriptifs tels que « ProScheduler ».</td>
      <td>N’utilisez pas de termes complexes ou de caractères spéciaux.</td>
    </tr>
    <tr>
      <td rowspan="5">Style de communication de la marque</td>
      <td>Caractéristiques de la personnalité d’une marque</td>
      <td>Amical et accessible.</td>
      <td>Ne sois pas défaitiste.</td>
    </tr>
    <tr>
      <td>Mécanique de l'écriture</td>
      <td>Faites en sorte que les phrases soient courtes et percutantes.</td>
      <td>N'utilisez pas trop de jargon.</td>
    </tr>
    <tr>
      <td>Ton Situationnel</td>
      <td>Maintenir un ton professionnel dans les communications de crise.</td>
      <td>Ne méprisez pas les communications d’assistance.</td>
    </tr>
    <tr>
      <td>Instructions relatives au choix de mots</td>
      <td>Utilisez des mots comme « innovant » et « intelligent ».</td>
      <td>Évitez les mots tels que « bon marché » ou « hack ».</td>
    </tr>
    <tr>
      <td>Normes linguistiques</td>
      <td>Respectez les conventions américaines en anglais.</td>
      <td>Ne mélangez pas l'orthographe britannique et américaine.</td>
    </tr>
    <tr>
      <td rowspan="3">Normes De Conformité Légale</td>
      <td>Normes relatives aux marques</td>
      <td>Utilisez toujours le symbole ™ ou ®.</td>
      <td>N’omettez pas les symboles légaux si nécessaire.</td>
    </tr>
    <tr>
      <td>Normes de copyright</td>
      <td>Incluez les avis de copyright sur les supports marketing.</td>
      <td>N’utilisez pas de contenu tiers sans autorisation.</td>
    </tr>
    <tr>
      <td>Normes de non-responsabilité</td>
      <td>Afficher de manière lisible les clauses de non-responsabilité sur les ressources numériques.</td>
      <td>Ne masquez pas les clauses de non-responsabilité dans les zones non visibles.</td>
    </tr>
</table>

+++

</br>

Pour personnaliser votre **[!UICONTROL Style d’écriture]** :

1. Dans l’onglet **[!UICONTROL Style d’écriture]**, cliquez sur ![](assets/do-not-localize/Smock_Add_18_N.svg) pour ajouter une directive, une exception ou une exclusion.

1. Saisissez votre règle, votre exception ou votre exclusion, puis cliquez sur **[!UICONTROL Ajouter]**.

   ![](assets/brands-3.png)

1. Sélectionnez l’une des instructions ou exclusions à mettre à jour ou à supprimer.

1. Cliquez sur le ![Texte secondaire de l’image de plongée](assets/do-not-localize/Smock_Edit_18_N.svg "Modifier") pour modifier votre exemple ou sur l’icône ![Texte secondaire de l’image de plongée](assets/do-not-localize/Smock_Delete_18_N.svg "Supprimer") pour le supprimer.

   ![](assets/brands-11.png)

Vous pouvez désormais personnaliser davantage votre marque ou [publier votre marque](#create-brand-kit).

### Contenu visuel {#visual-content}

La section **[!UICONTROL Contenu visuel]** définit les normes en matière d’imagerie et de conception, en détaillant les spécifications nécessaires pour conserver une apparence de marque unifiée et cohérente.

+++ Catégories et exemples disponibles

<table>
  <thead>
    <tr>
      <th>Catégorie</th>
      <th>Exemple de directives</th>
      <th>Exemple d’exclusions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Normes de photographie</td>
      <td>Utiliser l'éclairage naturel pour les prises de vue extérieures.</td>
      <td>Évitez les images trop modifiées ou pixellisées.</td>
    </tr>
    <tr>
      <td>Normes d'illustration</td>
      <td>Utilisez des styles épurés et minimalistes.</td>
      <td>Éviter les situations trop complexes.</td>
    </tr>
    <tr>
      <td>Normes des icônes</td>
      <td>Utilisez un système de grille cohérent de 24 px.</td>
      <td>Ne mélangez pas les dimensions des icônes, n’utilisez pas d’épaisseurs de contour incohérentes ou ne vous écartez pas des règles de grille.</td>
    </tr>
    <tr>
      <td>Instructions d’utilisation</td>
      <td>Choisissez des images de style de vie qui reflètent des clients réels utilisant le produit dans des environnements professionnels.</td>
      <td>N’utilisez pas d’images qui contredisent le ton de la marque ou semblent hors contexte.</td>
    </tr>
</table>

+++

</br>

Pour personnaliser votre **[!UICONTROL contenu visuel]** :

1. Dans l’onglet **[!UICONTROL Contenu visuel]**, cliquez sur ![](assets/do-not-localize/Smock_Add_18_N.svg) pour ajouter une directive, une exclusion ou un exemple.

1. Saisissez votre règle, exclusion ou exemple et cliquez sur **[!UICONTROL Ajouter]**.

   ![Ajout d’un bouton d’exclusion ou d’exemple](assets/brands-4.png)

1. Pour ajouter une image montrant une utilisation correcte, sélectionnez **[!UICONTROL Exemple]** et cliquez sur **[!UICONTROL Sélectionner une image]**. Vous pouvez également ajouter une image montrant une utilisation incorrecte comme exemple d’action à ne pas faire.

   ![Ajout d’une image en tant qu’exemple](assets/brands-13.png)

1. Sélectionnez l’une des instructions ou exclusions à mettre à jour ou à supprimer.

1. Sélectionnez l’une de vos directives ou exclusions pour la mettre à jour. Cliquez sur l’icône ![Texte secondaire de l’image de plongée](assets/do-not-localize/Smock_Delete_18_N.svg "Supprimer") pour le supprimer.

   ![Supprimer l’exclusion ou la consigne](assets/brands-14.png)

Vous pouvez désormais personnaliser davantage votre marque ou [publier votre marque](#create-brand-kit).
