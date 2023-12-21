---
title: Utiliser des destinataires et des audiences
description: Découvrez comment utiliser des destinataires Campaign Web
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 686bcc06591d56c2827a6826286503659ee6b26c
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 95%

---

# Utiliser des destinataires et des audiences {#about-recipients}

Dans Adobe Campaign, la population cible d’une diffusion est une audience. Une audience est un ensemble de personnes qui partagent des comportements et/ou des caractéristiques similaires. Cette collection de personnes peut être générée, sélectionnée ou chargée [comme décrit ci-dessous](#audiences). Dans la plupart des cas, l’audience est composée de profils stockés sous la forme de [destinataires](#recipients) dans Adobe Campaign. Vous pouvez également travailler avec d’autres mappings de ciblage en modifiant la dimension, tel qu’expliqué [dans cette section](#targeting-dimensions).

## Que sont les destinataires ? {#recipients}


>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Destinataires"
>abstract="Créez de nouveaux destinataires et surveillez-les à l’aide de puissants rapports et outils. Accédez au profil de votre destinataire, utilisez les options de filtrage pour parcourir la liste des destinataires, éditer et mettre à jour ses attributs."

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profils"
>abstract="Un profil est un individu qui cible les messages envoyés par Adobe Campaign. Dans Adobe Campaign, les destinataires sont les profils par défaut ciblés pour l’envoi de diffusions (e-mails, SMS). Depuis cette liste, vous pouvez visualiser le profil du ou de la destinataire, en fonction de vos autorisations. Utilisez les options de filtrage pour parcourir cette liste. Vous pouvez modifier et mettre à jour un petit ensemble d’attributs de votre destinataire."

Un ou une destinataire est un profil ciblé pour recevoir les messages envoyés par Adobe Campaign. Dans Adobe Campaign, les destinataires sont les profils par défaut ciblés pour l’envoi de diffusions (e-mails, SMS, etc.). Les données de destinataire stockées dans la base de données permettent de créer des audiences qui recevront une diffusion donnée ainsi que d’ajouter des données de personnalisation dans le contenu de votre diffusion. D’autres types de profils existent dans la base de données. Ils sont conçus pour différentes utilisations : par exemple, des profils de contrôle sont créés pour tester vos diffusions avant leur envoi à l’audience finale.

Les destinataires ne peuvent être ajoutés que depuis la console cliente Campaign. Ils sont cependant visibles dans Campaign Web, à partir de l’entrée **Destinataires** du rail de navigation de gauche. Vous pouvez également modifier les attributs des destinataires à partir de cet écran.

Pour modifier les données d’un ou d’une destinataire, cliquez sur les trois points en regard de son nom et sélectionnez **Modifier**.

![Modifier le profil d’un ou d’une destinataire](assets/recipient-edit.png)

Vous pouvez mettre à jour un ensemble limité d’attributs, à savoir : son prénom, son nom, son e-mail et son numéro de téléphone.

![Mettre à jour un profil de destinataire](assets/recipient-update.png)

>[!NOTE]
>
>Ce formulaire de modification de profil limité est fourni uniquement pour le test du programme Bêta. Il sera amélioré dans la prochaine version. Il permet à l’utilisateur ou l’utilisatrice d’ajouter rapidement une adresse e-mail et un numéro de téléphone à n’importe quel profil afin de pouvoir tester les canaux e-mail et SMS et de recevoir les messages envoyés.

Vous pouvez filtrer les destinataires à l’aide du champ de recherche, à l’aide du bouton **Afficher les filtres**.

Vous pouvez également accéder aux destinataires à partir de la vue **Explorateur**, parcourir et créer des dossiers et des sous-dossiers, ainsi que vérifier les autorisations associées.

![Liste des destinataires à partir de la vue Explorateur](assets/recipients-from-explorer.png)

>[!NOTE]
>
>En fonction de vos autorisations, il se peut que vous n’ayez pas accès à la liste complète des destinataires stockés dans la base de données. Pour en savoir plus sur les autorisations, consultez [cette section](../get-started/permissions.md).

En outre, vous pouvez gérer l’abonnement et le désabonnement de vos destinataires à des services tels que les newsletters. Découvrez comment utiliser les services d’abonnement sur [cette page](manage-services.md).

Vous pouvez créer des workflows pour dédupliquer, enrichir, combiner des profils et créer des audiences. En savoir plus dans [cette section](../workflows/gs-workflows.md).

## Que sont les audiences ? {#audiences}

L’audience est la cible principale de votre diffusion : les destinataires qui reçoivent les messages. Le type d’audience dépend du mapping de ciblage défini dans le modèle de diffusion. Apprenez-en plus sur les modèles de diffusion sur [cette page](../msg/delivery-template.md).

Pour définir la population d’une audience, vous pouvez :

* [Créer de nouvelles audiences](create-audience.md) à partir du menu **[!UICONTROL Audiences]**.
* [Sélectionner une audience existante](add-audience.md) créée sous la forme d’une liste dans la console cliente ou provenant d’Adobe Experience Platform.
* [Créer une nouvelle audience](segment-builder.md) avec le créateur de règles en définissant et combinant des critères de filtrage,
* [Utiliser une audience depuis un fichier externe](file-audience.md). Cette option est disponible uniquement pour les diffusions d’e-mails autonomes et ne peut pas être utilisée dans les diffusions de campagne.

Lors du ciblage d’une audience, vous pouvez également définir des **populations témoins** afin d’éviter d’envoyer des messages à une partie de votre audience et pour mesurer l’impact de vos campagnes. [Découvrez comment définir une population témoin](control-group.md)

>[!NOTE]
>
>Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience est définie dans une activité de workflow **Créer une audience** spécifique. Dans ce contexte, vous ne pouvez pas charger une audience depuis un fichier pour une diffusion par e-mail, et l’audience n’est définie que dans cette activité dédiée. Découvrez comment définir l’audience de votre diffusion dans un workflow de campagne dans [cette section](../workflows/activities/build-audience.md).

## Dimensions de ciblage {#targeting-dimensions}

La dimension de ciblage, c’est-à-dire le mapping de ciblage, est le type de données qu’une opération traite. Il permet de définir la population ciblée : destinataires, bénéficiaires de contrats, opérateurs et opératrices, abonnés et abonnées, etc.

La dimension de ciblage d’un workflow est définie par la première activité **[!UICONTROL Créer une audience]** et est utilisée dans toutes les autres activités jusqu’à la fin du workflow. Si vous effectuez par exemple une requête sur les destinataires de la base de données, la transition sortante contiendra des données de type destinataire et sera transmise à l’activité suivante.

Notez que vous pouvez changer la dimension de ciblage dans un workflow à l’aide d’une activité [Changer une dimension](../workflows/activities/change-dimension.md). Vous pouvez ainsi, par exemple, interroger la base de données sur un tableau spécifique tel que des achats ou des inscriptions, puis changer la dimension de ciblage par Destinataires afin d’envoyer des diffusions aux destinataires correspondants.

Par défaut, les modèles de diffusion par e-mail et SMS ciblent les **[!UICONTROL destinataires]**. Leur dimension de ciblage utilise donc les champs du tableau **nms:recipient**. Pour les notifications push, la dimension de ciblage par défaut est **Applications Abonnés (nms:appSubscriptionRcp)**, qui est liée au tableau des destinataires.

Vous pouvez également utiliser d’autres mappings de ciblage intégrés dans vos workflows et diffusions répertoriés ci-dessous :

| Nom | Utilisez pour | Schéma |
|---|---|---|
| Destinataires | Diffuser aux destinataires (tableau de destinataires intégré) | nms:recipient |
| Visiteurs | Diffuser aux visiteurs dont les profils ont été collectés par le biais d’une recommandation (marketing viral), par exemple. | mns:visitor |
| Abonnements  | Diffuser aux destinataires abonnés à un service d&#39;information, par exemple une newsletter | nms:subscription |
| Abonnements des visiteurs | Diffuser à des visiteurs abonnés à un service d&#39;information | nms:visitorSub |
| Les opérateurs | Diffuser aux opérateurs Adobe Campaign | nms:operator |
| Fichier externe | Diffuser depuis un fichier contenant les toutes informations nécessaires à la diffusion | Aucun schéma associé, aucune cible renseignée |
| Applications abonnés | Diffuser aux destinataires abonnés à une application | nms:appSubscriptionRcp |

En outre, vous pouvez créer un nouveau mapping de ciblage selon vos besoins. Cette opération est effectuée à partir de la console cliente. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr#new-mapping){target="_blank"}.
