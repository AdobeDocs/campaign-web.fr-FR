---
title: Surveillance et gestion des profils
description: Découvrez comment surveiller et gérer les profils dans le Web de Campaign.
badge: label="Disponibilité limitée"
source-git-commit: 41c38ff3b18c28fbcb6fd07dd398600a207f53cb
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 9%

---

# Surveillance et gestion des profils {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Affichage 360 de vos profils"
>abstract="Créez de nouveaux profils et surveillez-les à l’aide de puissants rapports et outils. Accédez aux attributs, interactions et logs de vos profils. Utilisez les options de filtrage pour parcourir la liste des profils, éditer et mettre à jour leur profil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Voir les notes de mise à jour"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profils"
>abstract="Un profil est une personne ciblée pour recevoir les messages envoyés par Adobe Campaign. Dans cette liste, vous pouvez afficher les détails des profils en fonction de vos autorisations. Utilisez les options de filtrage pour parcourir cette liste. Vous pouvez modifier et mettre à jour un petit ensemble d’attributs de vos profils."

## Prise en main des profils {#gs}

Un profil dans Adobe Campaign Web est un individu stocké dans la base de données. Il sert de composant clé pour créer des audiences pour les diffusions et ajouter des données de personnalisation à votre contenu. Différents types de profils sont stockés dans la base de données, tels que les profils de test, qui sont conçus pour tester vos diffusions avant leur envoi à l&#39;audience finale. [Découvrez comment utiliser des profils de test](test-profiles.md)

Les profils ne peuvent être ajoutés que depuis la console cliente Campaign. Toutefois, elles sont accessibles dans le Web Adobe Campaign à partir de la variable **Profils** dans le rail de navigation de gauche. Vous pouvez également y accéder à partir de la **Explorateur** où vous pouvez parcourir, créer des dossiers, des sous-dossiers et vérifier les autorisations associées.

Vous pouvez filtrer la liste des profils à l’aide du champ de recherche ou des filtres disponibles dans la variable **Afficher les filtres** bouton .

![](assets/profiles-list.png)

>[!NOTE]
>
>En fonction de vos permissions, il se peut que vous n&#39;ayez pas accès à la liste complète des profils stockés dans la base de données. Pour en savoir plus sur les autorisations, consultez [cette section](../get-started/permissions.md).

## Accès et modification des attributs des profils {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Détails de base"
>abstract="Cette section donne des informations sur les détails de base du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Coordonnées"
>abstract="Cette section donne des informations sur les coordonnées du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Adresse"
>abstract="Cette section donne des informations sur l’adresse postale du profil et la qualité des adresses. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Détails du compte"
>abstract="Cette section fournit des informations sur les détails du compte du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Personnes destinataires : ne plus contacter"
>abstract="Cette section donne des informations sur les préférences de contact du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Champs personnalisés"
>abstract="Les champs personnalisés sont des attributs spécifiques, adaptés à vos besoins, qui ont été configurés pour votre instance. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Autres"
>abstract="Cette section fournit des attributs intégrés supplémentaires. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Liste des abonnements des personnes destinataires"
>abstract="Cet onglet répertorie tous les services auxquels le profil est abonné."

Pour accéder aux détails d&#39;un profil, cliquez sur son nom dans la liste des profils.

![](assets/profiles-details.png)

Dans cet écran, vous pouvez accéder à des informations détaillées sur le profil :

* La variable **[!UICONTROL Détails]** vous permet de parcourir les attributs intégrés et personnalisés du profil. Pour modifier un attribut, apportez des modifications dans le champ souhaité, puis cliquez sur le bouton **[!UICONTROL Enregistrer]** bouton .
* La variable **[!UICONTROL Abonnements]** fournit des informations sur les services auxquels le profil est abonné. [Découvrez comment utiliser les services d’abonnement](manage-services.md)
* La variable **[!UICONTROL Journaux]** situé dans le coin supérieur droit de l&#39;écran, le bouton permet de visualiser l&#39;historique des interactions du profil par le biais des logs d&#39;envoi, d&#39;exclusion et de tracking, ainsi que les propositions présentées au profil.
