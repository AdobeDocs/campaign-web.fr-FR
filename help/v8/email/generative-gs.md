---
audience: end-user
title: Commencer avec l’accélérateur de contenu de l’Assistant IA
description: Commencer avec l’accélérateur de contenu de l’assistant IA
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 87%

---

# Utiliser l’accélérateur de contenu de l’assistant IA  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Accélérateur de contenu de l’assistant IA"
>abstract="L’assistant IA rend la création et l’exécution de campagnes marketing sur plusieurs canaux (comme les e-mails, les SMS et les notifications push) intuitives, simples et sans accroc tout en gagnant du temps, en améliorant l’efficacité et en obtenant de meilleurs résultats."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=fr" text="Voir les notes de mise à jour"


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Assistant IA"
>abstract="Une fois que vous avez conçu et personnalisé votre diffusion, vous pouvez utiliser l’assistant IA pour améliorer votre contenu. Cette fonctionnalité simplifie le processus de personnalisation et d’amélioration du contenu en vous permettant d’affiner le contenu à travers la description de ce que vous souhaitez générer."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Définir le contexte à l’aide de l’assistant IA dans Campaign"
>abstract="Pour utiliser le contenu sélectionné comme entrée pour la génération de contenu, activez le bouton (bascule) **Améliorer le contenu actuel**. Vous pouvez également charger vos ressources de marque pour les utiliser comme source. Si vous n’utilisez pas le contenu sélectionné, le chargement et la sélection de ressources de marque sont obligatoires."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Conditions de l’IA Generative d’Adobe"
>abstract="L’accès à cette fonctionnalité est soumis à votre acceptation des directives d’utilisation de l’IA générative d’Adobe Experience Cloud. Veuillez vérifier la précision des résultats de cette fonctionnalité et vous assurer qu’ils sont adaptés à votre cas d’utilisation."
>additional-url="https://www.adobe.com/fr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directives à l’intention des utilisateurs de l’IA générative Adobe"

>[!INFO]
>
>Plongez dans une expérience pratique avec la [prévisualisation de notre fonctionnalité en direct](https://experienceleague.adobe.com/fr/apps/journey-optimizer/ai-assistant-content-accelerator), conçue pour explorer ses capacités en avant-première et comprendre pleinement ses possibilités.


À mesure que le secteur du marketing devient plus compétitif, les marques cherchent des moyens efficaces de générer du contenu ayant un impact de manière efficace et rapide. L’accélérateur de contenu de l’assistant d’IA dans Adobe Campaign Web, optimisé par Microsoft Azure OpenAI et Adobe Firefly, est la fonctionnalité de génération de contenu de l’IA de l’Adobe qui révolutionne la manière dont les marketeurs créent du contenu professionnel et cohérent sur le plan de la marque sur plusieurs canaux tels que Email, SMS, Push. Grâce aux modèles avancés de GenAI et à une compréhension approfondie des directives de la marque, l’assistant IA génère automatiquement du contenu personnalisé, attrayant et efficace en fonction de l’objectif marketing, avec un contenu optimisé pour les styles, les mises en page, le ton et bien plus encore.

L’assistant IA rend la création et l’exécution de campagnes marketing sur plusieurs canaux (comme les e-mails, les SMS et les notifications push) intuitives, simples et sans accroc tout en gagnant du temps, en améliorant l’efficacité et en obtenant de meilleurs résultats.

>[!IMPORTANT]
>
>* Avant de commencer à utiliser cette fonctionnalité, lisez la section connexe [Mécanismes de sécurisation et limitations](#generative-guardrails).
>
>* Vous devez accepter un [ contrat utilisateur](https://www.adobe.com/fr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) avant de pouvoir utiliser l’accélérateur de contenu de l’assistant d’IA dans Adobe Campaign Web. Pour plus d’informations, contactez votre personne représentante Adobe.

## Accéder à l’accélérateur de contenu de l’assistant IA {#generative-access}

L’accélérateur de contenu de l’assistant IA pour les e-mails, les notifications push et les SMS est désormais disponible en disponibilité générale (GA) et est disponible pour tous les utilisateurs et utilisatrices. Les autorisations et les étapes requises pour accorder l’accès aux utilisateurs et utilisatrices sont détaillées ci-dessous.

+++  Découvrez comment attribuer des autorisations liées à la génération de contenu.

1. **Créer un profil de produit** : dans [Admin Console](https://stage.adminconsole.adobe.com/), créez un profil de produit avec le modèle spécifique suivant :
   `Campaign - <instance-name> - AIAssistant`

1. **Ajouter des utilisateurs et utilisatrices** : ajoutez la personne requise à ce profil de produit,
ou
   **Créer un groupe d’utilisateurs et d’utilisatrices** : ajoutez ce groupe d’utilisateurs et d’utilisatrices au profil de produit et ajoutez des utilisateurs et utilisatrices à ce profil de produit.

Découvrez comment définir des autorisations dans Campaign dans [cette section](../get-started/permissions.md).

+++

## Mécanismes de sécurisation et limitations {#generative-guardrails}

Les instructions générales pour l’utilisation de l’accélérateur de contenu de l’assistant d’IA dans le Web Adobe Campaign pour la génération d’emails sont répertoriées ci-dessous :

* La qualité du contenu généré est fortement influencée par l’invite/l’objectif marketing que vous définissez. Utilisez une invite bien définie pour que le modèle GenAI soit interprété avec précision. 
* Chargez les ressources de marque pour qu’elles soient précises sur le contenu de la marque. Autrement, le contenu est basé sur des informations disponibles au public. Le contenu chargé peut se présenter dans les formats suivants : fichiers PDF, JPEG, PNG ou ZIP (avec les formats de fichiers pris en charge).
* La taille maximale pour la ressource de marque chargée est de 50 Mo.Des fichiers plus volumineux ou de nombreuses images peuvent fonctionner, mais le temps de traitement sera plus long.
* Utilisez des [modèles d’e-mails intégrés](../email/create-email-templates.md), un modèle de marque spécifique ou un modèle personnalisé pour créer le contenu de votre e-mail à l’aide de l’accélérateur de contenu. Il est recommandé d’utiliser des modèles d’e-mail contenant jusqu’à 8-10 images.
* Veillez à signaler les sorties problématiques à l’aide des icônes de pouce vers le haut, de pouce vers le bas ou d’indicateur lors de la sélection de variantes.
* Votre utilisation de l’assistant IA est soumise aux directives d’utilisation de l’IA générative d’Adobe Experience Cloud. [En savoir plus](https://www.adobe.com/fr/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Dans le cadre de l’engagement d’Adobe à promouvoir la transparence dans l’utilisation d’outils d’IA générative dans la création de médias, Adobe appliquera Content Credentials (informations de traçabilité du contenu) lorsque le contenu ou un projet qui incluait une ressource générée par un Firefly est téléchargé ou exporté. [En savoir plus](https://helpx.adobe.com/fr/firefly/using/content-credentials.html)

Les restrictions suivantes s’appliquent à l’accélérateur de contenu de l’assistant d’IA dans Adobe Campaign Web :

* L’accélérateur de contenu de l’assistant d’IA dans Adobe Campaign Web est actuellement pris en charge en anglais uniquement. Les entrées non anglaises peuvent produire des résultats incohérents ou erronés. Les questions portant sur des réponses non anglaises ne seront pas traitées ni améliorées pour le moment.
* Uniquement disponible pour les canaux e-mail, push et SMS.
* Il est possible que le contenu de GenAI ne soit pas toujours précis : envoyez-nous vos commentaires pour que nos ingénieures et ingénieurs puissent affiner les modèles.
* Vous pouvez charger plusieurs ressources de marque, mais vous ne pouvez en utiliser qu’une seule pour une génération spécifique.

## Fonctionnalités de génération de contenu de l’assistant IA {#generative-features}

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
