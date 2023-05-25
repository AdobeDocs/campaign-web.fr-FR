---
audience: end-user
title: Prise en main des messages et des diffusions dans Campaign v8 Web
description: Découvrez comment utiliser les diffusions et envoyer des messages à l’aide de Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 14e9ef2a45a1c7a2c8e089c536abd950cdb1b0a3
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 38%

---

# Prise en main des messages dans Campaign Web {#gs-messages}

Avec Adobe Campaign, vous pouvez envoyer des campagnes cross-canal, y compris des emails, des SMS et des notifications push, et mesurer leur efficacité à l’aide de différents rapports dédiés. Ces messages sont conçus et envoyés par le biais de diffusions, et peuvent être personnalisés pour chaque destinataire. Ces diffusions peuvent être autonomes ou incluses dans le cadre d&#39;une campagne marketing.

Adobe Campaign v8 propose les canaux de diffusion suivants :

* **Canal e-mail** : les diffusions e-mail permettent d&#39;envoyer des e-mails personnalisés à la population cible. Découvrez comment créer et envoyer un email dans [cette page](../email/create-email.md).

* **Canal SMS**: les diffusions sur canaux mobiles permettent d&#39;envoyer des SMS personnalisés à la population cible.  Découvrez comment créer et envoyer des SMS dans [cette page](../sms/create-sms.md).

* **Canal applications mobiles** : les diffusions d&#39;applications mobiles vous permettent d&#39;envoyer des notifications aux systèmes iOS et Android.  Découvrez comment créer et envoyer des notifications push dans [cette page](../push/gs-push.md).

## Création dʼune diffusion

Vous pouvez créer des diffusions autonomes à partir du **Diffusion** ou créer des diffusions dans le cadre d&#39;une campagne marketing.

>[!BEGINTABS]

>[!TAB Créer une diffusion autonome]

Pour créer une diffusion autonome, procédez comme suit :

1. Accédez au **[!UICONTROL Diffusions]** dans le volet de navigation de gauche, puis cliquez sur l’icône **[!UICONTROL Créer une diffusion]** bouton .
1. Sélectionnez un canal pour la diffusion. En savoir plus sur les canaux de diffusion et la définition d&#39;un contenu de diffusion dans les sections suivantes :

   * [Canal email](../email/create-email.md)
   * [Canal des notifications push](../push/gs-push.md)
   * [Canal SMS](../sms/create-sms.md)

1. Définissez l&#39;audience de la diffusion, pour la cible principale et la population témoin. En savoir plus sur les audiences dans [cette section](../audience/about-audiences.md).
1. Définition du contenu du message.
1. (Facultatif) Définissez le calendrier de remise. Si aucune planification n’est définie, les messages sont envoyés immédiatement après avoir cliqué sur la variable **[!UICONTROL Envoyer]** bouton .
1. Cliquez sur le bouton  **[!UICONTROL Vérifier et envoyer]** pour vérifier vos paramètres.
1. Utilisez la variable  **[!UICONTROL Simulation du contenu]** pour tester votre diffusion et vos paramètres de personnalisation. En savoir plus sur la simulation des messages dans [cette section](../preview-test/preview-test.md).
1. Cliquez sur le bouton  **[!UICONTROL Préparer]** pour calculer la population cible et générer les messages. L’étape de préparation peut prendre quelques minutes. Une fois la préparation terminée, les messages sont prêts à être envoyés. En cas d’erreur, accédez à la **Journaux** pour vérifier les alertes et les avertissements.
1. Vérifiez les résultats, puis cliquez sur le bouton  **[!UICONTROL Envoyer]** pour commencer à envoyer des messages.
1. Une fois les messages envoyés, accédez à la section Rapports pour accéder aux mesures clés. En savoir plus sur les rapports de diffusion dans [cette section](../reporting/reports.md).

>[!TAB Créer une diffusion dans une campagne]

Pour créer une diffusion dans une opération, procédez comme suit :

1. Créez une campagne ou ouvrez une campagne existante.

Pour plus d&#39;informations sur le paramétrage d&#39;une opération,

>[!ENDTABS]


## Choisir comment envoyer vos messages{#gs-send-msg}

Une fois votre message créé et son contenu conçu et testé, vous pouvez choisir la façon dont vous souhaitez l&#39;envoyer.

Campaign offre un ensemble de fonctionnalités pour :

* Envoyer les messages manuellement à la cible principale

* Envoyer des messages associés à une [campagne marketing](../campaigns/gs-campaigns.md)

* Envoyer des messages via un [workflow](../workflows/channel-activities.md)


## Ajouter de la personnalisation{#personalization}

Les messages diffusés par Adobe Campaign peuvent être personnalisés de différentes façons


## Logs de tracking et de diffusion{#gs-tracking-logs}

La surveillance de vos diffusions après leur envoi est une étape clé pour vous assurer que vos campagnes marketing sont efficaces et atteignent vos clients. Vous pouvez ainsi surveiller une diffusion après son envoi et comprendre la gestion des diffusions en échec et des quarantaines.
