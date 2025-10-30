---
audience: end-user
title: Créer votre première requête à l’aide du créateur de modèles de requête
description: Découvrez comment créer votre première requête dans le créateur de modèles de requête Adobe Campaign Web.
exl-id: efd762b5-a7ae-49b4-ab74-5b43da1e574d
source-git-commit: 6a2bc8f2c36db04c466ed51a96e281156b224d48
workflow-type: tm+mt
source-wordcount: '2921'
ht-degree: 100%

---


# Créer votre première requête {#build-query}

Pour commencer à créer une requête, accédez au concepteur de requête à partir de l’emplacement de votre choix, en fonction de l’action que vous souhaitez effectuer. Le concepteur de requête s’ouvre et affiche une zone de travail vierge. Cliquez sur le bouton **+** pour configurer le premier nœud de votre requête.

>[!IMPORTANT]
>
>Une toute nouvelle interface pour le concepteur de requête est disponible. Le nouveau créateur de règles, grâce à son interface simplifiée, vous permet de créer votre requête plus facilement. Pour passer à cette expérience, appuyez sur le bouton (bascule) dans le coin supérieur droit. Vous pouvez revenir au concepteur de requête classique à tout moment en appuyant simplement sur le bouton (bascule) pour désactiver la nouvelle interface. Vous pouvez appliquer les mêmes principes que le concepteur de requête dans cette nouvelle interface.
>>![Image montrant le bouton (bascule) de la nouvelle interface du créateur de règles](assets/query-modeler-toggle.png){zoomable="yes"}

Vous pouvez ajouter deux types d’éléments :

* Les **composants de filtrage** (condition personnalisée, audience sélectionnée, filtre prédéfini) vous permettent de créer vos propres règles, de sélectionner une audience ou d’utiliser un filtre prédéfini pour affiner votre requête. Ils sont ajoutés au début de votre requête et sur les transitions en pointillés. [Découvrir comment utiliser les composants de filtrage](#filtering)

  Exemple : *personnes destinataires abonnées à la newsletter « Sports »*, *personnes destinataires résidant à New York*, *personnes destinataires résidant à San Francisco*.

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

![Exemple d’ajout de composants de filtrage à une requête.](assets/query-add-component.png){zoomable="yes"}


>[!TAB Nouveau créateur de règles]

![Exemple d&#39;ajout de composants de filtrage à une requête.](assets/ruleb-1.png){zoomable="yes"}

>[!ENDTABS]



* Les **opérateurs de groupe** (ET, OU, SAUF) vous permettent de regrouper les composants de filtrage dans le diagramme. Ils sont ajoutés sur les transitions existantes avant un composant de filtrage. [Découvrir comment utiliser les opérateurs](#filtering)

  Exemple : * Destinataires Super VIP **ET** VIP pour récompenser les destinataires **OU** Démo VIP, **SAUF** âgés de moins de 21 ans et de plus de 45 ans.

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

![Description : exemple d’ajout d’opérateurs de groupe à une requête.](assets/ruleb-13.png){zoomable="yes"}

>[!TAB Nouveau créateur de règles]

![Exemple d’ajout de composants de filtrage à une requête.](assets/ruleb-14.png){zoomable="yes"}

>[!ENDTABS]


## Répartition des valeurs dans une requête {#distribution-values-query}

La répartition des valeurs affiche le pourcentage de chaque valeur d’un champ dans un tableau, selon les paramètres de requête actuels. Connaître la répartition des valeurs dans une requête peut vous aider à affiner votre segmentation.

Pour accéder à cette option, dans votre requête, cliquez sur le bouton de sélection d’attribut comme illustré ci-dessous. Cliquez ensuite sur l’icône **[!UICONTROL Informations]** en regard de l’attribut sélectionné. Vous pouvez accéder au bouton **[!UICONTROL Répartition des valeurs]**.

![Description : accès à l’option de répartition des valeurs dans une requête.](assets/values_query.png){zoomable="yes"}

>[!NOTE]
>
>* Pour les champs comportant de nombreuses valeurs, seules les vingt premières valeurs sont affichées. Dans ce cas, une notification **[!UICONTROL Chargement partiel]** vous en informe.
>* L’option **[!UICONTROL Répartition des valeurs]** est accessible dans chaque sélecteur d’attributs. [Découvrir comment sélectionner des attributs](../get-started/attributes.md)
>* Vous pouvez ajouter des conditions sur les résultats à l’aide des **[!Afiltres avancés]**. [En savoir plus ici](../get-started/work-with-folders.md#filter-the-values).

## Ajouter des composants de filtrage {#filtering}

Les composants de filtrage vous permettent d’affiner votre requête à l’aide des éléments suivants :

* **[Conditions personnalisées](#custom-condition)** : filtrez votre requête en créant votre propre condition avec des attributs de la base de données et des expressions avancées.
* **[Audiences](#audiences)** : filtrez votre requête à l’aide d’une audience existante.
* **[Filtre prédéfini](#predefined-filters)** : filtrez votre requête à l’aide de filtres prédéfinis existants.

### Configurer une condition personnalisée {#custom-condition}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condition personnalisée"
>abstract="Les conditions personnalisées sont des composants de filtrage qui vous permettent de filtrer votre requête en créant votre propre condition avec des attributs de la base de données et des expressions avancées."

Pour filtrer votre requête à l’aide d’une condition personnalisée, procédez comme suit :

1. Cliquez sur le bouton **+** sur le nœud souhaité, puis sélectionnez **[!UICONTROL Condition personnalisée]**. Le volet des propriétés de condition personnalisée s’ouvre sur le côté droit.

1. Dans le champ **Attribut**, sélectionnez l’attribut de la base de données que vous souhaitez utiliser pour créer votre condition. La liste des attributs comprend tous les attributs de votre base de données de campagne, y compris les attributs de vos tableaux liés. [Découvrir comment sélectionner des attributs et les ajouter aux favoris](../get-started/attributes.md)

   ![Sélection des attributs d’une condition personnalisée dans une requête.](assets/query-custom-condition-fields.png){zoomable="yes"}

   >[!NOTE]
   >
   >Le bouton **Modifier une expression** permet d’utiliser l’éditeur d’expression de Campaign Web pour définir manuellement une expression à l’aide de champs de la base de données et de fonctions d’assistance. [Découvrez comment modifier des expressions](expression-editor.md)

1. Sélectionnez l’opérateur à appliquer dans la liste déroulante. Différents opérateurs sont disponibles. Notez que les opérateurs disponibles dans la liste déroulante dépendent du type de données de l’attribut.

   +++Liste des opérateurs disponibles

   | Opérateur | Intérêt | Exemple |
   |---|---|---|
   | Égal à | Obtenir un résultat rigoureusement identique à ce qui est entré dans la seconde colonne Valeur. | Nom (@lastName) égal à « Jones ». Ici ne seront renvoyées que les personnes destinataires dont le nom est « Jones ». |
   | Différent de | Obtenir un résultat différent de la valeur renseignée. | Langue (@language) différente de « Anglais ». |
   | Supérieur à | Obtenir un résultat supérieur à la valeur indiquée. | Age (@age) supérieur à 50 renvoie toutes les valeurs supérieures à « 50 », donc « 51 », « 52 », etc. |
   | Inférieur à | Obtenir un résultat inférieur à la valeur indiquée. | Date de création (@created) plus tôt que « DaysAgo(100) » renvoie toutes les personnes destinataires créées il y a moins de 100 jours. |
   | Supérieur ou égal à | Obtenir un résultat rigoureusement égal ou supérieur à la valeur renseignée. | Age (@age) supérieur ou égal à « 30 » renvoie toutes les personnes destinataires dont l’âge est de 30 ans ou plus. |
   | Inférieur ou égal à | Obtenir un résultat rigoureusement égal ou inférieur à la valeur renseignée. | Âge (@age) inférieur ou égal à « 60 », afin de retrouver les personnes destinataires dont l’âge est de 60 ans et moins. |
   | Compris dans | Obtenir les résultats compris dans les valeurs indiquées. Ces valeurs doivent être séparées par une virgule. | Date de naissance (@birthDate) est compris dans « 12/10/1979,12/10/1984 ». Les personnes destinataires nées entre ces dates sont alors renvoyées. |
   | Pas dans | Le principe est le même qu’avec l’opérateur Est compris dans. Ici, les personnes destinataires sont exclues en fonction des valeurs saisies. | La date de naissance (@birthDate) n’est pas incluse dans 12/10/1979,12/10/1984. Les personnes destinataires nées entre ces dates ne seront pas renvoyées. |
   | Est vide | Renvoie les résultats correspondant à une valeur vide dans la seconde colonne Valeur. | Mobile (@mobilePhone) est vide afin de retrouver toutes les personnes destinataires ne disposant pas d’un numéro de téléphone mobile. |
   | N’est pas vide | Le principe est contraire à l’opérateur Est vide. Il n’est pas nécessaire de saisir de données dans la seconde colonne Valeur. | E-mail (@email) n’est pas vide. |
   | Commence par | Renvoie des résultats commençant par la valeur indiquée. | N° de compte (@account) commence par « 32010 ». |
   | Ne commence pas par | Renvoie les résultats qui ne commencent pas par la valeur renseignée. | N° de compte (@account) ne commence pas par « 20 ». |
   | Contient | Renvoies les résultats comportant au moins la valeur renseignée. | Domaine d’e-mail (@domain) contient « mail ». Ici, tous les noms de domaine comportant la valeur « mail », comme « gmail.com », seront renvoyés en résultat. |
   | Ne contient pas | Ne pas obtenir de résultats contenant au moins la valeur renseignée. | Domaine d’e-mail (@domain) ne contient pas « vo ». Les noms de domaine contenant « vo », tels que « voila.fr », n’apparaîtront pas dans les résultats. |
   | Comme | Quasiment identique à l’opérateur « Contient ». Il permet d’insérer un caractère générique « % » dans la valeur. | Nom (@lastName) comme « Jon%s ». Le caractère générique agit comme un « joker » pour trouver des noms tels que « Jones ». |
   | Pas comme | Quasiment identique à l’opérateur « Contient ». Il permet d’insérer un caractère générique « % » dans la valeur. | Nom (@lastName) pas comme « Smi%h ». Les personnes destinataires dont le nom est « Smith » ne seront pas renvoyées. |

   +++

1. Dans le champ **Valeur**, définissez la valeur attendue. Vous pouvez également utiliser l’éditeur d’expression de Campaign Web pour définir manuellement une expression à l’aide de champs de la base de données et de fonctions d’assistance. Pour ce faire, cliquez sur le bouton **Modifier une expression**. [Découvrez comment modifier des expressions](expression-editor.md)

   *Exemple de requête renvoyant tous les profils âgés de 21 ans ou plus :*

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

![Exemple de requête ciblant des profils âgés de 21 ans ou plus.](assets/query-custom-condition.png){zoomable="yes"}

>[!TAB Nouveau créateur de règles]

![Exemple de requête ciblant des profils âgés de 21 ans ou plus.](assets/ruleb-3.png){zoomable="yes"}

>[!ENDTABS]

Pour les attributs de type date, des valeurs prédéfinies sont disponibles à l’aide de l’option **[!UICONTROL Préréglages]**.

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

![Exemple d’utilisation de préréglages de date dans une requête.](assets/date-presets.png){zoomable="yes"}

>[!TAB Nouveau créateur de règles]

![Exemple d’utilisation de préréglages de date dans une requête.](assets/ruleb-4.png){zoomable="yes"}

>[!ENDTABS]

#### Conditions personnalisées sur les tables liées (liens 1-1 et 1-N){#links}

Les conditions personnalisées vous permettent d’interroger des tables liées à la table actuellement utilisée par votre règle. Cela inclut les tables avec un lien de cardinalité 1-1 ou les tables de collection (lien 1-N).

Pour un **lien 1-1**, accédez à la table liée, sélectionnez l’attribut souhaité et définissez la valeur attendue.

Vous pouvez également sélectionner directement un lien de table dans le sélecteur de **Valeur** et confirmer. Dans ce cas, les valeurs disponibles pour la table sélectionnée doivent être sélectionnées à l’aide d’un sélecteur dédié, comme illustré dans l’exemple ci-dessous.

+++Exemple d&#39;édition d&#39;une requête

Ici, la requête cible les marques dont le libellé est « running ».

1. Naviguez dans la table **Marque** et sélectionnez l’attribut **Libellé**.

   ![Capture d’écran de la table des marques](assets/1-1-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. Définissez la valeur attendue de l’attribut.

   ![Exemple de valeur attendue définie](assets/1-1-table.png){zoomable="yes"}{width="85%" align="center"}

Voici un exemple de requête dans laquelle un lien de table a été directement sélectionné. Les valeurs disponibles pour cette table doivent être sélectionnées avec un sélecteur dédié.

![Exemple de requête](assets/1-1-table-direct.png){zoomable="yes"}{width="85%" align="center"}

+++ 

Pour un **lien 1-N**, vous pouvez définir des sous-conditions afin d’affiner votre requête, comme illustré dans l’exemple ci-dessous.

+++Exemple d&#39;édition d&#39;une requête

Ici, la requête cible les destinataires ayant effectué des achats liés au produit BrewMaster, pour un montant total d’au moins 100 $.

1. Sélectionnez le tableau **Achats** et confirmez.

   ![Capture d’écran de la table des achats](assets/1-N-collection.png){zoomable="yes"}{width="50%" align="center"}

1. Une transition sortante est ajoutée, vous permettant ainsi de créer des sous-conditions.

   ![Exemple de transition sortante](assets/1-n-subcondition.png){zoomable="yes"}{width="85%" align="center"}

1. Sélectionnez l’attribut **Prix** et ciblez les achats de 1 000 $ ou plus.

   ![Capture d’écran de l’attribut Prix](assets/1-n-price.png){zoomable="yes"}{width="85%" align="center"}

1. Ajoutez des sous-conditions adaptées à vos besoins. Ici, nous avons ajouté une condition pour cibler les profils ayant acheté un produit BrewMaster.

   ![Exemples de sous-conditions](assets/custom-condition-1-N.png){zoomable="yes"}{width="85%" align="center"}

+++ 

#### Utiliser des données agrégées {#aggregate}

Les conditions personnalisées vous permettent d’effectuer des opérations d’agrégat. Pour cela, vous devez sélectionner directement un attribut dans un tableau de collection :

1. Naviguez dans le tableau de collection souhaité et sélectionnez l’attribut sur lequel vous souhaitez effectuer une opération d’agrégat.

   ![Capture d’écran de la liste des attributs](assets/aggregate-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. Dans le volet des propriétés, activez l’option **Données agrégées** et sélectionnez la fonction d’agrégat souhaitée.

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

![Capture d’écran de l’option Données agrégées](assets/aggregate.png){zoomable="yes"}{width="85%" align="center"}

>[!TAB Nouveau créateur de règles]

![Capture d&#39;écran de l’option Données agrégées](assets/ruleb-5.png){zoomable="yes"}{width="85%" align="center"}

>[!ENDTABS]

### Sélectionner une audience {#audiences}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Sélectionner une audience"
>abstract="En utilisant l’option **Sélectionner l’audience**, vous pouvez choisir l’audience que vous souhaitez utiliser pour filtrer votre requête."

Pour filtrer votre requête à l’aide d’une audience existante, procédez comme suit :

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

1. Cliquez sur le bouton **+** sur le nœud souhaité, puis choisissez **[!UICONTROL Sélectionner une audience]**.

1. Le volet de propriétés **Sélectionner une audience** s’ouvre sur le côté droit. Sélectionnez l’audience à utiliser pour filtrer votre requête.

   *Exemple de requête renvoyant tous les profils appartenant à l’audience « Festivaliers » :*

   ![Capture d’écran d’un exemple de requête](assets/query-audience.png){zoomable="yes"}

>[!TAB Nouveau créateur de règles]

1. Cliquez sur le bouton **Développer** en regard du bouton **[!UICONTROL Ajouter une condition]**, puis choisissez **[!UICONTROL Sélectionner une audience]**.

1. Le volet de propriétés **Sélectionner une audience** s’ouvre sur le côté droit. Sélectionnez l’audience à utiliser pour filtrer votre requête.

   *Exemple de requête renvoyant tous les profils appartenant à l’audience « Tâches liées au café » :*

   ![Capture d’écran d’un exemple de requête](assets/ruleb-7.png){zoomable="yes"}

>[!ENDTABS]

### Utiliser un filtre prédéfini {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtre prédéfini"
>abstract="En utilisant l’option **Filtre prédéfini** vous pouvez sélectionner un filtre prédéfini dans la liste des filtres personnalisés ou parmi les favoris."

Pour filtrer votre requête à l’aide d’un filtre prédéfini, procédez comme suit :

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

1. Cliquez sur le bouton **+** sur le nœud souhaité, puis sélectionnez **[!UICONTROL Filtre prédéfini]**.

1. Le volet Propriétés **Filtre prédéfini** s’ouvre sur le côté droit. Sélectionnez un filtre prédéfini dans la liste des filtres personnalisés ou dans les favoris.

   *Exemple de requête renvoyant tous les profils correspondant au filtre prédéfini « Clients inactifs » :*

   ![Capture d’écran d’un exemple de requête](assets/query-predefined-filter.png){zoomable="yes"}

>[!TAB Nouveau créateur de règles]

1. Cliquez sur le bouton **Développer** en regard du bouton **[!UICONTROL Ajouter une condition]**, puis sélectionnez **[!UICONTROL Filtre prédéfini]**.

1. Le volet Propriétés **Filtre prédéfini** s’ouvre sur le côté droit. Sélectionnez un filtre prédéfini dans la liste des filtres personnalisés ou dans les favoris.

   *Exemple de requête renvoyant tous les profils correspondant au filtre prédéfini « Clients inactifs » :*

   ![Capture d’écran d’un exemple de requête](assets/ruleb-8.png){zoomable="yes"}

>[!ENDTABS]

### Copier-coller des composants {#copy}

Le concepteur de requête vous permet de copier un ou plusieurs composants de filtrage et de les coller à la fin d’une transition. Cette opération peut être exécutée dans la zone de travail de la requête actuelle ou dans n’importe quelle zone de travail de votre instance.

>[!NOTE]
>
>La sélection copiée est conservée tant que vous travaillez dans votre instance. Si vous vous déconnectez et vous reconnectez, votre sélection ne sera plus disponible pour le collage.

>[!IMPORTANT]
>
>Il est actuellement impossible de copier et coller des composants dans l’expérience du nouveau créateur de règles. Pour suivre les étapes suivantes, cliquez sur le bouton (bascule) **[!UICONTROL Revenir à l’expérience classique]** dans la partie supérieure pour utiliser le concepteur de requête classique.


Pour copier-coller des composants de filtrage, procédez comme suit :

1. Sélectionnez le composant de filtrage à copier en cliquant dessus dans la zone de travail de la requête. Pour sélectionner plusieurs composants, utilisez l’outil de sélection multiple disponible dans la barre d’outils située dans le coin supérieur droit de la zone de travail.

1. Cliquez sur le bouton **[!UICONTROL Copier]** dans le volet des propriétés du composant ou dans le ruban bleu situé en bas de l’écran si vous avez sélectionné plusieurs composants.

   | Copier un seul composant | Copier plusieurs composants |
   |  ---  |  ---  |
   | ![](assets/copy-single-component.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} | ![](assets/copy-multiple-components.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |

1. Pour coller le ou les composants, cliquez sur le bouton + situé à la fin de la transition souhaitée et sélectionnez **Coller n éléments**.

   ![Exemple de collage de composants](assets/copy-paste.png){zoomable="yes"}

## Faire glisser et déposer des composants {#drag-and-drop}

>[!IMPORTANT]
>
>Cette fonctionnalité n’est disponible que pour la nouvelle expérience du créateur de règles.

Lorsque vous ajoutez des composants à votre requête, vous pouvez les déplacer vers le haut et vers le bas à l’aide de la fonction glisser-déposer.

À gauche de chaque composant, vous pouvez cliquer sur les trois points et les maintenir enfoncés pour faire glisser le composant vers le haut et le bas en fonction de l’emplacement où vous souhaitez placer et regrouper les composants.

![GIF montrant comment faire glisser et déposer les composants dans le nouveau créateur de règles](assets/ruleb-drag.gif){zoomable="yes"}

## Combiner des composants de filtrage avec des opérateurs {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Groupe"
>abstract="Dans ce volet, vous pouvez modifier l’opérateur utilisé pour relier les conditions de filtrage."

Chaque fois que vous ajoutez un nouveau composant de filtrage à votre requête, il est automatiquement lié à l’autre composant par un opérateur **ET**. Cela signifie que les résultats des deux composants de filtrage sont combinés.

Dans cet exemple, nous avons ajouté de nouveaux composants de filtrage de type audience sur la seconde transition. Le composant est lié à la condition de filtre prédéfinie avec un opérateur **ET**, ce qui signifie que les résultats de la requête incluent les personnes destinataires ciblées par le filtre prédéfini « Personnes abonnées à la newsletter - MADRID » ET appartenant à l’audience « Acheteurs et acheteuses (Toutes les périodes) ».

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

![Exemple de requête](assets/query-operator.png){zoomable="yes"}

Pour changer l’opérateur utilisé pour relier les conditions de filtrage, cliquez dessus et sélectionnez-en un autre dans le volet **Groupe** qui s’ouvre sur la droite.

Les opérateurs disponibles sont les suivants :

* **ET (Intersection)** : combine les résultats correspondant à tous les composants de filtrage dans les transitions sortantes.
* **OU (Union)** : inclut des résultats correspondant à au moins un des composants de filtrage dans les transitions sortantes.
* **SAUF (Exclusion)** : exclut les résultats correspondant à tous les composants de filtrage dans la transition sortante.

![Exemple de requête](assets/query-operator-change.png){zoomable="yes"}

En outre, vous pouvez créer des groupes intermédiaires de composants en les regroupant dans un même groupe et en les reliant entre eux. Ainsi, l’opérateur ET est placé par défaut. Vous pouvez ensuite le remplacer par l’opérateur de votre choix.

>[!TAB Nouveau créateur de règles]

![Exemple de requête](assets/ruleb-9.png){zoomable="yes"}

Pour modifier l’opérateur utilisé pour relier les conditions de filtrage, cliquez dessus. Il devient OU, SAUF puis revient à ET, et sélectionnez l’opérateur de votre choix.

Les opérateurs disponibles sont les suivants :

* **ET (Intersection)** : combine les résultats correspondant à tous les composants de filtrage dans les transitions sortantes.
* **OU (Union)** : inclut des résultats correspondant à au moins un des composants de filtrage dans les transitions sortantes.
* **SAUF (Exclusion)** : exclut les résultats correspondant à tous les composants de filtrage dans la transition sortante.

![Exemple de requête](assets/ruleb-10.gif){zoomable="yes"}

>[!ENDTABS]

Dans l’exemple ci-dessous, nous avons créé un groupe intermédiaire pour inclure les résultats des audiences « VIP à récompenser » ou « Super VIP ».

>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

![Exemple de requête](assets/query-intermediate-group.png){zoomable="yes"}

>[!TAB Nouveau créateur de règles]

![Exemple de requête dans le nouveau créateur de règles](assets/ruleb-11.png){zoomable="yes"}

>[!ENDTABS]

## Vérifier et valider votre requête

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Propriétés de la règle"
>abstract="Une fois que vous avez créé votre requête dans la zone de travail, vous pouvez la vérifier à l’aide du volet **Propriétés des règles** situé sur le côté droit.<br/>Ce volet permet d’afficher les données obtenues, de récupérer une version de code SQL de la requête et de vérifier le nombre d’enregistrements ciblés.<br/>Utilisez le bouton **Sélectionner ou enregistrer un filtre** pour enregistrer votre requête en tant que filtre prédéfini ou remplacer le contenu de la zone de travail par un filtre existant."

Une fois que vous avez créé votre requête dans la zone de travail, vous pouvez la vérifier à l’aide du volet **Propriétés des règles** situé à droite. Ce dernier s’affiche lors de la création d’une requête pour créer une audience. Les opérations disponibles sont les suivantes :

* **Afficher les résultats** : affiche les données issues de votre requête.
* **Affichage du code** : affiche une version basée sur le code de la requête en SQL.
* **Calculer** : met à jour et affiche le nombre d’enregistrements ciblés par votre requête.
* **Sélectionner ou enregistrer un filtre** : choisissez un filtre prédéfini existant à utiliser dans la zone de travail ou enregistrez votre requête en tant que filtre prédéfini pour une réutilisation ultérieure. [Découvrez comment utiliser des filtres prédéfinis](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >Sélectionnez un filtre prédéfini dans le volet Propriétés de la règle pour remplacer la requête qui a été créée dans la zone de travail par le filtre sélectionné.

Lors de l’utilisation de la nouvelle expérience de créateur de règles, vous pouvez afficher la population cible directement sur chaque condition et groupe :

* Cliquez sur l’icône **Calculer la condition** sur la condition ou le groupe de votre choix pour calculer et afficher le nombre d’enregistrements ciblés par votre requête.
* Cliquez sur le nombre de résultats pour afficher la liste détaillée des enregistrements.

![Affichage de la population et des résultats](assets/ruleb-11bis.png){zoomable="yes"}

Lorsque votre requête est prête, cliquez sur le bouton **[!UICONTROL Confirmer]** dans le coin supérieur droit pour effectuer l’enregistrement.


>[!BEGINTABS]

>[!TAB Concepteur de requête classique]

Vous pouvez modifier votre requête à tout moment en l’ouvrant. Gardez à l’esprit que lors de l’ouverture d’une requête existante, elle s’affiche dans une vue simplifiée sans la visibilité des boutons **+**. Pour ajouter de nouveaux éléments à la requête, sélectionnez un composant ou un opérateur dans la zone de travail afin d’afficher les boutons **+**.

![Exemple de requête](assets/edit-audience.png){zoomable="yes"}

>[!TAB Nouveau créateur de règles]

Vous pouvez modifier votre requête à tout moment en l’ouvrant. Pour ce faire, cliquez sur le bouton **[!UICONTROL Ajouter une condition]** dans le coin supérieur gauche.

![Exemple de requête dans le nouveau créateur de règles](assets/ruleb-11.png){zoomable="yes"}

>[!ENDTABS]
