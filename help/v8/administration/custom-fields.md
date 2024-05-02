---
title: Champs personnalisés
description: Découvrez comment configurer des champs personnalisés
source-git-commit: 97769e885145d771685752f6367c5ea00831701d
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 8%

---

# Configuration des champs personnalisés {#custom-fields}

Les champs personnalisés sont des attributs supplémentaires ajoutés aux schémas d&#39;usine par le biais de la console Adobe Campaign. En savoir plus dans la [documentation d’Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=fr){target="_blank"}

Ces champs personnalisés sont affichés dans divers écrans, par exemple les détails d&#39;un profil ou d&#39;un profil de test.

Dans l’interface utilisateur web, vous ne pouvez pas créer de champs personnalisés, mais vous pouvez modifier leur mode d’affichage. Les modifications s’appliquent à tous les utilisateurs de Campaign.

>[!NOTE]
>
>Vous devez disposer des droits d’administrateur pour modifier les champs personnalisés.

Les champs personnalisés sont disponibles dans les schémas suivants :

* Destinataires (nms)
* Campagnes (nms)
* Diffusions (nms)
* Adresses de contrôle (nms)

Pour configurer des champs personnalisés, procédez comme suit :

1. Sous **Administration**, cliquez sur **Schémas**.

   ![](assets/custom-fields.png){zoomable=&quot;yes&quot;}

1. Recherchez le schéma souhaité, par exemple le **Destinataires (nms)** schéma.

   ![](assets/custom-fields2.png){zoomable=&quot;yes&quot;}

1. Cliquez sur le bouton **Autres actions** et sélectionnez **Modifier le détail personnalisé**.

   ![](assets/custom-fields3.png){zoomable=&quot;yes&quot;}

   La variable **Modifier le détail personnalisé** écran affiche tous les champs personnalisés et leur type.

   ![](assets/custom-fields4.png){zoomable=&quot;yes&quot;}

   Cet écran vous permet d’effectuer les actions suivantes :

   * modifiez l’ordre des différents champs à l’aide des flèches haut et bas.
   * renseignez le champ obligatoire : cochez la case **Obligatoire** de la boîte.
   * rendre le champ visible ou le masquer : cliquez sur le bouton **Visible** bouton .
   * ajoutez une condition de visibilité : cliquez sur le bouton **Visible si** et écrivez votre expression xtk à l’aide des fonctions xtk disponibles.

1. Accédez à l’écran qui affiche le champ personnalisé. Dans notre exemple, il s’agit de l’écran des détails du profil.

   ![](assets/custom-fields5.png){zoomable=&quot;yes&quot;}
