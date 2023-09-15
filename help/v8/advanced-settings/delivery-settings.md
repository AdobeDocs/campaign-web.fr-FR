---
audience: end-user
title: Paramètres de diffusion
description: En savoir plus sur les paramètres de diffusion dans Campaign Web
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Beta"
source-git-commit: d2497ad144e32f5d164d6be87ab690280c5e3dc9
workflow-type: tm+mt
source-wordcount: '2094'
ht-degree: 71%

---


# Paramètres de diffusion {#email-del-settings}

Les paramètres de diffusion des emails sont **paramètres de diffusion technique** qui sont définis dans le modèle d’email. Elles peuvent être surchargées pour chaque diffusion.

Ces paramètres sont disponibles à partir du **Configuration des paramètres de diffusion** icône disponible lors de l&#39;édition d&#39;une diffusion email ou d&#39;un modèle de diffusion email.


## Paramètres de diffusion d’e-mail {#email-delivery-settings}

>[!CAUTION]
>
>Ces paramètres sont décrits uniquement à titre d’information. Certains dépendent de votre configuration et de vos autorisations. Ils ne doivent pas être modifiées dans cette version du produit.

## Paramètres de typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="Typologie les règles permettent aux marketeurs de normaliser les pratiques commerciales, dans toutes les diffusions. Une typologie est un ensemble de règles de typologie qui vous permet de contrôler, filtrer et prioriser l&#39;envoi des diffusions. Les profils qui correspondent à des critères dans une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Paramètres de typologie de la diffusion"
>abstract="Les règles de typologie permettent aux marketeurs de normaliser les pratiques commerciales, dans toutes les diffusions. Une typologie est un ensemble de règles de typologie qui vous permet de contrôler, filtrer et prioriser l&#39;envoi des diffusions. Les profils qui correspondent à des critères dans une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation."


Les typologies sont des ensembles de **règles de typologie**, qui sont exécutés pendant la phase de préparation. Les règles de typologie permettent aux marketeurs de normaliser les pratiques commerciales, dans toutes les diffusions. Une typologie est un ensemble de règles de typologie qui vous permet de contrôler, filtrer et prioriser l&#39;envoi des diffusions. Les profils qui correspondent à des critères dans une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation de la diffusion.  Elles vous permettent de vous assurer que vos e-mails contiennent toujours certains éléments (comme un lien de désinscription ou une ligne d’objet) ou des règles de filtrage pour exclure des groupes de votre cible visée (tels que les clients et clientes désabonnés, les concurrents et les client(e)s ne faisant pas partie du programme de fidélité).

Les règles de typologie sont regroupées au sein d&#39;une typologie afin d&#39;appliquer facilement plusieurs règles de filtrage à une même diffusion.

Lors de l’association d’une typologie à un message ou à un modèle de message, les règles de typologie incluses dans la typologie sont exécutées pour vérifier la validité du message durant la préparation de celui-ci.

![](assets/delivery-settings-1.png)




### Paramètres de pression {#pressure-parameters}


>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Paramètres de pression pour la diffusion"
>abstract="Le poids des diffusions permet d&#39;identifier les diffusions prioritaires dans le cadre de la gestion de la fatigue. Les messages dont le poids est le plus élevé sont prioritaires."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Poids de la diffusion"
>abstract="Les poids de chaque diffusion permettent d’identifier les diffusions prioritaires dans un contexte de gestion de la pression. Les messages dont le poids est le plus important sont prioritaires."

Dans cette section, les paramètres de pression permettent de définir une **seuil** pour configurer des règles de gestion de la fatigue. Il s’agit du nombre maximum de messages qui peuvent être envoyés à un profil sur une période donnée. Une fois ce seuil atteint, aucune diffusion ne sera envoyée jusqu&#39;à la fin de la période concernée. Ce mode de fonctionnement permet d&#39;exclure automatiquement un profil d&#39;une diffusion si l&#39;envoi du message provoquait le dépassement du seuil défini, et ainsi une sur-sollicitation.

La valeur de ce seuil peut être constante ou variable. Pour une même période, le seuil peut donc varier d&#39;un profil à l&#39;autre, et même pour un même profil.

Dans le champ **Type de poids**, trois options sont disponibles :

* **Constant**
* **Dépend du destinataire**
* **Défini dans chaque règle**

Utilisez le champ **Poids de la diffusion** pour définir la priorité de diffusion. Chaque diffusion a un poids qui représente son niveau de priorité. Par défaut, le poids d’une diffusion est défini sur 5. Les règles de pression permettent de définir le poids des diffusions auxquelles elles s’appliquent. Le poids peut être fixe ou calculé au travers d’une formule afin de l’adapter en fonction des destinataires. Par exemple, vous pouvez définir le poids d’une diffusion en fonction des centres d’intérêt d’un(e) destinataire.


Utilisez le champ **Mode de diffusion** pour sélectionner le mode d’évaluation de la cible. Trois modes sont disponibles :

* **Estimation de la cible et personnalisation des messages**
* **Estimation et validation de la cible prévisionnelle**
* **Évaluation de la cible**

La gestion de la fatigue est comprise dans le module complémentaire **Optimisation de campagne**. En savoir plus sur les règles de pression et comment configurer la gestion de la fatigue dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=fr){target="_blank"}.

### Paramètres de capacité {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Paramètres de capacité pour la diffusion"
>abstract="Avant de diffuser des messages, utilisez les règles de capacité pour vous assurer que votre organisation peut traiter la diffusion, les messages entrants que la diffusion peut générer et le nombre d&#39;appels à passer pour contacter les abonnés, par exemple. Les règles de capacité sont définies dans la console Adobe Campaign v8. Dans cet écran, sélectionnez une règle associée au canal email."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Importance du destinataire"
>abstract="L’importance du destinataire est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées."


Dans cette section, vous pouvez sélectionner une règle de capacité définie dans la console Adobe Campaign v8. Cette règle est associée au canal e-mail.

Le champ **Importance du destinataire** est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées.

En savoir plus sur les règles de cohérence et de capacité et comment les configurer dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=fr){target="_blank"}.


## Paramètres de l’audience {#audience}


>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Paramètres d’audience pour la diffusion"
>abstract="Sélectionnez une **mapping de ciblage** parmi celles disponibles. Les mappings de ciblage sont définis dans la console Adobe Campaign v8. Vous pouvez également définir les paramètres d&#39;exclusion de la diffusion. "


Dans cette section, vous pouvez sélectionner un **mapping de ciblage** parmi ceux disponibles. Les mappings de ciblage sont définis dans la console Adobe Campaign v8.

En savoir plus sur les mappings de ciblage dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=fr){target="_blank"}.

## Diffusion {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Paramètres de diffusion pour la diffusion"
>abstract="Les paramètres de diffusion sont des paramètres techniques qui s’appliquent à votre diffusion. Vous pouvez activer Cci pour la diffusion et modifier les modes de diffusion et de routine. Ces options sont limitées aux utilisateurs experts uniquement."

Les paramètres de diffusion sont des paramètres techniques qui s’appliquent à votre diffusion.

* **Routage** : le compte externe de routage d’e-mail intégré est fourni par défaut. Il contient les paramètres techniques qui permettent à l’application d’envoyer des emails.

* **Tester la diffusion par SMTP** : cette option vous permet de tester l’envoi par SMTP. La diffusion est traitée jusqu’à la connexion au serveur SMTP mais n’est pas envoyée : pour chaque destinataire de la diffusion, Campaign se connecte au serveur du fournisseur SMTP, exécute la commande SMTP RCPT TO et ferme la connexion avant la commande SMTP DATA.

* **E-mail Cci** : cette option vous permet de stocker vos e-mails dans un système externe à l’aide de l’option Cci en ajoutant simplement une adresse e-mail à la cible de vos messages. En savoir plus sur la fonctionnalité Email Cci dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=fr){target="_blank"}.

### Web Analytics {#web-analytics}


>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Paramètres des analyses web pour la diffusion"
>abstract="Sélectionnez un compte Web Analytics. Ce compte est paramétré dans la console cliente Campaign. Vous pouvez également définir les balises partagées avec l’outil d’analyse que vous utilisez."

Dans cette section, vous pouvez sélectionner un compte Web Analytics. Ce compte est paramétré dans la console cliente Campaign.

Vous pouvez également définir les balises partagées avec l’outil d’analyse que vous utilisez.

En savoir plus sur Web Analytics et Campaign dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=fr){target="_blank"}.


### Reprises {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Nombre maximal de reprises"
>abstract="Si un message est en échec en raison d’une erreur temporaire, les reprises sont effectuées jusqu’à la fin de la durée de diffusion."

Les messages temporairement non diffusés en raison d’une erreur Soft ou Ignoré font l’objet d’une nouvelle tentative automatique. Par défaut, cinq reprises sont planifiées le premier jour de l’envoi, avec un intervalle minimum d’une heure, réparties sur les 24h de la journée.

En savoir plus sur la gestion des reprises dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=fr){target="_blank"}.

## Approbation {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Mode de validation de la diffusion"
>abstract="Sélectionnez le mode de validation. Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Mode de validation des diffusions"
>abstract="Sélectionnez le mode de validation des diffusions à partir de ce modèle. Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non."

Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non. Par défaut, l’utilisateur ou l’utilisatrice doit confirmer l’envoi des messages à la fin de la phase d’analyse : il s’agit d’une validation **manuelle**.

Vous pouvez sélectionner un autre mode de validation dans le champ correspondant. Les modes disponibles sont les suivants :

* **Manuel** : à la fin de la phase d’analyse, l’utilisateur ou l’utilisatrice doit confirmer la diffusion pour commencer l’envoi.

* **Semi-automatique** : les envois démarrent automatiquement si la phase d’analyse ne génère aucun message d’avertissement.

* **Automatique** : les envois démarrent automatiquement à la fin de la phase d’analyse, quel qu’en soit le résultat.


## Validité {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Validité des paramètres"
>abstract="Le champ « Durée de diffusion » permet de saisir la limite pour les reprises globales de diffusion. Cela signifie qu’Adobe Campaign envoie les messages à partir de la date de début, puis, pour les messages renvoyant une erreur uniquement, des reprises régulières et paramétrables sont effectuées jusqu’à ce que la limite de validité soit atteinte. Le champ « Limite de validité » est utilisé pour les ressources chargées, telles que la page miroir ou les images. Ces ressources sont valides pour une durée limitée. Une fois la limite atteinte, elles ne sont plus disponibles."



>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Limite de validité des ressources"
>abstract="Le champ Limite de validité est utilisé pour les ressources téléchargées, comme la page miroir ou les images. Ces ressources sont valides pour une durée limitée. Une fois la limite atteinte, elles ne sont plus disponibles."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Durée de diffusion"
>abstract="Le champ Durée de diffusion permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de validité n’est pas atteinte."
<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

Le champ **Durée de diffusion** permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n&#39;est pas atteinte.

Vous pouvez également choisir de spécifier des dates.Pour cela, cochez l&#39;option **Fixer explicitement les dates de validité**. Dans ce cas, les dates limites de diffusion et de validité permettent de préciser également l&#39;heure. Cette heure correspond par défaut à l&#39;heure courante mais peut être modifiée directement dans le champ de saisie.

Le champ **Limite de validité des ressources** est utilisé pour les ressources téléchargées, principalement pour la page miroir et les images. Les ressources de cette page ont une durée de validité limitée (afin d’économiser de l’espace disque). Au-delà de cette limite, ces ressources ne sont plus disponibles.

![](assets/delivery-settings-2.png)


En savoir plus sur la période de validité des diffusions dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=fr#validity-period){target="_blank"}.

### Gestion de la page miroir {#mirror}

La page miroir est une page HTML accessible en ligne via un navigateur web et dont le contenu est identique à celui de l’email. Par défaut, la page miroir est générée si le lien est inséré dans le contenu de l’email.

Outre le mode par défaut, les options disponibles sont les suivantes :


* **[!UICONTROL Forcer la génération de la page miroir]** : ce mode permet de générer la page miroir même si aucun lien vers celle-ci n’est inséré dans la diffusion.
* **[!UICONTROL Ne pas générer de page miroir]** : ce mode permet de ne pas générer de page miroir, même si le lien est présent dans la diffusion.
* **[!UICONTROL Générer une page miroir accessible depuis l’identifiant du message]** : ce mode permet d’accéder au contenu de la page miroir, dans la fenêtre du log de diffusion de la console cliente, lorsque l’e-mail ne contient pas de lien vers celle-ci.


### Tracking {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->




>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Période de validité"
>abstract="La période de validité définit la durée d&#39;activation du tracking sur les URL des messages."


Les paramètres de tracking sont définis dans la section correspondante. Les options possibles sont les suivantes :

**Limite de validité du tracking** : utilisez cette option pour définir la durée d’activation du tracking sur les URL.

**URL de substitution des URL périmées** : utilisez cette option pour renseigner une URL vers une page web de secours. Elle s’affiche après expiration du tracking.

## Paramètres de test {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Paramètres de test de la diffusion"
>abstract="Sélectionnez les paramètres d&#39;exclusion et personnalisez le libellé des emails de test."

Vous pouvez définir les paramètres d’exclusion dans cette section. Les options disponibles sont les suivantes :

* L’option **Conserver double** permet d’autoriser plusieurs diffusions vers des destinataires répondant à plusieurs critères de ciblage.

* L’option **Conserver les adresses placées sur la liste bloquée** permet de tenir à l’écart de la cible les profils qui ne sont plus ciblés par la diffusion, par exemple après une désinscription (opt-out).

* L’option **Conserver les adresses placées en quarantaine** permet de tenir à l’écart de la cible les profils dont l’adresse ne répond pas.

Vous pouvez également personnaliser le nom des e-mails de test.

Utilisez l’option **Conserver le code de diffusion pour le BAT** pour associer à l’e-mail de test le même code de diffusion que celui défini pour la diffusion à laquelle il se rapporte.

Par défaut, l’objet de l’e-mail de test est précédé du préfixe « BAT # », où # correspond au numéro de l’e-mail de test. Vous pouvez modifier ce préfixe dans le champ **Préfixe de libellé**.