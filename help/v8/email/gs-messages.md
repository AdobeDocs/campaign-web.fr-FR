---
audience: end-user
title: Prise en main des messages et des diffusions dans Campaign v8 Web
description: Découvrez comment utiliser les diffusions et envoyer des messages à l’aide de Campaign Web.
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: cd00fcf90283c99e4790789ab2375c3a1da0ce50
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 36%

---

# Prise en main des messages dans Campaign Web {#gs-messages}

Avec Adobe Campaign, vous pouvez envoyer des campagnes cross-canal, y compris des emails, des SMS et des notifications push, et mesurer leur efficacité à l’aide de différents rapports dédiés. Ces messages sont conçus et envoyés par le biais de diffusions, et peuvent être personnalisés pour chaque destinataire. Ces diffusions peuvent être autonomes ou incluses dans le cadre d&#39;une campagne marketing.

Adobe Campaign v8 propose les canaux de diffusion suivants :

* **Canal e-mail** : les diffusions e-mail permettent d&#39;envoyer des e-mails personnalisés à la population cible. Découvrez comment créer et envoyer un email dans [cette page](../email/create-email.md).

* **Canal SMS**: les diffusions sur canaux mobiles permettent d&#39;envoyer des SMS personnalisés à la population cible.  Découvrez comment créer et envoyer des SMS dans [cette page](../sms/create-sms.md).

* **Canal applications mobiles** : les diffusions d&#39;applications mobiles vous permettent d&#39;envoyer des notifications aux systèmes iOS et Android.  Découvrez comment créer et envoyer des notifications push dans [cette page](../push/gs-push.md).

## Création dʼune diffusion {#create-delivery}

Vous pouvez créer des diffusions autonomes à partir du **[!UICONTROL Diffusions]** dans le menu de gauche, ou créez des diffusions dans le cadre d&#39;une campagne marketing, à partir de la **[!UICONTROL Campagnes]** menu de gauche.

>[!BEGINTABS]

>[!TAB Créer une diffusion autonome]

Pour créer une diffusion autonome, procédez comme suit :

1. Accédez au **[!UICONTROL Diffusions]** dans le volet de navigation de gauche, puis cliquez sur l’icône **[!UICONTROL Créer une diffusion]** bouton .

   ![](assets/create-a-delivery.png)

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
1. Une fois les messages envoyés, accédez à la **Rapports** pour accéder aux mesures clés. En savoir plus sur les rapports de diffusion dans [cette section](../reporting/reports.md).

>[!TAB Créer une diffusion dans une campagne]

Pour créer une diffusion dans une opération, procédez comme suit :

1. Créez une campagne ou ouvrez une campagne existante. En savoir plus sur [campagnes marketing](../campaigns/gs-campaigns.md).
1. Créez un workflow ou ouvrez un workflow existant.
1. Ajout et configuration d’une **[!UICONTROL Créer une audience]** puis cliquez sur le bouton `+`bouton .

   ![](assets/add-delivery-in-wf.png)

   Le **[!UICONTROL Créer une audience]** L’activité est présentée dans la section [cette section](../workflows/targeting-activities.md).

1. Sélectionnez une activité de diffusion : **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Notification push (Android)]** ou **[!UICONTROL Notification push (iOS)]**. En savoir plus sur les activités des canaux de diffusion dans un workflow et comment définir un contenu de diffusion dans ce workflow [section](../workflows/channel-activities.md).
1. Démarrez le workflow et vérifiez les logs.

Vous pouvez également ajouter des diffusions dans une campagne sans créer de workflow. Pour ce faire, accédez à la **[!UICONTROL Diffusions]** de votre campagne, puis cliquez sur l’onglet **[!UICONTROL Créer une diffusion]** bouton .

![](assets/new-campaign-delivery.png)

Les étapes de configuration sont similaires à celles des diffusions autonomes.

Pour plus d&#39;informations sur la configuration d&#39;une opération et la gestion des diffusions qui appartiennent à une opération, reportez-vous à la section [cette section](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Ajouter de la personnalisation{#personalization}

Les messages diffusés par Adobe Campaign peuvent être personnalisés de différentes façons. [En savoir plus sur les fonctionnalités de personnalisation](../personalization/personalize.md).

Utilisez Campaign pour créer du contenu dynamique et envoyer des messages personnalisés. Vous pouvez cumuler les fonctionnalités de personnalisation afin d’améliorer vos messages et créer une expérience utilisateur personnalisée.

Vous pouvez personnaliser le contenu du message en procédant comme suit :

* Insérer des **champs de personnalisation** dynamiques.

   Les champs de personnalisation sont utilisés pour la personnalisation de premier niveau de vos messages. Vous pouvez sélectionner n’importe quel champ disponible dans la base de données de l’éditeur de personnalisation. Pour une diffusion, vous pouvez sélectionner n’importe quel champ associé au ou à la destinataire, au message ou à la diffusion. Ces attributs de personnalisation peuvent être insérés dans l’objet ou dans le corps de vos messages. [En savoir plus](../personalization/personalize.md)

* Insérer des **blocs de contenu** prédéfinis

   Campaign est fourni avec un ensemble de blocs de personnalisation qui contiennent un rendu spécifique que vous pouvez insérer dans vos diffusions. Vous pouvez par exemple ajouter un logo, un message de salutation ou un lien vers la page miroir du message. Les blocs de contenu sont disponibles à partir d’une entrée dédiée dans l’éditeur de personnalisation. [En savoir plus](../personalization/personalize.md#ootb-content-blocks)

* Créer du **contenu conditionnel**

   Configurez du contenu conditionnel et ajoutez une touche de personnalisation dynamique (basée sur le profil du ou de la destinataire, par exemple). Lorsqu’une condition est rencontrée, des blocs de texte et/ou des images sont alors insérés. [En savoir plus](../personalization/conditions.md)

* Ajouter **offres personnalisées**

   Insérez des offres personnalisées dans le contenu de votre message, en fonction de l&#39;emplacement du destinataire, de la météo actuelle ou du dernier bon de commande.


## Prévisualiser et tester vos diffusions

Une fois le contenu de votre message défini, vous pouvez le prévisualiser afin de contrôler le rendu de vos messages, et vérifier les paramètres de personnalisation avec les profils de test. [En savoir plus](../preview-test/preview-test.md)


## Logs de tracking et de diffusion{#gs-tracking-logs}

La surveillance de vos diffusions après leur envoi est une étape clé pour vous assurer que vos campagnes marketing sont efficaces et atteignent vos clients. Vous pouvez ainsi surveiller une diffusion après son envoi et comprendre la gestion des diffusions en échec et des quarantaines.

## Dupliquer une diffusion{#delivery-duplicate}

Vous pouvez créer une copie d&#39;une diffusion existante, depuis la liste de diffusion ou depuis le tableau de bord de la diffusion.

Pour dupliquer une diffusion à partir de la liste des diffusions, procédez comme suit :

1. Cliquez sur le bouton des trois points à droite, en regard du nom de la diffusion à dupliquer.
1. Sélectionner  **[!UICONTROL Dupliquer]**.
1. Confirmer la duplication : le nouveau tableau de bord des diffusions s&#39;ouvre dans l&#39;écran central.


Pour dupliquer une diffusion depuis son tableau de bord, procédez comme suit :

1. Ouvrez la diffusion et cliquez sur le bouton  **[!UICONTROL ...Plus]** dans la section supérieure de l’écran.
1. Sélectionner  **[!UICONTROL Dupliquer]**.
1. Confirmer la duplication : la nouvelle diffusion remplace la diffusion actuelle dans l&#39;écran central.

