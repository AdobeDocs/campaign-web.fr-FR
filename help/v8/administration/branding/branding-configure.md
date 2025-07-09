---
title: Branding
description: Découvrez comment configurer votre marque
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 2b4a818c819ae598d5555c1a2d64447b0793b5b8
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 47%

---

# Configuration des marques {#branding-configure}

>[!IMPORTANT]
>
>Les marques ne peuvent pas être créées ni modifiées par des utilisateurs finaux : ces opérations doivent être effectuées par l&#39;administrateur technique Adobe Campaign. Pour toute demande, contactez l&#39;Assistance clientèle Adobe.

Dans Adobe Campaign V8, les marques se trouvent dans le menu **[!UICONTROL Administration > Plateforme > Branding]**.

Une **[!UICONTROL marque]** est définie par les caractéristiques suivantes :

* Une **[!UICONTROL identité]** qui permet d&#39;identifier et de personnaliser votre marque. Cette section contient les champs suivants :

   * **[!UICONTROL Libellé]**, visible dans l&#39;interface
   * **[!UICONTROL ID]**
   * **[!UICONTROL Nom de la marque]**
   * **[!UICONTROL URL du site web]** et **[!UICONTROL Libellé du site web]** de la marque
   * **[!UICONTROL Logo de la marque]**

  ![](assets/branding_1.png)

* **[!UICONTROL Paramètres d&#39;en-tête des emails envoyés]** qui permettent de personnaliser les informations qui seront visibles par les destinataires de vos campagnes. Cette section contient les champs suivants :

   * **[!UICONTROL Expéditeur (adresse email)]** avec l&#39;adresse email de la marque
   * **[!UICONTROL Expéditeur (nom)]** avec le nom de la marque
   * **[!UICONTROL Répondre à (adresse email)]** avec l&#39;adresse email de réponse destinée au client
   * **[!UICONTROL Répondre à (nom)]** avec le nom de la marque
   * **[!UICONTROL Erreur (adresse email)]** avec l&#39;adresse email à utiliser en cas d&#39;erreur

  >[!IMPORTANT]
  >
  >Après avoir mis à jour les paramètres d&#39;en-tête des emails, si le nom et l&#39;adresse email de l&#39;expéditeur ne sont pas modifiés dans l&#39;email créé à partir du modèle, vérifiez les paramètres avancés de ce dernier.

  ![](assets/branding_2.png)

* **[!UICONTROL Configurations de marque]** définit les serveurs utilisés pour le suivi également pour l’accès aux pages de destination. Cette section contient les champs suivants :

   * **[!UICONTROL Sous-domaine de marque]** fait référence à l’URL de sous-domaine désignée spécifique à cette marque, demandée pour délégation à partir d’Adobe.

  Notez que la configuration des serveurs de suivi, de mise en miroir et d’application est stockée dans des comptes externes distincts associés au routage. Ces paramètres sont appliqués pendant l’approvisionnement et ne doivent pas être modifiés. Pour afficher les URL, accédez à l’onglet **[!UICONTROL Préfixes de branding]** à partir de votre compte externe.

  ![](assets/branding_3.png)

* Le menu **[!UICONTROL Configurations des URL de tracking]** vous permet d’améliorer le tracking des URL en définissant des paramètres supplémentaires pour l’intégration aux outils d’analyse web tels qu’Adobe Analytics et Google Analytics.

  Utilisez le menu **[!UICONTROL Paramètres d’URL supplémentaires]** pour créer des paramètres supplémentaires en tant que paires clé-valeur, ainsi que leurs conditions d’application. Chaque nom de paramètre doit être unique et non vide, et chaque valeur de paramètre doit être non vide. La condition d&#39;applicabilité peut être vide, mais aucune de ces valeurs ne peut inclure de balises JST.

  Ces paramètres seront appliqués aux URL suivies correspondant à tout nom de domaine spécifié dans la **[!UICONTROL Liste des noms de domaine]**, qui peut inclure des expressions régulières.
