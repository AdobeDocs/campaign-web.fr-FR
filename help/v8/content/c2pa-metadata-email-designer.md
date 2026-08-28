---
audience: end-user
product: campaign
title: Métadonnées C2PA dans les Designer de messagerie et de page de destination
description: Découvrez ce qu’il advient des métadonnées C2PA déjà jointes à une image lors de son déplacement dans le concepteur d’e-mail et de page de destination dans l’interface utilisateur web d’Adobe Campaign.
topic: Content Management
role: User
level: Beginner
source-git-commit: 645352d9e2ba12d5430ddf1b62852077344c3016
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 1%

---


# Métadonnées C2PA dans les Designer de messagerie et de page de destination {#c2pa-email-landing-page-designer}

>[!BEGINSHADEBOX]

**Sur cette page :** Découvrez ce qu’il advient des métadonnées C2PA déjà jointes à une image lors de son déplacement dans l’e-mail et le concepteur de page de destination dans l’interface utilisateur web d’Adobe Campaign.

>[!ENDSHADEBOX]

>[!INFO]
>
>De nouvelles lois émergent autour de la transparence générative de l’IA, et Adobe s’efforce de répondre aux exigences applicables dans toutes les juridictions. Les métadonnées C2PA sont l’outil de provenance utilisé par Adobe pour répondre aux exigences de ces lois.

Le concepteur d’e-mail et de page de destination ne génère ni ne modifie les images lui-même. Il fait référence à des images déjà générées ou modifiées avec l’IA générative dans un autre outil Adobe, tel que Generate Content, Adobe Express ou Firefly, ou dans un modèle de partenaire. Les métadonnées C2PA déjà associées à ces images sont conservées et inchangées lors de la création, de la publication et de l’envoi.

## Les métadonnées C2PA sont conservées lors de la création et de l’envoi {#c2pa-preserved}

Le tableau suivant résume ce qui se passe avec les métadonnées C2PA à chaque étape de création et d’envoi de contenu avec le concepteur d’e-mail et de page de destination.

| Action | Ce qui se passe | Métadonnées C2PA conservées ? | Exemple |
| --- | --- | --- | --- |
| **Insérer une image dans un modèle** | Le concepteur ajoute une référence à une image déjà générée ou modifiée avec l’IA générative ailleurs, par exemple Générer du contenu, Adobe Express, Firefly ou un modèle de partenaire. Le fichier image lui-même n’est pas modifié. | Oui, inchangé | Une bannière générée par Firefly est insérée dans un modèle d’e-mail. |
| **Redimensionner, repositionner ou ajouter du texte secondaire** | Affichez uniquement les propriétés dans la modification HTML du modèle. Le fichier image n’est pas réencodé. | Oui, inchangé | Une image est redimensionnée pour s’adapter à une disposition pour appareils mobiles et à un texte de remplacement donné. |
| **Publier** | L’e-mail ou la page de destination est publié et l’image est stockée pour diffusion. | Oui, inchangé | Une campagne est publiée et ses images sont stockées pour envoi. |
| **Envoyer un e-mail ou afficher une page de destination** | L’image est diffusée dans la boîte de réception du destinataire ou affichée sur la page active. | Oui, inchangé | Un destinataire ouvre l’e-mail et télécharge l’image ; les informations d’identification correspondent toujours à l’original. |

## Types de contenu et leur portée {#c2pa-content-types}

* **Images** : Couvert. Les métadonnées C2PA déjà associées à une image sont conservées lors de leur insertion, ajustement, publication et diffusion, comme illustré ci-dessus.
* **Vidéo, audio, texte** : Sans objet. Le concepteur d’e-mail et de page de destination ne génère ni ne modifie ces types de contenu avec l’IA générative.

## Ce qui se passe lorsque le contenu est déplacé {#c2pa-content-moves}

Les métadonnées C2PA accompagnent l’image dans l’e-mail et le concepteur de page de destination dans l’interface utilisateur web d’Adobe Campaign, de votre éditeur à la page active en passant par le stockage et la boîte de réception du destinataire. Aucune information d’identification n’est créée, modifiée ou supprimée à l’une de ces étapes.

Si une image ne contient pas de métadonnées C2PA d’IA générative, car elle n’a pas été générée ou modifiée avec l’IA générative, aucune information d’identification ne s’affiche ici. Cela est attendu, et non une erreur.

## Vérification d’informations d’identification {#c2pa-checking-credential}

Il n’existe pas encore de moyen d’inspecter un Content Credential directement dans l’e-mail ou le concepteur de page de destination.

## Autres ressources

* [Utiliser la fonctionnalité de génération de contenu](generative-gs.md)
* [Transparence du contenu d’IA générative](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)