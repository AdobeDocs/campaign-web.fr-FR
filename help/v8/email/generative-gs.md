---
audience: end-user
title: Commencer avec l’assistant IA
description: Commencer avec l’assistant IA
badge: label="Version bêta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: f249a73e25857e65e200f3cbd9516206aab918f9
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 90%

---

# Commencer avec l’assistant IA {#generative-gs}

>[!BEGINSHADEBOX]

**Table des matières**

* **[Commencer avec l’assistant IA](generative-gs.md)**
* [Génération d’e-mails avec l’assistant IA](generative-content.md)
* [Génération de SMS avec l’assistant IA](generative-sms.md)
* [Génération de notifications push avec l’assistant AI](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistant IA"
>abstract="Une fois que vous avez conçu et personnalisé votre diffusion, vous pouvez utiliser l’assistant IA pour améliorer votre contenu. Cette fonctionnalité simplifie le processus de personnalisation et d’amélioration du contenu en vous permettant d’affiner le contenu en décrivant ce que vous souhaitez générer."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Définir le contexte à l’aide de l’assistant IA dans Campaign"
>abstract="Pour utiliser le contenu sélectionné comme entrée pour la génération de contenu, activez le bouton (bascule) **Améliorer le contenu actuel**. Vous pouvez également charger vos ressources de marque pour les utiliser comme source. Si vous n’utilisez pas le contenu sélectionné, le chargement et la sélection de ressources de marque sont obligatoires."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Conditions de l’IA générative d’Adobe"
>abstract="L’accès à cette fonctionnalité est soumis à votre acceptation des directives d’utilisation de l’IA générative d’Adobe Experience Cloud et aux conditions suivantes : Les instructions, les informations contextuelles ou supplémentaires, ou toute autre information que vous saisissez dans cette fonctionnalité, doivent être liées à un contexte spécifique, ce qui peut inclure vos éléments de marque, le contenu de votre site web, vos données, les schémas de ces données, vos modèles ou autres documents approuvés, et ne doit pas contenir d’informations personnelles (les informations personnelles incluent tout ce qui peut être associé à une personne spécifique). Vous devez vérifier la précision des résultats de cette fonctionnalité et vous assurer qu’ils sont adaptés à votre cas d’utilisation."
>additional-url="https://www.adobe.com/fr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directives d’utilisation de l’IA générative d’Adobe"

L’assistant d’IA, optimisé par Azure OpenAI et Azure AI, constitue un outil précieux pour améliorer le contenu des emails. Il simplifie la personnalisation et l’amélioration du contenu, en optimisant vos diffusions e-mail afin de mieux résonner avec votre audience.

Cette fonctionnalité permet de gagner du temps et d’assurer une qualité cohérente en générant automatiquement un contenu d’e-mail complet. En utilisant l’IA générative, vous pouvez créer des e-mails attrayants sans effort, améliorant ainsi l’efficacité et la rapidité de vos communications.

>[!NOTE]
>
>Cette fonctionnalité est disponible dans sa version Alpha et peut être modifiée sans préavis. Elle sera activée début octobre.

## Mécanismes de sécurisation et limitations {#generative-guardrails}

Vous trouverez ci-dessous des instructions générales concernant l’utilisation de l’assistant IA dans Campaign pour la génération d’e-mails :

* La qualité du contenu généré est fortement influencée par l’invite/l’objectif marketing que vous définissez. Utilisez une invite bien définie pour que le modèle GenAI soit interprété avec précision. 
* Chargez les ressources de marque pour qu’elles soient précises sur le contenu de la marque. Autrement, le contenu est basé sur des informations disponibles au public. Le contenu chargé peut se présenter dans les formats suivants : fichiers PDF, JPEG, PNG ou ZIP (avec les formats de fichiers pris en charge).
* La taille recommandée pour la ressource de marque chargée est inférieure à 50 Mo.Des fichiers plus volumineux ou de nombreuses images peuvent faire l’objet d’un traitement, mais le temps de traitement sera plus long.
* Utilisez des modèles d’e-mails créés par Adobe Campaign, ou de préférence des [modèles d’e-mails intégrés](../email/create-email-templates.md), un modèle de marque spécifique ou un modèle personnalisé pour créer le contenu de votre e-mail. Il est recommandé d’utiliser un modèle d’e-mail contenant jusqu’à 8-10 images.
* Veillez à signaler les sorties problématiques à l’aide des icônes de pouce vers le haut, de pouce vers le bas ou d’indicateur lors de la sélection de variantes.
* Votre utilisation de l’assistant d’IA est soumise aux directives utilisateur de Adobe Experience Cloud Generative AI. [En savoir plus](https://www.adobe.com/fr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

Les restrictions suivantes s’appliquent à l’assistant IA dans Campaign :

* La seule langue prise en charge est l’anglais.
* Uniquement disponible pour les canaux e-mail, push et SMS.
* Il est possible que le contenu de GenAI ne soit pas toujours précis : envoyez-nous vos commentaires pour que nos ingénieures et ingénieurs puissent affiner les modèles.
* Vous pouvez charger plusieurs ressources de marque, mais vous ne pouvez en utiliser qu’une seule pour une génération spécifique.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Génération d’e-mails" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Génération d’e-mails avec l’assistant IA</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="Génération de SMS" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Génération de SMS avec l’assistant IA</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Génération de notifications push" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Génération de notifications push avec l’assistant IA</strong></a>
</div>
<p></td>
</tr></table>
