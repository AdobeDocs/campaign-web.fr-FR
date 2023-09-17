---
audience: end-user
title: Création d'audiences
description: Découvrez comment créer des audiences dans Adobe Campaign Web
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 1%

---


# Création d&#39;audiences {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiences"
>abstract="Dans cet écran, vous pouvez créer et combiner des audiences dans une zone de travail visuelle. Ajoutez diverses activités de workflow, telles que **Partage** ou **Exclure** pour générer de nouvelles audiences affinées."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Paramètres de l’audience"
>abstract="Saisissez le nom de l’audience et les options supplémentaires, puis cliquez sur le bouton **Création d’une audience** bouton ."

Campaign Web vous permet de créer de nouvelles audiences dans un canevas de workflow visuel. Au-delà du fait de commencer à zéro pour créer une audience simple, vous pouvez également tirer parti des activités de workflow pour affiner vos audiences. Par exemple, vous pouvez regrouper plusieurs audiences en une seule, enrichir les audiences avec des attributs externes ou diviser une audience donnée en plusieurs.

Une fois que vous avez conçu votre workflow, les audiences résultantes sont automatiquement stockées dans la base de données Campaign avec les audiences existantes. Ces audiences peuvent ensuite être ciblées dans des campagnes ou des diffusions autonomes.

Les étapes principales pour créer une audience sont les suivantes :

1. Créez un workflow d’audience.
1. Configurez une activité Créer une audience pour interroger la base de données selon vos besoins.
1. Ajoutez des activités de workflow pour affiner votre audience (facultatif).
1. Configurez une activité Sauvegarde d&#39;audience .
1. Exécutez le workflow pour enregistrer la ou les audiences qui en résultent dans la base de données.


## Créer votre première audience {#create}

Pour créer une audience, procédez comme suit :

1. Accédez au **[!UICONTROL Audiences]** et cliquez sur le bouton **[!UICONTROL Création d’une audience]** situé dans le coin supérieur droit.
1. Attribuez un libellé à votre audience.
1. Développez l’objet **[!UICONTROL Options supplémentaires]** pour configurer les paramètres d’audience avancés.

   Par défaut, les audiences sont créées dans la variable **[!UICONTROL Profils et cibles]** / **[!UICONTROL Listes]** menu de l’explorateur. Vous pouvez modifier l’emplacement de stockage par défaut à l’aide du **[!UICONTROL Dossier]** champ .

   ![](assets/audiences-settings.png)

1. Une fois les paramètres d’audience configurés, cliquez sur le bouton **[!UICONTROL Création d’une audience]** bouton .

1. Un canevas de workflow s’affiche, comprenant deux activités par défaut :

   * **[!UICONTROL Créer une audience]**: point de départ de votre workflow, vous permettant de créer une audience et de l’utiliser comme base de votre workflow. [Découvrez comment configurer une activité Créer une audience](../workflows/activities/build-audience.md)

   * **[!UICONTROL Sauvegarde d’audience]**: représente la dernière étape de votre workflow, ce qui vous permet d’enregistrer les résultats en tant que nouvelle audience. [Découvrez comment configurer une activité Sauvegarde d’audience](../workflows/activities/save-audience.md)

1. Si vous souhaitez effectuer d’autres opérations après la **[!UICONTROL Créer une audience]** , ajoutez autant d’activités que nécessaire dans votre workflow. Pour plus d’informations sur la configuration des activités de workflow, reportez-vous à la section [documentation sur les workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Les activités de canal ne peuvent pas être utilisées dans les workflows d’audience.

   ![](assets/audience-creation-canvas.png)

1. Lorsque votre workflow est prêt, cliquez sur **[!UICONTROL Début]** pour l’exécuter.

1. Le workflow est enregistré dans la variable **[!UICONTROL Workflows]** tandis que la ou les audiences obtenues sont accessibles dans la **[!UICONTROL Audiences]** liste. [Découvrez comment surveiller et gérer les audiences](access-audiences.md)

## Exemple de workflow d’audience {#example}

L’exemple ci-dessous montre un workflow d’audience configuré pour cibler les clientes vivant à New York et créer deux nouvelles audiences en fonction de leur centre d’intérêt dans le matériel Yoga ou Running . Les deux audiences sont enrichies d&#39;informations supplémentaires sur les achats des clients.

AJOUTER UNE CAPTURE D’ÉCRAN

1. L&#39;activité Créer une audience cible tous les profils féminins vivant à New York.
1. L&#39;activité Enrichissement permet d&#39;enrichir l&#39;audience avec des attributs de la table Achats .
1. L&#39;activité Partage divise le workflow en deux chemins d&#39;accès en fonction des centres d&#39;intérêt des clients.
1. Les activités Sauvegarde d&#39;audience à la fin de chaque chemin d&#39;accès pour sauvegarder chaque audience dans la base de données.
