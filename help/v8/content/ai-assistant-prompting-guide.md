---
title: Guide de création de prompt de contenu avec l’assistant IA
description: Découvrez comment créer des prompts efficaces pour la génération de contenu optimisée par l’IA à l’aide du cadre CO-STAR afin de créer du contenu marketing à conversion élevée et aligné sur la marque.
role: User
level: Intermediate
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: ht
source-wordcount: '2085'
ht-degree: 100%

---

# Bonnes pratiques relatives aux prompts de l’assistant IA {#ai-assistant-prompting-guide}

Ce guide vous aide à structurer les demandes, à communiquer l’intention avec clarté et à vous assurer que l’IA produit un message qui correspond aux directives de votre marque, aux besoins de l’audience et aux objectifs de vos campagnes.
Découvrez comment écrire des prompts efficaces qui permettent à l’assistant IA de générer du contenu marketing de haute qualité, conforme à votre marque et adapté à vos objectifs.

## Utiliser le cadre CO-STAR {#costar-framework}

Pour obtenir les meilleurs résultats avec l’assistant IA, organisez vos prompts en utilisant le cadre CO-STAR. Cette approche structurée garantit que l’IA comprend exactement ce dont vous avez besoin.

| Composant | Signification | Pourquoi est-ce important ? |
|-|-|-|
| **C - Context (contexte)** | Informations sur votre campagne, produit ou situation | Aide l’IA à comprendre la situation dans son ensemble. |
| **O - Objective (objectif)** | Votre objectif marketing spécifique | Détermine l’objectif que le contenu doit atteindre. |
| **S - Style** | Comment vous voulez communiquer. | Définit l’approche. |
| **T - Tone (ton)** | Style émotionnel et voix | Influence la façon dont votre message est perçu. |
| **A - Audience** | Audience ciblée | Garantit que le message trouve écho auprès des personnes appropriées. |
| **R - Requirements (exigences)** | Contraintes spécifiques ou exigences | Définit les limites et les éléments critiques. |

## Notions essentielles des prompts IA {#key-takeaways}


### À faire et à ne pas faire


<table style="table-layout: fixed; width: 100%; border: 0;">
<thead style="border: 0; background-color: #FFFFFF;">
<tr>
<th>À faire</th>
<th>À ne pas faire</th>
</tr>
</thead>
<tbody>
<tr style="border: 0;">
<td>
<p>Utiliser le cadre CO-STAR pour la structure</p>
<p>Être explicite en ce qui concerne le contenu nouveau par rapport au contenu existant.</p>
<p>Se concentrer sur l’utilisation des documents avec des conseils d’extraction spécifiques</p>
<p>Utiliser les sélections de menu déroulant pour le ton, la stratégie et le paramètre régional</p>
<p>Faire correspondre les objectifs marketing aux fonctionnalités de type de contenu</p>
<p>Générer plusieurs variantes pour les tests AB</p>
</td>
<td>
<p>Demander des modifications structurelles, de style ou de modification d’image dans les prompts</p>
<p>Mentionner le ton/la stratégie dans les prompts si disponible dans les listes déroulantes</p>
<p>Utiliser des objectifs vagues comme « Fais la promotion de notre produit »</p>
<p>Demander des sélections d’éléments conditionnels</p>
<p>Attendre des modifications de disposition via les prompts</p>
</td>
</tr>
</tbody>
</table>

### Contenu non pris en charge dans les prompts

>[!TIP]
>
>Utilisez l’**éditeur d’e-mail** pour apporter des modifications visuelles ou d’image.

Ces demandes ne sont pas prises en charge et doivent être traitées par d’autres outils :

<table style="table-layout: fixed; border: 0;">
<thead style="border: 0; background-color: #FFFFFF">
<tr>
<th>✕ Modifications de la structure des e-mails</th>
<th>✕ Modifications visuelles de style</th>
<th>✕ Opérations de modification d’images</th>
</tr>
</thead>
<tbody>
<tr style="border: 0;">
<td>
<ul>
<li>Sélection des sections spécifiques à modifier</li>
<li>Suppression ou clonage d’éléments</li>
<li>Sélections conditionnelles</li>
<li>Ajout ou suppression de sections de mise en page</li>
</ul>
</td>
<td>
<ul>
<li>Formatage du texte (gras, italique, taille de police)</li>
<li>Modifications des couleurs</li>
<li>Style de disposition (bordures, marge intérieure, marges)</li>
<li>Effets visuels (ombres)</li>
</ul>
</td>
<td>
<ul>
<li>Modifications en arrière-plan</li>
<li>Ajout de superpositions de texte ou de logos</li>
<li>Recadrage ou redimensionnement d’images</li>
<li>Réglages des couleurs</li>
<li>Remplacement d’image</li>
</ul>
</td>
</tr>
</tbody>
</table>

### Liste de contrôle de la qualité {#quality-checklist}

Avant de générer du contenu, vérifiez les points suivants :

&amp;check; **Objectif clair** : indique clairement l’action, le produit/service, la valeur et le contexte.

&amp;check; **Audience cible définie** : indique la population, le rôle ou le segment.

&amp;check; **Alignement sur le type de contenu** : l’objectif correspond au canal ou au format sélectionné.

&amp;check; **Sélections de liste déroulante configurées** : le ton, la stratégie et le paramètre régional sont sélectionnés, ne les incluez pas dans le prompt.

&amp;check; **Focalisation du document spécifiée** : met en évidence le contenu ou les sections à référencer.

&amp;check; **Marque appliquée** : les directives de marque appropriées sont sélectionnées.

&amp;check; **Portée réaliste** : évitez les demandes de modifications de disposition, de style ou de structure.

## Rédiger des objectifs marketing efficaces {#marketing-objectives}

### Être spécifique et s’orienter vers l’action

Lors de l’élaboration des objectifs marketing, assurez-vous qu’ils sont clairs, exploitables et mesurables. Évitez les énoncés vagues ou génériques.

**Exemples de bons objectifs :**

&amp;check; « Stimule les inscriptions à notre essai gratuit de 30 jours du nouveau tableau de bord d’analyse optimisé par l’IA »

&amp;check; « Génère des pistes pour notre webinaire B2B sur la &quot;réduction des coûts du cloud de 40 %&quot; qui aura lieu le 15 mars »

&amp;check; « Fais la promotion de notre réduction saisonnière de 25 % disponible pour une durée limitée sur les abonnements premium, valable jusqu’au 25 décembre »

**Exemples de ce qu’il faut éviter :**

✕ « Fais la promotion de notre produit » (trop vague)

✕ « Fais en sorte que les gens achètent des choses » (valeur non précisée)

✕ « Envoie des e-mails à propos des nouvelles fonctionnalités » (absence d’objectif)

### Structurer votre objectif

Fournissez toujours le contexte et la proposition de valeur afin que l’IA puisse générer du contenu pertinent.
Utilisez cette formule pour vous aider à rédiger des objectifs efficaces : **Action + Produit/Service + Valeur/Avantage + Urgence/Contexte**

**Exemples de bons objectifs :**

&amp;check; « Encourage les téléchargements de notre nouvelle application mobile qui aide les utilisateurs et utilisatrices à suivre les habitudes durables du quotidien avec des recommandations personnalisées et écologiques »

&amp;check; « Fais la promotion de l’inscription à notre atelier exclusif sur les techniques avancées de visualisation des données pour les spécialistes du marketing »

&amp;check; « Stimule la participation à notre événement de lancement de produit présentant l’assistant d’écriture IA révolutionnaire qui permet de gagner plus de 5 heures par semaine »

**Exemples de ce qu’il faut éviter :**

✕ « Annonce une nouvelle application » (proposition de valeur et contexte manquants)

✕ « Incite les gens à s’inscrire à l’atelier » (manque de précision concernant l’audience et l’avantage)

✕ « Fais la promotion de l’événement » (aucune action, valeur ou urgence claire)

## Créer du contenu ou modifier du contenu existant {#new-vs-modify}

Indiquez clairement si votre demande implique la génération de nouveau contenu ou la mise à jour de contenu existant. Cette distinction est importante, car elle guide l’IA dans le choix de l’approche appropriée et garantit un résultat plus précis et utile.

### Création de nouveau contenu

Appliquez cette stratégie lorsque vous lancez des campagnes marketing, dévoilez de nouveaux produits ou lancez tout type de communication mise à jour ou actualisée. Cela garantit que votre message commence fort et s’aligne sur vos objectifs.

**Comment rédiger un prompt** ➤ Lorsque vous créez du contenu, concentrez-vous sur votre objectif marketing sans faire référence à du contenu existant.

>[!BEGINSHADEBOX]

**Exemples :**

* **Essai SaaS** : « Lance notre nouveau logiciel CRM auprès des patronnes et patrons de petites entreprises, en soulignant les économies de temps de 50 %, la qualification de lead 90 % plus rapide et en offrant un essai gratuit de 30 jours avec intégration personnalisée. »
* **Annonce de fonctionnalités** : « Annonce de nouvelles fonctionnalités d’intégration d’API qui réduisent de 60 % le temps de développement pour la clientèle professionnelle, en ciblant les décideurs et décideuses techniques »
* **Promotion d’événements** : « Stimule les inscriptions à notre webinaire &quot;Tendances du marketing numérique 2024&quot; avec des spécialistes de Google, Meta et Adobe, en mettant en avant des informations exploitables et le nombre de places limitées (500 max) »

>[!ENDSHADEBOX]

### Modification de contenu existant

>[!TIP]
>
>Pour des modifications standard telles que le développement, la synthèse ou la simplification, utilisez la fonction **Affiner** au lieu d’écrire des prompts personnalisés. [En savoir plus](generative-uc.md##refine)

Appliquez cette modification lorsque vous devez mettre à jour, actualiser ou adapter vos campagnes marketing actuelles. Cette méthode prend en charge les améliorations consécutives afin que vos messages restent pertinents sans devoir repartir de zéro.

**Comment rédiger un prompt** ➤ Lorsque vous modifiez du contenu existant, indiquez clairement les éléments vous souhaitez modifier et la manière dont ils doivent être modifiés.

>[!BEGINSHADEBOX]

**Exemples :**

* **Actualisation de campagne** : « Modifie l’e-mail de lancement du produit pour mettre l’accent sur les fonctionnalités de sécurité adaptées aux entreprises plutôt que sur les bénéfices généraux de productivité, en ciblant les décideurs et décideuses informatiques avec des certifications de conformité »
* **Changement d’audience** : « Adapte notre invitation à la démonstration du logiciel pour cibler spécifiquement le secteur de la santé, en remplaçant les exemples génériques par des cas d’usage de la santé et les avantages liés à la conformité HIPAA »
* **Mise à jour saisonnière** : « Mets à jour notre campagne promotionnelle du T3 pour les achats du T4 pour les vacances, en passant de la rentrée des classes au cadeau de fêtes avec l’accent sur la livraison rapide »

>[!ENDSHADEBOX]

## Améliorer votre prompt avec les paramètres avancés {#personalize-prompt}

### Types de stratégies de communication

>[!TIP]
>
>Utilisez le menu déroulant Stratégie de communication du menu Paramètres de texte au lieu de le mentionner dans votre prompt pour un traitement spécialisé.

Votre stratégie de communication détermine la manière dont vous présentez votre message afin de maximiser son impact. Différentes stratégies fonctionnent mieux pour différents objectifs, que vous créiez l’urgence, établissiez la confiance ou stimuliez une action immédiate. Choisissez la stratégie qui correspond le mieux à vos objectifs de campagne et à l’état d’esprit de votre audience.

| **Stratégie** | **Idéale pour** | **Style des messages** | **Exemples** |
|--------------|--------------|------------------------|--------------|
| **Urgent** | Offres sensibles au facteur temps, échéances, action immédiate | Crée une pression immédiate avec un langage temporel. | « Agissez maintenant : l’offre expire à minuit. » <br> « Inscrivez-vous aujourd’hui avant qu’il n’y ait plus de places. » <br> « La vente flash de 48 heures commence maintenant. » |
| **FOMO (peur de manquer un événement)** | Offres limitées, événements, accès exclusif | Utilise des signaux d’urgence, de rareté et de pression temporelle. | « Il ne reste que 24 heures ! Stock limité à 40 % de réduction. » <br> « Dernière chance : les tarifs anticipés se terminent demain. » <br> « Il ne reste que 100 places en version bêta. » |
| **Preuve sociale** | Création de confiance, témoignages, produits populaires | Tire parti des expériences et de la validation des autres personnes. | « Rejoignez plus de 50 000 personnes satisfaites. » <br> « Noté 4,9/5 étoiles par les spécialistes du secteur. » <br> « Approuvé par des entreprises du Fortune 500. » |
| **Rareté** | Stock limité, sorties exclusives, articles à forte demande | Met en avant la disponibilité limitée et l’exclusivité. | « Seulement 5 articles restants en stock » <br> « Édition limitée : 100 unités disponibles » <br> « Sortie exclusive : premier arrivé, premier servi » |
| **Incitatif** | Promotions, programmes de récompenses, offres spéciales | Met en avant les avantages et les récompenses tangibles. | « Obtenez 20 % de réduction sur votre première commande » <br> « Gagnez deux fois plus de points ce week-end » <br> « Livraison gratuite pour les commandes de plus de 50 $ » |
| **Exclusivité** | Produits premium, expériences VIP, offres réservées aux personnes membres | Utilise le positionnement premium et le langage d’accès spécial. | « Invitation exclusive à notre aperçu privé » <br> « L’adhésion Elite débloque l’analyse avancée » <br> « Rejoignez certaines entreprises du Fortune 500 qui font déjà appel à nous » |
| **Gamification** | Campagnes d’engagement, programmes de fidélité, contenu interactif | Utilise la mécanique du jeu et le langage de l’accomplissement. | « Déverrouillez votre prochain niveau de récompense » <br> « Accomplissez des défis pour gagner des badges » <br> « Grimpez au classement pour obtenir des prix exclusifs » |
| **Informatif** | Éducation, recherche, produits complexes, leadership d’opinion | Utilise des faits, des données, des informations et des explications. | « 5 informations à partir de l’analyse de plus de 10 000 interactions » <br> « Une nouvelle recherche révèle 3 approches novatrices » <br> « Guide complet d’implémentation de l’IA dans le marketing » |
| **Éducation et informations** | Contenu d’apprentissage, tendances du secteur, bonnes pratiques | Fournit des connaissances précieuses et des points à retenir exploitables. | « Maîtrisez des techniques avancées avec notre guide spécialisé » <br> « Découvrez les 7 stratégies utilisées par les principaux professionnels du marketing » <br> « Découvrez comment optimiser votre workflow en 5 étapes » |

### Définir le bon ton {#tone}

>[!TIP]
>
>Utilisez la liste déroulante Ton du menu Paramètres de texte plutôt que de le spécifier dans votre prompt.

Le ton façonne la manière dont votre audience perçoit votre message et y répond. Sélectionnez toujours un ton qui correspond à la voix de votre marque et à l’étape du parcours de profil.

Utilisez le tableau ci-dessous pour explorer chaque ton en détail, y compris quand il fonctionne le mieux et des exemples de contenu adaptés à chaque style.

| Ton | Idéal pour | Exemple de contenu |
|-|-|-|
| Professionnel | Communications B2B, annonces formelles | « Nous nous réjouissons d’annoncer notre partenariat stratégique… » |
| Empathique | Assistance clientèle, sujets sensibles | « Nous comprenons à quel point cela doit être frustrant pour vous… » |
| Humoristique | Campagnes attrayantes, contenu décontracté | « Avertissement : peut entraîner de sérieux gains de productivité ! » |
| Enthousiasmant | Lancements de produits, promotions d’événements | « C’est le moment que vous attendiez ! » |
| Inspirant | Campagnes de motivation, objectif de la marque | « Ensemble, nous pouvons faire une différence dans le monde… » |
| Persuasif | Campagnes commerciales, conversions | « Ne manquez pas cette occasion d’une durée limitée pour… » |
| Amical | Engagement de la clientèle, messages de bienvenue | « Nous nous réjouissons que vous soyez ici avec nous. » |
| Formel | Communications juridiques, avis officiels | « Nous vous informons des modifications suivantes… » |
| Excuse | Reprise des services, résolution des problèmes | « Nous nous excusons sincèrement pour tout désagrément causé… » |
| Assertif | Contenu de leadership, messages faisant autorité | « Voici ce que vous devez faire maintenant… » |
| Mise en récit | Récits sur la marque, liens émotionnels | « Tout a commencé par une simple question… » |
| Conversationnel | Campagnes de suivi, développement des relations | « Parlons de la façon dont cela peut vous aider… » |

### Optimiser les ressources de votre marque {#brand-assets}

>[!TIP]
>
>Si vous avez déjà chargé une ressource de marque par l’intermédiaire du menu **Ressources de marque**, vous n’avez pas besoin de la référencer dans votre prompt. Le système utilise automatiquement tous les documents sélectionnés.

Les ressources de marque fournissent des informations factuelles qui enrichissent votre contenu généré avec des détails précis et spécifiques.
Lorsque vous chargez des documents généraux tels que des brochures de produit, ajoutez au prompt les parties sur lesquelles vous souhaitez mettre l’accent :

* **Au lieu de** _« Utilise la brochure produit »_, **écrivez plutôt** _« Concentre-toi sur les fonctionnalités de sécurité avancées et les certifications de conformité, en particulier la conformité à la norme SOC 2 et le chiffrement des données »_.

* **Au lieu de** _« Référence les études de cas »_, **écrivez plutôt** _« Mets en évidence les résultats du retour sur investissement de la clientèle du secteur de la santé, en particulier la réduction de 40 % des coûts au centre médical régional »_.

* **Au lieu de** _« Inclus les détails techniques »_, **écrivez plutôt** _« Mets l’accent sur les fonctionnalités d’intégration d’API et les avantages pour le développement, en te concentrant sur les points d’entrée de l’API REST et le contrat de niveau de service (SLA) à 99,9 % de disponibilité »_.

### Affinement du contenu

>[!TIP]
>
>Utilisez la fonctionnalité Affiner au lieu d’écrire un prompt lorsque vous souhaitez préciser, résumer, simplifier, changer de ton ou traduire le contenu existant. [En savoir plus](generative-uc.md#refine)

Une fois le contenu généré, utilisez la fonctionnalité **Affiner** pour l’itérer et l’améliorer avec les options suivantes :

| **Action** | **Cas d’utilisation** | **Exemple de prompt** |
|-|-|-|
| **Préciser** | Ajouter de la profondeur et des détails au contenu succinct | « Précise les avantages techniques de nos fonctionnalités de sécurité. » |
| **Résumer** | Condenser du contenu long pour différents formats | « Résume cette présentation de produit pour une publication sur les réseaux sociaux. » |
| **Simplifier** | Rendre le contenu complexe plus accessible | « Simplifie cette explication technique pour le grand public. » |
| **Changer le ton** | Adapter le contenu pour différentes audiences | « Adopte un ton plus décontracté pour un public plus jeune. » |
| **Transcréer** | Adaptation culturelle au-delà de la traduction | « Transcrée cette campagne pour le marché japonais. » |

## Exemples de prompts basés sur un scénario

### En fonction du type de contenu {#content-type-practices}

<table style="table-layout: fixed; border: 0;">
<thead>
<tr style="border: 0;background-color: #FFFFFF;">
<th>Canal</th>
<th>Exemple</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>E-mail</strong></td>
<td>« Stimule les prospects de l’entreprise en présentant trois témoignages de la clientèle avec des mesures de retour sur investissement détaillées (IBM : réduction des coûts de 45 %, Accenture : augmentation des prospects de 200 %, Microsoft : gains de temps de 60 %), ciblant les directeurs et directrices informatiques des entreprises de plus de 1 000 personnes. »</td>
</tr>
<tr>
<td><strong>SMS</strong></td>
<td>« Alerte la clientèle VIP sur une vente flash d’environ 4 heures sur des produits électroniques haut de gamme avec une remise de 40 %, limitée aux 100 premiers acheteurs et acheteuses. »</td>
</tr>
<tr>
<td><strong>Notifications push</strong></td>
<td>« Réengage les utilisateurs et utilisatrices qui n’ont pas ouvert l’application depuis 7 jours avec des recommandations de contenu personnalisé basées sur leur historique de lecture .»</td>
</tr>
<tr>
<td><strong>Pages de destination</strong></td>
<td>« Convertis les visiteurs et visiteuses B2B en prospects qualifiés en démontrant comment notre solution de sécurité d’entreprise prévient 99,9 % des cyberattaques, grâce aux témoignages Fortune 500 et à un audit de sécurité gratuit. »</td>
</tr>
</tbody>
</table>

### En fonction des approches spécifiques au secteur {#industry-approaches}

<table style="table-layout: fixed; border-collapse: collapse; border: 0;">
<thead>
<tr style="border: 0;background-color: #FFFFFF;">
<th>Secteur</th>
<th>Exemple de prompt</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Technologie B2B</strong></td>
<td>« Montre le retour sur investissement et les spécifications techniques tout en répondant aux préoccupations de sécurité des décideurs et décideuses informatiques qui évaluent notre solution d’infrastructure cloud, en mettant l’accent sur la disponibilité de 99,9 % du contrat de niveau de service (SLA), la conformité à la norme SOC 2 et les économies de 40 %. »</td>
</tr>
<tr>
<td><strong>E-commerce - Vente au détail</strong></td>
<td>« Crée l’urgence autour des articles de fêtes en stock limité tout en mettant en avant la livraison gratuite et les retours faciles pour les achats de dernière minute, en soulignant les quantités limitées (moins de 50 articles restants) et la limite de livraison de 24 heures. »</td>
</tr>
<tr>
<td><strong>Services financiers</strong></td>
<td>« Sensibilise la clientèle aux stratégies de diversification du portefeuille d’investissement tout en maintenant la conformité réglementaire, avec des conseils financiers certifiés et des avertissements sur les risques. »</td>
</tr>
<tr>
<td><strong>Santé et bien-être</strong></td>
<td>« Fais la promotion des avantages en matière de soins préventifs et des examens médicaux annuels tout en maintenant l’exactitude médicale, avec des recommandations médicales certifiées par le conseil d’administration et des garanties de confidentialité pour la patientèle. »</td>
</tr>
<tr>
<td><strong>Éducation et formation</strong></td>
<td>« Mets en avant les perspectives d’évolution de carrière et les certifications professionnelles tout en montrant l’expertise des formateurs et formatrices, en soulignant un taux de placement à l’emploi de 92 % et un programme basé sur des projets. »</td>
</tr>
<tr>
<td><strong>Plateformes SaaS</strong></td>
<td>« Mets en avant les gains de temps et les avantages de l’automatisation grâce à des mesures spécifiques tout en répondant aux problèmes d’intégration, avec un gain de temps hebdomadaire moyen de 25 heures et une intégration à plus de 200 outils populaires. »</td>
</tr>
</tbody>
</table>
