---
audience: end-user
title: Utiliser les activités de gestion des données des workflows
description: Découvrez comment utiliser les activités de gestion des données dans les workflows Web Adobe Campaign.
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 0b5bfea60b65fd52f397f276e0c31e854adddb7b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 100%

---

# Activités de gestion des données {#data-management}

Vue d’ensemble : utilisation
cas d’utilisation

liste des activités disponibles + brève description + référence à la section

## Enrichissement {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enrichissement activité"
>abstract="L’activité Enrichissement permet d’enrichir les données ciblées avec des informations supplémentaires provenant de la base de données. Elle est généralement utilisée dans un workflow après les activités de ciblage.<br/>Une fois que les données d’enrichissement ont été ajoutées au workflow, vous pouvez les utiliser dans les activités ajoutées après l’activité Enrichissement pour segmenter les clients en groupes distincts en fonction de leurs comportements, préférences et besoins. Vous pouvez également vous en servir pour créer des messages et des campagnes marketing personnalisés qui résonneront davantage auprès de votre audience cible."

L’activité Enrichissement permet d’enrichir les données ciblées avec des informations supplémentaires provenant de la base de données. Elle est généralement utilisée dans un workflow après les activités de ciblage.

Les données d’enrichissement tirent leur origine des sources suivantes :

* **Le même tableau de travail** que celui ciblé dans votre workflow :

   *Ciblez un groupe de clients et de clientes et ajoutez le champ « Date de naissance » au tableau de travail actuel.*

* **Un autre tableau de travail** :

   *Ciblez un groupe de clients et de clientes et ajoutez les champs « Montant » et « Type de produit » provenant du tableau « Achat »*.

Une fois que les données d’enrichissement ont été ajoutées au workflow, vous pouvez les utiliser dans les activités ajoutées après l’activité Enrichissement pour segmenter les clients et les clientes en groupes distincts en fonction de leurs comportements, préférences et besoins. Vous pouvez également vous en servir pour créer des messages et des campagnes marketing personnalisés qui résonneront davantage auprès de votre audience cible.

Par exemple, vous pouvez ajouter au tableau de travail du workflow des informations relatives aux achats des clients et clientes et utiliser ces données pour personnaliser les e-mails en fonction de leur dernier achat ou du montant dépensé pour ces achats.

Pour ajouter une activité Enrichissement à votre workflow, procédez comme suit :

1. ajouter une activité
1. sélectionner l’attribut à utiliser comme données d’enrichissement

   bouton i
afficher les champs avancés

   note : attributs de la dimension cible

1. Sélectionner la manière de collecter les données
1. le nombre d’enregistrements à récupérer si vous souhaitez récupérer une collection de plusieurs enregistrements
1. Appliquer des filtres et créer des règles

   sélectionner un filtre existant
enregistrer le filtre pour le réutiliser
consulter les résultats du filtre visuellement ou sous forme de code

1. trier les enregistrements à l’aide d’un attribut

tirer parti des données d’enrichissement dans les campagnes

application des données d’enrichissement : pour la personnalisation des e-mails et dans d’autres cas d’utilisation ?
