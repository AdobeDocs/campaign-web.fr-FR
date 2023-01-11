---
audience: end-user
title: Paramètres avancés
description: Documentation de l’application web de Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 50%

---

# Paramètres avancés {#advanced-settings}

![](../assets/do-not-localize/badge.png)

Ces paramètres sont les suivants : **paramètres de diffusion technique** qui sont définis dans le modèle d’email. Si vous souhaitez modifier l’une d’elles pour une diffusion spécifique, faites attention.

## Paramètres de diffusion email {#email-delivery-settings}

>[!NOTE]
>
> Modifiez uniquement les paramètres, aucune nouvelle création n’est autorisée. Sujet des droits d&#39;accès.

## Typology {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typology"
>abstract="La typologie permet de contrôler, filtrer et contrôler l&#39;envoi des diffusions."

Les typologies sont des ensembles de **règles de typologie**, qui sont exécutés pendant la phase d’analyse du message. Elles vous permettent de vous assurer que vos e-mails contiennent toujours certains éléments (comme un lien de désinscription ou une ligne d’objet) ou des règles de filtrage pour exclure des groupes de votre cible visée (tels que les clients désabonnés, les concurrents et les clients ne faisant pas partie du programme de fidélité).

Lors de l’association d’une typologie à un message ou à un modèle de message, les règles de typologie incluses dans la typologie sont exécutées pour vérifier la validité du message.

### Paramètres de pression {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Poids de la diffusion"
>abstract="Les poids de chaque diffusion permettent d&#39;identifier les diffusions prioritaires dans un contexte de gestion de la pression. Les messages dont le poids est le plus important sont prioritaires."

Dans cette section, les paramètres de pression permettent de définir une **seuil**. Il s’agit du nombre maximum de messages qui peuvent être envoyés à un profil sur une période donnée. Une fois ce seuil atteint, aucune diffusion ne sera envoyée jusqu&#39;à la fin de la période concernée. Ce mode de fonctionnement permet d&#39;exclure automatiquement un profil d&#39;une diffusion si l&#39;envoi du message provoquait le dépassement du seuil défini, et ainsi une sur-sollicitation.

La valeur de ce seuil peut être constante ou variable. Pour une même période, le seuil peut donc varier d&#39;un profil à l&#39;autre, et même pour un même profil.

Dans le **Type de poids** , trois options sont disponibles : (formule manquante selon l’option.)

* **Constante**
* **Dépend du destinataire**
* **Défini dans chaque règle**

Le **Poids de la diffusion** field : Chaque diffusion a un poids qui représente son niveau de priorité. Par défaut, le poids d&#39;une diffusion est défini sur 5. Les règles de pression permettent de définir le poids des diffusions auxquelles elles seront appliquées. Les poids peuvent être définis ou calculés à partir d&#39;une formule en fonction des destinataires. Vous pouvez par exemple définir le poids d&#39;une diffusion en fonction des centres d&#39;intérêt des destinataires.

Le **Mode de diffusion** champ.. ??

* **Estimation de la cible et personnalisation des messages**
* **Estimation et validation de la cible prévisionnelle**
* **Evaluation de la cible**

### Paramètres de capacité {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importance du destinataire"
>abstract="L&#39;importance du destinataire est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées."

Dans cette section, vous pouvez sélectionner une règle de capacité définie dans la console Adobe Campaign v8. Cette règle est associée au canal email.

Le **importance du destinataire** field est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées.

## Audience {#audience}

Dans cette section, vous pouvez choisir un **mapping de ciblage** définie dans la console Adobe Campaign v8. La création du mapping de ciblage est nécessaire dans le cas où vous utilisez une table de destinataires autre que celle fournie par Adobe Campaign.

## Diffusion {#delivery}

**Routage** selection : Le compte externe Routage e-mail intégré est fourni par défaut. Il contient les paramètres techniques qui permettent à l’application d’envoyer des emails.

**Tester la diffusion via SMTP** : cette option vous permet de tester la diffusion par SMTP. La diffusion est traitée jusqu’à la connexion au serveur SMTP mais n’est pas envoyée : pour chaque destinataire de la diffusion, Campaign se connecte au serveur du fournisseur SMTP, exécute la commande SMTP RCPT TO et ferme la connexion avant la commande SMTP DATA.

**E-mail Cci** : cette option vous permet de stocker vos e-mails dans un système externe à l’aide de l’option Cci en ajoutant simplement une adresse e-mail à la cible des messages.

### Reprises {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Nombre maximal de reprises"
>abstract="Si un message est en échec en raison d’une erreur temporaire, les reprises seront effectuées pendant la durée de la diffusion."

Les messages temporairement non diffusés en raison d’une erreur Soft ou Ignoré font l’objet d’une nouvelle tentative automatique. Par défaut, cinq reprises sont planifiées le premier jour de l’envoi, avec un intervalle minimum d’une heure, réparties sur les 24h de la journée. Une reprise par jour est ensuite programmée jusqu&#39;à la date limite d&#39;envoi, définie dans l&#39;onglet Validité .

## Validation {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Validation mode"
>abstract="Chaque étape d&#39;une diffusion peut faire l&#39;objet d&#39;une validation afin d&#39;assurer un suivi et un contrôle complets des différents processus."

**Manuel** : à la fin de la phase d’analyse, l’utilisateur doit confirmer la diffusion pour commencer l’envoi.

**Semi-automatique**: L&#39;envoi commence automatiquement si la phase d&#39;analyse ne génère aucun message d&#39;avertissement.

**Automatique** : les envois démarrent automatiquement à la fin de la phase d’analyse, quel qu’en soit le résultat.


## Validité {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Durée de diffusion"
>abstract="Le champ Durée de diffusion permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n&#39;est pas atteinte."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Validité des ressources"
>abstract="Le champ Limite de validité est utilisé pour les ressources téléchargées, principalement pour la page miroir et les images. Les ressources de cette page sont valides pendant une durée limitée."


Le champ **Durée de diffusion** permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n&#39;est pas atteinte.

Vous pouvez également choisir de spécifier des dates.Pour cela, cochez l&#39;option **Fixer explicitement les dates de validité**. Dans ce cas, les dates limites de diffusion et de validité permettent de préciser également l&#39;heure. Cette heure correspond par défaut à l&#39;heure courante mais peut être modifiée directement dans le champ de saisie.

**Limite de validité des ressources** est utilisé pour les ressources téléchargées, principalement pour la page miroir et les images. Les ressources de cette page ont une durée de validité limitée (afin d’économiser de l’espace disque).

### Gestion de la page miroir {#mirror}

**Gestion des pages miroir** contient quatre options :

* **Générer la page miroir si un lien miroir apparaît dans le contenu de l&#39;email**: la page miroir est générée si le lien est inséré dans le contenu du mail.
* **Forcer la génération de la page miroir** : même si aucun lien vers la page miroir n’est inséré dans les messages, la page miroir sera créée.
* **Ne pas générer de page miroir** : aucune page miroir n’est générée, même si le lien est présent dans les messages.
* **Génère une page miroir accessible à l’aide de l’identifiant du message uniquement**: cette option permet d&#39;accéder au contenu de la page miroir, avec les informations de personnalisation, dans la fenêtre des logs de diffusion.


### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Période de validité"
>abstract="Cette option définit la durée d’activation du tracking sur les URL."

**Limite de validité du suivi**: Cette option définit la durée d’activation du tracking sur les URL.

**URL de substitution des URL périmées** : utilisez cette option pour renseigner une URL vers une page web de secours. Elle s&#39;affiche après expiration du tracking.


## Paramètres de test {#test-setttings}

**Conserver double** permet d&#39;autoriser plusieurs diffusions vers des destinataires répondant à plusieurs critères de ciblage.

**Conserver les adresses placées sur la liste bloquée** permet de garder à l&#39;écart de la cible les profils qui ne sont plus ciblés par la diffusion, par exemple après une désinscription (opt-out).

**Conserver les adresses en quarantaine** permet de garder à l’écart de la cible les profils dont l’adresse ne répond pas.

**Conserver le code de diffusion pour le BAT** permet d&#39;attribuer au BAT le même code de diffusion que celui défini pour la diffusion à laquelle il correspond.

Par défaut, le sujet du BAT est précédé du préfixe ‘BAT #’, où # est le numéro du BAT. Vous pouvez modifier ce préfixe dans la variable **Préfixe d’étiquette** champ .