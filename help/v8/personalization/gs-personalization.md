---
title: Comment rendre votre contenu dynamique ?
description: Découvrez comment rendre votre contenu dynamique grâce à la personnalisation et au contenu conditionnel.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 91%

---

# Comment rendre votre contenu dynamique ? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personnalisation"
>abstract="L’éditeur d’expression vous permet de sélectionner, d&#39;organiser, de personnaliser et de valider toutes les données afin de créer une expérience personnalisée pour votre contenu. Vous pouvez personnaliser vos messages pour chaque destinataire en exploitant les données de son profil, et créer un contenu conditionnel afin d&#39;adapter votre message à chaque destinataire et uniquement afficher le contenu pertinent."

En tant que spécialiste marketing, il est essentiel de cibler les clientes et clients qui s’intéressent véritablement à vos offres et de les impliquer grâce à un contenu efficace et pertinent. Étant donné la diversité des destinataires que vous rencontrez, la création de plusieurs éléments de contenu marketing pour séduire différentes personnes peut représenter une perte de temps et d’argent. C’est là que le contenu dynamique entre en jeu.

Les fonctionnalités de contenu dynamique web d’Adobe Campaign vous permettent de personnaliser votre contenu en fonction des informations que vous avez collectées sur vos personnes destinataires. L’utilisation de contenu dynamique vous permet de vous assurer que vos efforts marketing sont plus pertinents, en évitant de commercialiser des produits ou services indésirables ou inutiles. Cette approche rend votre contenu plus attrayant et augmente la probabilité qu’il soit lu. De plus, elle vous permet de personnaliser votre contenu, donnant aux destinataires l’impression de recevoir des informations d’une personne plutôt que d’une machine.

## Comment rendre votre contenu dynamique ? {#make-content-dyn}

Vous pouvez rendre le contenu de votre message dynamique en insérant des éléments JavaScript dans l’éditeur d’expression web de Campaign. Lors de l’envoi d’un message, ces expressions sont interprétées par Adobe Campaign afin de diffuser le contenu correct à vos destinataires :

* **Personnalisez vos messages** pour chaque destinataire en utilisant des données de profil telles que son prénom, ses centres d’intérêt, son lieu de vie, ses achats, etc. Vous pouvez sélectionner n’importe quel champ disponible dans la base depuis l’éditeur de personnalisation associé au ou à la destinataire, au message ou à la diffusion. Ces attributs de personnalisation peuvent être insérés dans l’objet ou dans le corps de vos messages. La syntaxe suivante insère la ville du ou de la destinataire dans votre contenu : &lt;%= recipient.location.city %>.

  ![](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Créez du contenu conditionnel** pour adapter vos diffusions à chaque destinataire et afficher uniquement le contenu pertinent pour une cliente ou un client donné(e) en fonction des informations dont vous disposez à son sujet. Vous pouvez ainsi afficher des blocs de texte et/ou des images spécifiques en fonction de conditions. Par exemple, adaptez une bannière d’e-mail en fonction de l’abonnement des destinataires à un service spécifique.

  ![](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

## Accéder à l’éditeur d’expression {#access}

Adobe Campaign Web fournit un éditeur d’expression dans lequel vous pouvez sélectionner, organiser, personnaliser et valider toutes les données afin de créer une expérience personnalisée pour votre contenu. L’éditeur d’expression est disponible pour tous les canaux, dans tous les champs dotés de l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]**, par exemple le champ de l’objet ou les liens d’e-mail et les composants de contenu texte/bouton.

Voici quelques exemples d’accès à l’éditeur d’expression en fonction du contenu que vous souhaitez rendre dynamique :

* *Accès à l’éditeur d’expression à partir du champ Nom de l’expéditeur*

  ![](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *Accès à l’éditeur d’expression à partir d’un composant de texte d’e-mail*

  ![](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Accès à l’éditeur d’expression à partir d’un lien dans un e-mail*

  ![](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>Outre l’éditeur d’expression, vous pouvez également utiliser un créateur de contenu conditionnel dédié lors de la conception d’un e-mail. [Découvrez comment créer du contenu conditionnel dans les e-mails](conditions.md).
