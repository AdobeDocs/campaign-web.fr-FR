---
audience: end-user
title: Prise en main de l’assistant de contenu
description: Prise en main de l’assistant de contenu
badge: label="Beta"
source-git-commit: 2da9bdab7e8a5050d0e4e0531fc30f85870de70f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---


# Prise en main de l’assistant de contenu {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistant de contenu"
>abstract="Une fois que vous avez conçu et personnalisé votre diffusion, vous pouvez utiliser l’assistant de contenu pour améliorer votre contenu. Cette fonctionnalité simplifie le processus de personnalisation et d’amélioration du contenu en vous permettant d’affiner le contenu en décrivant ce que vous souhaitez générer."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Définition du contexte pour la génération de contenu"
>abstract="Pour utiliser le contenu sélectionné comme entrée pour la génération du contenu, activez la variable **Amélioration du contenu actuel** bascule. Vous pouvez également charger vos ressources de marque pour les utiliser comme source. Si vous n’utilisez pas le contenu sélectionné, le téléchargement et la sélection de ressources de marque sont obligatoires."

L’assistant de contenu, optimisé par une IA générative, est un outil précieux pour améliorer le contenu des emails. Elle simplifie la personnalisation et l’amélioration du contenu, optimisant vos diffusions email pour mieux résonner avec votre audience.

Cette fonctionnalité permet de gagner du temps et d’assurer une qualité cohérente en générant automatiquement un contenu d’email complet. En utilisant l’IA générique, vous pouvez créer des emails attrayants sans effort, améliorant ainsi l’efficacité et l’efficience de vos communications.

L&#39;assistant de contenu de Campaign est accessible dans vos emails pour : [générer des images ;](generative-image.md), [générer du contenu texte ;](generative-content.md), [générer le contenu complet du HTML ;](generative-email.md).


## Mécanismes de sécurisation et limitations {#generative-guardrails}

Vous trouverez ci-dessous des instructions générales concernant l’utilisation de l’assistant de contenu pour la génération de courriers électroniques :

* La qualité du contenu généré est fortement influencée par l’objectif/l’invite marketing que vous définissez. Utilisez une invite bien définie pour que le modèle GenAI soit interprété avec précision. 
* Chargez les ressources de marque pour qu’elles soient précises sur le contenu de la marque. Sinon, le contenu est basé sur des informations disponibles publiquement. Le contenu téléchargé peut être : des fichiers de PDF, des documents Microsoft Word, des fichiers JPEG, PNG ou ZIP (avec les formats de fichier pris en charge).
* La taille recommandée pour la ressource de marque chargée est inférieure à 10 Mo. Des fichiers plus volumineux ou de nombreuses images peuvent fonctionner, mais le temps de traitement est augmenté.
* Utilisez des modèles d’email créés par Adobe Campaign, ou de préférence [modèles de courrier électronique intégrés](../content/email-sample-templates.md) pour créer le contenu de votre email. Il est recommandé d’utiliser un modèle d’email contenant jusqu’à 8-10 images.


Les restrictions suivantes s’appliquent à l’assistant de contenu Campaign :

* La langue prise en charge est l’anglais uniquement
* Disponible uniquement pour le canal Email
* Le contenu de GenAI n&#39;est peut-être pas toujours précis : partagez vos commentaires pour que nos ingénieurs puissent affiner les modèles.
* Vous pouvez charger plusieurs ressources de marque, mais vous ne pouvez en exploiter qu’une seule pour une génération spécifique.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Génération de texte" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Génération de texte à l’aide de l’assistant de contenu</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Génération d’images" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Génération d’images à l’aide de l’assistant de contenu</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="Génération d&apos;emails" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>Génération d’emails à l’aide de l’assistant de contenu</strong></a>
</div>
<p></td>
</tr></table>

