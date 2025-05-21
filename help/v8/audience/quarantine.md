---
audience: end-user
title: À propos de la quarantaine
description: Comprendre la gestion des adresses en quarantaine
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 100%

---

# Gestion des quarantaines {#quarantines}

Adobe Campaign gère les adresses en quarantaine pour les canaux e-mail, push, SMS.

La quarantaine s’applique uniquement à une **adresse e-mail**, un **numéro de téléphone** ou un **jeton d’appareil**, mais pas au profil lui-même. Par exemple, un profil dont l’adresse e-mail est en quarantaine peut être mis à jour avec une nouvelle adresse. Le profil pourrait alors être ciblé de nouveau par des actions de diffusion. De même, si deux profils ont le même numéro de téléphone, ils seront tous deux affectés si le numéro est mis en quarantaine.

>[!CAUTION]
>
>La quarantaine dans Adobe Campaign respecte la casse.

## Qu’est-ce que la quarantaine ? {#quarantines-what}

La quarantaine est la méthode pour **gérer les adresses non valides dans les diffusions**.

Si une diffusion a un taux d’adresses non valides élevé, elle peut être considérée comme un spam. La gestion de ces adresses en quarantaine permet d’éviter que les fournisseurs d’accès à Internet soient placés sur la liste bloquée. Cela est important pour votre réputation.

Lorsqu’une adresse est mise en quarantaine dans Adobe Campaign, le profil est automatiquement exclu de la cible lors de l’analyse de la diffusion.

La quarantaine réduit les coûts d&#39;envoi des SMS en excluant les numéros de téléphone erronés des diffusions.

En savoir plus sur les quarantaines dans la [documentation de Campaign v8 (console)](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"}.

## Raisons de la mise en quarantaine d’une adresse {#quarantines-why}

Une adresse peut être mise en quarantaine pour de nombreuses raisons :

* Pour les SMS, des numéros de téléphone erronés.
* Pour les SMS, lorsque le profil répond à un SMS avec un mot-clé tel que « STOP ».
* Pour les e-mails, lorsque votre message est signalé comme un spam. Le message est automatiquement redirigé vers une boîte e-mail technique gérée par Adobe. L’adresse e-mail de l’utilisateur ou de l’utilisatrice est alors automatiquement mise en quarantaine avec le statut Placé sur la liste bloquée.
* Une adresse e-mail peut être mise en quarantaine, par exemple, lorsque la boîte de réception est pleine, si l’adresse n’existe pas ou si le serveur de messagerie n’est pas disponible.

En savoir plus sur les échecs de diffusions dans la [documentation de Campaign v8 (console)](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"}.

## Où trouver les adresses en quarantaine ? {#quarantines-where}

Vous pouvez afficher toutes les adresses en quarantaine de votre instance dans **[!UICONTROL Explorateur]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion de campagnes]** > **[!UICONTROL Gestion des échecs]** > **[!UICONTROL Échecs et adresses]**. Cette section répertorie les éléments en quarantaine pour les canaux e-mail, SMS et notification push.

![Emplacement de quarantaine dans l’interface d’Adobe Campaign](assets/quarantine_location.png){zoomable="yes"}

Vous pouvez également obtenir un rapport sur la quarantaine dans votre instance :

![Rapports de quarantaine dans l’interface d’Adobe Campaign](assets/quarantine_reports.png){zoomable="yes"}

Pour chaque diffusion, vous pouvez consulter le rapport Synthèse des diffusions. Il affiche le nombre d’adresses en quarantaine dans la cible de diffusion :

![Rapport de synthèse des diffusions présentant les adresses en quarantaine](assets/quarantine_delivery.png){zoomable="yes"}

Vous pouvez explorer d’autres options de gestion des adresses de quarantaine dans la console Adobe Campaign. [En savoir plus](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses).