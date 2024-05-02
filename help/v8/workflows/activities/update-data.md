---
audience: end-user
title: Utilisation de l’activité de workflow Mise à jour de données
description: Découvrez comment utiliser l’activité de workflow Mise à jour de données
source-git-commit: 347f8f84a8eda60538366eb3dc49f8d7e06379c3
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 31%

---

# Mise à jour de données {#update-data}

La variable **Mise à jour de données** est une activité **Data Management** activité. Il permet de mettre à jour en masse les champs de la base de données. Plusieurs options permettent de personnaliser la mise à jour des données.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## Configuration de l’activité Mise à jour de données{#update-data-configuration}

Pour configurer la variable **Mise à jour de données** , commencez par ajouter l’activité à votre workflow et définissez un libellé.

![](../assets/workflow-update-data.png)

### Type d&#39;opération

Le champ **Type d&#39;opération** permet de choisir le traitement à réaliser sur les données de la base :

* **Insérer ou mettre à jour**: insérer des données ou les mettre à jour si les enregistrements existent déjà dans la base.
* **Insérer**: ajouter des données uniquement. Les enregistrements déjà existants ne sont pas mis à jour. Si des critères de réconciliation sont définis, seuls les enregistrements non réconciliés sont ajoutés.
* **Mettre à jour** : mettre à jour des données des enregistrements déjà présents en base uniquement.
* **Supprimer** : supprimer des données.

Le champ **Taille des mises à jours** permet de sélectionner le nombre d&#39;éléments de la transition entrante qui seront mis à jour. Par exemple, si vous indiquez 500, les 500 premiers enregistrements traités seront mis à jour.

### Identification des enregistrements

Cette section vous permet de définir comment identifier les enregistrements dans la base de données :

* Si les données en entrée correspondent à une dimension de ciblage existante, sélectionnez la variable **Utiliser la dimension de ciblage** et sélectionnez-la dans la **Dimension de ciblage à mettre à jour** champ .
* Vous pouvez également sélectionner la variable **Utilisation de liens personnalisés** et spécifier un ou plusieurs liens qui permettront d&#39;identifier les données de la base.
* Si le type d’opération sélectionné nécessite une mise à jour, vous devez utiliser la variable **Utiliser des règles de réconciliation** .

### Champs à mettre à jour

Dans le **Champs à mettre à jour** , ajoutez les champs sur lesquels sera appliquée la mise à jour et, au besoin, ajoutez des conditions pour que cette mise à jour soit réalisée. Pour ce faire, utilisez la méthode **Pris en compte si** champ . Les conditions sont appliquées les unes après les autres, dans l&#39;ordre de la liste. Utilisez les flèches situées à droite pour modifier l&#39;ordre des mises à jour. Vous pouvez utiliser plusieurs fois le même champ de destination.

Vous pouvez associer automatiquement les champs à l’aide de la variable **Mappage automatique** bouton . L&#39;association automatique détecte les champs portant le même nom.

Durant : **Insérer ou mettre à jour** type d’opération, vous pouvez sélectionner individuellement l’opération à appliquer pour chaque champ. Pour ce faire, sélectionnez la valeur souhaitée dans la variable **Type d&#39;opération** champ .

### Options avancées

La variable **Options avancées** permet de définir des options supplémentaires pour la mise à jour des données et la gestion des doublons.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Les deux dernières options permettent d’effectuer des actions spécifiques :

* **Générer une transition sortante**: crée une transition sortante qui sera activée à la fin de l&#39;exécution. La mise à jour marque généralement la fin d&#39;un workflow de ciblage et l&#39;option n&#39;est donc pas activée par défaut.

* **Générer une transition sortante pour les rejets**: crée une transition sortante contenant les enregistrements qui n&#39;ont pas été correctement traités après la mise à jour (par exemple en cas de doublon). La mise à jour marque généralement la fin d’un workflow de ciblage et l’option n’est donc pas activée par défaut.
