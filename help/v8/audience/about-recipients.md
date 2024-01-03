---
title: Utiliser des destinataires et des audiences
description: Découvrez comment utiliser des destinataires Campaign Web
badge: label="Beta"
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 93%

---

# Utiliser des destinataires et des audiences {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360 vues de vos destinataires"
>abstract="Créez de nouvelles personnes destinataires et surveillez-les à l’aide de puissants rapports et outils. Accédez aux attributs, interactions et logs de votre destinataire. Utilisez les options de filtrage pour parcourir la liste des destinataires, éditer et mettre à jour leur profil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Voir les notes de mise à jour"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profils"
>abstract="Un profil est une personne ciblée pour recevoir les messages envoyés par Adobe Campaign. Dans Adobe Campaign, les destinataires sont les profils par défaut ciblés pour l’envoi de diffusions (e-mails, SMS). Depuis cette liste, vous pouvez visualiser le profil du ou de la destinataire, en fonction de vos autorisations. Utilisez les options de filtrage pour parcourir cette liste. Vous pouvez modifier et mettre à jour un petit ensemble d’attributs de votre destinataire."

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
