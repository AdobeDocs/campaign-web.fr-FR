---
audience: end-user
title: Utilisation de l’activité de workflow Partage
description: Découvrez comment utiliser l’activité de workflow Partage
badge: label="Alpha"
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---


# Partage {#split}

Le **Partage** est une activité **Ciblage** activité permettant de segmenter les populations entrantes en plusieurs sous-ensembles selon différents critères de sélection, tels que les règles de filtrage ou la taille de la population.

## Configuration {#general}

Procédez comme suit pour configurer la variable **Partage** activité :

1. Ajouter un **Partage** à votre workflow.

1. Le volet de configuration des activités s’ouvre avec un sous-ensemble par défaut. Cliquez sur le bouton **Ajouter un segment** pour ajouter autant de sous-ensembles que vous le souhaitez pour segmenter la population entrante.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Lorsque l&#39;activité Partage est exécutée, la population est segmentée entre les différents sous-ensembles dans l&#39;ordre dans lequel elle est ajoutée à l&#39;activité. Par exemple, si le premier sous-ensemble récupère 70 % de la population initiale, le sous-ensemble ajouté suivant n’appliquera ses critères de sélection qu’aux 30 % restants, etc.
   >
   > Avant de configurer vos sous-ensembles, assurez-vous de les avoir ajoutés dans l&#39;ordre approprié, car leur position ne peut pas être modifiée.

1. Une fois les sous-ensembles ajoutés, l&#39;activité affiche autant de transitions en sortie que de sous-ensembles. Nous vous recommandons vivement de modifier le libellé de chaque sous-ensemble afin de les identifier facilement dans la zone de travail du workflow.

1. Configurez la manière dont chaque sous-ensemble doit filtrer la population entrante. Pour ce faire, procédez comme suit :

   1. Ouvrez le sous-ensemble pour afficher ses propriétés.

   1. Pour appliquer une condition de filtrage au sous-ensemble, cliquez sur **[!UICONTROL Créer un filtre]** et configurez la règle de filtrage souhaitée. Par exemple, incluez les profils de la population entrante dont l&#39;adresse email existe dans la base de données.

   1. Pour limiter le nombre de profils sélectionnés par le sous-ensemble, activez la fonction **[!UICONTROL Activer la limite]** et indiquez le nombre ou les pourcentages de la population à inclure.

      >[!NOTE]
      >
      >Lorsque vous définissez une limite de population pour un sous-ensemble, vous pouvez classer les profils sélectionnés en fonction d&#39;un attribut de profil spécifique, dans un ordre croissant ou décroissant. Pour ce faire, activez la fonction **[!UICONTROL Activation du tri]** . Par exemple, vous pouvez restreindre un sous-ensemble afin de n&#39;inclure que les 50 premiers profils ayant le montant d&#39;achat le plus élevé.

   ![](../assets/workflow-split-subset.png)

1. Une fois que vous avez paramétré tous les sous-ensembles, vous pouvez sélectionner la population restante qui ne correspond à aucun des sous-ensembles et les inclure dans une transition sortante supplémentaire. Pour ce faire, activez la fonction **[!UICONTROL Générer le complémentaire]** .

   ![](../assets/workflow-split-complement.png)

L’activité est maintenant configurée. Lors de l&#39;exécution du workflow, la population sera segmentée dans les différents sous-ensembles, dans l&#39;ordre dans lequel elle a été ajoutée à l&#39;activité.

## Exemple

Dans l’exemple suivant, la variable **[!UICONTROL Partage]** L’activité sert à segmenter une audience en sous-ensembles distincts en fonction du canal de communication que nous voulons utiliser :

* **Sous-ensemble 1 &quot;push&quot;**: Ce sous-ensemble comprend tous les profils ayant installé notre application mobile.
* **Sous-ensemble 2 &quot;sms&quot;**: Utilisateurs de téléphone mobile : Pour la population restante qui n&#39;a pas fait partie du sous-ensemble 1, le sous-ensemble 2 applique une règle de filtrage afin de sélectionner les profils avec des téléphones mobiles dans la base de données.
* **Transition complémentaire**: Cette transition capture tous les profils restants qui ne correspondent pas au sous-ensemble 1 ou au sous-ensemble 2. Plus précisément, il inclut les profils qui n’ont pas installé l’application mobile ou qui n’ont pas de téléphone mobile, tels que les utilisateurs qui n’ont pas installé l’application mobile ou qui ne disposent pas d’un numéro de mobile enregistré.

![](../assets/workflow-split-example.png)
