---
audience: end-user
title: Créez votre première requête à l’aide du créateur de modèles de requête.
description: Découvrez comment créer votre première requête dans Adobe Campaign Web query modeler.
source-git-commit: cc909bdf7507e66e000297440e31f9b5260f1257
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 15%

---

# Créer votre première requête {#build-query}

Pour commencer à créer une requête, accédez au créateur de requêtes à partir de l’emplacement de votre choix, en fonction de l’action que vous souhaitez effectuer. Le modeleur de requête s’ouvre avec un canevas vierge. Cliquez sur le bouton **+** pour configurer le premier noeud de votre requête.

Vous pouvez ajouter deux types d’éléments :

* **Filtrage des composants** (Condition personnalisée, Sélectionner une audience, Filtre prédéfini) vous permettent de créer vos propres règles, de sélectionner une audience ou un filtre prédéfini pour affiner votre requête. [Découvrez comment utiliser les composants de filtrage](#filtering)

  Exemple :

  *Destinataires qui se sont inscrits à la newsletter &quot;Sports&quot;*. *Destinataires résidant à New York*, *Destinataires résidant à San Francisco*

* **Opérateurs de groupe** (ET, OU, SAUF) vous permettent de regrouper les composants de filtrage dans le diagramme en fonction de vos besoins. [Découvrez comment travailler avec des opérateurs](#filtering)

  Exemple :

  *Destinataires qui se sont inscrits à la newsletter &quot;Sports&quot;**ET**qui vivent à New York **OU**San Francisco*.

![](assets/query-add-component.png)

## Ajouter des composants de filtrage {#filtering}

Les composants de filtrage vous permettent d’affiner votre requête à l’aide des éléments suivants :

* **Conditions personnalisées**: filtrez votre requête en créant votre propre condition avec des attributs de la base de données et des expressions avancées.
* **Audiences**: filtrez votre requête à l’aide d’une audience existante.
* **Filtre prédéfini**: filtrez votre requête à l’aide de filtres prédéfinis existants.

### Configuration d’une condition personnalisée

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condition personnalisée"
>abstract="Condition personnalisée"

Pour filtrer votre requête à l’aide d’une condition personnalisée, procédez comme suit :

1. Cliquez sur le bouton **+** sur le noeud souhaité, puis sélectionnez **[!UICONTROL Condition personnalisée]**. Le volet des propriétés de condition personnalisée s’ouvre sur le côté droit.

1. Dans le **Attribut** , sélectionnez l’attribut de la base de données que vous souhaitez utiliser pour créer votre condition. La liste des attributs comprend tous les attributs de votre base de données Campaign, y compris les attributs liés à votre table.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Le bouton Editer l&#39;expression permet d&#39;utiliser l&#39;éditeur d&#39;expression Web de Campaign pour définir manuellement une expression à l&#39;aide de champs de la base de données et de fonctions d&#39;assistance.

1. Sélectionnez l&#39;opérateur à appliquer dans la liste déroulante. Plusieurs opérateurs sont disponibles. Notez que les opérateurs disponibles dans la liste déroulante dépendent du type de données de l&#39;attribut sélectionné.

   +++Liste des opérateurs disponibles

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

1. Dans le **Valeur** , définissez la valeur attendue. Vous pouvez également utiliser l&#39;éditeur d&#39;expression Web de Campaign pour définir manuellement une expression à l&#39;aide de champs de la base de données et de fonctions d&#39;assistance. Pour ce faire, cliquez sur le bouton **Expression d’édition** bouton .

   *Exemple de requête renvoyant tous les profils âgés de 21 ans ou plus :*

   ![](assets/query-custom-condition.png)

### Sélectionner une audience

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Sélectionner une audience"
>abstract="Sélectionner une audience"

Pour filtrer votre requête à l&#39;aide d&#39;une audience existante, procédez comme suit :

1. Cliquez sur le bouton **+** sur le noeud souhaité, puis choisissez **[!UICONTROL Sélection de l’audience]**.

1. La variable **Sélection de l’audience** le volet Propriétés s’ouvre sur le côté droit. Sélectionnez l&#39;audience que vous souhaitez utiliser pour filtrer votre requête.

   *Exemple de requête retournant tous les profils appartenant à l&#39;audience &quot;Goers du festival&quot; :*

   ![](assets/query-audience.png)

### Utiliser un filtre prédéfini

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtre prédéfini"
>abstract="Filtre prédéfini"

Pour filtrer votre requête à l’aide d’un filtre prédéfini, procédez comme suit :

1. Cliquez sur le bouton **+** sur le noeud souhaité, puis sélectionnez **[!UICONTROL Filtre prédéfini]**.

1. La variable **Filtre prédéfini** le volet Propriétés s’ouvre sur le côté droit. Sélectionnez un filtre prédéfini dans la liste des filtres personnalisés ou des favoris.

   *Exemple de requête retournant tous les profils correspondant au filtre prédéfini &quot;Clients inactifs&quot; :*

   ![](assets/query-predefined-filter.png)

## Combiner des composants de filtrage avec des opérateurs {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Groupe"
>abstract="Groupe"

Chaque fois que vous ajoutez un nouveau composant de filtrage à votre requête, il est automatiquement lié à l’autre composant par un opérateur AND. Cela signifie que les résultats des deux composants de filtrage sont combinés dans les résultats de la requête.

Dans cet exemple, nous avons ajouté de nouveaux composants de filtrage de type audience sur la seconde transition. Le composant est lié à la condition de type de filtre prédéfinie avec un opérateur AND, ce qui signifie que les résultats de la requête incluent les destinataires ciblés par le filtre prédéfini &quot;Madridians&quot; ET appartenant à l&#39;audience &quot;chasseurs de remises&quot;.

![](assets/query-operator.png)

Pour changer l&#39;opérateur utilisé pour relier les conditions de filtrage, cliquez dessus et sélectionnez l&#39;opérateur désiré dans le volet Groupe qui s&#39;ouvre sur la droite.

Les opérateurs disponibles sont les suivants :

* **AND (Intersection)**: combine les résultats de tous les composants de filtrage dans les transitions sortantes.
* **OU (Union)**: inclut les résultats d’au moins un des composants de filtrage dans les transitions sortantes.
* **SAUF (Exclusion)**: exclut les résultats de tous les composants de filtrage de la transition sortante.

![](assets/query-operator-change.png)

## Vérifier et valider votre requête

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Propriétés de la règle"
>abstract="Propriétés de la règle"

Une fois que vous avez créé votre requête dans la zone de travail, vous pouvez la vérifier à l’aide de la fonction **Propriétés des règles** situé sur le côté droit. Les opérations disponibles sont les suivantes :

* **Afficher les résultats :** Affiche les données issues de votre requête.
* **Affichage du code**: affiche une version de la requête basée sur un code dans SQL.
* **Calculer**: met à jour et affiche le nombre d&#39;enregistrements ciblés par votre requête.
* **Sélectionner ou enregistrer un filtre**: sélectionnez un filtre prédéfini existant à utiliser dans la zone de travail ou enregistrez votre requête en tant que filtre prédéfini pour une réutilisation ultérieure. [Découvrez comment utiliser des filtres prédéfinis](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >Sélectionnez un filtre prédéfini dans le volet Propriétés de la règle pour remplacer la requête qui a été créée dans la zone de travail par le filtre sélectionné.
