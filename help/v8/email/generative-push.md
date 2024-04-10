---
audience: end-user
title: Notification push avec l'assistant AI dans Campaign
description: Prise en main de l’assistant AI dans Campaign
badge: label="Version bêta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 886fd47b52d08b0a1bfcbeca03929d48b5bc2a3f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 34%

---

# Génération de notifications push avec l’assistant AI {#generative-push}

>[!BEGINSHADEBOX]

**Table des matières**

* [Prise en main de l’assistant IA](generative-gs.md)
* [Génération d’e-mails avec l’assistant AI](generative-content.md)
* [Génération de SMS avec l’assistant AI](generative-sms.md)
* **[Génération de notifications push avec l’assistant AI](generative-push.md)**

>[!ENDSHADEBOX]

Une fois que vous avez créé et personnalisé vos e-mails, utilisez l’assistant d’IA dans Campaign optimisé par l’IA générative pour faire passer votre contenu au niveau supérieur.

L’assistant d’IA peut vous aider à optimiser l’impact de vos diffusions en suggérant un contenu différent qui résonnera davantage auprès de votre audience.

>[!NOTE]
>
>Avant de commencer à utiliser cette fonctionnalité, lisez la section connexe [Mécanismes de sécurisation et limitations](generative-gs.md#guardrails-and-limitations).

1. Après avoir créé et configuré votre diffusion Notification push, cliquez sur **[!UICONTROL Modifier le contenu]**.

   Pour plus d&#39;informations sur la configuration de votre diffusion push, voir [cette page](../push/create-push.md).

1. Renseignez les **[!UICONTROL détails de base]** de votre diffusion. Une fois que vous avez terminé, cliquez sur **[!UICONTROL Modifier le contenu]**.

1. Personnalisez votre notification push selon vos besoins. [En savoir plus](../push/content-push.md)

1. Accéder au **[!UICONTROL Afficher l’assistant AI]** menu.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. Ajustez le contenu en décrivant ce que vous souhaitez générer dans le **[!UICONTROL Invite]** champ .

   Si vous avez besoin d’aide pour concevoir votre invite, accédez au **[!UICONTROL Bibliothèque d’invites]** qui propose une gamme variée d&#39;idées rapides pour améliorer vos diffusions.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. Activer le **[!UICONTROL Améliorer avec le contexte actuel]** option permettant à l’assistant AI de personnaliser le nouveau contenu en fonction de votre diffusion, du nom de la diffusion et de l’audience sélectionnée.

   >[!IMPORTANT]
   >
   > Votre invite doit toujours être liée à un contexte spécifique en chargeant une ressource de marque ou en activant la variable **[!UICONTROL Améliorer le contenu actuel]** option.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. Sélectionner **[!UICONTROL Charger une ressource de marque]** pour ajouter une ressource de marque dont le contenu peut fournir un contexte supplémentaire à l’assistant d’IA, procédez comme suit :

1. Choisissez le champ à générer : **[!UICONTROL Titre]**, **[!UICONTROL Sous-titre]** ou **[!UICONTROL Message]**.

1. Sélectionnez la **[!UICONTROL Stratégie de communication]** qui répond le mieux à vos besoins. Cette dernière a une incidence sur la tonalité et le style du texte généré.

1. Choisissez la **[!UICONTROL Langue]** et le **[!UICONTROL Ton]** à donner au texte. Vous vous assurez ainsi que le texte est adapté à votre audience et à votre objectif.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. Lorsque votre texte descriptif est prêt, cliquez sur **[!UICONTROL Générer]**.

1. Parcourez les **[!UICONTROL Variations]** générées et cliquez sur **[!UICONTROL Appliquer]** une fois que vous avez trouvé le contenu approprié.

   Cliquez sur **[!UICONTROL Aperçu]** pour afficher une version plein écran de la variation sélectionnée.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. Insérez des champs de personnalisation pour personnaliser votre contenu push en fonction des données de profil. [En savoir plus sur la personnalisation du contenu](../personalization/personalize.md).

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

1. Après avoir défini le contenu de votre message, cliquez sur le bouton **[!UICONTROL Simuler le contenu]** pour contrôler le rendu et vérifier les paramètres de personnalisation avec les profils de test. [En savoir plus](../preview-test/preview-content.md)

   ![](assets/push-genai-7.png){zoomable=&quot;yes&quot;}

1. Lorsque vous avez défini le contenu, l’audience et le planning, vous êtes prêt(e) à préparer votre diffusion push. [En savoir plus](../monitor/prepare-send.md)
