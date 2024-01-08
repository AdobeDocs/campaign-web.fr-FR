---
title: Créer des profils de test dans Campaign
description: Découvrez comment créer et gérer des profils de test dans Adobe Campaign.
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
badge: label="Disponibilité limitée"
source-git-commit: 1f8a6c9765350f1c39a009afd7c1852967835d73
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 13%

---

# Créer et gérer des profils de test {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Créer des profils de test"
>abstract="Les profils de test sont créés en tant qu’adresses de contrôle. Il s’agit de destinataires supplémentaires dans la base de données utilisés pour cibler des profils fictifs qui ne correspondent pas aux critères de ciblage définis."

Les profils de test sont créés en tant qu’adresses de contrôle. Il s’agit de destinataires supplémentaires dans la base de données utilisés pour cibler des profils fictifs qui ne correspondent pas aux critères de ciblage définis. Ils vous permettent de prévisualiser et de tester la personnalisation et le rendu avant l&#39;envoi de votre diffusion, en leur envoyant des BAT.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

Les étapes pour envoyer des messages de test aux adresses de contrôle sont présentées dans la section [cette section](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>Les profils de test sont automatiquement exclus des rapports sur les statistiques d&#39;envoi suivantes : **[!UICONTROL Clics]**, **[!UICONTROL Ouvertures]**, **[!UICONTROL Désabonnements]**. [En savoir plus sur les rapports]

## Accès et gestion des profils de test {#access-test-profiles}

Pour accéder à la liste des profils de test, sélectionnez **[!UICONTROL Gestion des clients]** > **[!UICONTROL Profils]** dans le menu de gauche, puis cliquez sur l’icône **[!UICONTROL Profils de test]** .

![](assets/test-profile-list.png)

* Vous pouvez filtrer selon un [folder](../get-started/permissions.md#folders) à l’aide de la liste déroulante ou en ajoutant des règles à l’aide de la fonction [query modeler](../query/query-modeler-overview.md).

  ![](assets/test-profile-list-filters.png)

* Vous pouvez dupliquer n’importe quel profil de test et le mettre à jour si nécessaire. Les étapes de modification d’un profil de test sont les mêmes que lorsque [création d’un profil de test](#create-test-profile).

* Pour supprimer un profil de test, sélectionnez l’option correspondante dans la **[!UICONTROL Autres actions]** .

  ![](assets/test-profile-list-delete.png)

* Pour modifier un profil de test, cliquez sur l’élément de votre choix dans la liste. Les étapes de modification d’un profil de test sont les mêmes que lorsque [création d’un profil de test](#create-test-profile).

Vous pouvez également accéder aux profils de test via la **[!UICONTROL Explorateur]** de la vue **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Adresses de contrôle]** noeud .

De là, vous pouvez parcourir, créer et gérer des dossiers ou des sous-dossiers, ainsi que vérifier les autorisations associées. [Découvrez comment créer des dossiers](../get-started/permissions.md#folders)

![](assets/test-profiles-folders.png)

Dans la **[!UICONTROL Explorateur]** vous pouvez également filtrer, supprimer, modifier et [create](#create-test-profile) profils de test.

## Créer un profil de test {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Tester les données additionnelles des profils"
>abstract="Renseignez les données de personnalisation utilisées pour les diffusions créées dans les workflows Data management et auxquelles vous souhaitez attribuer une valeur spécifique."

Pour créer un profil de test, procédez comme suit.

1. Accédez à **[!UICONTROL Gestion des clients]** > **[!UICONTROL Profils]** et sélectionnez la variable **[!UICONTROL Profils de test]** .

1. Cliquez sur le bouton **[!UICONTROL Créer un profil de test]** bouton .

   ![](assets/test-profile-create.png)

1. Renseignez les détails du profil de test si nécessaire. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >La variable **[!UICONTROL Libellé]** est automatiquement renseigné avec le prénom et le nom que vous avez définis.

1. Par défaut, les profils de test sont stockés dans la variable **[!UICONTROL Adresses de contrôle]** dossier. Vous pouvez la modifier en accédant à l’emplacement souhaité. [Découvrez comment utiliser des dossiers](../get-started/permissions.md#folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. Dans le **[!UICONTROL Coordonnées]** , saisissez l’adresse électronique et d’autres données pertinentes. L&#39;adresse email s&#39;affiche entre parenthèses après le libellé du profil de test.

   ![](assets/test-profile-address.png)

1. Si vous sélectionnez l’option **[!UICONTROL Ne plus contacter (tous canaux)]** , le profil de test est en liste bloquée. Ce destinataire n&#39;est plus ciblé sur aucun canal (email, SMS, etc.).

1. Dans le **[!UICONTROL Données additionnelles]** saisissez les données de personnalisation utilisées pour les diffusions créées dans les workflows Data management et auxquelles vous souhaitez affecter une valeur spécifique. [En savoir plus sur les workflows](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   Assurez-vous que les données additionnelles de la cible ont été définies avec un alias commençant par &#39;@&#39; dans l’activité du workflow **[!UICONTROL Enrichissement]**. Sinon, vous ne pourrez pas l&#39;utiliser correctement avec vos adresses de contrôle dans l&#39;activité de diffusion. [En savoir plus sur l’activité Enrichissement](../workflows/activities/enrichment.md)

1. Cliquer sur le bouton **[!UICONTROL Enregistrer]**.

Le profil de test que vous venez de créer est maintenant prêt à être utilisé pour envoyer un test. [En savoir plus](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->



