---
audience: end-user
title: Messages transactionnels
description: À propos des messages transactionnels avec Adobe Campaign Web
exl-id: 90830dca-acff-4aa3-a88b-1005e349cf52
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 44%

---

# À propos des messages transactionnels {#transactional-messaging}

>[!CONTEXTUALHELP]
>id="acw_transacmessages"
>title="Messages transactionnels"
>abstract="Les messages transactionnels constituent un module spécialisé d’Adobe Campaign conçu pour gérer les messages déclenchés."

<!-- >>[!CONTEXTUALHELP]
>id="acw_transacmessages_exclusionlogs"
>title="Transactional messaging exclusion logs"
>abstract="Transactional messaging exclusion logs" -->

Les messages transactionnels constituent un module spécialisé d’Adobe Campaign conçu pour gérer les messages déclenchés. Ces messages sont générés automatiquement en réponse aux événements provenant des systèmes d’information. Parmi les exemples courants de ces événements, citons le clic sur des boutons ou des liens, l’abandon de panier, la demande d’alertes de disponibilité des produits, la création ou la modification de compte.

Les messages transactionnels sont utilisés pour envoyer :

* des notifications importantes, telles que les confirmations de commande ou les réinitialisations de mot de passe ;
* Réponses en temps réel aux actions du client, telles que la création d’un compte ou l’achèvement de l’achat,
* du contenu non promotionnel essentiel aux interactions des clientes et clients.

Le module de messagerie transactionnelle s’intègre de manière transparente à vos systèmes d’information. Les événements, tels que les actions du client, sont transmis à Adobe Campaign, qui envoie le message personnalisé correspondant. Ces messages peuvent être envoyés individuellement ou par lots via divers canaux, tels que les e-mails, les SMS ou les notifications push.

Vous pouvez retrouver le module **[!UICONTROL Message transactionnel]** dans la section **[!UICONTROL Messages déclenchés]**.

![Interface de messagerie transactionnelle affichant les messages déclenchés et leurs états](assets/transactional.png){zoomable="yes"}

La page **[!UICONTROL Message transactionnel]** contient trois onglets :

* **[!UICONTROL Parcourir]**, où vous disposez de la liste des messages transactionnels avec leur statut,
* **[!UICONTROL Modèles]**, où vous trouvez et créez les modèles de messages transactionnels,
* **[!UICONTROL Historique]**, où vous disposez des détails sur tous les messages transactionnels qui ont été exécutés.

Dans cette documentation, découvrez comment effectuer les opérations suivantes :

* [Créer des messages transactionnels](create-transactional.md) à l’aide d’un modèle et connaître les paramètres nécessaires.
* [Validez le contenu de vos messages transactionnels](validate-transactional.md) et simulez la personnalisation,
* [Surveiller vos messages transactionnels](monitor-transactional.md).