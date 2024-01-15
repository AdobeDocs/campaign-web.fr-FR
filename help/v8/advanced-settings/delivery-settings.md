---
audience: end-user
title: Paramètres de diffusion
description: En savoir plus sur les paramètres de diffusion dans Campaign Web.
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Disponibilité limitée"
source-git-commit: 93402a91511cff9cb6510f696238e667ec812f8d
workflow-type: tm+mt
source-wordcount: '2260'
ht-degree: 67%

---


# Paramètres de diffusion d’e-mail {#email-del-settings}

Les paramètres de diffusion d’e-mail sont des **paramètres de diffusion techniques** définis dans le modèle d’e-mail. Ils peuvent être surchargés pour chaque diffusion.

Ces paramètres sont disponibles à partir du **Paramètres** est disponible lors de l&#39;édition d&#39;une diffusion email ou d&#39;un modèle de diffusion email.

## Paramètres de diffusion d’e-mail {#email-delivery-settings}

>[!CAUTION]
>
>Ces paramètres sont décrits uniquement à titre d’information. Certains dépendent de votre configuration et de vos autorisations. Ils ne doivent pas être modifiées dans cette version du produit.

## Paramètres de typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="Les règles de typologie permettent aux personnes spécialisées dans le marketing de normaliser les pratiques commerciales de l’ensemble des diffusions. Une typologie est un ensemble de règles de typologie permettant de contrôler, filtrer et prioriser l’envoi des diffusions. Les profils qui correspondent à des critères dans une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation. Les typologies et les règles de typologie sont créées dans la console cliente Campaign."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Paramètres de typologie de la diffusion"
>abstract="Les règles de typologie permettent aux personnes spécialisées dans le marketing de normaliser les pratiques commerciales de l’ensemble des diffusions. Une typologie est un ensemble de règles de typologie permettant de contrôler, filtrer et prioriser l’envoi des diffusions. Les profils qui correspondent à des critères dans une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation. Les typologies et les règles de typologie sont créées dans la console cliente Campaign."


Les typologies sont des ensembles de **règles de typologie** qui sont exécutés pendant la phase de préparation afin d&#39;appliquer facilement plusieurs règles de filtrage à une diffusion à la fois. Ils permettent aux marketeurs de normaliser les pratiques commerciales dans toutes les diffusions, car ils leur permettent de contrôler, filtrer et prioriser l’envoi des diffusions.

Lors de l&#39;association d&#39;une typologie à un message ou à un modèle de message, les règles de typologie incluses dans la typologie sont exécutées afin de vérifier la validité de la diffusion lors de la préparation du message. Les profils qui correspondent à des critères dans une règle de typologie sont alors exclus des audiences de diffusion.

Les typologies vous permettent de vous assurer que vos emails contiennent toujours certains éléments (comme un lien de désinscription ou une ligne d’objet) ou des règles de filtrage pour exclure des groupes de votre cible prévue (comme les clients désabonnés, les concurrents ou les clients ne faisant pas partie de la fidélité).

![](assets/delivery-settings-typology.png)

>[!NOTE]
>
>Les typologies et les règles de typologie sont créées dans la console cliente Campaign. En savoir plus sur les règles de pression et la configuration de la gestion de la fatigue dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html?lang=fr){target="_blank"}.

### Paramètres de pression {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Paramètres de pression de la diffusion"
>abstract="Le poids des diffusions permet d’identifier les diffusions prioritaires dans le cadre de la gestion de la fatigue. Les messages dont le poids est le plus élevé sont prioritaires."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Poids de la diffusion"
>abstract="Les poids de chaque diffusion permettent d’identifier les diffusions prioritaires dans un contexte de gestion de la pression. Les messages dont le poids est le plus important sont prioritaires."

Dans cette section, les paramètres de pression permettent de définir une **seuil** pour configurer des règles de gestion de la fatigue, qui est le nombre maximal de messages pouvant être envoyés à un profil sur une période donnée.

Une fois ce seuil atteint, aucune diffusion ne sera envoyée jusqu&#39;à la fin de la période concernée. Ce mode de fonctionnement permet d&#39;exclure automatiquement un profil d&#39;une diffusion si l&#39;envoi du message provoquait le dépassement du seuil défini, et ainsi une sur-sollicitation.

La valeur de ce seuil peut être constante ou variable. Pour une même période, le seuil peut donc varier d&#39;un profil à l&#39;autre, et même pour un même profil.

Dans le champ **[!UICONTROL Type de poids]**, trois options sont disponibles :

* **[!UICONTROL Constant]**
* **[!UICONTROL Dépend du destinataire]**
* **[!UICONTROL Défini dans chaque règle]**

Utilisez le champ **[!UICONTROL Poids de la diffusion]** pour définir la priorité de diffusion. Chaque diffusion a un poids qui représente son niveau de priorité. Par défaut, le poids d’une diffusion est défini sur 5. Les règles de pression permettent de définir le poids des diffusions auxquelles elles s’appliquent. Le poids peut être fixe ou calculé au travers d’une formule afin de l’adapter en fonction des destinataires. Par exemple, vous pouvez définir le poids d’une diffusion en fonction des centres d’intérêt d’un(e) destinataire.

Utilisez le champ **[!UICONTROL Mode de diffusion]** pour sélectionner le mode d’évaluation de la cible. Trois modes sont disponibles :

* **[!UICONTROL Estimation de la cible et personnalisation des messages]**
* **[!UICONTROL Estimation et validation de la cible prévisionnelle]**
* **[!UICONTROL Évaluation de la cible]**

>[!NOTE]
>
>La gestion de la fatigue est paramétrée dans la console cliente Campaign. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=fr){target="_blank"}.

### Paramètres de capacité {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Paramètres de capacité de la diffusion"
>abstract="Avant de diffuser des messages, utilisez les règles de capacité pour vous assurer que votre organisation peut traiter notamment la diffusion, les messages entrants que la diffusion peut générer et le nombre d’appels à passer pour contacter les personnes abonnées. Les règles de capacité sont définies dans la console Adobe Campaign v8. Dans cet écran, sélectionnez une règle associée au canal e-mail."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Importance du destinataire"
>abstract="L’importance du destinataire est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées."


Dans cette section, vous pouvez sélectionner une règle de capacité définie dans la console Adobe Campaign v8. Cette règle est associée au canal e-mail.

La variable **[!UICONTROL Importance du destinataire]** field est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées.

>[!NOTE]
>
>Les règles de typologie sont configurées dans la console cliente Campaign. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=fr){target="_blank"}.

## Paramètres de l’audience {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Paramètres d’audience de la diffusion"
>abstract="Sélectionnez un **mapping de ciblage** parmi ceux disponibles. Les mappings de ciblage sont définis dans la console Adobe Campaign v8. Vous pouvez également définir les paramètres d’exclusion de la diffusion. "

Dans cette section, vous pouvez sélectionner un **mapping de ciblage** parmi ceux disponibles. Les mappings de ciblage sont définis dans la console Adobe Campaign v8. Le mapping de ciblage est le type de données qu’une opération gère. Il permet de définir la population ciblée : destinataires, bénéficiaires de contrats, opérateurs et opératrices, abonnés et abonnées, etc.

Pour plus d’informations sur les mappings de ciblage, consultez [cette section](../audience/targeting-dimensions.md).

Dans le **[!UICONTROL Exclusion]** , vous pouvez sélectionner pour exclure les destinataires qui ne souhaitent plus être contactés ou qui sont mis en quarantaine. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

## Diffusion {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Paramètres de diffusion de la diffusion"
>abstract="Les paramètres de diffusion sont des paramètres techniques qui s’appliquent à votre diffusion. Vous pouvez activer la fonction Cci de la diffusion et modifier les modes de diffusion et de routine. Ces options sont limitées aux personnes expertes uniquement."

**[!UICONTROL Diffusion]** Les paramètres sont des paramètres techniques qui s&#39;appliquent à votre diffusion.

L&#39;email intégré **[!UICONTROL Routage]** le compte externe est fourni par défaut. Il contient les paramètres techniques qui permettent à l’application d’envoyer des emails.

Vous pouvez définir ce qui suit : **[!UICONTROL Envoi]** settings :

* **[!UICONTROL Tester la diffusion SMTP]**: cette option est utilisée pour tester l’envoi par SMTP. La diffusion est traitée jusqu’à la connexion au serveur SMTP mais n’est pas envoyée : pour chaque destinataire de la diffusion, Campaign se connecte au serveur du fournisseur SMTP, exécute la commande SMTP RCPT TO et ferme la connexion avant la commande SMTP DATA.

* **[!UICONTROL Email Cci]**: cette option est utilisée pour stocker les emails sur un système externe via Cci en ajoutant simplement une adresse email en Cci à votre cible de message. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=fr){target="_blank"}.

Vous pouvez également modifier le format des emails envoyés :

* **[!UICONTROL Tenir compte des préférences des destinataires]** (mode par défaut)

  Le format du message est défini en fonction des données stockées dans le profil du destinataire. Si un destinataire souhaite recevoir les messages dans un format particulier, ce format lui est envoyé. Si le champ n’est pas renseigné, un message multipart-alternative est envoyé (voir ci-dessous).

* **[!UICONTROL Laisser le mailer des destinataires choisir le format le plus adapté]**

  Le message contient les deux formats : texte et HTML. Le format affiché lors de la réception dépend de la configuration du logiciel de messagerie du destinataire (multipart-alternative).

  >[!IMPORTANT]
  >
  >Cette option inclut les deux versions du document et, par conséquent, impacte le débit de diffusion des messages, car le poids du message est plus élevé.

* **[!UICONTROL Envoyer tous les messages au format texte]**

  Le message est envoyé au format texte. Le format HTML ne sera pas envoyé, mais utilisé pour la page miroir uniquement lorsque le destinataire clique sur le message.

## Web Analytics {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Paramètres Web Analytics de la diffusion"
>abstract="Sélectionnez un compte Web Analytics. Ce compte est configuré dans la console cliente Campaign. Vous pouvez également définir les balises partagées avec l’outil d’analyse que vous utilisez."

Dans cette section, vous pouvez sélectionner un compte Web Analytics. Ce compte est paramétré dans la console cliente Campaign.

Vous pouvez également définir les balises partagées avec l’outil d’analyse que vous utilisez.

>[!NOTE]
>
>Les fonctionnalités Web Analytics sont configurées dans la console cliente de Campaign. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html#external-account-ac){target="_blank"}.

## Reprises {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Nombre maximal de reprises"
>abstract="Si un message est en échec en raison d’une erreur temporaire, les reprises sont effectuées jusqu’à la fin de la durée de diffusion."

<!--Currently not visible in UI > ??-->

Les messages temporairement non diffusés en raison d’une erreur Soft ou Ignoré font l’objet d’une nouvelle tentative automatique. Par défaut, cinq reprises sont planifiées le premier jour de l’envoi, avec un intervalle minimum d’une heure, réparties sur les 24 heures de la journée.

En savoir plus sur la gestion des reprises dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=fr){target="_blank"}.

## Approbation {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Mode d’approbation de la diffusion"
>abstract="Sélectionnez le mode d’approbation. Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Mode d’approbation des diffusions"
>abstract="Sélectionnez le mode d’approbation des diffusions à partir de ce modèle. Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non."

Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non. Par défaut, l’utilisateur ou l’utilisatrice doit confirmer l’envoi des messages à la fin de la phase d’analyse : il s’agit d’une validation **manuelle**.

Vous pouvez sélectionner un autre mode de validation dans le champ correspondant. Les modes disponibles sont les suivants :

* ****[!UICONTROL Manuel]**** : à la fin de la phase d’analyse, l’utilisateur ou l’utilisatrice doit confirmer la diffusion pour commencer l’envoi.

* **[!UICONTROL Semi-automatique]** : les envois démarrent automatiquement si la phase d’analyse ne génère aucun message d’avertissement.

* **[!UICONTROL Automatique]** : les envois démarrent automatiquement à la fin de la phase d’analyse, quel qu’en soit le résultat.

## Validité {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Validité des paramètres"
>abstract="Le champ **Durée de diffusion** permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n’est pas atteinte.<br>La variable **Limite de validité des ressources** est utilisé pour les ressources chargées, telles que la page miroir ou les images. Une fois la limite atteinte, les ressources ne sont plus disponibles."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Limite de validité des ressources"
>abstract="La variable **Limite de validité des ressources** est utilisé pour les ressources téléchargées, telles que la page miroir ou les images. Ces ressources sont valides pour une durée limitée. Une fois la limite atteinte, elles ne sont plus disponibles."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Durée de diffusion"
>abstract="Le champ **Durée de diffusion** permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n’est pas atteinte."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### Période de validité {#validity-period}

Le champ **[!UICONTROL Durée de diffusion]** permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n’est pas atteinte.

Vous pouvez également choisir de spécifier des dates. Pour ce faire, sélectionnez **[!UICONTROL Fixer explicitement les dates de validité]**. Dans ce cas, les dates limites de diffusion et de validité permettent également de définir l’heure. L’heure actuelle est utilisée par défaut, mais vous pouvez la modifier directement dans le champ de saisie.

**[!UICONTROL Limite de validité des ressources]** est utilisé pour les ressources téléchargées, principalement pour la page miroir et les images. Les ressources de cette page ont une durée de validité limitée (afin d’économiser de l’espace disque). Au-delà de cette limite, ces ressources ne sont plus disponibles.

![](assets/delivery-settings-validity.png)

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

En savoir plus sur la période de validité des diffusions dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=fr#validity-period){target="_blank"}.

### Gestion de la page miroir {#mirror}

La page miroir est une page HTML accessible en ligne via un navigateur web et dont le contenu est identique à celui de l’email. Par défaut, la page miroir est générée si le lien est inséré dans le contenu de l’email.

Outre le mode par défaut, les options disponibles sont les suivantes :

* **[!UICONTROL Forcer la génération de la page miroir]**: utilisez ce mode pour générer la page miroir même si aucun lien vers la page miroir n&#39;est inséré dans la diffusion.
* **[!UICONTROL Ne pas générer de page miroir]**: utilisez ce mode pour éviter de générer une page miroir, même si le lien est présent dans la diffusion.
* **[!UICONTROL Génère une page miroir accessible à l’aide de l’identifiant du message uniquement]**: lorsque le lien de la page miroir n&#39;est pas présent dans le contenu de l&#39;email, utilisez cette option pour permettre l&#39;accès au contenu de la page miroir, dans la fenêtre du log de diffusion, depuis la console cliente.


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
>abstract="La période de validité définit la durée d’activation du tracking sur les URL des messages."

**[!UICONTROL Tracking]** Les paramètres sont définis dans la section correspondante. Les options possibles sont les suivantes :

**[!UICONTROL Limite de validité du suivi]**: utilisez cette option pour modifier la durée d’activation du tracking sur les URL.

**[!UICONTROL URL de substitution des URL expirées]**: utilisez cette option pour saisir une URL vers une page web de secours : elle est affichée une fois le tracking expiré.

## Paramètres de BAT {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Définir les paramètres du BAT pour la diffusion"
>abstract="Sélectionnez les paramètres d&#39;exclusion et personnalisez le libellé des BAT."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

Vous pouvez définir les paramètres d’exclusion dans cette section. Les options disponibles sont les suivantes :

* ****[!UICONTROL Conserver les doublons]**** permet d&#39;autoriser plusieurs diffusions vers des destinataires répondant à plusieurs critères de ciblage.

* L’option **[!UICONTROL Conserver les adresses placées sur la liste bloquée]** permet de tenir à l’écart de la cible les profils qui ne sont plus ciblés par la diffusion, par exemple après une désinscription (opt-out).

* L’option **[!UICONTROL Conserver les adresses placées en quarantaine]** permet de tenir à l’écart de la cible les profils dont l’adresse ne répond pas.

Vous pouvez également personnaliser l’étiquette des BAT :

* Utilisez l’option **[!UICONTROL Conserver le code diffusion pour le BAT]** pour associer au BAT le même code diffusion que celui défini pour la diffusion à laquelle il se rapporte.

* Par défaut, le sujet du BAT est précédé du préfixe &#39;BAT #&#39;, où # est le numéro du BAT. Vous pouvez modifier ce préfixe dans le champ **[!UICONTROL Préfixe de libellé]**.