---
title: Créer une landing page
description: Découvrez comment configurer et publier une landing page dans le Web de Campaign
feature: Landing Pages
badge: label="Disponibilité limitée"
source-git-commit: e661517d68c2fe21f4209dbec2d98648740a3a86
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 7%

---

# Création et publication de landing pages {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Créer et gérer des landing pages"
>abstract="Adobe Campaign vous permet de créer, concevoir et partager des landing pages afin d’orienter vos utilisateurs vers des pages web en ligne où vous pouvez gérer des cas d’utilisation d’acquisition, d’abonnement/de désabonnement et de liste bloquée, en fonction de modèles intégrés."

L&#39;interface utilisateur Web de Campaign vous permet de créer, concevoir et publier des landing pages. Une fois publié, vous pouvez insérer un lien vers votre formulaire dans une diffusion. Une fois que les destinataires ont cliqué sur ce lien, ils sont redirigés vers la landing page correspondante.

[!DNL Adobe Campaign] est fourni avec quatre modèles pour gérer les cas d’utilisation suivants : **acquisition**, **abonnement**, **unsubscription**, et **liste bloquée**.

## Accès aux landing pages {#access-landing-pages}

Pour accéder à la liste des landing pages, sélectionnez **[!UICONTROL Gestion de campagne]** > **[!UICONTROL Landing pages]** dans le menu de gauche.

![](assets/lp-inventory.png)

La variable **[!UICONTROL Landing pages]** inventory affiche tous les éléments créés. Vous pouvez les filtrer à l’aide de la variable **Afficher les filtres** bouton . Vous pouvez limiter les résultats à un [dossier](../get-started/permissions.md#folders) spécifique à l’aide de la liste déroulante ou ajouter des règles à l’aide du [concepteur de requête](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Vous ne pouvez pas afficher ni modifier les landing pages créées à partir de la console cliente (formulaires web) dans l&#39;interface utilisateur Web de Campaign. En savoir plus dans la section [Documentation de la console Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Vous pouvez dupliquer ou supprimer une landing page. Cliquez sur les points de suspension en regard d’une landing page pour sélectionner l’action souhaitée.

## Créer une landing page {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Définir les propriétés de la landing page"
>abstract="Renseignez les champs des propriétés tels que le libellé et modifiez le schéma si nécessaire. De plus, vous pouvez modifier le nom interne, modifier le dossier dans lequel est stockée la landing page et fournir une description."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Définir le contenu de chaque page"
>abstract="Ajustez le contenu de chaque page qui fait partie de cette landing page, comme le formulaire lui-même, la page de confirmation qui s’affiche lors de l’envoi du formulaire, ou la page vers laquelle les utilisateurs sont redirigés en cas d’erreur."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Planification de votre landing page"
>abstract="Vous pouvez définir une date de début et une date de fin pour votre landing page. Lorsque la page atteint la fin de la période de validité, le formulaire n’est plus disponible. La variable **Expiration** s’affiche à la place."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Définition des paramètres de la page principale"
>abstract="La page principale s’affiche immédiatement pour les utilisateurs qui cliquent sur le lien vers votre page d’entrée (provenant, par exemple, d’un courrier électronique ou d’un site web)."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Définition de la landing page d’abonnement"
>abstract="Une page d’abonnement permet à vos clients de s’abonner à un service."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. Dans la **[!UICONTROL Landing pages]** inventory, cliquez sur **[!UICONTROL Créer une landing page]**.

   ![](assets/lp-create-button.png)

1. Sélectionnez un modèle :
   * **[!UICONTROL Acquisition]**: il s’agit du modèle par défaut des landing pages, qui vous permet de capturer et de mettre à jour les données de profil.
   * **[!UICONTROL Abonnement]**: utilisez ce modèle pour permettre aux utilisateurs de s’abonner à un [service](manage-services.md).
   * **[!UICONTROL Désabonnement]**: ce modèle peut être utilisé dans une diffusion envoyée aux abonnés d&#39;un service, afin de leur permettre de se désabonner. [service](manage-services.md).
   * **[!UICONTROL Liste bloquée]**: ce modèle doit être utilisé lorsqu’un profil ne souhaite plus être contacté par Campaign. En savoir plus sur la gestion des listes bloquées

   ![](assets/lp-templates.png)

1. Cliquez sur **[!UICONTROL Créer]**.

1. Renseignez les **[!UICONTROL Propriétés]** tels que le libellé.

   Par défaut, les landing pages sont stockées dans la variable **[!UICONTROL Applications web]** dossier. Vous pouvez la modifier en accédant à l’emplacement de votre choix dans le **[!UICONTROL Options supplémentaires]**. [Découvrez comment utiliser les dossiers](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. Dans le **[!UICONTROL Préchargement des données]** , les deux options ci-dessous sont sélectionnées par défaut :

   * La variable **[!UICONTROL Préremplir avec les données référencées dans le formulaire]** permet de précharger automatiquement les données correspondant aux champs de saisie et aux champs de fusion du formulaire.

   * L’option **[!UICONTROL Ignorer le pré-chargement si l’identification est vide]** doit être sélectionnée si vous ne souhaitez pas mettre à jour les profils. Dans ce cas, chaque profil saisi sera ajouté à la base de données après validation du formulaire. Cette option est utilisée, par exemple, lorsque le formulaire est publié sur un site web.

1. Dans le **[!UICONTROL Pages]** , cliquez sur le bouton **[!UICONTROL Modifier le contenu]** pour chaque page que vous souhaitez concevoir pour cette landing page. Le contenu de chaque page est déjà prérempli. Modifiez-les si nécessaire. [En savoir plus](lp-content.md)

   ![](assets/lp-pages.png)

1. La variable **[!UICONTROL Mise à jour de l’enregistrement préchargé]** est sélectionnée par défaut. Il permet de mettre à jour les profils stockés dans la base via la landing page. La boîte de préchargement permet d&#39;indiquer comment trouver l&#39;enregistrement à mettre à jour dans la base de données.

   Vous pouvez également choisir parmi les champs du contexte courant de la landing page, ceux qui seront utilisés pour trouver le profil correspondant dans la base de données. Pour ce faire, désélectionnez l’option **[!UICONTROL Mise à jour de l’enregistrement préchargé]** et cochez les champs de votre choix sous **[!UICONTROL Options de réconciliation]**.

   ![](assets/lp-storage.png)

1. Vous pouvez définir une date de début et une date de fin pour votre landing page. Sélectionner **[!UICONTROL Activation de la planification]** et définissez les dates.

   ![](assets/lp-schedule.png)

   * La landing page est automatiquement publiée à la date/l&#39;heure de début spécifiées.

     >[!NOTE]
     >
     >Si aucune date de début n&#39;est définie, la landing page devient active dès qu&#39;elle est publiée.

   * Lorsque la page atteint la date de fin, la landing page est automatiquement dépubliée et le formulaire n&#39;est plus disponible. La variable **[!UICONTROL Expiration]** s’affiche à la place.

     >[!NOTE]
     >
     >Pour des raisons de sécurité et de performances de la plateforme, Adobe vous recommande de définir une date de fin.

1. Cliquez sur **[!UICONTROL Révision et publication]**.

Une fois tous les paramètres définis et [conçu](lp-content.md) toutes les pages, vous pouvez [test](#test-landing-page) et [publier](#publish-landing-page) votre landing page.

## Tester la landing page {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simuler votre landing page"
>abstract="Vous pouvez afficher un aperçu de votre landing page dans l&#39;interface utilisateur Web de Campaign ou l&#39;ouvrir dans un nouvel onglet du navigateur Web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Prévisualiser et tester votre landing page"
>abstract="Une fois que vous avez défini les paramètres et le contenu de votre landing page, vous pouvez utiliser des profils de test pour la prévisualiser."

Une fois les paramètres et le contenu de votre landing page définis, vous pouvez utiliser des profils de test pour la prévisualiser. Si vous avez inséré [contenu personnalisé](../personalization/gs-personalization.md), vous pourrez vérifier l’affichage de ce contenu dans la landing page à l’aide des données de profil de test.

>[!CAUTION]
>
>Vous devez disposer de profils de test pour pouvoir prévisualiser vos messages et envoyer des bons à tirer. [En savoir plus sur les profils de test](../audience/test-profiles.md)

1. Cliquez ensuite sur **[!UICONTROL Révision et publication]**, sélectionnez la variable **[!UICONTROL Simulation du contenu]** dans le tableau de bord de la landing page pour accéder à la sélection du profil de test.

   ![](assets/lp-simulate-content.png)

1. Dans la **[!UICONTROL Simuler]** sélectionnez un ou plusieurs profils de test.

   Les étapes de sélection des profils de test sont les mêmes que lors du test d’un message. Elles sont détaillées dans la section [Aperçu et test](../preview-test/preview-test.md) .

1. Sélectionner **[!UICONTROL Ouvrir l’aperçu]** pour tester votre landing page.

   ![](assets/lp-open-preview.png)

1. L&#39;aperçu de votre landing page s&#39;ouvre dans un nouvel onglet. Les éléments personnalisés sont remplacés par les données de profil de test sélectionnées.

   Si vous avez sélectionné la variable **[!UICONTROL Préremplir avec les données référencées dans le formulaire]** dans les paramètres de la landing page, les champs du formulaire sont automatiquement préremplis avec les données de profil de test correspondantes.<!--TBC-->

   ![](assets/lp-preview.png)

1. Sélectionnez d&#39;autres profils de test pour prévisualiser le rendu pour chaque variante de votre landing page.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publier la landing page {#publish-landing-page}

Une fois votre landing page prête, publiez-la pour la rendre disponible dans une diffusion via le bouton correspondant.

Une fois publiée :

* La landing page est ajoutée à la liste de la landing page avec l’événement **[!UICONTROL Publié]** statut. Il est maintenant en ligne et prêt à être référencé dans votre contenu.

* Vous pouvez copier-coller le **[!UICONTROL URL de la landing page]** qui s’affiche en haut de la page dans un navigateur web.

![](assets/lp-published.png)

Vous pouvez surveiller les impacts de vos landing pages via les logs<!--and specific reports-->. Cliquez sur le bouton **[!UICONTROL Journaux]** bouton .
