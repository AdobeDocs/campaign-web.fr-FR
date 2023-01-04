---
audience: end-user
title: Paramètres avancés
description: Documentation de l’application web de Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 4fbb5e2eb0211712d17f1437986038c40ed15602
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 60%

---

# Paramètres avancés {#advanced-settings}

>[!NOTE]
>
>Cette documentation est en cours d’élaboration et est fréquemment mise à jour. La version finale de ce contenu sera prête en janvier 2023.

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
>title="Typology"
>abstract="La typologie permet de contrôler, filtrer et contrôler l&#39;envoi des diffusions."

Les typologies sont des ensembles de règles de typologie, qui sont exécutés pendant la phase d’analyse du message. Elles vous permettent de vous assurer que vos e-mails contiennent toujours certains éléments (comme un lien de désinscription ou une ligne d’objet) ou des règles de filtrage pour exclure des groupes de votre cible visée (tels que les clients désabonnés, les concurrents et les clients ne faisant pas partie du programme de fidélité).

Lors de l’association d’une typologie à un message ou à un modèle de message, les règles de typologie incluses dans la typologie sont exécutées pour vérifier la validité du message.

### Paramètres de pression {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Poids de la diffusion"
>abstract="Les poids de chaque diffusion permettent d&#39;identifier les diffusions prioritaires dans un contexte de gestion de la pression. Les messages dont le poids est le plus important sont prioritaires."

Dans cette section, les paramètres de pression permettent de définir un seuil. Il s’agit du nombre maximum de messages qui peuvent être envoyés à un profil sur une période donnée. Une fois ce seuil atteint, aucune diffusion ne sera envoyée jusqu&#39;à la fin de la période concernée. Ce mode de fonctionnement permet d&#39;exclure automatiquement un profil d&#39;une diffusion si l&#39;envoi du message provoquait le dépassement du seuil défini, et ainsi une sur-sollicitation.

La valeur de ce seuil peut être constante ou variable. Pour une même période, le seuil peut donc varier d&#39;un profil à l&#39;autre, et même pour un même profil.

Dans le **Type de poids** , trois options sont disponibles :

Le **Poids de la diffusion** field vous permet de :

Le **Mode de diffusion** champ..

### Paramètres de capacité {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importance du destinataire"
>abstract="L&#39;importance du destinataire est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées."

Dans cette section, vous pouvez sélectionner une règle de capacité définie dans la console Adobe Campaign v8. Cette règle est associée au canal email.

Le **importance du destinataire** field est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées.

## Audience {#audience}

Dans cette section, vous pouvez choisir un mapping de ciblage défini dans la console Adobe Campaign v8. La création du mapping de ciblage est nécessaire dans le cas où vous utilisez une table de destinataires autre que celle fournie par Adobe Campaign.

## Diffusion {#delivery}

Tester la diffusion via SMTP : cette option vous permet de tester la diffusion par SMTP. La diffusion est traitée jusqu’à la connexion au serveur SMTP mais n’est pas envoyée : pour chaque destinataire de la diffusion, Campaign se connecte au serveur du fournisseur SMTP, exécute la commande SMTP RCPT TO et ferme la connexion avant la commande SMTP DATA.

E-mail Cci : cette option vous permet de stocker vos e-mails dans un système externe à l’aide de l’option Cci en ajoutant simplement une adresse e-mail à la cible des messages.

### Reprises {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Nombre maximal de reprises"
>abstract="Si un message est en échec en raison d’une erreur temporaire, les reprises seront effectuées pendant la durée de la diffusion."

Les messages temporairement non diffusés en raison d’une erreur Soft ou Ignoré font l’objet d’une nouvelle tentative automatique. Par défaut, cinq reprises sont planifiées le premier jour de l’envoi, avec un intervalle minimum d’une heure, réparties sur les 24h de la journée. Une reprise par jour est ensuite programmée jusqu&#39;à la date limite d&#39;envoi, définie dans l&#39;onglet Validité .

## Validation {#approval}

**Manuelle**

**Semi-automatique**

**Automatique**

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Mode de validation"
>abstract="Chaque étape d&#39;une diffusion peut faire l&#39;objet d&#39;une validation afin d&#39;assurer un suivi et un contrôle complets des différents processus."

## Validité {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Durée de diffusion"
>abstract="Le champ Durée de diffusion permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n&#39;est pas atteinte."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Validité des ressources"
>abstract="Le champ Limite de validité est utilisé pour les ressources téléchargées, principalement pour la page miroir et les images. Les ressources de cette page sont valides pendant une durée limitée."


Le champ Durée de diffusion permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n&#39;est pas atteinte.

Vous pouvez également choisir de spécifier des dates.Pour cela, cochez l&#39;option Fixer explicitement les dates de validité. Dans ce cas, les dates limites de diffusion et de validité permettent de préciser également l&#39;heure. Cette heure correspond par défaut à l&#39;heure courante mais peut être modifiée directement dans le champ de saisie.

Limite de validité des ressources : le champ Limite de validité est utilisé pour les ressources téléchargées, principalement pour la page miroir et les images. Les ressources de cette page ont une durée de validité limitée (afin d’économiser de l’espace disque).

### Gestion de la page miroir {#mirror}

**Gestion de la page miroir**

### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Période de validité"
>abstract="Cette option définit la durée d’activation du tracking sur les URL."

**Limite de validité du suivi**: Cette option définit la durée d’activation du tracking sur les URL.

**URL de substitution des URL expirées**: TBC


## Paramètres de test{#test-setttings}

**Conserver double**

**Conserve les adresses placées sur la liste bloquée**

**Conserver les quarantaines**

**Conserver le code diffusion pour le BAT**

**Préfixe du libellé**