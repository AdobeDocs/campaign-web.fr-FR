---
title: Gestion des mappings de ciblage
description: Découvrez comment gérer les mappings de ciblage.
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 7%

---

# Gestion des mappings de ciblage {#target-mappings}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_list"
>title="Mappings de ciblage "
>abstract="Mappings de ciblage"

## À propos des mappings de ciblage {#about}

Chaque canal de communication utilise un mapping de ciblage par défaut pour cibler ses destinataires. Par exemple, par défaut, les modèles de diffusion par e-mail et SMS ciblent **[!UICONTROL Destinataires]**. Leur mapping de ciblage utilise donc les champs de la table **nms:recipient**. Pour les notifications push, le mapping de ciblage par défaut est **Applications Abonnés (nms:appSubscriptionRcp)**, qui est lié au tableau des destinataires.

Les mappings de ciblage sont accessibles à partir du menu **[!UICONTROL Administration]** > **[!UICONTROL Mappings de ciblage]**. Depuis cet écran, vous pouvez accéder aux détails de chaque mapping de ciblage ou en créer de nouveaux en fonction de vos besoins.

![](assets/target-mappings-list.png)

Pour plus d’informations sur les mappings de ciblage intégrés fournis avec Adobe Campaign, reportez-vous à la documentation de la console cliente [Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr){target="_blank"}.

## Créer un mapping de ciblage {#create-mapping}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_properties"
>title="Propriétés du mapping de ciblage"
>abstract="La section **[!UICONTROL Propriétés]** permet de définir des paramètres génériques pour le mapping de ciblage et la population ciblée."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_mapping"
>title="Mappage du mapping de ciblage"
>abstract="La section **[!UICONTROL Mapping]** vous permet d’identifier les attributs du schéma du mapping de ciblage à utiliser pour les différents champs d’adresses de diffusion."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_denylist"
>title="Liste bloquée du mapping de ciblage"
>abstract="Liste bloquée du mapping de ciblage"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_storage"
>title="Stockage du mapping de ciblage"
>abstract="La section **[!UICONTROL Stockage]** vous permet d’identifier l’emplacement où les journaux doivent être stockés."

Pour créer un nouveau mapping de ciblage, accédez au menu **[!UICONTROL Administration]** > **[!UICONTROL Mappings de ciblage]**. Cliquez sur le bouton **[!UICONTROL Créer un mappage]** puis suivez les étapes présentées dans les sections ci-dessous.

1. Dans la section **[!UICONTROL Propriétés]**, saisissez un **[!UICONTROL Libellé]** pour le mapping de ciblage.

1. Développez la section **[!UICONTROL Options supplémentaires]** pour définir des paramètres avancés tels que le nom interne du mapping de ciblage, le dossier de stockage et la description.

1. Choisir la population cible. Vous pouvez, au choix :

   * **[!UICONTROL Utiliser directement la dimension de ciblage]** : sélectionnez la dimension à cibler directement dans la liste des dimensions disponibles.
   * **[!UICONTROL Utiliser les données liées]** : cette option permet de partir d&#39;une dimension de ciblage (par exemple, les abonnements), puis de passer à la dimension de ciblage que vous souhaitez cibler (par exemple, les destinataires).

   ![](assets/target-mappings-properties.png)

1. Si la dimension sélectionnée n’est pas déjà utilisée par un mapping de ciblage existant, les schémas pour stocker les logs doivent être créés. Pour ce faire, des options supplémentaires sont disponibles dans la section **[!UICONTROL Stockage]**. Développez la section ci-dessous pour plus de détails.

   +++Options de stockage pour les nouvelles dimensions de ciblage

   1. **[!UICONTROL Espace de noms]** : identifiez l’espace de noms qui sera utilisé pour créer les journaux.
   1. **[!UICONTROL Suffixe du schéma d’extension]** : indiquez un suffixe pour le nouveau schéma.

      Dans l’exemple ci-dessous, le nom du broadlog est « cusbroadlogSupplier ».

      ![](assets/target-mappings-new.png)

   1. **[!UICONTROL Logs de diffusion]** : activez les options de cette section pour enrichir les logs d&#39;envoi avec un champ de code segment ou avec un champ contenant l&#39;adresse IP de diffusion. Par exemple, vous pouvez enregistrer un code segment calculé pendant le workflow dans les logs d’envoi afin d’affiner la cible ultérieurement. Cela vous permettra de cibler les profils ayant ce code segment spécifique.

   1. **[!UICONTROL Exclusions]** : indiquez comment stocker les journaux d’exclusions.

   1. **[!UICONTROL Logs de tracking]** : activez l&#39;option **[!UICONTROL Générer un schéma pour le tracking]** afin de générer un schéma de stockage pour les logs de tracking

+++

1. Utilisez la section **[!UICONTROL Mapping]** pour identifier les attributs du schéma du mapping de ciblage à utiliser pour chaque champ d’adresse de diffusion. Pour chaque champ, sélectionnez l’attribut souhaité à mapper. Vous pouvez également créer une expression pour identifier le champ. Par exemple, vous pouvez appliquer une fonction inférieure à l’attribut address.

   ![](assets/target-mappings-mapping.png)

1. Lorsque votre mapping de ciblage est prêt, cliquez sur le bouton **[!UICONTROL Créer]**. Le système crée automatiquement le mapping de ciblage et tous les schémas associés pour les logs.

Une fois votre mapping de ciblage créé, deux sections supplémentaires s&#39;affichent à l&#39;écran :

* **** : cette section permet d&#39;identifier les attributs du schéma du mapping de ciblage à utiliser pour les Placer sur la liste bloquée places sur la liste bloquée.

  ![](assets/target-mappings-denylisting.png)

* **[!UICONTROL Stockage]** : cette section permet d’identifier les tables à utiliser pour stocker les logs.

  ![](assets/target-mappings-storage.png)

   * **[!UICONTROL Schéma des messages]** : identifie le schéma à utiliser pour stocker les logs d’envoi.
   * **[!UICONTROL Messages exclus]** : cette section explique comment gérer l’enregistrement des diffusions et des logs d’exclusion.

      * **[!UICONTROL Stocker les exclusions et messages dans la même table]**
      * **[!UICONTROL Stocker les messages uniquement]** : ne pas stocker les exclusions.
      * **[!UICONTROL Stocker les exclusions et les messages dans des tables distinctes]** : sélectionnez le schéma à utiliser pour stocker les logs d&#39;exclusion dans le champ **[!UICONTROL Schéma de rejet]**.

   * **[!UICONTROL Logs de tracking]** : choisissez où stocker les logs de tracking et la source du trafic par défaut.
   * **[!UICONTROL Champs supplémentaires]** : cette section permet de spécifier une liste de champs supplémentaires à stocker dans les logs de diffusion. Ces champs peuvent stocker en permanence des informations sur les membres individuels de la cible (par exemple, `recipient/@firstName`) ou stocker des données additionnelles calculées lors du workflow (par ex. `[targetData/@offeCode]`)

     Pour ce faire, sélectionnez **[!UICONTROL Ajouter un champ]**. Identifiez les informations que vous souhaitez enregistrer dans le champ **[!UICONTROL Source]** et l’attribut à utiliser dans les journaux d’envoi pour enregistrer ces informations dans le champ **[!UICONTROL Destination]**.

     ![](assets/target-mappings-additional.png){width="50%" zoomable="yes"}
