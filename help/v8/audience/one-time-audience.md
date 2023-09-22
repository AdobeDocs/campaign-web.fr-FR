---
audience: end-user
title: Créer une audience unique pour une diffusion
description: Découvrez comment créer une audience unique pour une diffusion.
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 30%

---

# Créer une audience unique pour une diffusion {#sone-time}

Cette section décrit comment créer une audience lors de la création d’une diffusion. Dans ce cas, les destinataires à inclure dans l’audience de diffusion sont ciblés en interrogant la base de données avec le créateur de règles.

L&#39;audience obtenue n&#39;est utilisée qu&#39;une seule fois pour cette diffusion. Il n’est pas enregistré dans la liste des audiences.

Lors de la définition de la cible principale d&#39;une diffusion, vous pouvez également :

* [Sélectionner une audience existante](add-audience.md) de la **[!UICONTROL Audiences]** liste.
* [Chargement d’une audience à partir d’un fichier externe](file-audience.md) (pour les emails uniquement).

Pour créer une nouvelle audience directement depuis une diffusion, procédez comme suit :

1. Dans la section **Audience** de l’assistant de création de diffusion, cliquez sur le bouton **[!UICONTROL Sélectionner l’audience]**.

   ![](assets/segment-builder0.png)

1. Sélectionnez **Créez la vôtre**. Le créateur de règles s’affiche. Il permet de définir la population ciblée par votre diffusion en filtrant les données contenues dans la base de données. [Découvrez comment utiliser le créateur de règles](segment-builder.md)

   ![](assets/segment-builder.png)

1. Une fois votre requête prête, cliquez sur **Confirmer** pour utiliser l&#39;audience comme cible principale de votre diffusion.

   Vous pouvez également définir une population témoin afin de mesurer l’impact de vos campagnes. La population témoin ne reçoit pas le message. Vous pouvez ainsi comparer le comportement de la population qui a reçu le message avec celui des contacts qui ne l’ont pas reçu. [En savoir plus](control-group.md)
