---
audience: end-user
product: campaign
title: Métadonnées C2PA dans le concepteur d’e-mail et de page de destination
description: Découvrez ce qu’il advient des métadonnées C2PA déjà jointes à une image lorsque celle-ci est déplacée dans le concepteur d’e-mail et de page de destination dans l’interface d’utilisation d’Adobe Campaign Web.
topic: Content Management
role: User
level: Beginner
source-git-commit: 645352d9e2ba12d5430ddf1b62852077344c3016
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 100%
---

# Métadonnées C2PA dans le concepteur d’e-mail et de page de destination {#c2pa-email-landing-page-designer}

>[!BEGINSHADEBOX]

**Sur cette page :** découvrez ce qu’il advient des métadonnées C2PA déjà jointes à une image lorsque celle-ci est déplacée dans le concepteur d’e-mail et de page de destination dans l’interface d’utilisation d’Adobe Campaign Web.

>[!ENDSHADEBOX]

>[!INFO]
>
>De nouvelles lois relatives à la transparence de l’IA générative sont promulguées, et Adobe s’efforce de répondre aux exigences applicables dans toutes les juridictions. Les métadonnées C2PA sont l’outil de provenance utilisé par Adobe pour répondre aux exigences de ces lois.

Le concepteur d’e-mail et de page de destination ne génère ni ne modifie les images lui-même. Il fait référence à des images déjà générées ou modifiées avec l’IA générative dans un autre outil Adobe, tel que Générer du contenu, Adobe Express ou Firefly, ou dans un modèle de partenaire. Les métadonnées C2PA déjà jointes à ces images sont conservées et inchangées lors de la création, de la publication et de l’envoi.

## Les métadonnées C2PA sont conservées lors de la création et de l’envoi {#c2pa-preserved}

Le tableau suivant résume ce qu’il advient des métadonnées C2PA à chaque étape de création et d’envoi de contenu avec le concepteur d’e-mail et de page de destination.

| Action | Ce qui se passe | Métadonnées C2PA conservées ? | Exemple |
| --- | --- | --- | --- |
| **Insérer une image dans un modèle** | Le concepteur ajoute une référence à une image déjà générée ou modifiée ailleurs avec l’IA générative, par exemple Générer du contenu, Adobe Express, Firefly, ou un modèle de partenaire. Le fichier image lui-même n’est pas modifié. | Oui, sans modification. | Une bannière générée par Firefly est insérée dans un modèle d’e-mail. |
| **Redimensionner, repositionner ou ajouter du texte alternatif** | Seules les propriétés d’affichage dans le code HTML du modèle changent. Le fichier image n’est pas encodé à nouveau. | Oui, sans modification. | Une image est redimensionnée pour s’adapter à une mise en page mobile et reçoit du texte alternatif. |
| **Publier** | L’e-mail ou la page de destination est publiée et l’image est stockée pour diffusion. | Oui, sans modification. | Une campagne est publiée et ses images sont stockées pour envoi. |
| **Envoyer un e-mail ou afficher une page de destination** | L’image est envoyée dans la boîte de réception de la personne destinataire ou affichée sur la page en direct. | Oui, sans modification. | Une personne destinataire ouvre l’e-mail et télécharge l’image ; les informations d’identification correspondent toujours à l’original. |

## Types de contenu et leur portée {#c2pa-content-types}

* **Images** : couvert. Les métadonnées C2PA déjà jointes à une image sont conservées lorsque celle-ci est insérée, ajustée, publiée et diffusée, comme illustré ci-dessus.
* **Vidéo, audio, texte** : non applicable. Le concepteur d’e-mail et de page de destination ne génère ni ne modifie ces types de contenu avec l’IA générative.

## Ce qui se passe lorsque votre contenu est déplacé {#c2pa-content-moves}

Les métadonnées C2PA accompagnent l’image dans le concepteur d’e-mail et de page de destination dans l’interface d’utilisation d’Adobe Campaign Web, de votre éditeur, en passant par le stockage, jusqu’à la boîte de réception de la personne destinataire ou la page en direct. Aucune information d’identification n’est créée, modifiée ou supprimée au cours de ces étapes.

Si une image ne contient pas de métadonnées C2PA d’IA générative, car elle n’a pas été générée ou modifiée avec l’IA générative, aucune information d’identification ne s’affiche ici. Ceci est normal, et non une erreur.

## Vérification d’une information d’identification {#c2pa-checking-credential}

Il n’existe pas encore de moyen permettant d’inspecter un Content Credential directement dans le concepteur d’e-mail ou de page de destination.

## Autres ressources

* [Utiliser la fonctionnalité de génération de contenu](generative-gs.md)
* [Transparence du contenu d’IA générative](https://experienceleague.adobe.com/fr/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)