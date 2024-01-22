---
audience: end-user
title: Découvrir l’interface
description: Interface utilisateur web de Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Disponibilité limitée"
source-git-commit: 7e2345327e613a9606598fefd440ae97f5aac24b
workflow-type: tm+mt
source-wordcount: '1632'
ht-degree: 81%

---

# Découvrir l’interface {#user-interface}

La nouvelle interface web de Campaign v8 offre une expérience utilisateur moderne et intuitive, afin de simplifier la conception et la diffusion des campagnes marketing. Cette nouvelle interface est intégrée aux applications et solutions Adobe Experience Cloud.

Découvrez comment vous connecter à Adobe Campaign et découvrir les principes de navigation des Experience Cloud [dans cet article](connect-to-campaign.md).


>[!NOTE]
>
>Cette documentation est fréquemment mise à jour pour prendre en compte les dernières modifications apportées à l’interface utilisateur du produit. Cependant, certaines captures d’écran peuvent légèrement différer de votre interface utilisateur.

## Page d&#39;accueil de Campaign {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Récents"
>abstract="La liste **Récents** offre des raccourcis vers les diffusions récemment créées et modifiées. Cette liste affiche le canal, le statut, la personne propriétaire, les dates de création et de modification."

La page d’accueil de Campaign vous permet de parcourir rapidement et facilement les ressources clés, les indicateurs et les composants.

La section supérieure de la page d’accueil fournit des détails sur les dernières mises à jour et les nouvelles fonctionnalités disponibles dans le produit, avec un lien vers les notes de mise à jour et la documentation connexe.

![](assets/home.png)

Les **indicateurs clés de performance** vous permettent de vérifier l’efficacité de votre plateforme grâce aux KPI courants. Pour en savoir plus sur les KPI, consultez [cette page](../reporting/kpis.md).

La liste **Récents** offre des raccourcis vers les diffusions récemment créées et modifiées. Cette liste affiche le canal, le statut, la personne propriétaire, les dates de création et de modification. Cliquez sur le bouton **Afficher plus** pour charger d’autres diffusions.

De plus, vous pouvez accéder aux pages d&#39;aide de la clé Web de Campaign v8 à partir de la page **Formation** de la page.

## Menu de navigation gauche {#user-interface-left-nav}

Parcourez les liens situés à gauche pour accéder aux fonctionnalités de Campaign v8 Web. Plusieurs liens affichent des listes d’objets qui peuvent être triés et filtrés. Vous pouvez également configurer des colonnes pour afficher toutes les informations dont vous avez besoin. Consultez cette [section](#list-screens). Certains écrans de liste sont en lecture seule. Les éléments affichés dans le menu de navigation de gauche dépendent de vos autorisations. Pour en savoir plus sur les autorisations, consultez [cette section](permissions.md).


### Explorateur {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorateur"
>abstract="Le menu **Explorateur** affiche tous les composants et objets Campaign avec la même hiérarchie de dossiers que celle de la console cliente. Parcourez tous vos composants, dossiers et schémas Campaign v8, vérifiez les autorisations associées et créez des dossiers et des sous-dossiers à partir de ce menu."

Le menu **Explorateur** affiche toutes les ressources et tous les objets Campaign avec la même hiérarchie de dossiers que celle de la console cliente. Parcourez tous les composants, dossiers et schémas de Campaign v8 et créez des diffusions, des workflows et des campagnes.

Les éléments affichés dans l’**Explorateur** dépendent de vos autorisations. Vous pouvez également ajouter des dossiers et des sous-dossiers, si vous disposez des droits adéquats. Pour en savoir plus sur les autorisations, consultez [cette section](permissions.md).

Vous pouvez configurer des colonnes pour personnaliser l’affichage afin de consulter toutes les informations dont vous avez besoin. Consultez cette [section](#list-screens). Vous pouvez également ajouter des dossiers et des sous-dossiers, comme décrit dans [cette section](permissions.md#folders).

Pour plus d’informations sur l’explorateur Campaign, la hiérarchie des dossiers et les ressources, reportez-vous à la [documentation de Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=fr#ac-explorer-ui){target="_blank"}.

### Campaign Management {#user-interface-campaign-management}

Dans la section GESTION DE CAMPAGNES, vous pouvez accéder aux campagnes marketing, aux diffusions et aux workflows.

* **Campagnes** : il s’agit de la liste de vos campagnes et modèles de campagne. Par défaut, pour chaque campagne, vous pouvez afficher les dates de début, de fin, de création, de dernière modification, le statut actuel et le nom de l’opérateur ou de l’opératrice Campaign qui l’a créée. Vous pouvez filtrer la liste par statut, dates de début et de fin, ou par dossier, ou créer un filtre avancé afin de définir vos propres critères de filtrage. En savoir plus sur les campagnes [dans cette section](../campaigns/gs-campaigns.md).

* **Diffusions** - Parcourez votre liste de diffusions. Vous pouvez consulter leur état, date de dernière modification ainsi que les principaux KPI. Vous pouvez filtrer la liste par statut, date de contact ou canal. Pour obtenir une vue d’ensemble des détails d’une diffusion e-mail, cliquez sur celle-ci afin d’ouvrir son tableau de bord. Les diffusions sur d’autres canaux sont en lecture seule. Pour en savoir plus sur les diffusions, consultez [cette section](../msg/gs-messages.md).

  Utilisez le bouton **Autres actions** pour supprimer ou dupliquer une diffusion.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** : dans cet écran, vous pouvez accéder à la liste complète des workflows et des modèles de workflows. Vous pouvez vérifier leur statut, les dates de dernière exécution ou de prochaine exécution, et créer un nouveau workflow ou un nouveau modèle de workflow. Vous pouvez filtrer la liste selon les mêmes critères que pour les autres objets. En outre, vous pouvez filtrer les workflows appartenant ou non à une campagne. Pour en savoir plus sur les workflows, consultez [cette section](../workflows/gs-workflows.md).


### Gestion de contenu {#user-interface-content-management}

Dans la section GESTION DU CONTENU , vous pouvez afficher vos modèles de contenu et vos fragments.

* **Modèles de contenu** - Pour accélérer et améliorer le processus de conception, vous pouvez créer des modèles autonomes pour réutiliser facilement du contenu personnalisé dans tous les [!DNL Adobe Campaign]. Cette fonctionnalité, disponible uniquement pour les emails, permet aux utilisateurs orientés contenu de travailler sur des modèles autonomes afin que les utilisateurs marketing puissent les réutiliser et les adapter dans leurs propres campagnes email. En savoir plus dans [cette section](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Gestion des clients {#user-interface-customer-management}

Dans la section GESTION DES CLIENTS , vous pouvez afficher vos profils, audiences et abonnements. Ces listes sont en lecture seule.

* **Profils** - Créez et gérez des profils, et accédez à votre base de données de destinataires. Par défaut, vous pouvez consulter leur adresse e-mail, prénom et nom. En savoir plus sur les profils dans [cette section](../audience/about-recipients.md).
* **Audiences** - Il s’agit de votre liste d’audiences. Par défaut, vous pouvez consulter leur type, origine, date de création/dernière modification et libellé. Vous pouvez filtrer la liste par origine. Pour en savoir plus sur les audiences, consultez [cette section](../audience/about-recipients.md).
* **Services d’inscriptions** - Parcourez vos listes d&#39;abonnements. Par défaut, vous pouvez consulter leur type, mode et libellé. Découvrez comment gérer les abonnements et les désabonnements dans la [documentation d’Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=fr){target="_blank"}.
* **Filtres prédéfinis** - Les filtres prédéfinis sont des filtres personnalisés qui sont créés et enregistrés pour être disponibles pour une utilisation ultérieure. Ils peuvent être utilisés comme raccourcis lors de toute opération de filtrage avec le modeleur de requête, par exemple lors du filtrage d&#39;une liste de données ou de la création de l&#39;audience d&#39;une diffusion. En savoir plus dans [cette section](predefined-filters.md).


### Gestion des décisions {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offres"
>abstract="Parcourez les listes d’offres et de modèles d’offres qui ont été créées dans la console à l’aide du module **Interaction**. Ces listes sont en lecture seule."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=fr" text="Ajouter des offres à une diffusion"

Dans la section GESTION DES DÉCISIONS, vous pouvez visualiser les offres et les modèles d’offres. Ces listes sont en lecture seule.

* **Offres** - Parcourez la liste des offres et des modèles d’offres créés dans la console à l’aide du module **Interaction**. Par défaut, vous pouvez consulter leur statut, les dates de début/fin et leur environnement. Vous pouvez filtrer la liste par statut et par dates de début/fin. Des modèles d’offre sont également disponibles.

Découvrez comment créer et envoyer des offres dans des e-mails et des SMS dans [cette section](../msg/offers.md).

### Rapports {#left-nav-reporting}

* **Rapports** - La variable **Rapport** entry offre un résumé global consolidé des mesures de trafic et d’engagement pour chaque canal de votre environnement Campaign. Ces rapports se composent de différents widgets, chacun offrant une perspective différente des performances de vos campagnes ou diffusions. En savoir plus dans [cette section](../reporting/global-reports.md).


## Aide contextuelle {#user-interface-help}

Une aide contextuelle est disponible dans l’interface. Si elle est présente, cliquez sur l’icône `?` pour afficher des informations d’aide et des liens vers la documentation connexe.

![](assets/do-not-localize/context-help.png){width="40%" align="left"}

Disponible actuellement en tant que version bêta dans la nouvelle interface utilisateur web de Campaign, le **Assistant de connaissances optimisé par l&#39;IA** incorporé dans l’aide contextuelle révolutionne la recherche de documentation et la réponse aux questions pratiques en analysant facilement de vastes référentiels de documentation, en repérant instantanément les informations précises dont vous avez besoin.

Grâce aux fonctionnalités de l’IA générative de Campaign, cet assistant transforme votre expérience, en facilitant la récupération d’informations et la résolution de problèmes. Que vous soyez à la recherche de conseils dans une tâche complexe ou que vous parcouriez des documents volumineux, notre assistant de connaissances optimisé par l’IA devient votre meilleur compagnon, en vous offrant une efficacité et une précision inégalées à chaque interaction.

En savoir plus dans [cette section](using-ai.md).



## En savoir plus {#learn-more}

Découvrez [sur cette page](list-filters.md) comment parcourir, rechercher et filtrer les listes disponibles dans votre environnement Campaign.



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Autorisation requise"
>abstract="Avant de pouvoir créer un segment, votre administrateur ou administratrice doit vous accorder une autorisation."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Autorisation requise"
>abstract="Avant de pouvoir créer un segment, votre administrateur ou administratrice doit vous accorder une autorisation."

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Envoi de rapports globaux"
>abstract="Les mesures des rapports de suivi sont visibles dans cet écran."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Suivi des rapports globaux"
>abstract="Les mesures des rapports de suivi sont visibles dans cet écran."

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Liste des workflows dans une campagne"
>abstract="Liste des workflows dans une campagne"

<!-- delivery settings-->






<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->




<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Création de personnes destinataires"
>abstract="Création de personnes destinataires"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Vue d’ensemble de la carte des personnes destinataires"
>abstract="Vue d’ensemble de la carte des personnes destinataires"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Points de contact des personnes destinataires"
>abstract="Points de contact des personnes destinataires"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Sélection des abonnements des personnes destinataires"
>abstract="Sélection des abonnements des personnes destinataires"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Liste des offres éligibles des personnes destinataires"
>abstract="Liste des offres éligibles des personnes destinataires"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Aperçu des offres des personnes destinataires"
>abstract="Aperçu des offres des personnes destinataires"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="Profil en lecture seule des personnes destinataires"
>abstract="Profil en lecture seule des personnes destinataires"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Modèle de diffusion des abonnements"
>abstract="Modèle de diffusion des abonnements"

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Pages de destination"
>abstract="Pages de destination"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Propriétés des pages de destination"
>abstract="Propriétés des pages de destination"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Pages des pages de destination"
>abstract="Pages des pages de destination"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Planning des pages de destination"
>abstract="Planning des pages de destination"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Page principale des pages de destination"
>abstract="Page principale des pages de destination"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Abonnement aux pages de destination"
>abstract="Abonnement aux pages de destination"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Appel à l’action des pages de destination"
>abstract="Appel à l’action des pages de destination"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulation des pages de destination"
>abstract="Simulation des pages de destination"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Activité non modifiable"
>abstract="Activité non modifiable"




>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragments"
>abstract="Fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Enregistrement de fragments"
>abstract="Enregistrement de fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Création de fragments"
>abstract="Création de fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Propriétés des fragments"
>abstract="Propriétés des fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Type de fragment"
>abstract="Type de fragment"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Liste de fragments"
>abstract="Liste de fragments"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Détails des fragments"
>abstract="Détails des fragments"






>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Filtre d’enregistrement de contenu conditionnel"
>abstract="Filtre d’enregistrement de contenu conditionnel"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Filtre de sélection du contenu conditionnel"
>abstract="Filtre de sélection du contenu conditionnel"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Contenu conditionnel sur la ligne d’objet"
>abstract="Contenu conditionnel sur la ligne d’objet"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Condition de ligne d’objet de contenu conditionnel"
>abstract="Condition de ligne d’objet de contenu conditionnel"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Simuler des profils de test"
>abstract="Simuler des profils de test"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Simuler la sélection des profils de test"
>abstract="Simuler la sélection des profils de test"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Simuler l’envoi de profils de test"
>abstract="Simuler l’envoi de profils de test"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="Simuler le journal de l’e-mail"
>abstract="Simuler le journal de l’e-mail"


>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Contenu pour publipostage direct"
>abstract="Contenu pour publipostage direct"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propriétés de fichier pour publipostage direct"
>abstract="Propriétés de fichier pour publipostage direct"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Propriétés de contenu pour publipostage direct"
>abstract="Propriétés de contenu pour publipostage direct"


<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Afficher les attributs avancés"
>abstract="Seuls les attributs les plus courants sont affichés par défaut dans la liste des attributs. Activez le bouton (bascule) **Afficher les attributs avancés** pour afficher tous les attributs disponibles pour la liste actuelle dans la palette gauche du créateur de règles, tels que les nœuds, les regroupements, les liens 1-1 et les liens 1-N."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Champs avancés du créateur de règles"
>abstract="Seuls les attributs les plus courants sont affichés par défaut dans la liste des attributs. Activez le bouton (bascule) **Afficher les attributs avancés** pour afficher tous les attributs disponibles pour la liste actuelle dans la palette gauche du créateur de règles, tels que les nœuds, les regroupements, les liens 1-1 et les liens 1-N."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Attributs avancés du créateur de règles"
>abstract="Seuls les attributs les plus courants sont affichés par défaut dans la liste des attributs. Activez le bouton (bascule) **Afficher les attributs avancés** pour afficher tous les attributs disponibles pour la liste actuelle dans la palette gauche du créateur de règles, tels que les nœuds, les regroupements, les liens 1-1 et les liens 1-N."