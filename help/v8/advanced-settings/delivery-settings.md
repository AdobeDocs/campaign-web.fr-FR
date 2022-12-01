---
audience: end-user
title: Paramètres avancés
description: Documentation web de Campaign v8
source-git-commit: c90d8a5eff6169945d381f3250cb3e4d06194d31
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 41%

---

# Paramètres avancés {#advanced-settings}

>[!NOTE]
>
>Cette documentation est en cours de construction et fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

Ces paramètres sont des paramètres de diffusion techniques définis dans le modèle d’email. Si vous souhaitez modifier l’une d’elles pour une diffusion spécifique, faites attention.

## Paramètres de diffusion email {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

Tous les paramètres techniques de diffusion du modèle.
Modifiez uniquement les paramètres, pas de création ici.
En fonction des autorisations, les pragmatiques ne doivent pas modifier ce paramètre. Vérifier et modifier uniquement la règle de typologie -> reste défini dans le modèle

## Typology {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="La typologie permet de contrôler, filtrer et contrôler l&#39;envoi des diffusions."

### Paramètre de pression {#pressure-parameter}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Poids de la diffusion"
>abstract="Les poids de chaque diffusion permettent d&#39;identifier les diffusions prioritaires dans un contexte de gestion de la pression. Les messages dont le poids est le plus important sont prioritaires."

### Paramètres de capacité {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importance du destinataire"
>abstract="TBC"


## Audience {#audience}

## Diffusion {#delivery}

### Reprises {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Nombre maximal de reprises"
>abstract="Si un message est en échec en raison d’une erreur temporaire, les reprises seront effectuées pendant la durée de la diffusion."

## Validation {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Validation mode"
>abstract="Chaque étape d&#39;une diffusion peut faire l&#39;objet d&#39;une validation afin d&#39;assurer un suivi et un contrôle complets des différents processus."

## Validité {#validity}

### Période de validité {#validity-period}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Durée de diffusion"
>abstract="Le champ Durée de diffusion permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n&#39;est pas atteinte."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Validité des ressources"
>abstract="Le champ Limite de validité est utilisé pour les ressources téléchargées, principalement pour la page miroir et les images. Les ressources de cette page sont valides pendant une durée limitée."


### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Période de validité"
>abstract="Cette option définit la durée d’activation du tracking sur les URL."














