---
audience: end-user
title: Commencer avec l’assistant de contenu
description: Commencer avec l’assistant de contenu
badge: label="Alpha"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 686bcc06591d56c2827a6826286503659ee6b26c
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 100%

---

# Commencer avec l’assistant de contenu {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn5"
>title="IA générative pour le contenu d’e-mails"
>abstract="Notre technologie d’IA générative utilise des algorithmes avancés pour générer du contenu hautement attrayant et personnalisé. Augmentez les taux d’ouvertures, les taux de clics et les conversions grâce à la génération de contenu intelligent par l’IA générative. Gardez toujours une longueur d’avance sur la concurrence et optimisez votre marketing par e-mail avec la génération de contenu d’e-mails par IA générative."


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistant de contenu"
>abstract="Une fois que vous avez conçu et personnalisé votre diffusion, vous pouvez utiliser l’assistant de contenu pour améliorer votre contenu. Cette fonctionnalité simplifie le processus de personnalisation et d’amélioration du contenu en vous permettant d’affiner le contenu en décrivant ce que vous souhaitez générer."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Définition du contexte pour la génération de contenu"
>abstract="Pour utiliser le contenu sélectionné comme entrée pour la génération de contenu, activez le bouton (bascule) **Améliorer le contenu actuel**. Vous pouvez également charger vos ressources de marque pour les utiliser comme source. Si vous n’utilisez pas le contenu sélectionné, le chargement et la sélection de ressources de marque sont obligatoires."

L’assistant de contenu, optimisé par une IA générative, est un outil précieux qui permet d’améliorer le contenu des e-mails. Il simplifie la personnalisation et l’amélioration du contenu, en optimisant vos diffusions e-mail afin de mieux résonner avec votre audience.

Cette fonctionnalité permet de gagner du temps et d’assurer une qualité cohérente en générant automatiquement un contenu d’e-mail complet. En utilisant l’IA générative, vous pouvez créer des e-mails attrayants sans effort, améliorant ainsi l’efficacité et la rapidité de vos communications.


L’assistant de contenu de Campaign est accessible dans vos e-mails pour : [générer des images](generative-image.md), [générer du contenu texte](generative-content.md), [générer le contenu HML complet](generative-email.md).

>[!NOTE]
>
>Cette fonctionnalité est disponible dans sa version Alpha et peut être modifiée sans préavis. Elle sera activée début octobre.

## Mécanismes de sécurisation et limitations {#generative-guardrails}

Vous trouverez ci-dessous des instructions générales concernant l’utilisation de l’assistant de contenu pour la génération d’e-mails :

* La qualité du contenu généré est fortement influencée par l’invite/l’objectif marketing que vous définissez. Utilisez une invite bien définie pour que le modèle GenAI soit interprété avec précision. 
* Chargez les ressources de marque pour qu’elles soient précises sur le contenu de la marque. Autrement, le contenu est basé sur des informations disponibles au public. Le contenu chargé peut se présenter dans les formats suivants : fichiers PDF, JPEG, PNG ou ZIP (avec les formats de fichiers pris en charge).
* La taille recommandée pour la ressource de marque chargée est inférieure à 10 Mo.Des fichiers plus volumineux ou de nombreuses images peuvent être traités, mais le temps de traitement sera plus long.
* Utilisez des modèles d’e-mails créés par Adobe Campaign, ou de préférence des [modèles d’e-mails intégrés](../content/email-sample-templates.md) pour créer le contenu de votre e-mail. Il est recommandé d’utiliser un modèle d’e-mail contenant jusqu’à 8-10 images.


Les restrictions suivantes s’appliquent à l’assistant de contenu Campaign :

* La langue prise en charge est uniquement l’anglais.
* Disponible uniquement pour le canal e-mail.
* Il est possible que le contenu de GenAI ne soit pas toujours précis : partagez vos commentaires pour que nos ingénieures et ingénieurs puissent affiner les modèles.
* Vous pouvez charger plusieurs ressources de marque, mais vous ne pouvez en exploiter qu’une seule pour une génération spécifique.



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Génération de texte" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Génération de texte avec l’assistant de contenu</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Génération d’images" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Génération d’images avec l’assistant de contenu</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="Génération d’e-mails" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>Génération d’e-mails avec l’assistant de contenu</strong></a>
</div>
<p></td>
</tr></table>
