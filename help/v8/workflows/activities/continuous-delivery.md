---
audience: end-user
title: Utilisation de l’activité de workflow Diffusion continue
description: Découvrez comment utiliser l’activité de workflow Diffusion continue
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
TQID: https://experienceleague.adobe.com/uWGhvUmHdS0ixFI4d-uEPgpxSnZoOwNRMbn8aZfqA98
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 242
ht-degree: 100%

---

# Diffusion continue {#continuous-delivery}

L’activité **Diffusion continue** permet d’ajouter de nouveaux destinataires à une diffusion existante. Ce type de diffusion évite d’avoir à créer une diffusion à chaque fois, ce qui le rend plus efficace pour les alertes ou notifications à faible volume envoyées selon les besoins.

Une diffusion continue crée une instance de diffusion unique. Tous les logs de diffusion (broadLog) et les logs de tracking référencent cette diffusion, ce qui simplifie la surveillance et le reporting.

## Configuration de l’activité Diffusion continue {#configure}

1. Ajoutez une activité **Diffusion continue** à la zone de travail du workflow.

   ![Capture d’écran montrant l’activité Diffusion continue](../assets/continuous-delivery.png){zoomable="yes"}

1. Saisissez un **[!UICONTROL libellé]** personnalisé pour l’activité (facultatif).Par défaut, elle est nommée « Diffusion continue ».

1. En regard du champ **[!UICONTROL Modèle]**, cliquez sur l’icône de recherche pour sélectionner un modèle de diffusion.Seuls les modèles (et non les diffusions standard) peuvent être sélectionnés.Le modèle définit le canal de diffusion, le contenu et la configuration.

1. Dans les **[!UICONTROL Options de ciblage]**, choisissez le mode de définition de la population cible :

   * **[!UICONTROL Spécifiée par les événements entrants]** : la cible provient de la transition entrante (des activités en amont comme Créer une audience ou Requête incrémentale).Il s’agit de l’option la plus courante.

   * **[!UICONTROL Spécifiée dans le modèle de diffusion]** : la cible est définie dans le modèle.

   * **[!UICONTROL Fichier spécifié dans l’événement entrant]** : la cible est fournie via un fichier transmis par le workflow.

L’activité de diffusion continue génère automatiquement une transition sortante pour continuer le workflow.

## Rubriques connexes {#related}

* [À propos des activités de workflows](about-activities.md)
* [Diffusion automatisée](automated-delivery.md)
* [Activités e-mail, SMS, notification push, courrier](channels.md)
* [Modèles de diffusion](../../msg/delivery-template.md)
