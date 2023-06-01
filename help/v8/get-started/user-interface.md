---
audience: end-user
title: Découvrir l’interface
description: Interface utilisateur web de Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha" type="Positive"
source-git-commit: ec61c17d5a72b4d324d9a9a2cc71c85093c124ea
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 73%

---

# Découvrir l’interface {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Découvrir l’interface"
>abstract="La nouvelle interface web de Campaign v8 Web offre une expérience utilisateur intégrée, intuitive et cohérente."

La nouvelle interface web de Campaign v8 Web offre une expérience utilisateur moderne et intuitive, afin de simplifier la conception et la diffusion des campagnes marketing. Cette nouvelle interface est intégrée à Adobe Experience Platform.

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>Cette documentation est fréquemment mise à jour pour prendre en compte les dernières modifications apportées à l’interface utilisateur du produit. Cependant, certaines captures d’écran peuvent légèrement différer de votre interface utilisateur.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Menu de navigation gauche

Parcourez les liens situés à gauche pour accéder aux fonctionnalités de Campaign v8 Web. Plusieurs liens affichent des listes d’objets qui peuvent être triés et filtrés. Vous pouvez également configurer des colonnes pour afficher toutes les informations dont vous avez besoin. Consultez cette [section](#list-screens). Tous les écrans de type Liste sont en lecture seule, à l’exception de la liste de diffusion e-mail. La version Alpha ne permet pas de cliquer sur un élément de liste pour le modifier/visualiser. Toutes les listes pourront être modifiées dans les versions ultérieures. Les éléments affichés dans le menu de navigation de gauche dépendent de vos autorisations utilisateur.

![](assets/home.png)

### Accueil

Les liens et les ressources clés de cet écran offrent un accès rapide aux principales fonctionnalités de Campaign v8 Web. La liste **Récents** offre des raccourcis vers les diffusions récemment créées et modifiées. Cette liste affiche les dates et statuts de création et de modification.

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Accédez aux pages principales d’aide de Campaign v8 Web depuis la section inférieure de la page d’accueil.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorateur

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorateur"
>abstract="Le menu **Explorateur** affiche la même hiérarchie de dossiers que celle de la console cliente. Parcourez tous vos composants, dossiers et schémas Campaign v8. Tous les écrans de type Liste sont en lecture seule, à l’exception de la liste de diffusion e-mail."

Le menu **Explorateur** affiche la même hiérarchie de dossiers que celle de la console cliente. Parcourez tous vos composants, dossiers et schémas Campaign v8.

Les éléments affichés dans l’Explorateur dépendent de vos autorisations utilisateur.

Comme dans n’importe quel écran de liste, vous pouvez configurer des colonnes pour personnaliser l’affichage en fonction des informations que vous souhaitez. Consultez cette [section](#list-screens).

Pour plus d’informations sur l’explorateur de Campaign, consultez cet [article](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html?lang=fr#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campagnes"
>abstract="Il s’agit de la liste de vos campagnes. Vous pouvez afficher des informations utiles telles que leurs dates de début, de fin ou de dernière modification, ainsi que leur statut. Vous pouvez filtrer la liste par statut ou date de début/fin. Cliquez sur le bouton &quot;Créer une campagne&quot; pour ajouter une nouvelle campagne. Sélectionnez une opération pour afficher son contenu, ses diffusions et ses détails. Accédez à l&#39;onglet &quot;Modèles&quot; pour afficher et créer des modèles."

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Diffusions"
>abstract="Parcourez votre liste de diffusions. Vous pouvez consulter leur statut, les dates de contact et de modification, les indicateurs clés de performance. Vous pouvez filtrer la liste par état, date de contact ou canal. Cliquez sur le bouton &quot;Créer une diffusion&quot; pour ajouter une nouvelle diffusion. Sélectionnez une diffusion pour afficher son contenu, son audience et ses détails."

Dans la section CAMPAIGN MANAGEMENT , vous pouvez accéder aux opérations marketing, diffusions et workflows.

* **Campagnes** - Il s’agit de la liste de vos campagnes et modèles de campagne. Par défaut, pour chaque opération, vous pouvez visualiser les dates de début/fin/création/dernière modification, l&#39;état actuel et le nom de l&#39;opérateur Campaign qui l&#39;a créée. Vous pouvez filtrer la liste par statut, dates de début/fin, dossier ou créer un filtre avancé afin de définir vos propres critères de filtrage. En savoir plus sur les campagnes [dans cette section](../campaigns/gs-campaigns.md).

* **Diffusions** - Parcourez votre liste de diffusions. Vous pouvez consulter leur état, date de dernière modification ainsi que les principaux KPI. Vous pouvez filtrer la liste par état, date de contact ou canal. Pour obtenir une vue d’ensemble des détails d’une diffusion e-mail, cliquez sur celle-ci afin d’ouvrir son tableau de bord. Les diffusions sur d’autres canaux sont en lecture seule. En savoir plus sur les diffusions [dans cette section](../email/gs-messages.md).

   Utilisez le bouton **Autres actions** pour supprimer ou dupliquer une diffusion.

   ![](assets/more-actions.png){width="70%" align="left"}

* **Workflows** - Dans cet écran, vous pouvez accéder à la liste complète des workflows et des modèles de workflows. Vous pouvez vérifier leur état, les dates de dernière exécution/prochaine exécution et créer un nouveau workflow ou un nouveau modèle de workflow. Vous pouvez filtrer la liste selon les mêmes critères que pour les autres objets. En outre, vous pouvez filtrer les workflows appartenant à une campagne ou non. En savoir plus sur les workflows [dans cette section](../workflows/gs-workflows.md).


### Gestion des clients

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Destinataires"
>abstract="Accédez à la base de données des destinataires. Vous pouvez consulter des informations utiles telles que leur adresse e-mail, prénom et nom. Cette liste est en lecture seule."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="Il s’agit de votre liste d’audiences. Vous pouvez consulter leur type, origine, date de création/dernière modification et libellé. Vous pouvez filtrer la liste par origine. Cette liste est en lecture seule."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Listes d’abonnements"
>abstract="Parcourez les listes d’abonnements. Vous pouvez consulter leur type, mode et libellé. Cette liste est en lecture seule."

* **Destinataires** - Accédez à la base de données des destinataires. Par défaut, vous pouvez consulter leur adresse e-mail, prénom et nom. Cette liste est en lecture seule.
* **Audiences** - Il s’agit de votre liste d’audiences. Par défaut, vous pouvez consulter leur type, origine, date de création/dernière modification et libellé. Vous pouvez filtrer la liste par origine. Cette liste est en lecture seule.
* **Listes d’abonnements** - Parcourez vos listes d’abonnements. Par défaut, vous pouvez consulter leur type, mode et libellé. Cette liste est en lecture seule.

### Gestion des décisions

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Offres"
>abstract="Parcourez votre liste d’offres Interaction. Par défaut, vous pouvez consulter leur état, les dates de début/fin et leur environnement. Vous pouvez filtrer la liste par état et par date de début/fin. Des modèles d’offre sont également disponibles. Ces listes sont en lecture seule."

* **Offres** - Parcourez votre liste d’offres d’interaction. Par défaut, vous pouvez consulter leur état, les dates de début/fin et leur environnement. Vous pouvez filtrer la liste par état et par date de début/fin. Des modèles d’offre sont également disponibles. Ces listes sont en lecture seule.

## Barre supérieure  

La barre supérieure de l’interface vous permet de :

* partager vos commentaires en tant que testeur ou testeuse Alpha,
* basculer entre les organisations et les instances,
* basculer entre les applications Adobe Experience Cloud,
* accéder aux pages d’aide, contacter le support et partager vos commentaires. Vous pouvez rechercher des articles et des vidéos d’aide dans le champ de recherche.

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Configurer les écrans de liste {#list-screens}

Plusieurs liens du menu de navigation de gauche, par exemple **Diffusions** ou **Campagnes**, affichent des listes d’objets. Ces écrans de type Liste sont en lecture seule, à l’exception de la liste de diffusion d’e-mails.

Pour trouver les éléments plus rapidement, vous pouvez utiliser la barre de recherche ou filtrer la liste selon des critères contextuels.

![](assets/filter.png){width="70%" align="left"}

Les listes sont affichées en colonnes. Vous pouvez également afficher des informations supplémentaires en modifiant la configuration des colonnes. Pour ce faire, cliquez sur l’icône dans le coin supérieur droit de la liste. Vous pouvez ajouter ou supprimer des colonnes et modifier leur ordre d’affichage.

![](assets/columns.png){width="70%" align="left"}

Vous pouvez trier les éléments de la liste en cliquant sur l’en-tête d’une colonne. Une flèche s’affiche (vers le haut ou vers le bas) pour indiquer que la liste est triée sur cette colonne. Pour les colonnes numériques ou de date, la flèche vers le haut indique que la liste est triée par ordre croissant, tandis que la flèche vers le bas indique un ordre décroissant. Pour les colonnes de type chaîne ou alphanumérique, les valeurs sont classées par ordre alphabétique.

## Aide contextuelle et guide d’intégration

Une aide contextuelle est disponible dans l’interface. Lorsquʼelle est disponible, cliquez sur l&#39;icône **?** pour afficher les informations dʼassistance et les liens des documents connexes.

![](assets/context-help.png){width="70%" align="left"}

Un guide d’intégration est également disponible pour vous aider à commencer à utiliser Campaign v8 Web. Cliquez sur l’icône dans le coin inférieur droit, sélectionnez l’un des scénarios détaillés disponibles, puis suivez simplement les instructions.

![](assets/onboarding.png){width="70%" align="left"}

## Navigateurs pris en charge {#browsers}

Campaign v8 Web est conçu pour fonctionner de manière optimale dans la dernière version de Google Chrome, Safari et Microsoft Edge. Vous pouvez rencontrer des problèmes lors de l’utilisation de certaines fonctionnalités sur des versions plus anciennes ou d’autres navigateurs.

## Préférences de langue {#language-pref}

Campaign v8 Web est actuellement disponible dans les langues suivantes :

<table>
<tr>
<td>
<p>Anglais (États-Unis) - EN-US</p>
<p>Français - FR</p>
<p>Allemand - DE</p>
<p>Italien - IT</p>
</td>
<td>
<p>Espagnol - ES</p>
<p>Portugais (Brésil) - PTBR</p>
<p>Japonais - JP</p>
</td>
<td>
<p>Coréen - KR</p>
<p>Chinois simplifié - CHS</p>
<p>Chinois traditionnel - CHT</p>
</td>
</tr>
</table>

La langue de votre interface par défaut est déterminée par la langue préférée spécifiée dans votre profil utilisateur.

Pour changer de langue :

1. Cliquez sur l’icône de votre profil, en haut à droite, puis sélectionnez **Préférences**.

   ![](assets/preferences.png){width="70%" align="left"}

1. Cliquez ensuite sur la langue affichée sous votre adresse e-mail.

   ![](assets/preferences2.png)

1. Sélectionnez la langue de votre choix et cliquez sur **Enregistrer**. Vous pouvez sélectionner une seconde langue au cas où le composant que vous utilisez n’est pas localisé dans votre première langue.

   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Définition de l&#39;audience SMS"
>abstract="Sélectionnez la meilleure audience pour votre SMS."

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="Synthèse du rapport SMS"
>abstract="Découvrez les mesures de création de rapports pour votre diffusion SMS."

>[!CONTEXTUALHELP]
>id="acw_push_report_overview"
>title="Synthèse du rapport des notifications push"
>abstract="Découvrez les mesures de création de rapports pour votre diffusion push."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Attributs avancés du créateur de règles"
>abstract="Utilisez des attributs avancés pour définir votre règle."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Mesures envoyées"
>abstract="Nombre de courriers électroniques remis."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Mesures des erreurs"
>abstract="Nombre d&#39;emails avec le statut d&#39;erreur."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Contenu de notification push pour Android"
>abstract="Définissez le contenu Android push."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Contenu de notification push pour iOS"
>abstract="Définissez le contenu iOS push."

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Personnes abonnées à l’application"
>abstract="Prévisualisez et testez le message en ajoutant des abonnés à l’application à la cible principale. "

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Population test"
>abstract="Sélectionnez un mode de population test."

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Mode Aperçu"
>abstract="Prévisualisez et testez le message en incluant la population test à la cible principale."

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Données d’enrichissement"
>abstract="À déterminer"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personnalisation"
>abstract="À déterminer"


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Envoi des rapports"
>abstract="Consultez les indicateurs d&#39;envoi pour le reporting de l&#39;opération."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Tracking des rapports"
>abstract="Consultez les indicateurs de tracking pour le reporting de l&#39;opération."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Présentation des rapports"
>abstract="Mesures clés de votre diffusion."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Rapports sur les statistiques cibles"
>abstract="Cette section affiche des mesures spécifiques en fonction des audiences."

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="Rapports agrégés pour les diffusions"
>abstract="Sélectionnez au moins deux diffusions pour afficher un rapport de données agrégées."


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Champs de déduplication"
>abstract="À déterminer"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Paramètres de déduplication"
>abstract="À déterminer"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Complémentaire de déduplication"
>abstract="À déterminer"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Complémentaire de dimension"
>abstract="À déterminer"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Autorisation requise"
>abstract="Avant de pouvoir créer un segment, votre administrateur doit vous accorder des autorisations."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Autorisation requise"
>abstract="Avant de pouvoir créer un segment, votre administrateur doit vous accorder des autorisations."

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Champs avancés du sélecteur d’attributs"
>abstract="Configurez les colonnes avec des champs avancés."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Champs avancés du créateur de règles"
>abstract="Configurez les colonnes avec des champs avancés."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propriétés de diffusion push"
>abstract="Gérez les propriétés de la diffusion push."

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nouvelle mesure de mises en quarantaine"
>abstract="Nouvelle mesure de mise en quarantaine."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Sélection du modèle de SMS"
>abstract="Sélectionnez un modèle prédéfini pour démarrer votre diffusion SMS."

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Diffusés"
>abstract="IPC distribués"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Ouvertures (Opens)"
>abstract="Ouvertures (Opens) KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clics"
>abstract="IPC de clics"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Désinscriptions (Unsubscriptions)"
>abstract="Désinscriptions (Unsubscriptions) KPI"

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Indésirables"
>abstract="IPC de spam"
