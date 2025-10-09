---
audience: end-user
title: Configurer une diffusion multilingue
description: Découvrez comment configurer une diffusion multilingue
source-git-commit: d8d78f97cdf99e67c59827a91c54851b1cbbeb16
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 18%

---

# Configurer une diffusion multilingue {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Ajouter des langues"
>abstract="Dans cet onglet, vous trouverez une liste des langues dans lesquelles la diffusion doit être envoyée. Vous pouvez ajouter d’autres langues en cliquant sur le bouton Ajouter une langue, ou en dupliquant une autre langue via cet onglet."

Dans l’interface utilisateur web de Campaign, vous pouvez configurer vos diffusions en tant que multilingues, ce qui vous permet d’envoyer des messages en fonction de la langue préférée d’un profil. Lorsqu’aucune préférence n’est définie, le message est envoyé dans la langue par défaut.

Dans une diffusion multilingue, la gestion des langues repose sur des variantes. Chaque variante représente une langue. Lors de la création de la diffusion, vous pouvez ajouter plusieurs variantes linguistiques pour correspondre au nombre de langues requises dans votre message. Vous pouvez également modifier la langue par défaut à tout moment après l’ajout de ces variantes.

La fonctionnalité multilingue est actuellement disponible pour les e-mails, les notifications push, les messages transactionnels et les SMS.

>[!AVAILABILITY]
>
>Les notifications push, messages transactionnels et SMS multilingues ne sont disponibles que pour un ensemble d’organisations (disponibilité limitée) et seront déployés dans le monde entier dans une prochaine version. Votre serveur doit être mis à niveau vers la version 8.8.2 ou ultérieure.

Pour configurer des diffusions multilingues, procédez comme suit :

1. Ajouter une variante de langue, [en savoir plus](#add-variant)
1. Définir le contenu pour chaque variante, [en savoir plus](#define-content)
1. Gérer les variantes de langue, [en savoir plus](#manage-variant)

## Ajouter une variante linguistique{#add-variant}

Pour créer des variantes linguistiques, procédez comme suit :

1. Dans le tableau de bord de la diffusion, cliquez sur l&#39;icône en forme de crayon pour accéder à l&#39;écran d&#39;édition du contenu de la diffusion, puis cliquez sur **[!UICONTROL Ajouter une langue]**.

   >[!IMPORTANT]
   >
   >Le bouton **[!UICONTROL Ajouter une langue]** n’est disponible que si la dimension cible contient le schéma **Langue**. Pour en savoir plus sur les schémas et les dimensions cibles, consultez la [documentation détaillée](../audience/targeting-dimensions.md).

   ![](assets/edit-content_2.png){zoomable="yes"}

1. Dans le menu déroulant **Ajouter une langue**, sélectionnez la langue à ajouter, puis confirmez.

   La première langue que vous ajoutez est automatiquement définie par défaut et le contenu existant devient la version par défaut. Lorsque d’autres langues sont ajoutées, leur contenu est initialement copié à partir de la langue par défaut.

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >Les langues disponibles dans cette liste dépendent des valeurs définies par l’attribut **Language** (valeurs telles que : system, user, dbenum, etc.). En savoir plus sur la gestion des énumérations dans cette [section](../administration/enumerations.md).

1. Répétez cette opération pour ajouter d’autres langues. Le panneau **[!UICONTROL Langues]**, sur la gauche, affiche la liste des langues sélectionnées, le nombre de langues et la langue par défaut.

   Par exemple, si vous avez choisi l’anglais, le français et le suédois, vous pouvez voir ces 3 langues comme illustré ci-dessous :

   ![](assets/edit-content_9.png){zoomable="yes"}

   Pour savoir comment gérer les variantes de langue, consultez cette [section](#manage-variant).

## Définition du contenu pour chaque variante{#define-content}

Une fois les langues définies, définissez le contenu de la diffusion pour chaque langue.

1. Dans l’écran d’édition du contenu de la diffusion, sélectionnez une langue dans le panneau **[!UICONTROL Langues]** à gauche.

   ![](assets/edit-content_11.png){zoomable="yes"}

1. Définissez le contenu de votre message pour cette langue. En savoir plus dans cette [section](../msg/create-deliveries.md).

1. Répétez cette opération pour chaque langue.

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

Pour prévisualiser la diffusion, cliquez sur le bouton **[!UICONTROL Simuler du contenu]** et sélectionnez des profils. Assurez-vous que le contenu approprié s’affiche pour chaque profil.

![](assets/edit-content_5.png){zoomable="yes"}

## Gestion des variantes linguistiques{#manage-variant}

Dans le panneau de gauche, toutes les informations sur les variantes linguistiques s’affichent. Pour supprimer toutes les langues, cliquez sur le bouton de développement, puis sur **[!UICONTROL Supprimer toutes les variantes]**.

![](assets/edit-content_13.png){zoomable="yes"}

Dans la liste des variantes de langue, vous pouvez effectuer les actions suivantes :

* **Modifier** : modifiez la langue tout en conservant le contenu associé.
* **Définir comme langue par défaut** : définissez la langue comme langue par défaut. Lorsqu’aucun langage n’est défini pour un profil, le message est envoyé dans la langue par défaut.
* **Dupliquer** : dupliquez le contenu défini pour cette langue et choisissez une autre variante.
* **Supprimer** : supprimez la variante et son contenu associé.

![](assets/edit-content_13-sms.png){zoomable="yes"}

