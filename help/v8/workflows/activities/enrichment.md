---
audience: end-user
title: Utiliser l’activité de workflow Enrichissement
description: Découvrez comment utiliser l’activité de workflow Enrichissement.
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
TQID: https://experienceleague.adobe.com/yYV7iC9u6wWwpJMEUUlwGRAPsuDiZkPvLD-cmw4IPf4
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616a
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 3207311cda7b2b88b68ef194d2776ae40e907f48
workflow-type: ht
source-wordcount: 2327
ht-degree: 100%

---

# Enrichissement {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Activité Enrichissement"
>abstract="L’activité **Enrichissement** permet d’enrichir les données ciblées avec des informations supplémentaires provenant de la base de données. Elle est généralement utilisée dans un workflow après les activités de segmentation."

L’activité **Enrichissement** est une activité de **ciblage**. Elle améliore les données ciblées avec des informations supplémentaires provenant de la base de données. Elle est généralement utilisée dans un workflow après les activités de segmentation.

>[!NOTE]
>
>L’activité **Créer une audience** (type de requête) prend également en charge les **données d’enrichissement**.Consultez [En savoir plus](build-audience.md#build-audience-configuration).

Les données d’enrichissement tirent leur origine des sources suivantes :

* **La même table de travail** que celle ciblée dans votre workflow :
   * Ciblez un groupe de clientes et de clients et ajoutez le champ « Date de naissance » à la table de travail actuelle.

* **Une autre table de travail** :
   * Ciblez un groupe de clients et de clientes et ajoutez les champs « Montant » et « Type de produit » provenant du tableau « Achat ».

Une fois que les données d’enrichissement ont été ajoutées au workflow, elles peuvent être utilisées dans les activités suivantes pour segmenter les clientes et clients en groupes distincts en fonction de leurs comportements, préférences et besoins. Elles peuvent également être utilisées pour créer des messages et des campagnes marketing personnalisés qui résonnent auprès de votre audience cible.

Par exemple, vous pouvez ajouter des informations relatives aux achats des clientes et clients au tableau de travail du workflow et utiliser ces données pour personnaliser les e-mails en fonction de leur dernier achat ou du montant dépensé pour ces achats.

## Ajouter une activité Enrichissement {#enrichment-configuration}

Pour configurer l’activité **Enrichissement**, procédez comme suit :

1. Ajoutez des activités telles que **Créer une audience** et **Combiner**.
1. Ajoutez une activité **Enrichissement**.
1. Si plusieurs transitions ont été configurées dans votre workflow, vous pouvez utiliser le champ **[!UICONTROL Ensemble principal]** pour définir la transition à utiliser comme ensemble principal pour l’enrichissement.

## Ajouter des données d’enrichissement {#enrichment-add}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Données d’enrichissement"
>abstract="Sélectionnez les données à utiliser pour enrichir votre workflow. Vous pouvez sélectionner deux types de données d’enrichissement : un seul attribut d’enrichissement de la dimension cible ou un lien de collection, qui est un lien avec une cardinalité 1-N entre les tables."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Activité Enrichissement"
>abstract="Une fois que les données d’enrichissement ont été ajoutées au workflow, vous pouvez les utiliser dans les activités suivantes pour segmenter les clientes et clients en groupes distincts en fonction de leurs comportements, préférences et besoins ou pour créer des messages et des campagnes marketing personnalisés qui résonneront auprès de votre audience cible."

La section **Données d’enrichissement** est disponible dans les activités **Enrichissement** et **Créer une audience** (type requête).Elle permet d’enrichir les données ciblées avec des informations supplémentaires issues de la base de données, comme des références de contrat ou des abonnements à la newsletter.Ces données sont stockées avec l’audience dans la **table de travail** de workflows et sont disponibles pour les activités suivantes.Vous pouvez ajouter des attributs d’enrichissement uniques, des liens de collection ou des expressions et accéder à des options avancées.

Cliquez sur **Ajouter des données d’enrichissement** et sélectionnez l’attribut à utiliser pour l’enrichissement. [Découvrez comment sélectionner des attributs et les ajouter aux favoris](../../get-started/attributes.md).

Vous pouvez sélectionner deux types de données d’enrichissement : un attribut d’enrichissement unique de la dimension cible, ou un lien de collection. Chacun des types est détaillé dans les exemples ci-dessous :

* [Attribut d’enrichissement unique](#single-attribute)
* [Lien de collection](#collection-link)

>[!NOTE]
>
>Le **bouton Modifier l’expression** dans l’écran de sélection d’attributs vous permet de créer des expressions avancées pour sélectionner l’attribut. [Découvrez comment utiliser l’éditeur d’expression](../../query/expression-editor.md).

![Copie d’écran affichant l’écran de sélection des données d’enrichissement](../assets/workflow-enrichment1.png)

Après avoir ajouté au moins un attribut d’enrichissement, cliquez sur **[!UICONTROL Paramètres avancés]** pour configurer la manière dont les données d’enrichissement sont créées, y compris le regroupement, la déduplication, la gestion des clés primaires et les données d’événement entrant.Ces options reflètent la console cliente et sont destinées aux scénarios de workflow avancés.

![Copie d’écran affichant les paramètres avancés de l’enrichissement](../assets/workflow-query-advanced-parameters.png)

>[!NOTE]
>
>Les options disponibles diffèrent entre les activités **Créer une audience** et **Enrichissement**.

Les options suivantes sont disponibles pour chaque activité :

+++ Activité de création d’audience (type de requête)

* **[!UICONTROL Conserver toutes les données additionnelles de l’ensemble principal]** : conserve les colonnes supplémentaires de l’ensemble entrant principal dans la transition de sortie.
* **[!UICONTROL Regrouper les données par élément de dimension de ciblage]** : regroupe le résultat afin que chaque enregistrement ciblé n’apparaisse qu’une seule fois.
* **[!UICONTROL Supprimer les lignes en double (DISTINCT)]** : supprime les lignes en double du jeu de résultats.
* **[!UICONTROL Désactiver l’ajout automatique des clés primaires de la dimension de ciblage]** : empêche l’activité d’ajouter automatiquement les clés primaires de la dimension de ciblage au résultat.
* **[!UICONTROL Désactiver le filtrage automatique des enregistrements d’ID 0]** : conserve les enregistrements dont la valeur d’identifiant est 0 au lieu de les filtrer automatiquement.
* **[!UICONTROL Utiliser les données d’événement entrant]** : utilise les données de la transition entrante comme entrée de travail de l’activité.

+++

+++ Activité Enrichissement

* **[!UICONTROL Regrouper les données par élément de dimension de ciblage]** : regroupe le résultat afin que chaque enregistrement ciblé n’apparaisse qu’une seule fois.
* **[!UICONTROL Supprimer les lignes en double (DISTINCT)]** : supprime les lignes en double du jeu de résultats.
* **[!UICONTROL Désactiver le filtrage automatique des enregistrements d’ID 0]** : conserve les enregistrements dont la valeur d’identifiant est 0 au lieu de les filtrer automatiquement.
* **[!UICONTROL Ajouter un identifiant pour chaque ligne du résultat]** : ajoute un identifiant unique à chaque ligne de sortie.

+++

## Créer de liens entre les tables {#create-links}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_simplejoin"
>title="Définition du lien"
>abstract="Créez un lien entre les données du tableau de travail et la base de données Adobe Campaign. Par exemple, si vous chargez les données d’un fichier contenant le numéro de compte, le pays et l’adresse e-mail des destinataires, vous pouvez maintenant créer un lien vers le tableau des pays afin de mettre à jour cette information dans leur profil."

La section **[!UICONTROL Définition du lien]** permet de créer un lien entre les données de la table de travail et la base de données Adobe Campaign. Par exemple, si vous chargez les données d’un fichier contenant le numéro de compte, le pays et l’adresse e-mail des destinataires, vous pouvez maintenant créer un lien vers le tableau des pays afin de mettre à jour cette information dans leur profil.

Plusieurs types de liens sont disponibles :

* **[!UICONTROL Lien simple de cardinalité 1]** : chaque enregistrement de l’ensemble principal est associé à un seul enregistrement des données liées.
* **[!UICONTROL Lien simple de cardinalité 0 ou 1]** : chaque enregistrement de l’ensemble principal est associé à 0 ou 1 enregistrement des données liées (et pas plus de un).
* **[!UICONTROL Lien de collection de cardinalité N]** : chaque enregistrement de l’ensemble principal peut être associé à 0, 1 ou plus (N) d’enregistrements des données liées.

Pour créer un lien, procédez comme suit :

1. Dans la section **[!UICONTROL Définition du lien]**, cliquez sur le bouton **[!UICONTROL Ajouter un lien]**.

   ![Copie d’écran affichant la section de définition des liens](../assets/workflow-enrichment-link.png)

1. Dans la liste déroulante **Type de relation**, sélectionnez le type de lien que vous souhaitez créer.

1. Identifiez la cible à laquelle vous souhaitez lier l’ensemble principal :

   * Pour lier une table existante dans la base de données, choisissez **[!UICONTROL Schéma de base de données]** et sélectionnez la table souhaitée dans le champ **[!UICONTROL Schéma cible]**.
   * Pour créer un lien avec les données de la transition en entrée, choisissez **Schéma temporaire** et sélectionnez la transition dont vous souhaitez utiliser les données.

1. Définissez les critères de réconciliation pour faire correspondre les données de l’ensemble principal avec le schéma lié. Deux types de jointures sont disponibles :

   * **Jointure simple** : sélectionnez un attribut spécifique pour faire correspondre les données des deux schémas. Cliquez sur **Ajouter une jointure** et sélectionnez les attributs **Source** et **Destination** à utiliser comme critères de réconciliation.
   * **Jointure avancée** : créez une jointure à l’aide de conditions avancées. Cliquez sur **Ajouter une jointure** puis sur le bouton **Créer une condition** pour ouvrir le concepteur de requête.

Un exemple de workflow utilisant des liens est disponible dans la section [Exemples](#link-example).

## Réconciliation des données {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_reconciliation"
>title="Réconciliation"
>abstract="L’activité **Enrichissement** peut être utilisée pour réconcilier des données provenant du schéma de la base de données Campaign avec des données issues d’un autre schéma, ou avec des données provenant d’un schéma temporaire, comme des données chargées à l’aide d’une activité Chargement de fichier. Ce type de lien définit une réconciliation vers un enregistrement unique. Adobe Campaign crée un lien vers un tableau cible en ajoutant une clé étrangère permettant de stocker une référence vers l’enregistrement unique."

L’activité **Enrichissement** peut être utilisée pour réconcilier des données provenant du schéma de la base de données Campaign avec des données issues d’un autre schéma, ou avec des données provenant d’un schéma temporaire, comme des données chargées à l’aide d’une activité Chargement de fichier. Ce type de lien définit une réconciliation vers un enregistrement unique. Adobe Campaign crée un lien vers un tableau cible en ajoutant une clé étrangère permettant de stocker une référence vers l’enregistrement unique.

Par exemple, vous pouvez utiliser cette option pour réconcilier le pays d’un profil, indiqué dans un fichier chargé, avec l’un des pays disponibles dans le tableau dédié de la base de données Campaign.

Procédez comme suit pour configurer une activité **Enrichissement** avec un lien de réconciliation :

1. Cliquez sur le bouton **Ajouter un lien** dans la section **Réconciliation**.
1. Identifiez les données avec lesquelles vous souhaitez créer un lien de réconciliation.

   * Pour créer un lien de réconciliation avec les données de la base de données Campaign, sélectionnez **Schéma de base de données** et choisissez le schéma dans lequel la cible est stockée.
   * Pour créer un lien de réconciliation avec les données provenant de la transition en entrée, sélectionnez **Schéma temporaire** et choisissez la transition de workflow dans laquelle les données cibles sont stockées.

1. Les champs **Libellé** et **Nom** sont renseignés automatiquement en fonction du schéma cible sélectionné. Vous pouvez modifier leurs valeurs si nécessaire.

1. Dans la section **Critères de réconciliation**, indiquez comment vous souhaitez réconcilier les données des tableaux source et de destination :

   * **Jointure simple** : réconciliez un champ spécifique du tableau source avec un autre champ du tableau de destination. Pour ce faire, cliquez sur le bouton **Ajouter une jointure** et renseignez les champs **Source** et **Destination** à utiliser pour la réconciliation.

     >[!NOTE]
     >
     >Vous pouvez utiliser une **Jointure simple**, ou plusieurs, auquel cas elles doivent toutes être vérifiées afin que les données puissent être liées.

   * **Jointure avancée** : utilisez le concepteur de requête pour configurer les critères de réconciliation. Pour ce faire, cliquez sur le bouton **Créer une condition**, puis définissez vos critères de réconciliation en créant votre propre règle à l’aide des opérations ET et OU.

L’exemple ci-dessous montre un workflow configuré pour créer un lien entre le tableau des personnes destinataires de la base de données Adobe Campaign et un tableau temporaire généré par une activité **Chargement de fichier**. Dans cet exemple, l’activité Enrichissement réconcilie les deux tableaux en utilisant l’adresse e-mail comme critère de réconciliation.

![](../assets/enrichment-reconciliation.png)

## Ajouter des offres {#add-offers}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_offer_proposition"
>title="Proposition d&#39;offres"
>abstract="L’activité Enrichissement permet d’ajouter des offres pour chaque profil."

L’activité **[!UICONTROL Enrichissement]** vous permet d’ajouter des offres pour chaque profil.

Pour ce faire, suivez les étapes pour configurer une activité **[!UICONTROL Enrichissement]** avec une offre :

1. Dans l’activité **[!UICONTROL Enrichissement]**, dans la section **[!UICONTROL Proposition d’offre]**, cliquez sur le bouton **[!UICONTROL Ajouter une offre]**.

   ![](../assets/enrichment-addoffer.png)

1. Vous avez le choix entre deux options pour la sélection d’offre :

   * **[!UICONTROL Rechercher la meilleure offre dans une catégorie]** : cochez cette option et définissez les paramètres de l’appel au moteur d’offres (emplacement, catégorie ou thème(s), date de contact, nombre d’offres à conserver). Le moteur calculera la ou les meilleures offres à ajouter en fonction de ces paramètres. Il est conseillé de renseigner l’un ou l’autre des champs Catégorie et Thème, mais pas les deux en même temps.

     ![](../assets/enrichment-bestoffer.png)

   * **[!UICONTROL Une offre prédéfinie]** : cochez cette option et définissez un emplacement, une offre précise, ainsi qu&#39;une date de contact afin de directement paramétrer l&#39;offre que vous souhaitez ajouter, sans appeler le moteur d&#39;offres.

     ![](../assets/enrichment-predefinedoffer.png)

1. Après avoir sélectionné votre offre, cliquez sur le bouton **[!UICONTROL Confirmer]**.

Vous pouvez maintenant utiliser l’offre dans l’activité de diffusion.

### Utilisation des offres de l’activité Enrichissement

Dans un workflow, si vous souhaitez utiliser les offres que vous obtenez d’une activité Enrichissement dans votre diffusion, procédez comme suit :

1. Ouvrez l’activité de diffusion et accédez à l’édition de contenu. Cliquez sur le bouton **[!UICONTROL Paramètres des offres]** et sélectionnez l’**[!UICONTROL Espace d’offres]** correspondant à votre offre dans la liste déroulante.
Si vous souhaitez afficher uniquement les offres de l’activité Enrichissement, définissez le nombre de **[!UICONTROL Propositions]** sur 0, puis enregistrez les modifications.

   ![](../assets/offers-settings.png)

1. Dans le concepteur d’e-mail, lors de l’ajout d’une personnalisation avec des offres, cliquez sur l’icône **[!UICONTROL Propositions]** qui affiche la ou les offres que vous obtenez de l’activité **[!UICONTROL Enrichissement]**. Ouvrez l’offre que vous souhaitez sélectionner en cliquant dessus.

   ![](../assets/offers-propositions.png)

   Accédez à **[!UICONTROL Fonctions de rendu]** et sélectionnez **[!UICONTROL Rendu HTML]** ou **[!UICONTROL Rendu de texte]** en fonction de vos besoins.

   ![](../assets/offers-rendering.png)

>[!NOTE]
>
>Si vous choisissez d’avoir plusieurs offres dans l’activité **[!UICONTROL Enrichissement]** à l’option **[!UICONTROL Nombre d’offres à conserver]**, toutes les offres sont affichées en cliquant sur l’icône **[!UICONTROL Propositions]**.

## Exemples {#example}

### Attribut d’enrichissement unique {#single-attribute}

Ici, nous ajoutons un seul attribut d’enrichissement, par exemple, la date de naissance. Procédez comme suit :

1. Cliquez dans le champ **Attribut**.
1. Sélectionnez un champ simple dans la dimension de ciblage, la date de naissance dans notre exemple.
1. Cliquez sur **Confirmer**.

![](../assets/workflow-enrichment2.png)

### Lien de collection {#collection-link}

Dans ce cas pratique plus complexe, nous sélectionnons un lien de collecte qui est un lien avec une cardinalité 1-N entre les tableaux. Récupérons les trois derniers achats inférieurs à 100 USD. Pour cela, vous devez définir :

* un attribut d’enrichissement : le champ **Prix** ;
* le nombre de lignes à récupérer : 3 ;
* un filtre : filtrez les éléments supérieurs à 100 USD ;
* un tri : tri descendant sur le champ **Date de commande**.

#### Ajouter l’attribut {#add-attribute}

C’est là que vous sélectionnez le lien de collecte à utiliser comme données d’enrichissement.

1. Cliquez dans le champ **Attribut**.
1. Cliquez sur **Afficher les attributs avancés**.
1. Sélectionnez le champ **Prix** dans le tableau **Achats**.

<!-- ![](../assets/workflow-enrichment3.png) -->

#### Définir les paramètres de la collecte{#collection-settings}

Définissez ensuite la manière dont les données sont collectées et le nombre d’enregistrements à récupérer.

1. Sélectionnez **Collecter des données** dans le menu déroulant **Sélectionner la manière de collecter les données**.
1. Saisissez « 3 » dans le champ **Lignes à récupérer (Colonnes à créer)**.

![](../assets/workflow-enrichment4bis.png)

Si vous souhaitez, par exemple, obtenir le montant moyen des achats d’un client ou une cliente, sélectionnez **Données agrégées**, puis **Moyenne** dans le menu déroulant **Fonction d’agrégat**.

Utilisez les champs **Libellé** et **Alias** de votre attribut afin de le rendre plus compréhensible comme illustré ci-dessous.

![](../assets/workflow-enrichment5bis.png)

#### Définir des filtres{#collection-filters}

Ici, nous définissons la valeur maximale de l’attribut d’enrichissement. Nous filtrons les éléments supérieurs à 100 $. [Découvrez comment utiliser le concepteur de requête](../../query/query-modeler-overview.md)

1. Cliquez sur **Créer des filtres**.
1. Ajoutez les deux filtres suivants : **Prix** existe ET **Prix** est inférieur à 100. Le premier filtre les valeurs NULL, car elles apparaissent comme la valeur la plus élevée.
1. Cliquez sur **Confirmer**.

![](../assets/workflow-enrichment6bis.png)

#### Définir le tri{#collection-sorting}

Nous devons maintenant appliquer un tri pour récupérer les trois **derniers** achats.

1. Activez l’option **Activer le tri**.
1. Cliquez dans le champ **Attribut**.
1. Sélectionnez le champ **Date de commande**.
1. Cliquez sur **Confirmer**.
1. Sélectionnez **Descendant** dans le menu déroulant **Tri**.

![](../assets/workflow-enrichment7bis.png)

### Enrichissement avec des données liées {#link-example}

L’exemple ci-dessous montre un workflow configuré pour créer un lien entre deux transitions. La première transition cible les données de profil à l’aide d’une activité **Requête**, tandis que la seconde transition inclut les données d’achat stockées dans un fichier chargé via une activité Chargement de fichier.

![](../assets/enrichment-uc-link.png)

* La première activité **Enrichissement** lie l’ensemble principal (données issues de l’activité **Requête**) au schéma de l’activité **Chargement de fichier**. Cela nous permet de faire correspondre chaque profil ciblé par la requête avec les données d’achat correspondantes.

  ![](../assets/enrichment-uc-link-purchases.png)

* Une seconde activité **Enrichissement** est ajoutée afin d’enrichir les données de la table de workflow avec les données d’achat provenant de l’activité **Chargement de fichier**. Cela nous permet d’utiliser ces données dans d’autres activités, par exemple pour personnaliser les messages envoyés aux clientes et clients avec des informations sur leur achat.

  ![](../assets/enrichment-uc-link-data.png)

