---
audience: end-user
title: Créer une audience unique pour une diffusion
description: Découvrez comment créer une audience unique pour une diffusion.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
TQID: https://experienceleague.adobe.com/96G-USwsSAOJUSeXTpgpCTgeCNfwgIBHorvcxvObcuw
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 251
ht-degree: 91%

---

# Créer une audience ponctuelle {#one-time}

Cette section explique comment créer une audience lors de la création d’une nouvelle diffusion. Dans ce scénario, les profils inclus dans l’audience de diffusion sont ciblés en interrogeant la base de données à l’aide du concepteur de requête. L’audience obtenue est utilisée une seule fois pour cette diffusion et n’est pas enregistrée dans la liste des audiences.

Lors de la définition de la cible principale d’une diffusion, vous pouvez également :
* [Sélectionnez une audience existante](add-audience.md) dans la liste **[!UICONTROL Audiences]**.
* [Chargez une audience depuis un fichier externe](file-audience.md) (pour les e-mails uniquement).

Pour créer une audience unique pour une diffusion, procédez comme suit :

1. Dans la section **Audience** de l’assistant de création de diffusion, cliquez sur le bouton **[!UICONTROL Sélectionner une audience]**.

   [Capture d’écran affichant la section Audience de l’assistant de création de diffusion avec le bouton Sélectionner une audience en surbrillance](assets/segment-builder0.png){zoomable="yes"}

1. Sélectionnez **Créer la vôtre** pour ouvrir le concepteur de requête. Le concepteur de requête permet de définir la population ciblée en filtrant les données contenues dans la base de données. [Découvrir comment utiliser le concepteur de requête](../query/query-modeler-overview.md).

   [Capture d’écran montrant l’interface du requêteur](assets/query-modeler.png){zoomable="yes"}

1. Une fois votre requête prête, cliquez sur **Confirmer** pour utiliser l’audience créée comme cible principale de votre diffusion.

   Vous pouvez également définir une population témoin afin de mesurer l’impact de vos campagnes. La population témoin ne reçoit pas le message. Vous pouvez ainsi comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l’ont pas reçu. [En savoir plus](control-group.md).