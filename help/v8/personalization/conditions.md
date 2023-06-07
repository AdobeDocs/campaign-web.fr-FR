---
title: Créer du contenu conditionnel
description: Découvrez comment personnaliser votre contenu dans l’interface utilisateur web d’Adobe Campaign.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 8%

---

# Création de contenu conditionnel{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Créer du contenu conditionnel"
>abstract="Créez un contenu conditionnel pour définir une personnalisation dynamique basée sur le profil du destinataire, en remplaçant automatiquement les blocs de texte et les images lorsque certaines conditions sont remplies. Cette fonctionnalité permet d’augmenter le nombre de campagnes et de proposer des expériences hautement ciblées et personnalisées à votre audience."

Le contenu conditionnel est une puissante fonctionnalité qui permet de créer une personnalisation dynamique basée sur le profil du destinataire, en remplaçant automatiquement les blocs de texte et les images lorsque certaines conditions sont remplies. Cette fonctionnalité permet d’augmenter le nombre de campagnes et de proposer des expériences hautement ciblées et personnalisées à votre audience.

En configurant des champs de contenu conditionnel, vous pouvez créer une personnalisation dynamique avancée basée sur le profil du destinataire, par exemple. Les blocs de texte, liens, objet et/ou images sont remplacés dans le contenu du message lorsqu’une condition particulière est remplie. Par exemple, vous pouvez afficher &quot;M.&quot; ou &quot;Mme&quot; en fonction de la valeur du champ Genre dans la base de données Adobe Campaign, ou inclure un lien différent en fonction de la langue préférée du destinataire.

## Syntaxe de la personnalisation{#perso-syntax}

## Utilisation de conditions dans l’éditeur de personnalisation{#condition-perso-editor}

Pour définir un contenu conditionnel pour une diffusion :

1. Ouvrez une diffusion et éditez son contenu.
1. Cliquez sur le bouton **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]** par exemple, pour SMS, à droite du champ Message .

   ![](assets/open-perso-editor-sms.png)

1. Dans l’éditeur de personnalisation, accédez à **[!UICONTROL Fonctions d’assistance]**.
1. Cliquez sur l’icône &quot;+&quot; en regard de l’option **If** fonction . La ligne suivante est ajoutée à l&#39;écran central :
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Remplacer `<FIELD>` par un champ de personnalisation. Par exemple, la société du destinataire : `recipient.company`.
1. Remplacer `<VALUE>` par la valeur à satisfaire. Par exemple, `ADOBE`.

## Exemple : ligne d&#39;objet du SMS conditionnel{#condition-subject-line}

Pour créer un objet conditionnel pour un SMS, procédez comme suit :

1. Ouvrez une diffusion et éditez son contenu.
1. Cliquez sur l’icône Ouvrir la boîte de dialogue de personnalisation située à droite de l’objet.
1. Dans l’éditeur de personnalisation, accédez à


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
