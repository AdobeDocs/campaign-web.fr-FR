---
audience: end-user
title: Contenu génératif
description: Découvrez comment générer des expériences de contenu texte à l’aide de l’IA
exl-id: da60d57e-d17f-40eb-9c24-0bfea940d236
TQID: https://experienceleague.adobe.com/yV28iGW0nS-R6ZgQnfOrpfZlCzQu-1Ng1TH6aWD8QOg
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d4e22ba88bcb6dc74d22e8a927c1640f21d75d3e
workflow-type: tm+mt
source-wordcount: 1450
ht-degree: 75%

---

# Générer du texte {#generative-text}

>[!IMPORTANT]
>
>Avant de commencer à utiliser cette fonctionnalité, lisez la section sur les [Mécanismes de sécurisation et limitations](generative-gs.md#generative-guardrails).
></br>
>
>Vous devez accepter un [contrat d’utilisateur](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} avant d’utiliser l’IA pour générer du contenu dans Adobe Campaign Web. Pour plus d’informations, contactez votre représentant ou représentante Adobe.

Utilisez l’IA dans Adobe Campaign Web pour générer du texte attrayant qui résonne avec votre audience. Que vous amélioriez la copie des e-mails, créiez du contenu de page de destination convaincant, écriviez des messages de notification push ou composiez du texte de SMS, l’IA vous aide à diffuser une communication claire et percutante.

## Pour les e-mails et les pages de destination {#email-web-channels}

Utilisez l’IA pour générer du contenu texte de haute qualité pour vos diffusions e-mail et vos pages de destination. Cette fonctionnalité vous permet de créer des messages attrayants et conformes à votre marque, qui résonnent auprès de votre audience sur l’ensemble des points de contact numériques.

### Accéder et configurer {#access-configure}

Avant de pouvoir commencer à générer du contenu texte avec l’IA, vous devez configurer votre diffusion et accéder à l’éditeur de contenu. Pour préparer votre espace de travail, procédez comme suit et ouvrez le panneau Générer du contenu .

1. Créez et configurez votre diffusion :

   * **E-mail** : après avoir créé et configuré votre diffusion par e-mail, cliquez sur **[!UICONTROL Modifier le contenu]**. [En savoir plus](../email/create-email-content.md)
   * **Page de destination** : après avoir créé et configuré votre page de destination, cliquez sur **[!UICONTROL Modifier le contenu]**. [En savoir plus](../landing-pages/create-lp.md)

1. Sélectionnez un **[!UICONTROL composant de texte]** pour cibler un contenu spécifique, puis accédez au menu **[!UICONTROL Générer du contenu]**.

   ![Capture d’écran montrant la sélection du composant de texte dans Adobe Campaign Web](assets/text-genai-1.png){zoomable="yes"}

### Générer du texte {#generate-content}

Découvrez comment créer des invites claires, affiner les paramètres et générer du texte personnalisé à l’aide de l’IA, en veillant à ce que votre messagerie s’aligne sur vos objectifs de marque et de communication.

1. Sélectionnez votre **[!UICONTROL marque]** pour vous assurer que le contenu généré par l’IA correspond aux spécifications de votre marque. [En savoir plus](brands.md) sur les marques.

1. Ajustez le contenu en décrivant ce que vous souhaitez générer dans le champ **[!UICONTROL Prompt]**.

   Si vous avez besoin d’aide pour concevoir votre prompt, accédez à la **[!UICONTROL Bibliothèque de prompts]** qui vous met à disposition un large éventail d’idées de prompts pour améliorer vos diffusions. [En savoir plus sur les bonnes pratiques relatives aux prompts](ai-assistant-prompting-guide.md).

   ![Capture d’écran montrant la bibliothèque de prompts dans Adobe Campaign Web](assets/text-genai-2.png){zoomable="yes"}

1. Adaptez votre prompt à l’aide de l’option **[!UICONTROL Paramètres de texte]** :

   * **[!UICONTROL Stratégie de communication]** : choisissez le style de communication le plus adapté au texte généré.
   * **[!UICONTROL Langues]** : sélectionnez la langue du contenu généré.
   * **[!UICONTROL Ton]** : le ton de votre e-mail doit résonner auprès de votre audience. Que vous souhaitiez donner une impression informative, ludique ou persuasive, l’IA adapte le message en conséquence.
   * **Longueur de texte** : utilisez le curseur pour sélectionner la longueur souhaitée de votre texte.

     ![Capture d’écran montrant les options de paramètres de texte dans Adobe Campaign Web](assets/text-genai-4.png){zoomable="yes"}

1. Dans le menu **[!UICONTROL Contenu de référence]**, cliquez sur **[!UICONTROL Télécharger le fichier]** pour ajouter une ressource de marque contenant du contenu pouvant fournir une IA contextuelle supplémentaire ou sélectionnez une ressource précédemment chargée.

   Les fichiers précédemment chargés sont disponibles dans la liste déroulante **[!UICONTROL Contenu de référence chargé]**. Activez simplement les ressources que vous souhaitez inclure dans votre génération.

1. Lorsque votre prompt est prêt, cliquez sur **[!UICONTROL Générer]**.

### Affiner et finaliser {#refine-finalize}

Découvrez comment réviser le texte généré, apporter des améliorations et appliquer une personnalisation pour finaliser votre contenu, créer des messages soignés et attrayants prêts à être diffusés.

1. Parcourez les **[!UICONTROL variations]** générées.

1. Cliquez sur l’icône de pourcentage pour afficher votre **[!UICONTROL score d’alignement sur la marque]** et identifier les alignements incorrects avec votre marque.

   En savoir plus sur le [score d’alignement sur la marque](brands-score.md).

   ![](assets/text-genai-6.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Aperçu]** pour afficher une version en plein écran de la variation sélectionnée ou sur **[!UICONTROL Appliquer]** pour remplacer votre contenu actuel.

1. Accédez à l’option **[!UICONTROL Affiner]** dans la fenêtre **[!UICONTROL Aperçu]** pour accéder à d’autres fonctionnalités de personnalisation :

   * **[!UICONTROL Utiliser comme contenu de référence]** : la variante choisie sert de contenu de référence pour générer d’autres résultats.
   * **[!UICONTROL Élaborer]** : permet de développer des sujets spécifiques, en fournissant des détails supplémentaires pour une meilleure compréhension et un meilleur engagement.
   * **[!UICONTROL Résumer]** : permet de condenser des points clés en résumés clairs et concis qui retiennent l’attention et encouragent la lecture.
   * **[!UICONTROL Reformuler]** : permet de reformuler le message de différentes manières en conservant une écriture soignée et attrayante pour diverses audiences.
   * **[!UICONTROL Utiliser un langage plus simple]** : simplifiez votre texte pour en garantir la clarté et l’accessibilité pour une audience plus large.
   * **[!UICONTROL Traduire]** : simplifiez votre texte pour garantir la clarté et l’accessibilité afin de toucher une audience plus large.

   Vous pouvez également modifier le **[!UICONTROL Ton]** et la **[!UICONTROL Stratégie de communication]** de votre texte.

   ![Capture d’écran affichant les options d’affinement dans Adobe Campaign Web](assets/text-genai-5.png){zoomable="yes"}

1. Ouvrez l’onglet **[!UICONTROL Alignement sur la marque]** pour voir comment votre contenu s’aligne sur vos [directives de marque](../content/brands.md).

1. Cliquez sur **[!UICONTROL Sélectionner]** une fois que vous avez trouvé le contenu approprié.

1. Insérez des champs de personnalisation pour personnaliser votre contenu en fonction des données de profil. Cliquez ensuite sur le bouton **[!UICONTROL Simuler le contenu]** pour contrôler le rendu et vérifier les paramètres de personnalisation avec les profils de test. [En savoir plus](../preview-test/preview-content.md)

1. Examinez et activez votre contenu :
   * **E-mail** : lorsque vous avez défini le contenu, l’audience et le planning, vous pouvez préparer votre diffusion par e-mail. [En savoir plus](../monitor/prepare-send.md)
   * **Page de destination** : une fois votre page de destination prête, vous pouvez la publier afin de pouvoir l’utiliser dans un message. [En savoir plus](../landing-pages/create-lp.md)

## Pour les canaux mobiles {#mobile-channels}

Utilisez l’IA pour générer du contenu texte attrayant pour vos notifications push et vos SMS, ce qui vous permet de créer des communications mobiles attrayantes qui entrent en contact avec votre audience à travers tous les points de contact mobiles.

### Accéder et configurer {#mobile-access-configure}

Avant de commencer à générer du texte avec l’IA pour les canaux mobiles, vous devez configurer votre diffusion et accéder à Générer du contenu.

1. Créez et configurez votre diffusion mobile :
   * **Notifications push** : après avoir créé et configuré votre diffusion de notifications push, cliquez sur **[!UICONTROL Modifier le contenu]**. [En savoir plus](../push/create-push.md)
   * **SMS** : après avoir créé et configuré votre diffusion SMS, cliquez sur **[!UICONTROL Modifier le contenu]**. [En savoir plus](../sms/create-sms.md)

1. Personnalisez votre message selon vos besoins :
   * **Notifications push** : [en savoir plus](../push/content-push.md)
   * **SMS** : [en savoir plus](../sms/content-sms.md)

1. Accédez au menu **[!UICONTROL Afficher générer le contenu]**.

   ![Capture d’écran affichant le menu Afficher générer le contenu](assets/sms-genai-1.png){zoomable="yes"}

### Générer du texte {#mobile-generate-content}

Une fois que vous avez accédé à Générer du contenu, vous pouvez configurer les paramètres de génération pour créer du contenu mobile correspondant à votre marque et aux objectifs de diffusion. Personnalisez les paramètres de texte, ajoutez des ressources de marque et fournissez des prompts pour guider l’IA dans la génération de variations pertinentes.

1. Sélectionnez votre **[!UICONTROL marque]** pour vous assurer que le contenu généré par l’IA correspond aux spécifications de votre marque. [En savoir plus](brands.md) sur les marques.

1. Ajustez le contenu en décrivant ce que vous souhaitez générer dans le champ **[!UICONTROL Prompt]**.

   Si vous avez besoin d’aide pour concevoir votre prompt, accédez à la **[!UICONTROL Bibliothèque de prompts]** qui offre un large éventail d’idées de prompts pour améliorer votre diffusion. [En savoir plus sur les bonnes pratiques relatives aux prompts](ai-assistant-prompting-guide.md)

   ![Générer le contenu avec le champ et les options d’invite](assets/sms-genai-2.png){zoomable="yes"}

1. **Pour les notifications push**, sélectionnez le champ de texte à générer : **[!UICONTROL Titre]**, **[!UICONTROL Sous-titre]** et/ou **[!UICONTROL Message]**.

1. Adaptez votre prompt avec les options **[!UICONTROL Paramètres de texte]** :

   * **[!UICONTROL Stratégie de communication]** : choisissez le style de communication le plus adapté au texte généré.
   * **[!UICONTROL Langues]** : sélectionnez la langue du contenu généré.
   * **[!UICONTROL Ton]** : le ton doit trouver écho auprès de votre audience. Que vous souhaitiez donner une impression informative, ludique ou persuasive, l’IA peut adapter le message en conséquence.
   * **[!UICONTROL Longueur]** : sélectionnez la longueur de votre contenu à l’aide du curseur de plage.

     ![Panneau Paramètres de texte](assets/sms-genai-3.png){zoomable="yes"}

1. Dans le menu **[!UICONTROL Contenu de référence]**, cliquez sur **[!UICONTROL Télécharger le fichier]** pour ajouter une ressource de marque contenant du contenu pouvant fournir une IA contextuelle supplémentaire ou sélectionnez une ressource précédemment chargée.

   Les fichiers précédemment chargés sont disponibles dans la liste déroulante **[!UICONTROL Contenu de référence chargé]**. Activez simplement les ressources que vous souhaitez inclure dans votre génération.

1. Lorsque votre prompt est prêt, cliquez sur **[!UICONTROL Générer]**.

### Affiner et finaliser {#mobile-refine-finalize}

Après avoir généré des variations de texte pour vos messages mobiles, vous pouvez affiner les résultats pour vous assurer qu’ils répondent exactement à vos besoins. Examinez l’alignement sur la marque, ajustez le ton et le langage, puis préparez le contenu pour l’activation.

1. Après la génération, parcourez les **[!UICONTROL variations]**.

1. Cliquez sur l’icône de pourcentage pour afficher votre **[!UICONTROL score d’alignement sur la marque]** et identifier les alignements incorrects avec votre marque.

   En savoir plus sur le [score d’alignement sur la marque](brands-score.md).

   ![Menu Affiner](assets/sms-genai-4.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Aperçu]** pour afficher une version en plein écran de la variation sélectionnée ou cliquez sur **[!UICONTROL Appliquer]** pour remplacer votre contenu actuel.

1. Naviguez vers l’option **[!UICONTROL Affiner]** dans la fenêtre **[!UICONTROL Aperçu]** pour accéder à d’autres fonctionnalités de personnalisation :

   * **[!UICONTROL Utiliser comme contenu de référence]** : la variante choisie servira de contenu de référence pour générer d’autres résultats.

   * **[!UICONTROL Reformuler]** : réécrivez le message tout en préservant sa signification. Cette option vous permet de générer une autre formulation, d’améliorer le flux ou d’ajuster les expressions sans modifier le message principal.

   * **[!UICONTROL Utiliser un langage plus simple]** : utilisez l’IA pour modifier/affiner votre langue, en garantissant la clarté et l’accessibilité pour une audience plus large.

   * **[!UICONTROL Traduire]** : simplifiez votre texte pour garantir la clarté et l’accessibilité afin de toucher une audience plus large.

   * **[!UICONTROL Changer de ton]** : ajustez le ton du message pour mieux correspondre à votre style de communication, c’est-à-dire le rendre plus convivial, professionnel, urgent ou inspirant.

   * **[!UICONTROL Modifier la stratégie de communication]** : modifiez l’approche des messages en fonction de vos objectifs, tels que créer un sentiment d’urgence ou mettre en avant un aspect attractif et enthousiasmant.

     ![Variations de texte générées avec le score d’alignement sur la marque](assets/sms-genai-5.png){zoomable="yes"}

1. Ouvrez l’onglet **[!UICONTROL Alignement sur la marque]** pour voir comment votre contenu s’aligne sur vos [directives de marque](brands.md).

1. Cliquez sur **[!UICONTROL Sélectionner]** une fois que vous avez trouvé le contenu approprié.

1. Insérez des champs de personnalisation pour personnaliser votre contenu en fonction des données des profils. Cliquez ensuite sur le bouton **[!UICONTROL Simuler le contenu]** pour contrôler le rendu et vérifier les paramètres de personnalisation avec les profils de test. [En savoir plus](../personalization/personalize.md)

1. Examinez et activez votre contenu :
   * **Notification push** : lorsque vous avez défini le contenu, l’audience et le planning, vous pouvez préparer votre diffusion de notifications push. [En savoir plus](../push/send-push.md)
   * **SMS** : une fois votre SMS prêt, vous pouvez le publier afin de pouvoir l’utiliser dans un message. [En savoir plus](../sms/send-sms.md)
