---
title: Utilisation de pages JavaScript dynamiques
description: Découvrez comment utiliser des pages JavaScript dynamiques.
exl-id: b7de9f55-2aef-4ba9-a2a1-e9ca15deacfb
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2df9759bb21eae0630bcbe9130a1a20b165e8cca
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 11%

---

# Utilisation de pages JavaScript dynamiques {#dynamic-javascript-pages}

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_list"
>title="Pages dynamiques JavaScript"
>abstract="Les pages Dynamic JavaScript (JSSP) vous permettent de créer des pages côté serveur, qui génèrent du contenu dynamique lors d’un accès via une URL, tel que des API personnalisées, des exports ou une logique d’application web. Dans cette liste, vous pouvez créer, modifier, dupliquer ou supprimer une page de JavaScript dynamique."

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_create"
>title="Créer une page dynamique JavaScript"
>abstract="Définissez un espace de noms, un nom et un libellé pour votre page de JavaScript dynamique, puis écrivez son contenu à l’aide du code JavaScript. Une fois créés, l’espace de noms et le nom ne peuvent pas être modifiés."

## À propos des pages Dynamic JavaScript {#about}

Les pages Dynamic JavaScript (JSSP) vous permettent de créer des pages côté serveur, qui génèrent du contenu dynamique lors d’un accès via une URL, tel que des API personnalisées, des exports ou une logique d’application web. Ces pages sont stockées dans le menu **[!UICONTROL Administration]** > **[!UICONTROL Pages Dynamic JavaScript]** dans le volet de navigation de gauche.

![Interface de liste des pages Dynamic JavaScript affichant les options disponibles](assets/dynamic-javascript-pages.png)

À partir de la liste des pages Dynamic JavaScript, vous pouvez :

* **Dupliquer ou supprimer une page** : cliquez sur le bouton représentant des points de suspension et sélectionnez l’action souhaitée.
* **Modifier une page** : cliquez sur le nom d’une page pour ouvrir ses propriétés, apporter vos modifications et les enregistrer.
* **Création d’une page Dynamic JavaScript** : cliquez sur le bouton **[!UICONTROL Créer une page Dynamic JavaScript]**.

<!--
>[!NOTE]
>
>In the Campaign console, dynamic JavaScript pages are available under **[!UICONTROL Administration]** > **[!UICONTROL Configuration]** > **[!UICONTROL Dynamic JavaScript pages]**. Although the menu location differs from the Web user interface, the list is identical and operates like a mirror.
-->

## Création d’une page JavaScript dynamique {#create}

Pour créer une page JavaScript dynamique, procédez comme suit :

1. Accédez au menu **[!UICONTROL Pages Dynamic JavaScript]**, puis cliquez sur le bouton **[!UICONTROL Créer une page Dynamic JavaScript]**.

1. Définissez les propriétés de la page :

   * **[!UICONTROL Espace de noms]** : spécifiez l’espace de noms pertinent pour vos ressources personnalisées. Par défaut, l’espace de noms est « cus », mais il peut varier en fonction de votre implémentation.
   * **[!UICONTROL Name]** : identifiant unique utilisé pour référencer la page.
   * **[!UICONTROL Libellé]** : libellé descriptif affiché dans la liste des pages Dynamic JavaScript.

   ![Interface de création de page Dynamic JavaScript affichant les champs d’espace de noms, de nom et de libellé](assets/dynamic-javascript-pages2.png)

   >[!NOTE]
   >
   >Une fois créés, les champs **[!UICONTROL Espace de noms]** et **[!UICONTROL Nom]** ne peuvent plus être modifiés. Pour apporter des modifications, dupliquez la page et mettez-la à jour si nécessaire.

1. Cliquez sur le bouton **[!UICONTROL Créer un code]** pour définir le contenu de la page, puis écrivez votre code JSSP à l’aide de directives `<%@ page %>` et d’appels `NL.require()` pour charger les bibliothèques principales.

   ![Éditeur de code de page Dynamic JavaScript](assets/dynamic-javascript-pages4.png)

1. Cliquez sur **[!UICONTROL Confirmer]** pour enregistrer votre code.

1. Lorsque votre page Dynamic JavaScript est prête, cliquez sur **[!UICONTROL Créer]**. La page est désormais accessible à partir d’une URL créée à partir de son espace de noms et de son nom, au format `https://<your-instance>/<namespace>/<name>`. Par exemple, une page nommée `recipientAPI.jssp` dans l’espace de noms `cus` est accessible sur `https://<your-instance>/cus/recipientAPI.jssp`.

Pour plus d’informations sur les fonctions JavaScript réutilisables, voir [Utilisation des codes JavaScript](javascript-codes.md).
