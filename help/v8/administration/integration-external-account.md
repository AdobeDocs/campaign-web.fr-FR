---
title: Gérer un compte externe
description: Découvrir comment configurer des comptes externes
exl-id: 99648377-112b-428a-8faf-5268d730f19a
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: ht
source-wordcount: '206'
ht-degree: 100%

---

# Comptes externes d’intégration de solution Adobe {#integration-external-account}

Selon le type de compte externe d’intégration de solution Adobe que vous avez sélectionné, suivez les étapes ci-dessous pour configurer les paramètres de connexion et de compte afin d’assurer une intégration transparente aux services Adobe.

## Adobe Experience Cloud

Pour vous connecter à la console Adobe Campaign à l’aide d’un Adobe ID, vous devez configurer le compte externe Adobe Experience Cloud (MAC).

![Capture d’écran montrant les champs de configuration du compte externe Adobe Experience Cloud MAC.](assets/external-MAC.png)

Pour configurer le compte externe **[!UICONTROL Adobe Experience Cloud]**, renseignez les champs suivants :

* **[!UICONTROL Serveurs IMS]**

  URL de votre serveur IMS. Assurez-vous que les instances de test et de production pointent sur le même point de terminaison de production IMS.

* **[!UICONTROL Scope IMS]**

  Les périmètres définis ici doivent être un sous-ensemble de ceux provisionnés par IMS.

* **[!UICONTROL Identifiant du client IMS]**

  ID de votre client IMS.

* **[!UICONTROL Secret client IMS]**

  Informations d’identification de votre secret client IMS.

* **[!UICONTROL Serveur de rappel]**

  URL d’accès à votre instance Adobe Campaign.

* **[!UICONTROL Identifiant de l&#39;organisation IMS]**

  Identifiant de votre organisation. Pour trouver l’ID de votre organisation, reportez-vous à [cette page](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=fr){target=_blank}.

* **[!UICONTROL Masque de correspondance]**

  Syntaxe qui permettra la synchronisation des noms de configuration dans Enterprise Dashboard avec les groupes dans Adobe Campaign.

* **[!UICONTROL Serveur]**

  URL de votre instance Adobe Experience Cloud.

* **[!UICONTROL Tenant]**

  Nom de votre tenant Adobe Experience Cloud.
