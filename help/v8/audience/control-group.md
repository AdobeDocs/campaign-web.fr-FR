---
audience: end-user
title: Configurer une population témoin
description: Découvrez comment définir une population témoin pour vos messages dans l’interface utilisateur web de Campaign
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 71%

---

# Configurer une population témoin {#control-group}

Vous pouvez utiliser des populations témoins pour éviter d’envoyer des messages à une partie de votre audience afin de mesurer l’impact de vos campagnes.

Créez une population témoin lors de la définition de l’audience de votre diffusion. Les profils sont ajoutés à la population témoin de manière aléatoire, filtrés ou non, ou selon des critères. Vous pouvez ensuite comparer le comportement de la population cible qui a bien reçu le message au comportement des contacts qui n&#39;ont pas été ciblés.

La population témoin peut être extraite de manière aléatoire de la cible principale et/ou sélectionnée dans une population spécifique. Par conséquent, vous pouvez définir une population témoin de deux manières principales :

* En extrayant un certain nombre de profils de la cible principale.
* En excluant certains profils en fonction de critères définis dans une requête.

Vous pouvez utiliser les deux méthodes lors de la définition d’une population témoin.

Tous les profils faisant partie de la population témoin à l’étape de préparation de la diffusion sont supprimés de la cible principale. Ils ne reçoivent pas le message.

Pour créer une population témoin, cliquez sur le bouton **[!UICONTROL Définir la population témoin]** à partir de la section **Audience** de l’assistant de création de diffusion.

![](assets/control-group1.png)

## Extraire à partir de la cible {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extraire à partir de la cible"
>abstract="TBC"

Pour définir une population témoin, vous pouvez choisir d’extraire, de manière aléatoire ou selon un tri, un pourcentage ou un nombre fixe de profils de la population cible.

Tout d&#39;abord, définissez la manière dont les profils sont extraits de la cible : de manière aléatoire ou selon un tri.

Dans la section **Extraire à partir de la cible**, sélectionnez un **Type d’exclusion** :

* **Random**: lors de la préparation de la diffusion, Adobe Campaign extrait de manière aléatoire un certain nombre de profils correspondant au pourcentage ou au nombre maximum défini comme limite de taille.

   ![](assets/control-group.png)

* **Classement par attribut(s)** : cette option permet d’exclure un jeu de profils en fonction d’un ou de plusieurs attributs spécifiques dans un ou plusieurs ordres de tri spécifiques.

   ![](assets/control-group2.png)

Définissez ensuite la variable **Limite de taille** : vous devez définir la manière dont vous allez limiter le nombre de profils que vous extrayez de la cible principale.

**Exemple**

Vous pouvez consulter les logs pour vérifier et identifier les profils exclus. Prenons l’exemple suivant d’une exclusion aléatoire sur cinq profils.

![](assets/control-group4.png)

Après la préparation de la diffusion, vous pouvez visualiser les exclusions sur les écrans suivants :

* L’indicateur clé de performance (KPI) **À exclure** dans le tableau de bord de la diffusion, avant l’envoi.

   ![](assets/control-group5.png)

* Le **Exclus** afficher chaque profil et l’exclusion associée ; **Motif**.

   ![](assets/control-group6.png)

* Le **Exclusions appliquées** afficher le nombre de profils exclus pour chaque règle de typologie.

   ![](assets/control-group7.png)

Pour plus d’informations sur les logs de diffusion, consultez [cette section](../monitor/delivery-logs.md).

## Population supplémentaire {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Population supplémentaire"
>abstract="TBC"

Vous pouvez également définir une population témoin en excluant une population spécifique de la cible. Pour cela, vous pouvez utilisez une audience existante ou définir une requête.

Dans la section **Population supplémentaire** de l’écran de définition de la **Population témoin**, cliquez sur le bouton **[!UICONTROL Sélectionner une audience]**.

![](assets/control-group3.png)

* Pour utiliser une audience existante, cliquez sur **Sélectionner une audience**. Reportez-vous à cette [section](add-audience.md).

* Pour définir une nouvelle requête, sélectionnez **Créer la vôtre** et définissez les critères d’exclusion à l’aide du créateur de règles. Reportez-vous à cette [section](segment-builder.md).

Les profils inclus dans l&#39;audience ou correspondant au résultat de la requête sont exclus de la cible.