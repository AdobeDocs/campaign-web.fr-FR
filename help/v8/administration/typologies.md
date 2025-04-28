---
audience: end-user
title: Utiliser les règles métier (typologies)
description: Découvrez comment utiliser les typologies et les règles de typologie pour contrôler, filtrer et surveiller l’envoi des diffusions.
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: f676ecd055cd9b9ea5c0e724c479e9ba6dbda73d
workflow-type: tm+mt
source-wordcount: '1474'
ht-degree: 39%

---

# Utiliser les règles métier (typologies) {#typologies}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Règles métier"
>abstract="Vous pouvez désormais créer des typologies et des règles de typologie dans l’interface d’utilisation web d’Adobe Campaign. Les typologies permettent de contrôler, de filtrer et de hiérarchiser l’envoi des diffusions."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"

>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="Typologies et règles de typologie"
>abstract="Les typologies vous permettent de normaliser les pratiques commerciales sur toutes les diffusions. Une typologie est un ensemble de règles de typologie qui vous permet de contrôler, de filtrer et de hiérarchiser l’envoi des diffusions. Les profils répondant aux critères au sein d’une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_type"
>title="Filtrage"
>abstract=" Deux types de règles de typologie sont disponibles : les règles <br/><br/>**de contrôle** qui assurent la qualité et la validité du message avant son envoi, telles que l&#39;affichage des caractères, la longueur des SMS, le format des adresses ou le raccourcissement des URL. <br/><br/>**Filtrage** règles qui excluent des segments de l’audience cible en fonction de critères spécifiques, tels que l’âge, le lieu, le pays ou les numéros de téléphone."

## À propos des typologies

Les typologies vous permettent de normaliser les pratiques commerciales sur toutes les diffusions. Une **typologie** est un ensemble de **règles de typologie** qui vous permet de contrôler, de filtrer et de hiérarchiser l’envoi des diffusions. Les profils répondant aux critères au sein d’une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation.

Les typologies s’assurent que vos diffusions contiennent toujours certains éléments, tels qu’un lien de désinscription ou une ligne d’objet, ou des règles de filtrage pour exclure des groupes de votre cible prévue, tels que les désabonnés, les concurrents ou les clients non fidèles.

Les typologies sont accessibles via le menu **[!UICONTROL Administration]** > **[!UICONTROL Règles métier]**. Depuis cet écran, accédez à toutes les typologies et règles de typologie existantes, ou créez-en de nouvelles en fonction de vos besoins.

![Liste des règles métier dans l’interface](assets/business-rules-list.png)

>[!NOTE]
>
>La liste **[!UICONTROL Règles de typologie]** affiche toutes les règles existantes créées à ce jour dans l’interface d’utilisation web ou la console cliente. Toutefois, seules les règles **Contrôle** et **Filtrage** peuvent être créées dans l’interface d’utilisation web. Pour créer d’autres types de règles de typologie, telles que les règles de pression ou de capacité, utilisez la console cliente Campaign v8. [Découvrez comment créer des règles de typologie dans la console cliente](https://experienceleague.adobe.com/fr/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

Voici les principales étapes à suivre pour appliquer des typologies à vos messages :

1. [Créez une typologie](#typology).
1. [Créez des règles de typologie](#typology-rules).
1. [Référencez les règles de typologie dans la typologie](#add-rules).
1. [Appliquez la typologie à un message](#message).

## Créer une typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="Propriétés de la typologie"
>abstract="Définissez les propriétés de la typologie et développez la section **[!UICONTROL Options supplémentaires]** pour accéder aux paramètres avancés. Utilisez le champ **[!UICONTROL Affinité IP]** pour associer des affinités IP aux typologies. Vous pouvez ainsi mieux contrôler le trafic SMTP sortant en définissant les adresses IP spécifiques qui peuvent être utilisées pour chaque affinité."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="Affinité avec l’adresse IP"
>abstract="La gestion des affinités avec les adresses IP permet un meilleur contrôle du trafic SMTP sortant en associant différentes adresses IP à chaque type de trafic selon la typologie de son action de diffusion."

Pour créer une typologie, procédez comme suit :

1. Accédez au menu **[!UICONTROL Règles métier]**, puis sélectionnez l’onglet **[!UICONTROL Typologie]**.

1. Cliquez sur le bouton **[!UICONTROL Créer une typologie]** et saisissez un **[!UICONTROL Libellé]** pour la typologie.

1. Développez la section **[!UICONTROL Options supplémentaires]** pour définir des paramètres avancés, tels que le nom interne de la typologie, le dossier de stockage et la description.

   ![Interface de création de typologie](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >Le champ **[!UICONTROL Affinité IP]** vous permet d’associer des affinités IP à des typologies. Cela permet de mieux contrôler le trafic SMTP sortant en définissant les adresses IP spécifiques qui peuvent être utilisées pour chaque affinité. Vous pouvez, par exemple, utiliser une affinité par pays ou sous-domaine. Vous pouvez ensuite créer une typologie par pays et associer chaque affinité à la typologie correspondante.

1. Cliquez sur **[!UICONTROL Créer]** pour confirmer la création de la typologie.

Les détails de la typologie s’ouvrent. Sur cet écran, référencez directement les règles de typologie existantes ou créez de nouvelles règles de typologie à référencer ultérieurement :
* [Découvrir comment créer une règle de typologie](#add-rules)
* [Découvrir comment référencer des règles dans une typologie](#add-rules)

## Créer une règle de typologie {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="Propriétés de la règle de typologie"
>abstract="Définissez les propriétés de la règle de typologie. Les règles **Contrôle** vérifient la qualité et la validité du message avant l’envoi, tandis que les règles **Filtrage** excluent des segments de l’audience cible en fonction de critères spécifiques.<br/><br/>Vous pouvez également modifier l’ordre d’exécution de la règle pour gérer la séquence d’exécution des règles de typologie lorsque plusieurs règles du même type sont exécutées au cours de la même phase de traitement des messages."

Pour créer une règle de typologie, accédez au menu **[!UICONTROL Règles métier]**, puis sélectionnez l’onglet **[!UICONTROL Règles de typologie]**.

Cliquez sur le bouton **[!UICONTROL Créer une règle de typologie]**, puis suivez les étapes détaillées ci-dessous.

### Définir les propriétés de la règle de typologie {#properties}

Définissez les propriétés de la règle de typologie :

1. Saisissez un **[!UICONTROL libellé]** pour la règle.

   ![Interface de création des règles de contrôle](assets/business-rules-control-rule.png)

1. Sélectionnez le **[!UICONTROL type]** de la règle de typologie :

   * **Contrôle** : assure la qualité et la validité de la pré-envoi du message, comme l’affichage des caractères, la longueur du SMS, le format de l’adresse ou le raccourcissement de l’URL. Ces règles sont créées à l’aide d’une interface de script pour définir une logique complexe pour les vérifications et modifications de contenu.

   * **Filtrage** : exclut des segments de l’audience cible en fonction de critères spécifiques, tels que l’âge, le lieu, le pays ou les numéros de téléphone. Ces règles sont liées à une dimension de ciblage.

   >[!NOTE]
   >
   >Actuellement, seules les règles de typologie **Contrôle** et **Filtrage** peuvent être créées à partir de l’interface utilisateur web. Pour créer d’autres types de règles, utilisez la console cliente. [Découvrez comment créer des règles de typologie dans la console cliente](https://experienceleague.adobe.com/fr/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. Sélectionnez un **[!UICONTROL Canal]** à associer à la règle.

1. Désactivez l’option **[!UICONTROL Actif]** si vous ne souhaitez pas que la règle soit active immédiatement après sa création.

1. Définissez l’ordre d’exécution **[!UICONTROL la règle]**.

   Par défaut, l’ordre des règles de typologie est défini sur 50. Adaptez cette valeur pour gérer la séquence dans laquelle les règles de typologie seront exécutées lorsque plusieurs règles du même type sont exécutées au cours de la même phase de traitement des messages. Par exemple, une règle de filtrage dont l’ordre d’exécution est défini sur 20 sera exécutée avant une règle de filtrage dont l’ordre d’exécution est défini sur 30.

1. Développez la section **[!UICONTROL Options supplémentaires]** pour accéder aux paramètres avancés, tels que le nom interne de la règle, l’espace de stockage du dossier et la description.

1. Pour les règles de contrôle, deux champs supplémentaires sont disponibles dans les options supplémentaires. Indiquez à quel moment la règle doit s’appliquer et son niveau d’alerte :

   * **[!UICONTROL Phase]** : indiquez à quel moment du cycle de vie de la diffusion la règle sera appliquée. Sélectionnez la valeur dans la liste déroulante **[!UICONTROL Phase]**. Développez la section ci-dessous pour plus d’informations sur les valeurs possibles.

   +++Phases des règles de contrôle :

   **[!UICONTROL Au début du ciblage]** : permet d&#39;éviter l&#39;exécution de l&#39;étape de personnalisation en cas d&#39;erreur.

   **[!UICONTROL Après ciblage]** : sélectionnez cette phase si vous avez besoin de connaître le volume de la cible pour appliquer la règle de pilotage. Par exemple, la règle de contrôle **[!UICONTROL Vérifier la taille du BAT]** s&#39;applique après chaque étape de ciblage. Cette règle empêche la personnalisation des messages s’il y a trop de destinataires de BAT.

   **[!UICONTROL Au début de la personnalisation]** : sélectionnez cette phase si le contrôle porte sur la validation de la personnalisation du message. La personnalisation des messages est réalisée au cours de la phase d’analyse.

   **[!UICONTROL À la fin de l’analyse]** : effectuez des vérifications nécessitant une personnalisation complète du message.

+++

   * **[!UICONTROL Niveau]** : indiquez le niveau d’alerte de la règle. Pour plus d’informations, développez la section ci-dessous.

   +++Niveaux des règles de contrôle :

   **[!UICONTROL Erreur]** : arrêtez la préparation du message.

   **[!UICONTROL Avertissement]** : affichez un avertissement dans les logs de préparation.

   **[!UICONTROL Info]** : affichez des informations dans les logs de préparation.

   **[!UICONTROL Verbeux]** : affichez les informations dans les logs serveur.

+++

### Créer le contenu de la règle {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="Filtrage"
>abstract="Les règles **Filtrage** excluent des segments de l’audience cible en fonction de critères spécifiques, tels que l’âge, le lieu, le pays ou les numéros de téléphone. Sélectionnez la dimension de ciblage de la règle de typologie et cliquez sur le bouton **[!UICONTROL Ajouter des règles]** pour accéder au concepteur de requête et créer la règle."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="Code"
>abstract="Les règles **Contrôle** vérifient la qualité et la validité de la pré-envoi du message, telles que l’affichage des caractères, la longueur du SMS, le format de l’adresse ou le raccourcissement des URL. Ces règles sont créées à l’aide du code JavaScript."

Une fois les propriétés de la règle de typologie définies, créez le contenu de la règle.

* Pour les **règles de contrôle**, cliquez sur le bouton **Modifier le code** et saisissez la logique de la règle en JavaScript. Dans l&#39;exemple ci-dessous, une règle est créée pour afficher un avertissement dans les logs si la cible est vide.

  ![Éditeur de code de règle de contrôle](assets/business-rules-code.png)

* Pour les **règles de filtrage**, sélectionnez la dimension de ciblage et cliquez sur le bouton **[!UICONTROL Ajouter des règles]** pour définir les critères de filtrage à l’aide du [concepteur de requête](../query/query-modeler-overview.md).

  ![Modéliseur de requête de règle de filtrage](assets/business-rules-query.png)

Lorsque votre règle est prête, cliquez sur le bouton **[!UICONTROL Créer]** pour créer la règle de typologie. Référencez la règle dans une typologie pour l&#39;appliquer aux messages.

## Référencer des règles de typologie dans une typologie {#add-rules}

Pour référencer une ou plusieurs règles dans une typologie, procédez comme suit :

1. Accédez à l’onglet **[!UICONTROL Typologie]** et ouvrez la typologie dans laquelle vous souhaitez référencer la ou les règles.

1. Sélectionnez l’onglet **[!UICONTROL Règles de typologie]** et cliquez sur le bouton **[!UICONTROL Ajouter des règles de typologie]**.

   ![Ajouter une interface de règles de typologie](assets/business-rules-reference.png)

1. Sélectionnez une ou plusieurs règles de typologie à associer à la typologie et confirmez.

   ![Interface Enregistrer les règles de typologie](assets/business-rules-typology-save.png)

1. Cliquez sur **[!UICONTROL Enregistrer]**.

Vous pouvez désormais appliquer la typologie à des messages. Une fois cette opération terminée, toutes les règles de typologie sélectionnées seront exécutées pour effectuer les vérifications définies.

## Appliquer des typologies à des messages {#message}

Pour appliquer une typologie à un message ou à un modèle de message, sélectionnez la typologie dans les paramètres du message. [Découvrir comment configurer les paramètres de diffusion](../advanced-settings/delivery-settings.md#typology)

![Appliquer la typologie à l&#39;interface des messages](assets/business-rules-apply.png)

Une fois appliquées, les règles de typologie incluses dans la typologie sont exécutées pour vérifier la validité de la diffusion pendant la préparation du message. Les profils répondant aux critères d’une règle de typologie sont exclus des audiences de diffusion.