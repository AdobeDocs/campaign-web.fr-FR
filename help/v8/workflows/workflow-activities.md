---
audience: end-user
title: Utilisation des activités de workflows
description: Découvrez comment workflows des activités
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: ec569f7d5acc06a027416794c056328d5fce1567
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 78%

---


# Activités de workflows {#workflow-activities}

## Activités de ciblage {#targeting}

Ces activités permettent de construire une ou plusieurs cibles en définissant des ensembles, puis en partitionnant ou en combinant ces ensembles à l’aide des opérations d’intersection, d’union ou d’exclusion.

### Créer une audience {#build-audience}

Cette activité permet de définir une audience. Vous pouvez sélectionner une instance Campaign existante ou utiliser le créateur de règles pour définir votre propre requête.

Le **Créer une audience** peut être placée au début du workflow ou après toute autre activité. N’importe quelle activité peut être placée après le **Créer une audience**.

Pour créer votre propre requête :

1. Sélectionner **Créez votre propre (requête)**.
1. Choisissez la **Dimension de ciblage**. La dimension de ciblage permet de définir la population ciblée par l&#39;opération : destinataires, bénéficiaires d&#39;un contrat, opérateur, abonnés, etc. Par défaut, la cible est sélectionnée parmi les destinataires. Reportez-vous à la section [Documentation v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Cliquez sur **Continuer**.
1. Utilisez le créateur de règles pour définir votre requête, de la même manière que vous créez une audience lors de la conception d’un nouvel email. Reportez-vous à cette [section](../audience/segment-builder.md).

Pour sélectionner une audience existante, procédez comme suit :

1. Sélectionner **Lecture d’audience**.
1. Cliquez sur **Continuer**.
1. Sélectionnez votre audience, de la même manière que vous utilisez une audience lors de la conception d&#39;un nouvel email. Reportez-vous à cette [section](../audience/add-audience.md).

### Combiner {#combine}

Le **Combiner** peut être placée après toute autre activité, mais pas au début du workflow. N’importe quelle activité peut être placée après le **Combiner**.

### Enrichissement {#enrichment}

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


## Activités des canaux {#channel}

Adobe Campaign Web vous permet d’automatiser et d’exécuter des campagnes marketing sur plusieurs canaux, tels que les e-mails, les SMS ou les notifications push. Avec les workflows Adobe Campaign, vous pouvez combiner des activités de canal dans la zone de travail afin de créer des workflows cross-canal pouvant déclencher des actions en fonction du comportement du client ou de la cliente.

Vous pouvez par exemple créer une campagne par e-mail de bienvenue qui comprend une série de messages sur différents canaux, tels que les e-mails, les SMS et les notifications push. Vous pouvez également envoyer un e-mail de relance une fois qu’un client ou une cliente a effectué un achat, ou encore envoyer un message d’anniversaire personnalisé par SMS.

Grâce aux activités de canal, vous pouvez créer des campagnes personnalisées et complètes qui impliquent des clients et clientes sur plusieurs points de contact et génèrent des conversions.

Les activités de canal sont disponibles à partir de la palette, dans la partie gauche de l’écran, dans la section Canaux.

### E-mail {#email}

description, les cas d’utilisation possibles (autres activités courantes que vous pouvez lier avant ou après l’activité)

comment ajouter et configurer l’activité

exemple d’activité configurée dans un workflow


L’activité Diffusion E-mail permet de paramétrer l’envoi d’un e-mail dans un workflow.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Les destinataires des e-mails sont définis en amont de l’activité dans le même workflow, via une activité de ciblage d’audience.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### Notification push (Android) {#push-android}

### Notification push (iOS) {#push-ios}

## Activités de contrôle de flux {#flow-control}

contenu à déterminer

<!--à reformuler-->Ces activités permettent de construire une ou plusieurs cibles en définissant des ensembles, puis en partitionnant ou en combinant ces ensembles à l’aide des opérations d’intersection, d’union ou d’exclusion.

Les activités de contrôle de flux servent à coordonner les activités de workflow.

### Branchement {#fork}

### Rendez-vous {#join}


### Attente {#wait}

### Fin {#end}

## Activités de gestion des données {#data-management}

Vue d’ensemble : utilisation
cas d’utilisation

liste des activités disponibles + brève description + référence à la section

