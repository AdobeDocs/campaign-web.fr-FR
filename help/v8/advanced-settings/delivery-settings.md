---
audience: end-user
title: Configuration des paramètres de diffusion
description: Découvrez comment configurer les paramètres de diffusion dans Campaign Web
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: e4e1a7eee0f4a48366e711feb2a8bd107f3320bd
workflow-type: tm+mt
source-wordcount: '2417'
ht-degree: 79%

---


# Configurer les paramètres de diffusion {#del-settings}

Les paramètres de diffusion sont **paramètres de diffusion technique** qui sont définis dans le modèle de diffusion. Elles peuvent être surchargées pour chaque diffusion. Ces paramètres sont disponibles à partir du **Paramètres** est disponible lors de l&#39;édition d&#39;une diffusion ou d&#39;un modèle de diffusion.

>[!CAUTION]
>
>Ces paramètres sont décrits uniquement à titre d’information. Certains dépendent de votre configuration et de vos autorisations. Ils ne doivent pas être modifiées dans cette version du produit.

## Paramètres de typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="Les règles de typologie permettent aux spécialistes marketing de normaliser les pratiques commerciales de l’ensemble des diffusions. Une typologie est un ensemble de règles de typologie qui permet de contrôler, filtrer et prioriser l’envoi des diffusions. Les profils qui correspondent à des critères dans une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation. La création de typologies et de règles de typologie s’effectue dans la console cliente Campaign."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Paramètres de typologie de la diffusion"
>abstract="Les règles de typologie permettent aux spécialistes marketing de normaliser les pratiques commerciales de l’ensemble des diffusions. Une typologie est un ensemble de règles de typologie qui permet de contrôler, filtrer et prioriser l’envoi des diffusions. Les profils qui correspondent à des critères dans une règle de typologie sont exclus des audiences de diffusion lors de la phase de préparation. La création de typologies et de règles de typologie s’effectue dans la console cliente Campaign."

Les typologies sont des ensembles de **règles de typologie** qui sont exécutées pendant la phase de préparation afin d’appliquer facilement plusieurs règles de filtrage en même temps à une diffusion. Elles permettent aux personnes spécialisées dans le marketing de normaliser les pratiques commerciales pour toutes les diffusions, en contrôlant, filtrant et gérant la priorité de l’envoi des diffusions.

Lors de l’association d’une typologie à un message ou à un modèle de message, les règles de typologie incluses dans la typologie sont exécutées pour vérifier la validité du message durant la préparation de celui-ci. Les profils qui correspondent à des critères inclus dans une règle de typologie sont exclus des audiences de diffusion.

Les typologies vous permettent de vous assurer que vos diffusions contiennent toujours certains éléments (comme un lien de désinscription ou une ligne d’objet) ou des règles de filtrage pour exclure des groupes de votre cible prévue (comme les clients qui se désabonnent, les concurrents ou les clients qui ne sont pas fidèles).

![](assets/delivery-settings-typology.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>La création de typologies et de règles de typologie s’effectue dans la console cliente Campaign. En savoir plus sur les règles de pression et la configuration de la gestion de la fatigue dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html?lang=fr){target="_blank"}.

### Paramètres de pression {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Paramètres de pression de la diffusion"
>abstract="Le poids des diffusions permet d’identifier les diffusions prioritaires dans le cadre de la gestion de la fatigue. Les messages dont le poids est le plus élevé sont prioritaires."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Poids de la diffusion"
>abstract="Le poids des diffusions permet d’identifier les diffusions prioritaires dans le cadre de la gestion de la pression. Les messages dont le poids est le plus important sont prioritaires."

Dans cette section, les paramètres de pression vous permettent de définir un **seuil** pour configurer des règles de gestion d’usure, qui est le nombre maximal de messages pouvant être envoyés à un profil sur une période donnée.

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
>La configuration de la gestion de l’usure s’effectue dans la console cliente Campaign. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=fr){target="_blank"}.

### Paramètres de capacité {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Paramètres de capacité de la diffusion"
>abstract="Avant de diffuser des messages, utilisez les règles de capacité pour vous assurer que votre organisation peut traiter notamment la diffusion, les messages entrants que la diffusion peut générer et le nombre d’appels à passer pour contacter les personnes abonnées, par exemple. La définition des règles de capacité s’effectue dans la console Adobe Campaign v8. Dans cet écran, sélectionnez une règle associée au canal."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Importance du destinataire"
>abstract="L’importance du destinataire est une formule utilisée pour déterminer les destinataires qui sont conservés lorsque les règles de typologie de capacité sont dépassées."

Dans cette section, vous pouvez sélectionner une règle de capacité définie dans la console Adobe Campaign v8. Cette règle est associée au canal.

Le champ **[!UICONTROL Importance de la personne destinataire]** est une formule utilisée pour déterminer les personnes destinataires conservées lorsque les règles de typologie de capacité sont dépassées.

>[!NOTE]
>
>La configuration de règles de typologie s’effectue dans la console cliente Campaign. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=fr){target="_blank"}.

## Paramètres de l’audience {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Paramètres d’audience de la diffusion"
>abstract="Sélectionnez un **mapping de ciblage** parmi ceux disponibles. Les mappings de ciblage sont définis dans la console Adobe Campaign v8. Vous pouvez également définir les paramètres d’exclusion de la diffusion."

Dans cette section, vous pouvez sélectionner un **mapping de ciblage** parmi ceux disponibles. Les mappings de ciblage sont définis dans la console Adobe Campaign v8. Le mapping de ciblage est le type de données qu’une opération traite. Il permet de définir la population ciblée : destinataires, bénéficiaires de contrats, opérateurs, abonnés, etc. [En savoir plus sur les mappings de ciblage](../audience/targeting-dimensions.md).

Dans le champ **[!UICONTROL Exclusion]**, vous pouvez choisir d’exclure des personnes destinataires qui ne souhaitent plus être contactées ou qui sont mises en quarantaine. [En savoir plus](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=fr){target="_blank"}

## Diffusion {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Paramètres de diffusion de la diffusion"
>abstract="Les paramètres de diffusion sont des paramètres techniques qui s’appliquent à votre diffusion. Vous pouvez modifier les modes de diffusion et de routine, activer E-mail Cci, envoyer par vagues et choisir le format des e-mails envoyés. Ces options sont limitées aux personnes expertes uniquement."

Les paramètres de **[!UICONTROL Diffusion]** sont des paramètres techniques qui s’appliquent à votre diffusion.

![](assets/delivery-settings-delivery.png){zoomable=&quot;yes&quot;}

L&#39;intégration **[!UICONTROL Routage]** le compte externe est fourni par défaut. Elle contient les paramètres techniques qui permettent à l’application d’envoyer des diffusions.

Vous pouvez définir les paramètres d’**[!UICONTROL Envoi]** ci-dessous.

* **[!UICONTROL Priorité de diffusion]** : utilisez cette option pour modifier l’ordre d’envoi de vos diffusions en configurant leur niveau de priorité : normal, élevé ou faible.

* **[!UICONTROL Nombre de messages groupés]** : utilisez cette option pour définir le nombre de messages regroupés dans un même package d’envoi XML. Si le paramètre est défini sur 0, les messages sont automatiquement regroupés. La taille du paquet est définie par le calcul `<delivery size>/1024`, avec un minimum de 8 messages et un maximum de 256 messages par package.

  >[!IMPORTANT]
  >
  >Lorsque vous créez la diffusion en dupliquant une diffusion existante, vous réinitialisez également ce paramètre.

* **[!UICONTROL Tester la diffusion SMTP]** (canal email) : cette option est utilisée pour tester l’envoi via SMTP. L&#39;email est traité jusqu&#39;à la connexion au serveur SMTP, mais n&#39;est pas envoyé : pour chaque destinataire de l&#39;email, Campaign se connecte au serveur du fournisseur SMTP, exécute la commande SMTP RCPT TO et ferme la connexion avant la commande SMTP DATA.

* **[!UICONTROL Email Cci]** (canal email) : cette option est utilisée pour stocker les emails sur un système externe via Cci en ajoutant simplement une adresse email en Cci à votre cible de message. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/email-bcc.html){target="_blank"}.

Dans la section **[!UICONTROL Définition de vague]**, sélectionnez l’option **[!UICONTROL Envoyer en plusieurs vagues]** pour augmenter progressivement le volume envoyé par vagues. Cela évitera que les emails soient marqués comme spam ou pour limiter le nombre de messages par jour. Grâce aux vagues, vous pouvez répartir les envois en plusieurs lots au lieu d’envoyer de gros volumes de messages en même temps. [En savoir plus](send-using-waves.md)

Pour les emails, vous pouvez également modifier la variable **[!UICONTROL Formats de messagerie]** des messages envoyés, comme décrit ci-dessous.

* **[!UICONTROL Utiliser les préférences des destinataires]** (mode par défaut) : le format des emails est défini en fonction des données stockées dans le profil du destinataire. Si un destinataire souhaite recevoir des emails dans un format donné, il s&#39;agit du format envoyé. Si le champ n’est pas renseigné, un email multipart-alternative est envoyé (voir ci-dessous).

* **[!UICONTROL Laisser le client de messagerie du destinataire choisir le format le plus approprié]**: l&#39;email contient les deux formats : texte et HTML. Le format affiché à la réception dépend de la configuration du logiciel de messagerie du destinataire (multipart-alternative).

  >[!IMPORTANT]
  >
  >Cette option inclut les deux versions du document. Cela a donc un impact sur le taux de diffusion, car la taille de l&#39;email est supérieure.

* **[!UICONTROL Envoyer tous les messages au format texte]**: l&#39;email est envoyé au format texte. Le format HTML ne sera pas envoyé, mais utilisé pour la page miroir uniquement lorsque le destinataire clique sur l&#39;email.

## Web Analytics {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Paramètres Web Analytics de la diffusion"
>abstract="Sélectionnez un compte Web Analytics. La configuration de ce compte s’effectue dans la console cliente Campaign. Vous pouvez également définir les balises partagées avec l’outil d’analyse que vous utilisez."

Dans cette section, vous pouvez sélectionner un compte Web Analytics. La configuration de ce compte s’effectue dans la console cliente Campaign.

Vous pouvez également définir les balises partagées avec l’outil d’analyse que vous utilisez.

>[!NOTE]
>
>La configuration des fonctionnalités Web analytics s’effectue dans la console cliente Campaign. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=fr#external-account-ac){target="_blank"}.

## Reprises {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Nombre maximal de reprises"
>abstract="Si un message est en échec en raison d’une erreur temporaire, les reprises sont effectuées jusqu’à la fin de la durée de diffusion."

<!--Currently not visible in UI > ??-->

Les messages temporairement non diffusés en raison d’une erreur Soft ou Ignoré font l’objet d’une nouvelle tentative automatique. Par défaut, cinq reprises sont planifiées le premier jour de l’envoi, avec un intervalle minimum d’une heure, réparties sur les 24 heures de la journée.

## Validation (canal email) {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Mode d’approbation de la diffusion"
>abstract="Sélectionnez le mode d’approbation. Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Mode d’approbation des diffusions"
>abstract="Sélectionnez le mode d’approbation des diffusions à partir de ce modèle. Si des avertissements sont générés lors de la préparation de la diffusion, vous pouvez configurer celle-ci pour définir si elle doit quand même être exécutée ou non."

Si des avertissements sont générés lors de la préparation d&#39;une diffusion email, vous pouvez configurer la diffusion pour définir si elle doit être exécutée ou non. Par défaut, l&#39;utilisateur doit confirmer l&#39;envoi des emails à la fin de la phase d&#39;analyse : c&#39;est-à-dire **manuel** validation.

Vous pouvez sélectionner un autre mode de validation dans le champ correspondant. Les modes disponibles sont les suivants :

* **[!UICONTROL Manuel]** : à la fin de la phase d’analyse, l’utilisateur ou l’utilisatrice doit confirmer la diffusion pour commencer l’envoi.
* **[!UICONTROL Semi-automatique]** : les envois démarrent automatiquement si la phase d’analyse ne génère aucun message d’avertissement.
* **[!UICONTROL Automatique]** : les envois démarrent automatiquement à la fin de la phase d’analyse, quel qu’en soit le résultat.

## Validité {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Validité des paramètres"
>abstract="Le champ **Durée de diffusion** permet de saisir la limite pour des reprises globales de diffusion. Concrètement, Adobe Campaign diffuse les messages à partir de la date de lancement. Puis, pour les messages en erreur uniquement, des reprises régulières et paramétrables sont effectuées tant que la limite de diffusion n’est pas atteinte.<br>Le champ **Limite de validité des ressources** est utilisé pour les ressources chargées, comme la page miroir ou les images. Au-delà de cette limite, ces ressources ne sont plus disponibles."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Limite de validité des ressources"
>abstract="Le champ **Limite de validité des ressources** est utilisé pour les ressources chargées, comme la page miroir ou les images. Ces ressources sont valides pour une durée limitée. Une fois la limite atteinte, elles ne sont plus disponibles."

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

La **[!UICONTROL Limite de validité des ressources]** est utilisée pour les ressources chargées, principalement pour la page miroir et les images. Les ressources de cette page ont une durée de validité limitée (afin d’économiser de l’espace disque). Au-delà de cette limite, ces ressources ne sont plus disponibles.

![](assets/delivery-settings-validity.png){zoomable=&quot;yes&quot;}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

En savoir plus sur la période de validité des diffusions dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=fr#validity-period){target="_blank"}.

### Gestion des pages miroir (canal email) {#mirror}

La page miroir est une page HTML accessible en ligne via un navigateur web et dont le contenu est identique à celui de l’e-mail. Par défaut, la page miroir est générée si le lien est inséré dans le contenu de l&#39;email.

Outre le mode par défaut, les options disponibles sont les suivantes :

* **[!UICONTROL Forcer la génération de la page miroir]**: utilisez ce mode pour générer la page miroir même si aucun lien vers la page miroir n&#39;est inséré dans l&#39;email.
* **[!UICONTROL Ne pas générer de page miroir]**: utilisez ce mode pour éviter de générer une page miroir, même si le lien est présent dans l&#39;email.
* **[!UICONTROL Générer une page miroir accessible via l’identifiant du message uniquement]** : ce mode permet d’accéder au contenu de la page miroir, dans la fenêtre du log de diffusion de la console cliente, lorsque l’e-mail ne contient pas de lien vers la page miroir.

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

Les paramètres de **[!UICONTROL Tracking]** sont définis dans la section correspondante. Les options possibles sont les suivantes :

* **[!UICONTROL Limite de validité du tracking]** : utilisez cette option pour définir la durée d’activation du tracking sur les URL.
* **[!UICONTROL URL de substitution des URL arrivées à expiration]** : utilisez cette option pour renseigner une URL vers une page web de secours. Celle-ci s’affiche après l’expiration du tracking.

## Paramètres de BAT {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Configurer les paramètres de BAT pour la diffusion"
>abstract="Sélectionnez les paramètres d’exclusion et personnalisez le libellé des BAT."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

Vous pouvez définir les paramètres d’exclusion dans cette section. Les options disponibles sont les suivantes :

* **[!UICONTROL Conserver les doublons]** vous permet d’autoriser plusieurs diffusions vers des personnes destinataires répondant à plusieurs critères de ciblage.
* L’option **[!UICONTROL Conserver les adresses placées sur la liste bloquée]** permet de tenir à l’écart de la cible les profils qui ne sont plus ciblés par la diffusion, par exemple après une désinscription (opt-out).
* L’option **[!UICONTROL Conserver les adresses placées en quarantaine]** permet de tenir à l’écart de la cible les profils dont l’adresse ne répond pas.

Vous pouvez également personnaliser le libellé des BAT :

* Utilisez l’option **[!UICONTROL Conserver le code diffusion pour le BAT]** pour associer au BAT le même code de diffusion que celui défini pour la diffusion à laquelle il se rapporte.
* Par défaut, l’objet du BAT est précédé du préfixe « BAT # », où # correspond au numéro du BAT. Vous pouvez modifier ce préfixe dans le champ **[!UICONTROL Préfixe de libellé]**.
