---
audience: end-user
title: Commencer avec les audiences
description: Découvrez comment utiliser les audiences dans l’interface utilisateur web de Campaign.
badge: label="Beta"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 100%

---


# Commencer avec les audiences {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


L’audience est la cible principale de votre diffusion : les destinataires qui reçoivent les messages. Le type d’audience dépend du mapping de ciblage défini dans le modèle de diffusion. Découvrez ce qu’est un modèle de diffusion [dans cette section](../msg/delivery-template.md).

Pour définir la population de l’audience, vous pouvez :

* Sélectionnez une audience existante, créée sous forme de liste dans la console cliente. [En savoir plus](add-audience.md)
* Sélectionnez une audience Adobe Experience Platform. [En savoir plus](aep-audience.md)
* Créez une nouvelle audience avec le créateur de règles en définissant et combinant des critères de filtrage. [En savoir plus](segment-builder.md)
* Utiliser une audience depuis un fichier externe : cette option est disponible uniquement pour les diffusions d’e-mail autonomes et ne peut pas être utilisée dans les diffusions de campagne. [En savoir plus](file-audience.md)

Lors de l’envoi de messages dans le cadre d’un workflow de campagne, l’audience est définie dans une activité de workflow **Lecture d’audience** spécifique. Dans ce contexte, vous ne pouvez pas charger une audience depuis un fichier pour une diffusion par e-mail, et l’audience n’est définie que dans cette activité dédiée. Découvrez comment définir l’audience de votre diffusion dans un workflow de campagne [dans cette section](../workflows/orchestrate-activities.md).

Vous pouvez également définir des populations témoins afin d’éviter d’envoyer des messages à une partie de votre audience et pour mesurer l’impact de vos campagnes. [En savoir plus](control-group.md)

![](assets/about-audience.png)

