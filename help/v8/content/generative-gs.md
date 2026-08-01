---
audience: end-user
title: Prise en main de la génération de contenu
description: Prise en main de la génération de contenu
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
TQID: https://experienceleague.adobe.com/jpw4u-Vy7M2Q9qRyQ2J3rJ-Mr8UKLUpxhw39tglbbNc
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: d4e22ba88bcb6dc74d22e8a927c1640f21d75d3e
workflow-type: tm+mt
source-wordcount: 887
ht-degree: 63%

---

# Utilisation de l’option Générer du contenu {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Generate Content"
>abstract="Après avoir conçu et personnalisé votre diffusion, utilisez l’IA pour améliorer votre contenu. Cette fonctionnalité simplifie le processus de personnalisation et d’amélioration du contenu en vous permettant d’affiner le contenu à travers la description de ce que vous souhaitez générer."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Définition du contexte avec l’option Générer du contenu dans Campaign"
>abstract="Pour utiliser le contenu sélectionné comme entrée pour la génération de contenu, activez le bouton (bascule) **Améliorer avec le contenu actuel**. Vous pouvez également charger vos ressources de marque pour les utiliser comme source. Si vous n’utilisez pas le contenu sélectionné, le chargement et la sélection de ressources de marque sont obligatoires."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Conditions de l’IA générative d’Adobe"
>abstract="L’accès à cette fonctionnalité est soumis à votre acceptation des directives d’utilisation de l’IA générative d’Adobe Experience Cloud. Vérifiez la précision des résultats de cette fonctionnalité et assurez-vous qu’ils sont adaptés à votre cas d’utilisation."
>additional-url="https://www.adobe.com/fr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directives à l’intention des utilisateurs de l’IA générative Adobe"

>[!INFO]
>
>Plongez dans une expérience pratique avec la [prévisualisation de notre fonctionnalité en direct](https://experienceleague.adobe.com/fr/apps/journey-optimizer/ai-assistant-content-accelerator), conçue pour explorer ses capacités en avant-première et comprendre pleinement ses possibilités.

À mesure que le secteur du marketing devient plus compétitif, les marques cherchent des moyens efficaces de générer rapidement du contenu percutant. Générer du contenu dans Adobe Campaign Web, optimisé par Microsoft Azure OpenAI et Adobe Firefly, est une fonctionnalité de génération de contenu de l’IA d’Adobe qui transforme la manière dont les professionnels du marketing créent du contenu professionnel et cohérent pour la marque sur plusieurs canaux tels que les e-mails, les SMS et les notifications push. Grâce aux modèles GenAI avancés et à une compréhension approfondie des directives de la marque, Generate Content génère automatiquement du contenu personnalisé, attrayant et efficace en fonction de l’objectif marketing, en optimisant le contenu pour les styles, les mises en page, le ton et plus encore des contours de la marque.

Générer du contenu prend en charge la génération **dans plusieurs langues** ce qui vous permet d’atteindre et d’impliquer diverses audiences internationales. L’option Générer le contenu est disponible dans les langues suivantes :

<table style="table-layout:fixed; margin-top: 0px; margin-bottom: 0px;">
  <tbody>
    <tr style="border: 0;background-color: #FFFFFF;">
      <td>
        <ul>
          <li>Chinois (Hong Kong)</li>
          <li>Chinois (simplifié)</li>
          <li>Chinois (Taïwan)</li>
          <li>Néerlandais</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Français</li>
          <li>Allemand</li>
          <li>Italien</li>
          <li>Japonais</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Norvégien</li>
          <li>Portugais</li>
          <li>Espagnol</li>
          <li>Suédois</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

L’option Générer du contenu simplifie la création et l’exécution de campagnes marketing sur plusieurs canaux tels que les e-mails, les SMS et les notifications push, ce qui permet de gagner du temps, d’améliorer l’efficacité et d’obtenir de meilleurs résultats.

>[!IMPORTANT]
>
>* Avant de commencer à utiliser cette fonctionnalité, lisez la section connexe sur les [Mécanismes de sécurisation et limitations](#generative-guardrails).
>
>* Vous devez accepter un [contrat d’utilisateur](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) avant d’utiliser l’IA pour générer du contenu dans Adobe Campaign Web. Pour plus d’informations, contactez votre représentant ou représentante Adobe.

## Accéder à Generate Content {#generative-access}

Le contenu généré pour les e-mails, les notifications push, les pages de destination et les SMS est désormais disponible pour tous les utilisateurs. Les autorisations et les étapes requises pour accorder l’accès aux utilisateurs et utilisatrices sont détaillées ci-dessous.

+++ En savoir plus sur l’attribution des autorisations liées à la génération de contenu

1. **Accédez à [Admin Console](https://adminconsole.adobe.com/)**, au menu **Produits**, puis sélectionnez **Adobe Campaign Managed Cloud**.

1. Accédez à l’instance pour laquelle vous souhaitez accorder des autorisations, puis cliquez sur **Nouveau profil** pour créer un profil de produit avec le nom de profil de produit spécifique suivant :

   `Campaign - <instance-name> - AIAssistant`

1. Configurez le profil de produit avec les autorisations requises pour l’accès Générer du contenu .

1. **Ajoutez des personnes ou des groupes d’utilisateurs et d’utilisatrices**. Choisissez l’une des options suivantes :
   * **Ajouter des personnes individuelles** : ajoutez les personnes requises directement à ce profil de produit.
   * **Ajouter des groupes d’utilisateurs et d’utilisatrices** : créez un groupe d’utilisateurs et d’utilisatrices, ajoutez des personnes à ce groupe, puis ajoutez le groupe au profil de produit.

Découvrez comment définir des autorisations dans Campaign dans [cette section](../get-started/permissions.md).

+++

## Mécanismes de sécurisation et limitations {#generative-guardrails}

Les instructions générales concernant l’utilisation de l’IA pour générer du contenu dans Adobe Campaign Web pour la génération d’e-mails sont répertoriées ci-dessous :

* La qualité du contenu généré est fortement influencée par le prompt ou l’objectif marketing que vous définissez. Utilisez un prompt bien défini pour que le modèle GenAI soit interprété avec précision.
* Chargez des ressources de marque pour garantir un contenu précis et intégré à la marque. Autrement, le contenu est basé sur des informations disponibles au public. Le contenu chargé peut se présenter dans les formats suivants : fichiers PDF, JPEG, PNG ou ZIP (avec les formats de fichiers pris en charge).
* La taille maximale pour les ressources de marque chargées est de 50 Mo. Des fichiers plus volumineux ou de nombreuses images peuvent augmenter le temps de traitement.
* Utilisez des [modèles d’e-mail intégrés](../content/create-email-templates.md), des modèles spécifiques à la marque ou des modèles personnalisés pour créer le contenu de vos e-mails à l’aide de l’IA. Il est recommandé d’utiliser des modèles d’e-mail contenant jusqu’à 8 à 10 images.
* Signalez les sorties problématiques à l’aide des icônes de pouces vers le haut, vers le bas ou d’indicateurs lors de la sélection de variantes.
* Votre utilisation de Generate Content est soumise aux directives d’utilisation d’Adobe Experience Cloud Generative AI. [En savoir plus](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Dans le cadre de l’engagement d’Adobe à la transparence dans l’utilisation d’outils d’IA générative dans la création de médias, Adobe applique Content Credentials (informations de traçabilité du contenu) lorsque le contenu ou un projet qui inclut une ressource générée par un Firefly est téléchargé ou exporté. [En savoir plus](https://helpx.adobe.com/fr/firefly/using/content-credentials.html).

Les restrictions suivantes s’appliquent à Generate Content in Adobe Campaign Web :

* Generate Content in Adobe Campaign Web est actuellement pris en charge en anglais uniquement. Les entrées non anglaises peuvent produire des résultats incohérents ou erronés. Les questions portant sur des réponses non anglaises ne seront pas traitées ni améliorées pour le moment.
* Uniquement disponible pour les canaux e-mail, push et SMS.
* Le contenu de GenAI peut ne pas toujours être précis. Partagez vos commentaires afin que l’équipe d’ingénierie puisse affiner les modèles.
* Vous pouvez charger plusieurs ressources de marque, mais vous ne pouvez en exploiter qu’une seule pour une génération spécifique.

## Fonctionnalités de génération de contenu {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Génération complète du contenu avec Générer le contenu]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong>Génération de contenu complet avec Generate Content</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Génération de contenu texte avec Générer du contenu]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong>Génération de texte avec Générer du contenu</strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Génération d’images avec Générer du contenu]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong>Génération d’images avec l’option Générer le contenu</strong></a>
</div>
<p></td>
</tr></table>