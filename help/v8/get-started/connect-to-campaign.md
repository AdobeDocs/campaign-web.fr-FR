---
title: Se connecter à l’interface web d’Adobe Campaign
description: Découvrir comment vous connecter à l’interface utilisateur d’Adobe Campaign Web
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
TQID: 'https://experienceleague.adobe.com/TSbgkDH1v-9HH-szfGQx0z6-6fP8tny4s7Vx2SE8gUo'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
topic_v2:
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 7bbc2d4c383886788afc1ef83cdd27e7ec4b24ae
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 81%
---
# Connexion à Adobe Campaign {#connect-to-campaign}

[!DNL Adobe CX Enterprise] Adobe la famille intégrée d’applications, de produits et de services de marketing numérique d’. Grâce à son interface intuitive, vous pouvez accéder rapidement à vos applications cloud, fonctionnalités de produit et services. Découvrez comment vous connecter à [!DNL CX Enterprise] et accéder à l’interface web d’Adobe Campaign sur cette page.

## Se connecter à [!DNL Adobe CX Enterprise] {#sign-in-to-exc}

Vous pouvez également utiliser l’authentification unique (SSO) pour vous connecter à Campaign. En règle générale, les administrateurs [!DNL CX Enterprise] accordent l’accès aux applications et services. Suivez les étapes de votre invitation par e-mail à [!DNL CX Enterprise].

Pour vous connecter à [!DNL Adobe CX Enterprise], procédez comme suit :

1. Accédez à [[!DNL Adobe CX Enterprise]](https://experience.adobe.com/){target="_blank"}.

1. Connectez-vous à l’aide de votre Adobe ID ou de votre Enterprise ID. Pour en savoir plus sur les types d’identités chez Adobe, consultez [cet article](https://helpx.adobe.com/fr/enterprise/using/identity.html){target="_blank"}.

   Après vous être connecté à [!DNL CX Enterprise], vous pouvez accéder rapidement à toutes vos solutions et applications.

   ![Capture d&#39;écran affichant la page d&#39;accueil de Adobe CX Enterprise](assets/exc-home.png){zoomable="yes"}

1. Vérifiez que vous vous trouvez dans la bonne organisation.

   ![Capture d’écran montrant la sélection de l’organisation dans Adobe CX Enterprise](assets/exc-orgs.png){zoomable="yes"}{width="50%"}

   En savoir plus sur les organisations dans [!DNL Adobe CX Enterprise] dans [cet article](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=fr){target="_blank"}.

## Accéder à Adobe Campaign {#access-to-campaign}

Pour accéder à votre environnement Campaign, sélectionnez **Campaign** dans la section **Accès rapide** de la page d’accueil [!DNL Adobe CX Enterprise].

Si vous êtes déjà connecté à une autre solution [!DNL Adobe CX Enterprise], accédez à votre environnement Campaign à partir du sélecteur de solution en haut à droite de votre écran.

![Capture d’écran affichant le sélecteur de solutions dans Adobe CX Enterprise](assets/solution-switcher.png){zoomable="yes"}

Si vous avez accès à plusieurs environnements, y compris le panneau de contrôle Campaign, cliquez sur le bouton **Démarrer** de l’instance appropriée.

![Capture d’écran montrant le bouton Lancer pour Adobe Campaign](assets/launch-campaign.png){zoomable="yes"}

Vous êtes maintenant connecté(e) à Campaign. Découvrez comment commencer à utiliser l’interface utilisateur sur [cette page](user-interface.md).

### Contrôle d’accès {#access-control}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="Autorisation requise"
>abstract="Avant de pouvoir créer cet objet, votre administrateur ou administratrice doit vous accorder une autorisation."

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="Cette audience est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier cette audience. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="Ce service est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier ce service. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="Profil en lecture seule des personnes destinataires"
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier ce profil. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Cette campagne est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier cette campagne. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="Cette diffusion est en lecture seule."
>abstract="Vous ne disposez pas des autorisations nécessaires pour modifier cette diffusion. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="Ce workflow est en lecture seule."
>abstract="Vous ne disposez pas des permissions nécessaires pour modifier ce workflow. Si nécessaire, contactez votre administrateur ou administratrice, qui vous accordera l’accès."

Le contrôle d’accès permet de restreindre l’accès aux objets et données des listes principales, telles que les diffusions, les destinataires ou les workflows. Ces restrictions s’appliquent également dans l’arborescence de navigation de l’explorateur. En outre, vous avez besoin d’autorisations pour créer, supprimer, dupliquer et modifier des objets à partir de l’interface utilisateur.

Toutes les autorisations de Campaign Web sont synchronisées avec celles de la console cliente Campaign. Seuls les administrateurs ou les administratrices de Campaign peuvent définir et modifier les autorisations utilisateur.

Lorsque vous naviguez dans l’interface d’utilisation de Campaign Web, vous pouvez accéder aux données, aux objets et aux fonctionnalités selon vos autorisations. Par exemple, si vous ne disposez pas des autorisations d’accès à un dossier, vous ne pouvez pas l’afficher. Vos autorisations ont également une incidence sur la gestion des objets et des données. Sans autorisation d’écriture pour un dossier spécifique, vous ne pouvez pas créer de diffusion dans ce dossier, même si vous pouvez l’afficher dans l’interface utilisateur.

Vous pouvez apprendre à [afficher et gérer les autorisations ici](permissions.md).

## Navigation supérieure [!DNL Adobe CX Enterprise] {#top-bar}

La barre supérieure de l&#39;interface vous donne un accès rapide aux principales fonctionnalités de [!DNL CX Enterprise].

![Capture d’écran affichant la barre de navigation supérieure de Adobe CX Enterprise](assets/do-not-localize/unified-shell.png){zoomable="yes"}

Utilisez la barre supérieure pour effectuer les opérations suivantes :

* Partager des commentaires à propos de l’interface d’utilisation de Campaign Web
* Basculer entre vos organisations
* Basculez entre vos [!DNL Adobe CX Enterprise] solutions et applications.
* Rechercher de l’aide sur [Adobe Experience League](https://experienceleague.adobe.com/docs/?lang=fr){target="_blank"}
* Afficher les notifications de vos produits.
* Modifier votre profil Adobe et gérer les paramètres, par exemple [mettre à jour la langue préférée](#language-pref) ou [basculer entre les thèmes clair et sombre](#dark-theme).

## Navigateurs pris en charge {#browsers}

Adobe Campaign Web est conçu pour fonctionner de manière optimale dans la dernière version de Google Chrome, Safari et Microsoft Edge. Vous pouvez rencontrer des problèmes lors de l’utilisation de certaines fonctionnalités sur des versions plus anciennes ou d’autres navigateurs.

## Préférences de langue {#language-pref}

Adobe Campaign Web est actuellement disponible dans les langues suivantes :

* Anglais (États-Unis) - EN-US
* Français - FR
* Allemand - DE
* Italien - IT
* Espagnol - ES
* Portugais (Brésil) - PTBR
* Japonais - JP
* Coréen - KR
* Chinois simplifié - CHS
* Chinois traditionnel - CHT

En outre, un formatage spécifique aux paramètres régionaux (comme les dates, heures, calendriers, nombres) peut également être disponible dans différentes variantes des langues prises en charge par l’interface d’utilisation :

* Anglais (Israël)
* Anglais (Royaume-Uni)
* Espagnol (Mexique)
* Espagnol (Amérique latine)
* Français (Canada)

La langue par défaut pour Campaign Web est déterminée par la langue préférée spécifiée dans votre profil utilisateur. Elle n’est pas liée à la langue de votre serveur Campaign et de votre console cliente.

Pour changer de langue :

1. Cliquez sur l’icône de votre profil, en haut à droite, puis sélectionnez **Préférences**.
1. Cliquez ensuite sur le lien de la langue sous votre adresse e-mail.
1. Sélectionnez la langue de votre choix et cliquez sur **Enregistrer**. Vous pouvez sélectionner une seconde langue si le composant que vous utilisez n’est pas localisé dans votre première langue.


## Thèmes sombre et clair {#dark-theme}

Adobe Campaign est disponible dans les thèmes clair et sombre. Par défaut, l’interface utilisateur est activée avec le thème clair. Pour passer au thème sombre, cliquez sur l’icône de votre profil, puis cliquez sur le bouton (bascule) **Thème sombre** pour l’activer ou le désactiver.

Les paramètres de profil utilisateur et les préférences de compte sont présentées dans [cette section](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=fr#preferences){target="_blank"}.

Pour en savoir plus sur les composants de l’interface centrale d’Experience Cloud, consultez [cette documentation](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=fr){target="_blank"}.