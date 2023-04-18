---
audience: end-user
title: Utilisation des activités de Data Management des workflows
description: Découvrez comment utiliser les activités de Data Management dans les workflows web Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 0b5bfea60b65fd52f397f276e0c31e854adddb7b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 4%

---

# Activités de Data Management {#data-management}

aperçu : ce qu’ils sont utilisés, auquel cas vous pouvez les utiliser ;

liste des activités disponibles + brève description + référence à la section

## Enrichissement {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enrichissement activité"
>abstract="L&#39;activité Enrichissement permet d&#39;améliorer les données ciblées avec des informations supplémentaires de la base de données. Il est généralement utilisé dans un workflow après des activités de ciblage.<br/>Une fois que les données d&#39;enrichissement ont été ajoutées au workflow, elles peuvent être utilisées dans les activités ajoutées après l&#39;activité Enrichissement pour segmenter les clients en groupes distincts en fonction de leurs comportements, préférences et besoins, ou pour créer des messages marketing personnalisés et des campagnes qui ont plus de chances de répondre à votre audience cible."

L&#39;activité Enrichissement permet d&#39;améliorer les données ciblées avec des informations supplémentaires de la base de données. Il est généralement utilisé dans un workflow après des activités de ciblage.

Les données d’enrichissement peuvent venir :

* **A partir de la même table de travail** comme celui ciblé dans votre workflow :

   *Ciblez un groupe de clients et ajoutez le champ &quot;Date de naissance&quot; à la table de travail actuelle.*

* **A partir d&#39;une autre table de travail**:

   *Ciblez un groupe de clients et ajoutez les champs &quot;Montant&quot; et &quot;Type de produit&quot; provenant de la table &quot;Achat&quot;*.

Une fois que les données d&#39;enrichissement ont été ajoutées au workflow, elles peuvent être utilisées dans les activités ajoutées après l&#39;activité Enrichissement pour segmenter les clients en groupes distincts en fonction de leurs comportements, préférences et besoins, ou pour créer des messages marketing personnalisés et des campagnes plus susceptibles de répondre à votre audience cible.

Par exemple, vous pouvez ajouter à la table de travail du workflow des informations relatives aux achats des clients et utiliser ces données pour personnaliser les emails avec leur dernier achat ou le montant dépensé pour ces achats.

Pour ajouter une activité Enrichissement à votre workflow, procédez comme suit :

1. ajouter une activité
1. sélectionner l’attribut à utiliser comme données d’enrichissement

   bouton afficher les champs avancés

   remarque : attributs de la dimension cible

1. Sélectionner la manière de collecter les données
1. nombre d’enregistrements à récupérer si vous souhaitez récupérer une collection de plusieurs enregistrements
1. Application de filtres et de règles de création

   sélectionner un filtre existant enregistrer le filtre pour réutiliser les résultats des vues du filtre visuellement ou en mode code

1. tri des enregistrements à l’aide d’un attribut

exploiter les données d’enrichissement dans campaign

où nous pouvons utiliser les données d&#39;enrichissement : personnaliser l&#39;email, d&#39;autres cas pratiques ?
