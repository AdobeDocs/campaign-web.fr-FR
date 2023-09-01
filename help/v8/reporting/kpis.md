---
title: Indicateurs de performance clés
description: Découvrez comment comprendre les indicateurs clés de performance
badge: label="Beta"
source-git-commit: e784f9aeb0805269561065c10ccbbf6756e62e44
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 98%

---

# Indicateurs de performance clés {#kpis}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Indésirables"
>abstract="KPI pour le courrier indésirable"

Accédez à la page d’accueil pour vérifier les indicateurs clés de performances de votre plateforme. Ces indicateurs indiquent le nombre et le pourcentage de messages diffusés, ouverts, mais aussi les clics, les désinscriptions et les taux d’erreur.

Par défaut, les mesures sont calculées pour les diffusions au cours des 7 derniers jours. Vous pouvez modifier la période dans la liste déroulante située dans la section supérieure droite de la vignette. Les messages envoyés aux profils de test sont exclus.

Vous pouvez sélectionner le canal à afficher. Par défaut, ces indicateurs reflètent les mesures pour le canal e-mail.

![](assets/kpi.png)

## Message diffusé {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Diffusés"
>abstract="Cette mesure indique, pour le canal sélectionné, le nombre de tous les messages traités et le pourcentage de messages diffusés par rapport au nombre total de messages envoyés."

Le nombre de messages diffusés reflète votre taux de délivrabilité. Ce taux ne peux jamais être de 100 % pour les raisons suivantes : certaines adresses e-mail ou numéros de téléphone peuvent être erronés, les bloqueurs de spam des fournisseurs de messagerie peuvent rejeter vos messages ou des problèmes de délivrabilité peuvent se produire.

L’indicateur **Diffusés** montre les KPI suivants, pour chaque canal :

* Pourcentage du nombre de messages diffusés par rapport au nombre total de messages envoyés.

* Nombre de messages traités.

Dans Adobe Campaign, la règle pour marquer un message comme « Diffusé » est la suivante :

Nombre de messages pour lesquels le champ « adresse de contrôle » est égal à « Non » et dont le statut est égal à « Pris en compte par le prestataire » (pour les SMS) ou « Envoyé » (pour les e-mails) ou « Reçu sur le mobile » (pour les notifications push).


## Total des ouvertures {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Ouvertures"
>abstract="Cette mesure indique, pour le canal sélectionné, le nombre de messages ouverts et le pourcentage de messages ouverts par rapport au nombre total de messages diffusés."

Le nombre d’e-mails ouverts est calculé par le tracking du nombre de fois où un message est ouvert, indépendamment du nombre de personnes destinataires individuelles qui ont ouvert ces messages. Cet indicateur n’est disponible que pour les e-mails.

L’indicateur **Ouvertures** montre les KPI suivants, pour chaque canal :

* Pourcentage du nombre de messages ouverts par rapport au nombre total de messages diffusés.

* Nombre total de messages ouverts, par canal.

Adobe Campaign détecte les messages ouverts lorsque la personne destinataire télécharge les images dans l’e-mail. Les e-mails HTML et Multipart/Alternative incluent une image de 0 pixel, qui vous permet de détecter les messages ouverts. Les messages au format texte ne contenant aucune image, il est impossible de détecter s’ils ont été ouverts ou non. Les valeurs calculées à partir du nombre de messages ouverts sont toujours des estimations, en raison de la marge d’erreur liée à l’affichage des images.



## Taux de clic publicitaire {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clics"
>abstract="Cette mesure indique, pour le canal sélectionné, le nombre de toutes les URL ayant fait l’objet d’un clic dans les messages, ainsi que le pourcentage de clics par rapport au nombre total de messages diffusés."

Dans votre message, vous pouvez ajouter des URL qui redirigent les personnes destinataires vers une page spécifique. Le taux de clic publicitaire mesure le nombre et le pourcentage de personnes destinataires ayant cliqué sur un lien dans le message.

L’indicateur **Clics** montre les KPI suivants, pour chaque canal :

* Pourcentage du nombre de clics par rapport au nombre total de messages diffusés.

* Nombre de personnes distinctes ayant cliqué au moins une fois pour une même diffusion. Les liens de désinscription et les liens vers la page miroir de l’email sont exclus.

Ces mesures sont basées sur la table de tracking consolidé (`nms:trackingStats`). Cette table agrégée est utilisée pour des raisons de performances lors de l’affichage des rapports, à la place de la table des logs de tracking des personnes destinataires (`nms:trackingLogRcp`) et elle n’est pas calculée en temps réel. La table est générée quelques minutes après la récupération des logs de tracking.


## Taux de désinscription {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Désinscriptions"
>abstract="Cette mesure indique, pour le canal sélectionné, le nombre de toutes les désinscriptions à un service, ainsi que le pourcentage de désinscriptions par rapport au nombre total de messages diffusés."

Les personnes destinataires doivent pouvoir se désinscrire des e-mails et des SMS par le biais d’un lien de désinscription dédié dans le contenu de l’email, ou en répondant STOP à un SMS.

L’indicateur **Désinscriptions** montre les KPI suivants, pour chaque canal :

* Pourcentage du nombre de désinscriptions par rapport au nombre total de messages diffusés.

* Nombre total de tous les clics sur un lien de désinscription, soit une catégorie d’URL égale à « opt-out ».


## Taux d’erreur {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Erreurs"
>abstract="Nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des rebonds. Le taux associé est le ratio par rapport au nombre de messages à diffuser."

Certains messages envoyés par votre plateforme Adobe Campaign peuvent ne pas arriver à destination. Cela peut se produire lorsque l’adresse de l’utilisateur ou de l’utilisatrice ou le numéro de téléphone contient des fautes de frappe, si la personne destinataire a modifié son adresse e-mail, ou si sa boîte de réception est pleine. Si un message ne peut pas être envoyé à un profil, le serveur distant envoie automatiquement un message d’erreur à Adobe Campaign. Cette erreur est qualifiée pour déterminer si l’adresse e-mail, le numéro de téléphone ou l’appareil doit être mis en quarantaine.

Par conséquent, vous devez toujours vérifier et mettre à jour votre base de données, et vous assurer que tous les profils sont actifs et réels. Les erreurs de diffusion peuvent être temporaires ou permanentes (rebonds temporaires ou définitifs), selon la raison pour laquelle le message n’a pas été diffusé.

L’indicateur **Erreurs** montre les KPI suivants, pour chaque canal :

* Pourcentage du nombre d’erreurs, par rapport au nombre total de messages à diffuser.

* Nombre total d’erreurs cumulées lors des diffusions et du traitement automatique des rebonds.

