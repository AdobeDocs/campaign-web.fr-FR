---
audience: end-user
title: Utiliser l’activité de workflow Partage
description: Découvrez comment utiliser l’activité de workflow Partage.
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 90%

---

# Partage {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Activité Partage"
>abstract="L’activité **Partage** permet de segmenter les populations entrantes en plusieurs sous-ensembles selon différents critères de sélection, tels que les règles de filtrage ou la taille de la population."

L’activité **Partage** est une activité de **ciblage** vous permettant de segmenter les populations entrantes en plusieurs sous-ensembles selon différents critères de sélection, tels que les règles de filtrage ou la taille de la population.

## Configurer l’activité Partage {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segments de l’activité de partage"
>abstract="Ajoutez autant de sous-ensembles que vous le souhaitez pour segmenter la population entrante.<br/></br>Lorsque l’activité **Partage** est exécutée, la population est segmentée entre les différents sous-ensembles dans l’ordre dans lequel ils sont ajoutés à l’activité. Avant de démarrer votre workflow, assurez-vous d’avoir trié les sous-ensembles dans l’ordre qui vous convient à l’aide des boutons fléchés."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Filtre de l’activité Partage"
>abstract="Pour appliquer une condition de filtrage au sous-ensemble, cliquez sur **[!UICONTROL Créer un filtre]** et configurez la règle de filtrage de votre choix à l’aide du modèle de requête. Par exemple, incluez les profils de la population entrante dont l’adresse e-mail existe dans la base de données."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Utiliser le concepteur de requête"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Limite de l’activité Partage"
>abstract="Pour limiter le nombre de profils sélectionnés par le sous-ensemble, activez la fonction **[!UICONTROL Activer la limite]** et indiquez le nombre ou les pourcentages de la population à inclure."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Tri de l’activité Partage"
>abstract="Lorsque vous définissez une limite de population pour un sous-ensemble, vous pouvez classer les profils sélectionnés en fonction d’un attribut de profil spécifique, dans un ordre croissant ou décroissant. Pour ce faire, activez l’option **Activer le tri**. Par exemple, vous pouvez restreindre un sous-ensemble afin de n’inclure que les 50 premiers profils ayant le montant d’achat le plus élevé."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Partager le complément de génération"
>abstract="Une fois que vous avez paramétré tous les sous-ensembles, vous pouvez sélectionner la population restante qui ne correspond à aucun des sous-ensembles et les inclure dans une transition sortante supplémentaire. Pour ce faire, activez l’option **Générer le complémentaire**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Générer tous les sous-ensembles dans le même tableau"
>abstract="Activez cette option pour regrouper tous les sous-ensembles en une seule transition de sortie."

Pour configurer l’activité **Partage**, procédez comme suit :

1. Ajoutez une activité **Partage** à votre workflow.

1. Le volet de configuration des activités s’ouvre avec un sous-ensemble par défaut. Cliquez sur le bouton **Ajouter un segment** pour ajouter autant de sous-ensembles que vous le souhaitez pour segmenter la population entrante.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Lorsque l’activité **Partage** est exécutée, la population est segmentée entre les différents sous-ensembles dans l’ordre dans lequel ils sont ajoutés à l’activité. Par exemple, si le premier sous-ensemble récupère 70 % de la population initiale, le sous-ensemble ajouté suivant n’appliquera ses critères de sélection qu’aux 30 % restants, etc.
   >
   >Avant de démarrer votre workflow, vérifiez que vous avez trié les sous-ensembles dans l’ordre qui vous convient. Pour ce faire, utilisez les boutons fléchés pour changer la position d’un sous-ensemble.

1. Une fois les sous-ensembles ajoutés, l’activité propose autant de transitions en sortie que de sous-ensembles : Nous vous recommandons vivement de modifier le libellé de chaque sous-ensemble afin de les identifier facilement dans la zone de travail du workflow.

1. Configurez la manière dont chaque sous-ensemble doit filtrer la population entrante. Pour ce faire, procédez comme suit :

   1. Ouvrez le sous-ensemble pour afficher ses propriétés.

   1. Pour appliquer une condition de filtrage au sous-ensemble, cliquez sur **[!UICONTROL Créer un filtre]** et configurez la règle de filtrage de votre choix à l’aide du modèle de requête. Par exemple, incluez les profils de la population entrante dont l&#39;adresse email existe dans la base de données. [Découvrez comment utiliser le concepteur de requêtes](../../query/query-modeler-overview.md).

   1. Pour limiter le nombre de profils sélectionnés par le sous-ensemble, activez la fonction **[!UICONTROL Activer la limite]** et indiquez le nombre ou les pourcentages de la population à inclure.

      ![](../assets/workflow-split-subset.png)


      >[!NOTE]
      >
      >Lorsque vous définissez une limite de population pour un sous-ensemble, vous pouvez classer les profils sélectionnés en fonction d’un attribut de profil spécifique, dans un ordre croissant ou décroissant. Pour ce faire, activez l’option **[!UICONTROL Activer le tri]**. Par exemple, vous pouvez restreindre un sous-ensemble afin de n’inclure que les 50 premiers profils ayant le montant d’achat le plus élevé.

1. Une fois que vous avez paramétré tous les sous-ensembles, vous pouvez sélectionner la population restante qui ne correspond à aucun des sous-ensembles et les inclure dans une transition sortante supplémentaire. Pour ce faire, activez l’option **[!UICONTROL Générer le complémentaire]**.

   ![](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >La variable **[!UICONTROL Générer tous les sous-ensembles dans la même table]** permet de regrouper tous les sous-ensembles dans une seule transition sortante.

L’activité est désormais configurée. Lors de l’exécution du workflow, la population sera segmentée dans les différents sous-ensembles, dans l’ordre dans lequel ils ont été ajoutés à l’activité.

## Exemple{#split-example}

Dans l’exemple suivant, l’activité **[!UICONTROL Partage]** sert à segmenter une audience en sous-ensembles distincts en fonction du canal de communication que nous voulons utiliser :

* **Sous-ensemble 1 « notification push »** : ce sous-ensemble comprend tous les profils ayant installé notre application mobile.
* **Sous-ensemble 2 « SMS »** : utilisateurs et utilisatrices de téléphone mobile : pour la population restante qui ne faisait pas partie du sous-ensemble 1, le sous-ensemble 2 applique une règle de filtrage afin de sélectionner les profils avec des téléphones mobiles dans la base de données.
* **Transition complémentaire** : cette transition capture tous les profils restants qui ne correspondent pas au sous-ensemble 1 ou au sous-ensemble 2. Plus précisément, elle inclut les profils qui n’ont pas installé l’application mobile ou qui n’ont pas de téléphone mobile, tels que les utilisateurs et utilisatrices qui n’ont pas installé l’application mobile ou qui ne disposent pas d’un numéro de mobile enregistré.

![](../assets/workflow-split-example.png)
