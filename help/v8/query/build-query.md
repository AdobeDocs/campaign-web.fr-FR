---
audience: end-user
title: Créez votre première requête à l’aide du créateur de modèles de requête.
description: Découvrez comment créer votre première requête dans Adobe Campaign Web query modeler.
source-git-commit: 119b7a65cb39d3cdfb225a673ae6452d2a5359fc
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 13%

---

# Créer votre première requête {#build-query}

Pour commencer à créer une requête, accédez au créateur de requêtes à partir de l’emplacement de votre choix, en fonction de l’action que vous souhaitez effectuer. Le modeleur de requête s’ouvre avec un canevas vierge. Cliquez sur le bouton + pour ajouter le premier noeud de votre requête.

![](assets/query-add-component.png)

Vous pouvez ajouter deux types d’éléments :

* Les composants de filtrage (Condition personnalisée, Sélectionner une audience, Filtre prédéfini) vous permettent de créer vos propres règles, de sélectionner une audience ou un filtre prédéfini pour affiner votre requête.

  Exemple *Destinataires qui se sont inscrits à la newsletter &quot;Sports&quot;*. *Destinataires résidant à New York*, *Destinataires résidant à San Francisco*

* Les opérateurs de groupe (ET, OU, SAUF) vous permettent de regrouper les composants de filtrage dans le diagramme en fonction de vos besoins.

  Exemple : *Destinataires qui se sont inscrits à la newsletter &quot;Sports&quot;**ET**qui vivent à New York **OU**San Francisco*.

Vous trouverez ci-dessous des étapes détaillées pour ajouter et combiner des composants de filtrage et des opérateurs de groupe.

## Ajouter des composants de filtrage

Les composants de filtrage vous permettent d’affiner votre requête à l’aide des éléments suivants :

* **Conditions personnalisées**: filtrez votre requête en créant votre propre condition avec des attributs de la base de données et des expressions avancées.
* **Audiences**: filtrez votre requête à l’aide d’une audience existante.
* **Filtre prédéfini**: filtrez votre requête à l’aide de filtres prédéfinis existants.

### Création d’une condition personnalisée

Pour filtrer votre requête à l’aide d’une condition personnalisée, procédez comme suit :

1. Cliquez sur le bouton + sur le noeud souhaité, puis sélectionnez **[!UICONTROL Condition personnalisée]**.
1. Le volet des propriétés de condition personnalisée s’ouvre sur le côté droit. Dans le champ Attribut , sélectionnez l’attribut de la base de données que vous souhaitez utiliser pour créer votre condition.

   Les attributs disponibles représentent tous les champs de la base de données Campaign, y compris les champs des tables liées à la table Destinataires .

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Le bouton Editer l&#39;expression permet d&#39;utiliser l&#39;éditeur d&#39;expression Web de Campaign pour définir manuellement une expression à l&#39;aide de champs de la base de données et de fonctions d&#39;assistance.

1. Sélectionnez l&#39;opérateur à appliquer dans la liste déroulante.

   +++Liste des opérateurs disponibles

   >[!NOTE]
   >
   >Les opérateurs disponibles dans la liste déroulante dépendent du type de données de l&#39;attribut sélectionné.

   | Opérateur | Intérêt | Exemple |
   |  ---  |  ---  |  ---  |
   | Egal à | Retrouver un résultat rigoureusement identique à ce qui est entré dans la seconde colonne Valeur. | Nom (@lastName) égal à &#39;Jones&#39;, ne renverra que les destinataires dont le nom est &#39;Martin&#39;. |
   | Différent de | Le résultat retourné ne doit pas être identique à la valeur renseignée. | Langue (@language) égale à &#39;Anglais&#39; |
   | Supérieur à | Obtenir un résultat supérieur à la valeur indiquée. | Age (@age) supérieur à 50 ans</strong>, renvoie toutes les valeurs supérieures à &quot;50&quot;, c’est-à-dire &quot;51&quot;, &quot;52&quot;, etc. |
   | Inférieur à | Obtenir un résultat inférieur à la valeur indiquée. | Date de création (@created) avant &quot;DaysAgo(100)&quot;</strong>, renverra tous les destinataires créés il y a moins de 100 jours. |
   | Supérieur ou égal à | Obtenir un résultat rigoureusement égal ou supérieur à la valeur renseignée. | Age (@age) supérieur ou égal à &#39;30&#39;</strong>, renverra tous les destinataires âgés de 30 ans ou plus. |
   | Inférieur ou égal à | Obtenir un résultat rigoureusement égal ou inférieur à la valeur renseignée. | Age (@age) inférieur ou égal à &#39;60&#39;</strong>, renverra tous les destinataires âgés de 60 ans ou moins. |
   | Inclus dans | Obtenir les résultats compris dans les valeurs indiquées. Ces valeurs doivent toujours être séparées par une virgule. | La date de naissance (@birthDate) est incluse dans &#39;12/10/1979,12/10/1984&#39;, renverra les destinataires nés entre ces dates. |
   | Not in | Fonctionne comme l’opérateur Est inclus dans . Ici, nous allons exclure les destinataires en fonction des valeurs renseignées. | La date de naissance (@birthDate) n’est pas incluse dans &quot;12/10/1979,12/10/1984&quot;. Contrairement à l’exemple précédent, les destinataires nés à cette date ne seront pas renvoyés. |
   | Est vide | Dans ce cas, le résultat recherché correspond à une valeur vide dans la seconde colonne Valeur. | Le champ Mobile (@mobilePhone) est vide renvoie tous les destinataires qui n&#39;ont pas de numéro de mobile. |
   | N&#39;est pas vide | Revient à l’opérateur Est vide . Il n&#39;est pas nécessaire de saisir des données dans la seconde colonne Valeur. | Email (@email) n&#39;est pas vide. |
   | Commence par | Obtenir des résultats commençant par la valeur indiquée. | N° de compte (@account) commence par &#39;32010&#39;. |
   | Ne commence pas par | Obtenir des résultats qui ne commencent pas par la valeur renseignée | N° de compte (@account) ne commence pas par &quot;20&quot; |
   | contient | Obtenir un résultat comportant au moins la valeur qui est renseignée. | Domaine de l&#39;email (@domain) contient &#39;mail&#39;</strong>, renverra tous les noms de domaine contenant &quot;mail&quot;. Le domaine &#39;gmail.com&#39; sera donc également retourné. |
   | Ne contient pas | Ne pas obtenir de résultats contenant au moins la valeur renseignée. | Domaine de l&#39;email (@domain) ne contient pas &#39;vo&#39;</strong>. Dans ce cas, les noms de domaine contenant &quot;vo&quot; ne seront pas renvoyés. Le nom de domaine &#39;voila.fr&#39; n&#39;apparaîtra pas dans les résultats. |
   | Comme | Comme est très similaire à l’opérateur Contient . Il vous permet d’insérer un caractère joker % dans la valeur. | Nom (@lastName) comme &#39;Jon%s&#39;. Ici, le caractère joker est utilisé comme &quot;joker&quot; pour trouver le nom &quot;Jones&quot;, si l&#39;opérateur a oublié la lettre manquante entre le &#39;n&#39; et le &#39;s&#39;. |
   | Pas comme | Comme est très similaire à l’opérateur Contient . Il vous permet d’insérer un caractère joker % dans la valeur. | Nom (@lastName) différent de &#39;Smi%h&#39;. Ici, les destinataires dont le nom est &#39;Smi%h&#39; ne seront pas retournés. |

+++

1. Dans le champ Valeur , sélectionnez la valeur attendue.

   Vous pouvez également utiliser l&#39;éditeur d&#39;expression Web de Campaign pour définir manuellement une expression à l&#39;aide de champs de la base de données et de fonctions d&#39;assistance. Pour cela, cliquez sur le bouton Editer l&#39;expression .

   *Exemple : requête retournant tous les profils âgés de 21 ans ou plus*

   ![](assets/query-custom-condition.png)

<!--
querying linked tables
collect additional information on the targeted population, e.g. contract numbers, subscriptions to newsletters or origin.
Select the type of data you want to add. This can be data belonging to the filtering dimension or data stored in linked tables. Select the table which contains the information you want to collect and click Next.

aggregates: Define a calculation mode for the field to be added, such as an aggregate for example.-->

### Sélectionner une audience

Pour filtrer votre requête à l&#39;aide d&#39;une audience existante, procédez comme suit :

1. Cliquez sur le bouton + sur le noeud souhaité, puis sélectionnez **[!UICONTROL Sélection de l’audience]**.

1. Le volet de sélection des propriétés de l’audience s’ouvre sur le côté droit. Sélectionnez l’audience que vous souhaitez utiliser pour filtrer votre requête.

   *Exemple : requête renvoyant tous les profils appartenant à l’audience &quot;Goers du festival&quot;*

   ![](assets/query-audience.png)

### Utiliser un filtre prédéfini

Pour filtrer votre requête à l’aide d’un filtre prédéfini, procédez comme suit :

1. Cliquez sur le bouton + sur le noeud souhaité, puis sélectionnez **[!UICONTROL Filtre prédéfini]**.

1. Le volet de sélection des propriétés de l’audience s’ouvre sur le côté droit. Sélectionnez un filtre prédéfini dans la liste des filtres personnalisés ou des favoris.

   *Exemple : requête retournant tous les profils correspondant au filtre prédéfini &quot;Clients inactifs&quot;.*

   ![](assets/query-predefined-filter.png)

## Combiner des composants de filtrage avec des opérateurs

Lors de l&#39;ajout d&#39;un composant de filtrage à votre requête, une nouvelle transition est automatiquement créée sur le canevas de la requête, et le nouveau composant de filtrage est lié au premier par un opérateur AND. Cela signifie que les résultats des deux composants de filtrage sont combinés dans les résultats de la requête.

Dans cet exemple, de nouveaux composants de filtrage de type audience sont ajoutés à la zone de travail. Il est automatiquement ajouté sur une nouvelle transition et associé à la condition de type filtre prédéfinie avec un opérateur AND. Dans ce cas, les résultats de la requête incluent les destinataires ciblés par le filtre prédéfini &quot;Madridiens&quot; ET appartenant à l&#39;audience &quot;chasseurs de remises&quot;.

![](assets/query-operator.png)

Pour changer l&#39;opérateur utilisé pour associer les conditions de filtrage, cliquez dessus et sélectionnez l&#39;opérateur désiré dans la section Vous pouvez changer l&#39;opérateur en cliquant dessus et en sélectionnant l&#39;opérateur désiré dans le volet Groupe qui s&#39;ouvre sur la droite.

![](assets/query-operator-change.png)

Les opérateurs disponibles sont les suivants :

* AND (Intersection) : combine les résultats de tous les composants de filtrage dans les transitions sortantes.
* OR (Union) : regroupe les résultats d&#39;au moins un des composants de filtrage dans les transitions sortantes.
* SAUF (Exclusion) : exclut les résultats de tous les composants de filtrage de la transition sortante.

## Vérifier et valider votre requête

Une fois votre requête créée dans la zone de travail, vous pouvez la vérifier à l’aide du volet Propriétés de la règle situé sur le côté droit. Les opérations disponibles sont les suivantes :

* **Afficher les résultats :** affiche les données issues de votre requête.
* **Affichage du code**: affiche une version de la requête basée sur un code dans SQL.
* **Calculer**: met à jour et affiche le nombre d&#39;enregistrements ciblés par votre requête.
* **Sélectionner ou enregistrer un filtre**: choisissez un filtre prédéfini existant à utiliser dans la zone de travail ou enregistrez votre requête en tant que filtre prédéfini pour une réutilisation ultérieure. [Découvrez comment utiliser des filtres prédéfinis](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >Sélectionnez un filtre prédéfini dans le volet Propriétés de la règle pour remplacer la requête qui a été créée dans la zone de travail par le filtre sélectionné.
