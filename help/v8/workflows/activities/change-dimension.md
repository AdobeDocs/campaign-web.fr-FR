---
audience: end-user
title: Utiliser l’activité de workflow Changement de dimension
description: Découvrez comment utiliser l’activité de workflow Changement de dimension.
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 54%

---

# Changement de dimension {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Générer un complément"
>abstract="Vous pouvez générer une transition sortante supplémentaire avec la population restante, qui a été exclue en tant que doublon. Pour ce faire, activez l’option **Générer un complément**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Activité Changement de dimension"
>abstract="Cette activité vous permet de modifier la dimension de ciblage à mesure que vous créez une audience. Elle déplace l’axe en fonction du modèle de données et de la dimension d’entrée. Par exemple, vous pouvez passer de la dimension « contrats » à la dimension « clients »."

L’activité **Changement de dimension** est une activité de **ciblage**. Cette activité permet de modifier la dimension de ciblage au fur et à mesure de la construction de votre workflow. Elle déplace l’axe en fonction du modèle de données et de la dimension d’entrée. [Découvrez les dimensions de ciblage](../../audience/about-recipients.md#targeting-dimensions).

Par exemple, vous pouvez basculer la dimension de ciblage d’un workflow de « Destinataires » vers « Application des abonnés » pour envoyer des notifications push aux destinataires ciblés.

>[!IMPORTANT]
>
>Notez que les activités **[!UICONTROL Changer la dimension]** et **[!UICONTROL Modifier la source de données]** ne doivent pas être ajoutées sur une même ligne. Si vous devez utiliser les deux activités de manière consécutive, incluez une activité **[!UICONTROL Enrichissement]** entre elles. Cela garantit une bonne exécution et évite les erreurs et conflits potentiels.

## Configurer l’activité Changement de dimension {#configure}

Pour configurer l’activité **Changement de dimension**, procédez comme suit :

1. Ajoutez une activité **Changement de dimension** à votre workflow.

   ![Capture d’écran montrant l’activité Changement de dimension ajoutée à un workflow](../assets/workflow-change-dimension.png)

1. Définissez la **Nouvelle dimension cible**. Lors du changement de dimension, tous les enregistrements sont conservés. D’autres options ne sont pas encore disponibles.

1. Exécutez le workflow pour afficher le résultat. Comparez les données dans les tableaux avant et après l’activité Changement de dimension et comparez la structure des tableaux de workflow.

## Exemple {#example}

Dans cet exemple, envoyez une diffusion SMS à tous les profils qui ont effectué un achat. Tout d’abord, utilisez une activité **[!UICONTROL Créer une audience]** liée à une dimension de ciblage « Achat » personnalisée pour cibler tous les achats effectués.

Ensuite, utilisez une activité **[!UICONTROL Modifier la dimension]** pour basculer la dimension de ciblage du workflow sur « Destinataires ». Cela permet de cibler les destinataires qui correspondent à la requête.

![Capture d’écran montrant un exemple de l’activité Changement de dimension utilisée dans un workflow](../assets/workflow-change-dimension-example.png)