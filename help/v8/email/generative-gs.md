---
audience: end-user
title: Prise en main de l’assistant d’IA
description: Prise en main de l’assistant AI
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 18%

---

# Utiliser l’assistant d’IA {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistant IA"
>abstract="Après avoir conçu et personnalisé votre diffusion, utilisez l’assistant AI pour améliorer votre contenu. Cette fonctionnalité simplifie la personnalisation et l’amélioration du contenu en vous permettant d’affiner le contenu en décrivant ce que vous souhaitez générer."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Définir le contexte à l’aide de l’assistant IA dans Campaign"
>abstract="Pour utiliser le contenu sélectionné comme entrée pour la génération de contenu, activez le bouton (bascule) **Améliorer avec le contenu actuel**. Vous pouvez également charger vos ressources de marque pour les utiliser comme source. Si vous n’utilisez pas le contenu sélectionné, le chargement et la sélection des ressources de marque sont obligatoires."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Conditions de l’IA Generative d’Adobe"
>abstract="L’accès à cette fonctionnalité dépend de votre accord avec les directives d’utilisation de Adobe Experience Cloud Generative AI. Examinez toute sortie de cette fonctionnalité pour en vérifier la précision et assurez-vous qu’elle est appropriée à votre cas d’utilisation."
>additional-url="https://www.adobe.com/fr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directives à l’intention des utilisateurs de l’IA générative Adobe"

>[!INFO]
>
>Plongez dans une expérience pratique avec la [prévisualisation de notre fonctionnalité en direct](https://experienceleague.adobe.com/fr/apps/journey-optimizer/ai-assistant-content-accelerator), conçue pour explorer ses capacités en avant-première et comprendre pleinement ses possibilités.

À mesure que le secteur du marketing devient plus compétitif, les marques cherchent des moyens efficaces de générer rapidement du contenu percutant. L’assistant AI dans Adobe Campaign Web, optimisé par Microsoft Azure OpenAI et Adobe Firefly, est une fonctionnalité de génération de contenu d’IA d’Adobe qui transforme la manière dont les professionnels du marketing créent du contenu professionnel et cohérent pour la marque sur plusieurs canaux tels que les e-mails, les SMS et les notifications push. Grâce à des modèles GenAI avancés et à une compréhension approfondie des directives de la marque, AI Assistant génère automatiquement du contenu personnalisé, attrayant et efficace en fonction de l’objectif marketing, en optimisant le contenu pour les styles, les mises en page, le ton et plus encore des contours de la marque.

L’assistant AI simplifie la création et l’exécution de campagnes marketing sur des canaux tels que les e-mails, les SMS et les notifications push, ce qui permet de gagner du temps, d’améliorer l’efficacité et d’obtenir de meilleurs résultats.

>[!IMPORTANT]
>
>* Avant d’utiliser cette fonctionnalité, passez en revue les [mécanismes de sécurisation et limites](#generative-guardrails) associés.
>
>* Vous devez accepter un [contrat utilisateur](https://www.adobe.com/fr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) avant d’utiliser l’assistant AI dans Adobe Campaign Web. Pour plus d’informations, contactez votre représentant ou représentante Adobe.

## Accéder à l’assistant AI {#generative-access}

L’assistant AI pour les e-mails, les notifications push et les SMS est désormais à disponibilité générale (GA) et disponible pour tous les utilisateurs. Les autorisations et les étapes requises pour accorder l’accès aux utilisateurs et utilisatrices sont détaillées ci-dessous.

+++ Découvrez comment attribuer des autorisations liées à la génération de contenu

1. **Créer un profil de produit** - Dans [Admin Console](https://stage.adminconsole.adobe.com/), créez un profil de produit selon le modèle spécifique suivant :
   `Campaign - <instance-name> - AIAssistant`

1. **Ajouter des utilisateurs** - Ajoutez l’utilisateur requis à ce profil de produit,\
   ou\
   **Créer un groupe d’utilisateurs** et ajouter ce groupe d’utilisateurs au profil de produits, puis ajouter des utilisateurs à ce profil de produits.

Découvrez comment définir des autorisations dans Campaign dans [cette section](../get-started/permissions.md).

+++

## Mécanismes de sécurisation et limitations {#generative-guardrails}

Les instructions générales pour l’utilisation de l’assistant AI dans Adobe Campaign Web pour la génération d’e-mails sont répertoriées ci-dessous :

* La qualité du contenu généré dépend en grande partie de l’objectif ou de l’invite marketing que vous définissez. Utilisez une invite bien définie pour que le modèle GenAI l’interprète avec précision.
* Chargez des ressources de marque pour garantir un contenu précis et intégré à la marque. Dans le cas contraire, le contenu est basé sur des informations accessibles au public. Le contenu chargé peut être aux formats suivants : fichiers PDF, JPEG, PNG ou ZIP (avec les formats de fichiers pris en charge).
* La taille maximale des ressources de marque chargées est de 50 Mo. Des fichiers plus volumineux ou de nombreuses images peuvent augmenter le temps de traitement.
* Utilisez des [modèles d’e-mail intégrés](../email/create-email-templates.md), des modèles spécifiques à la marque ou des modèles personnalisés pour créer le contenu de vos e-mails à l’aide de l’assistant AI. Il est recommandé d’utiliser des modèles d’e-mail contenant entre 8 et 10 images.
* Signalez les sorties problématiques à l’aide des icônes de pouces vers le haut, vers le bas ou d’indicateur lors de la sélection de variantes.
* Votre utilisation de l’assistant AI est soumise aux directives d’utilisation de Adobe Experience Cloud Generative AI. [En savoir plus](https://www.adobe.com/fr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Dans le cadre de l’engagement d’Adobe en faveur de la transparence dans l’utilisation des outils d’IA génératifs dans la création de médias, Adobe applique Content Credentials lorsque du contenu ou un projet contenant une ressource générée par Firefly est téléchargé ou exporté. [En savoir plus](https://helpx.adobe.com/fr/firefly/using/content-credentials.html).

Les restrictions suivantes s’appliquent à l’assistant IA dans Adobe Campaign Web :

* L’assistant IA dans Adobe Campaign Web est actuellement pris en charge en anglais uniquement. Les entrées non anglaises peuvent produire des résultats incohérents ou erronés. Les questions découlant des réponses non anglaises ne seront pas traitées ou améliorées pour le moment.
* Disponible uniquement pour les canaux e-mail, push et SMS.
* Le contenu de GenAI peut ne pas toujours être précis. Partagez vos commentaires afin que les ingénieurs puissent affiner les modèles.
* Vous pouvez charger plusieurs ressources de marque, mais ne pouvez en exploiter qu’une seule pour une génération spécifique.

## Fonctionnalités de génération de contenu de l’assistant IA {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[Génération d’e-mails avec l’assistant AI]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Génération d’e-mails avec l’assistant AI</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[Génération de SMS avec l’assistant AI]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Génération de SMS avec l’assistant AI</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Génération de notifications push avec l’assistant AI]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Génération de notifications push avec l’assistant AI</strong></a>
</div>
<p></td>
</tr></table>