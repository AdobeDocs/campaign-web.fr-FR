---
audience: end-user
title: Surveiller et gérer les audiences
description: Découvrez comment surveiller et gérer les audiences dans Adobe Campaign Web
badge: label="Beta"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: ht
source-wordcount: '289'
ht-degree: 100%

---

# Surveiller et gérer les audiences {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Erreur d’audience"
>abstract="Données d’audience non disponibles Veuillez attendre la fin de l’exécution du workflow."

La liste des audiences disponibles dans Campaign Web est accessible à partir du menu **[!UICONTROL Audiences]**.

![](assets/audiences-list.png)

Les audiences peuvent provenir de plusieurs sources. Les colonnes **[!UICONTROL Origine]** indiquent l’emplacement de création d’une audience donnée :

* **[!UICONTROL Adobe Campaign]** : ces audiences sont créées dans la console Adobe Campaign V8. En savoir plus dans la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=fr){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** : ces audiences sont créées dans Adobe Experience Platform et intégrées à Campaign Web à l’aide de l’intégration des sources et destinations Adobe. Découvrez comment configurer cette intégration dans la [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=fr){target="_blank"}.

>[!NOTE]
>
>Pour utiliser les audiences Adobe Experience Platform dans Campaign, vous devez configurer l’intégration aux sources et destinations Adobe. Consultez la [documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=fr){target="_blank"}.

* **[!UICONTROL Interface utilisateur web d’Adobe Campaign]** : ces audiences sont créées à l’aide des workflows d’audience de Campaign Web. [Découvrez comment créer des audiences](create-audience.md)

Pour obtenir plus d’informations sur une audience, ouvrez-la dans la liste. Les propriétés de l’audience s’affichent, avec le nombre de profils inclus dans l’audience. Vous pouvez actualiser le nombre d’audiences à tout moment à l’aide du bouton **[!UICONTROL Calculer]**.

L’onglet **[!UICONTROL Données]** vous permet de visualiser les profils qui font partie de l’audience. Vous pouvez personnaliser cette vue en ajoutant d’autres colonnes ou en utilisant des filtres avancés pour affiner les données affichées.

![](assets/audiences-details.png)

Pour dupliquer ou supprimer une audience, cliquez sur le bouton **[!UICONTROL Plus d’action]** disponible dans la liste des audiences, en regard du nom de l’audience ou dans un écran détaillé de l’audience.
