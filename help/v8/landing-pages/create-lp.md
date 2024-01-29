---
title: Créer une landing page
description: Découvrez comment configurer et publier une landing page dans le Web de Campaign
badge: label="Disponibilité limitée"
source-git-commit: 2a02015d9d7a7de67f0bcffd328d37080c0f50c4
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 8%

---

# Création et publication de landing pages {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Créer et gérer des landing pages"
>abstract="Adobe Campaign vous permet de créer et de concevoir des landing pages afin d’orienter vos utilisateurs vers des formulaires en ligne où ils peuvent s’inscrire ou se désinscrire de la réception de vos communications, ou s’abonner à un service spécifique tel qu’une newsletter."

Pour diriger vos clients vers une page web définie que vous souhaitez afficher lorsqu’ils cliquent sur un lien spécifique, créez une landing page dans [!DNL Adobe Campaign], concevez son contenu, testez-le et publiez-le.

## Accès aux landing pages {#access-landing-pages}

Pour accéder à la liste des landing pages, sélectionnez **[!UICONTROL Gestion de campagne]** > **[!UICONTROL Landing pages]** dans le menu de gauche.

![](assets/lp-inventory.png)

La variable **[!UICONTROL Landing pages]** inventory affiche tous les éléments créés. Vous pouvez les filtrer à l’aide de la variable **Afficher les filtres** bouton . Vous pouvez limiter les résultats à un [dossier](../get-started/permissions.md#folders) spécifique à l’aide de la liste déroulante ou ajouter des règles à l’aide du [concepteur de requête](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!NOTE]
>
>Vous ne pouvez pas afficher les landing pages créées à partir de la console cliente dans Campaign Web. En savoir plus dans la section [Documentation de la console Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Vous pouvez dupliquer ou supprimer une landing page. Cliquez sur les trois points en regard d’une landing page pour sélectionner l’action souhaitée.

## Créer une landing page {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Définir les propriétés de la landing page"
>abstract="Renseignez les champs des propriétés tels que le libellé et modifiez le schéma si nécessaire. De plus, vous pouvez modifier le nom interne, modifier le dossier dans lequel est stockée la landing page et fournir une description."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Définition du contenu des pages"
>abstract="Editez le contenu de chaque page qui fait partie de cette landing page."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Planification de votre landing page"
>abstract="Vous pouvez définir une date de début et une date de fin pour votre landing page. Lorsque la page a expiré, la variable **Expiration** s’affiche."


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
   * **[!UICONTROL Acquisition]**: il s’agit du modèle par défaut des landing pages, qui permet de capturer et de mettre à jour les données de profil.
   * **[!UICONTROL Abonnement]**: utilisez ce modèle pour proposer des abonnements à un service.
   * **[!UICONTROL Désabonnement]**: ce modèle peut être lié à un email envoyé aux abonnés à un service afin de leur permettre de se désabonner de ce service.
   * **[!UICONTROL Liste bloquée]**: ce modèle doit être utilisé lorsqu’un profil ne souhaite plus être contacté par Campaign. En savoir plus sur la gestion des listes bloquées

   ![](assets/lp-templates.png)

1. Cliquez sur **[!UICONTROL Créer]**.

1. Renseignez les champs des propriétés, tels que le libellé. Par défaut, les landing pages sont stockées dans la variable **[!UICONTROL Applications web]** dossier. Vous pouvez la modifier en accédant à l’emplacement de votre choix dans le **[!UICONTROL Options supplémentaires]**. [Découvrez comment utiliser les dossiers](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. Dans le **[!UICONTROL Préchargement des données]** , les deux options ci-dessous sont sélectionnées par défaut :

   * La variable **[!UICONTROL Préremplir avec les données référencées dans le formulaire]** permet de précharger automatiquement les données correspondant aux champs de saisie et aux champs de fusion du formulaire.

   * L’option **[!UICONTROL Ignorer le pré-chargement si l’identification est vide]** doit être sélectionnée si vous ne souhaitez pas mettre à jour les profils. Dans ce cas, chaque profil saisi sera ajouté à la base de données après validation du formulaire. Cette option est utilisée, par exemple, lorsque le formulaire est publié sur un site web.

1. Dans le **[!UICONTROL Pages]** , cliquez sur le bouton **[!UICONTROL Modifier le contenu]** pour chaque page que vous souhaitez concevoir pour cette landing page. Le contenu de chaque page est déjà prérempli. Modifiez-les si nécessaire. [En savoir plus](lp-content.md)

   ![](assets/lp-pages.png)

1. La variable **[!UICONTROL Mise à jour de l’enregistrement préchargé]** est sélectionné par défaut. Si vous souhaitez mettre à jour les profils stockés dans la base via la landing page, vous pouvez utiliser une boîte de préchargement. La boîte de préchargement permet d&#39;indiquer comment trouver l&#39;enregistrement à mettre à jour dans la base de données. Vous pouvez également choisir parmi les champs du contexte courant de la landing page, ceux qui seront utilisés pour trouver le profil correspondant dans la base de données.

   ![](assets/lp-storage-schedule.png)

1. Vous pouvez définir une date de début et une date de fin pour votre landing page. Sélectionner **[!UICONTROL Activation de la planification]** et définissez les dates. Lorsque la page a expiré, la variable **[!UICONTROL Expiration]** s’affiche.

1. Cliquez sur **[!UICONTROL Révision et publication]**.

Une fois que vous avez configuré et conçu toutes les pages, vous pouvez [test](#test-landing-page) et [publier](#publish-landing-page) votre landing page.

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
>Vous devez disposer de profils de test pour pouvoir prévisualiser vos messages et envoyer des bons à tirer. Découvrez comment [créer des profils de test](../audience/test-profiles.md).

1. Dans l’interface de la landing page, cliquez sur le bouton **[!UICONTROL Simulation du contenu]** pour accéder à la sélection du profil de test.

   ![](assets/lp-simulate-content.png)

1. Dans la **[!UICONTROL Simuler]** sélectionnez un ou plusieurs profils de test.

   Les étapes de sélection des profils de test sont les mêmes que lors du test d’un message. Elles sont détaillées dans la section [Aperçu et test](../preview-test/preview-test.md) .

1. Sélectionner **[!UICONTROL Ouvrir l’aperçu]** pour tester votre landing page.

   ![](assets/lp-open-preview.png)

1. L&#39;aperçu de votre landing page s&#39;ouvre dans un nouvel onglet. Les éléments personnalisés sont remplacés par les données de profil de test sélectionnées.

   ![](assets/lp-preview.png)

1. Sélectionnez d&#39;autres profils de test pour prévisualiser le rendu pour chaque variante de votre landing page.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publier la landing page {#publish-landing-page}

Une fois votre landing page prête, vous pouvez la publier afin de la rendre disponible pour une utilisation dans un message.

Une fois votre landing page publiée, elle est ajoutée à la liste des landing pages avec l&#39;événement **[!UICONTROL Publié]** statut. Il est maintenant en ligne et prêt à être utilisé.

![](assets/lp-published.png)

Une fois la publication effectuée, vous pouvez copier-coller le **[!UICONTROL URL de la landing page]** qui s’affiche en haut de la page dans un navigateur web.

Vous pouvez surveiller les impacts de vos landing pages par le biais de logs et de rapports spécifiques.
