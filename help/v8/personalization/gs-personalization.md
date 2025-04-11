---
title: Comment rendre votre contenu dynamique ?
description: Découvrez comment rendre votre contenu dynamique à l’aide de la personnalisation et du contenu conditionnel.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 47%

---

# Comment rendre votre contenu dynamique ? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personnalisation"
>abstract="L’éditeur de personnalisation vous permet de sélectionner, d’organiser, de personnaliser et de valider toutes les données afin de créer une expérience personnalisée pour votre contenu. Vous pouvez personnaliser vos messages pour chaque destinataire en utilisant les données de son profil, et créer un contenu conditionnel afin d’adapter votre message à chaque destinataire et uniquement afficher le contenu pertinent."

En tant que spécialiste marketing, il est essentiel de cibler les clients qui sont véritablement intéressés par vos offres et de les impliquer en fournissant du contenu efficace et pertinent. Étant donné la diversité des destinataires que vous rencontrez, la création de plusieurs éléments de contenu marketing pour séduire différentes personnes peut représenter une perte de temps et d’argent. C’est là que le contenu dynamique devient essentiel.

Les fonctionnalités de contenu dynamique d’Adobe Campaign Web vous permettent de personnaliser votre contenu en fonction des informations que vous avez collectées sur vos destinataires. L’utilisation de contenu dynamique vous permet de vous assurer que vos efforts marketing sont plus pertinents, en évitant de commercialiser des produits ou services indésirables ou inutiles. Cette approche rend votre contenu plus attrayant et augmente la probabilité qu’il soit lu. De plus, elle vous permet de personnaliser votre contenu, donnant aux destinataires l’impression de recevoir des informations d’une personne plutôt que d’une machine.

## Comment rendre votre contenu dynamique ? {#make-content-dyn}

Vous pouvez rendre le contenu de votre message dynamique en insérant des éléments JavaScript dans l’éditeur d’expression web de Campaign. Lors de l’envoi d’un message, Adobe Campaign interprète ces expressions pour diffuser le contenu correct à chacun de vos destinataires :

* **Personnalisez vos messages** pour chaque destinataire en utilisant des données de profil telles que son prénom, ses centres d’intérêt, son lieu de vie, ses achats, etc. Vous pouvez sélectionner n’importe quel champ disponible dans la base de données à partir de l’éditeur de personnalisation associé au ou à la destinataire, au message ou à la diffusion. Ces attributs de personnalisation peuvent être insérés dans l’objet ou dans le corps de vos messages. La syntaxe suivante insère la ville du destinataire dans votre contenu : `<%= recipient.location.city %>`.

  [Description : exemple d’insertion de la ville du destinataire dans la ligne d’objet à l’aide d’attributs de personnalisation.](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Créez du contenu conditionnel** pour adapter vos diffusions à chaque destinataire et afficher uniquement le contenu pertinent pour une cliente ou un client donné(e) en fonction des informations dont vous disposez à son sujet. Vous pouvez ainsi afficher des blocs de texte et/ou des images spécifiques en fonction de conditions. Par exemple, adaptez une bannière d’e-mail en fonction de l’abonnement des destinataires à un service spécifique.

  [Description : exemple de contenu conditionnel dans une bannière d’e-mail en fonction de l’abonnement du destinataire.](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [Découvrir cette fonctionnalité en vidéo](#video)

## Accéder à l’éditeur d’expression {#access}

Adobe Campaign Web fournit un éditeur d’expression dans lequel vous pouvez sélectionner, organiser, personnaliser et valider toutes les données afin de créer une expérience personnalisée pour votre contenu. L’éditeur d’expression est disponible pour tous les canaux, dans chaque champ de l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]**, par exemple le champ de l’objet ou les liens d’e-mail et les composants de contenu texte/bouton.

Voici quelques exemples d’accès à l’éditeur d’expression en fonction du contenu que vous souhaitez rendre dynamique :

* *Accès à l’éditeur d’expression à partir du champ Nom de l’expéditeur*

  [Description : exemple d’accès à l’éditeur d’expression à partir du champ Nom de l’expéditeur ](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}.

* *Accès à l’éditeur d’expression à partir d’un composant de texte d’e-mail*

  [Description : exemple d’accès à l’éditeur d’expression à partir d’un composant de texte d’e-mail.](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Accéder à l’éditeur d’expression à partir d’un lien dans un e-mail*

  [Description : exemple d&#39;accès à l&#39;éditeur d&#39;expression à partir d&#39;un lien dans un e-mail.](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>Outre l’éditeur d’expression, vous pouvez également utiliser un créateur de contenu conditionnel dédié lors de la conception d’un e-mail. [Découvrez comment créer du contenu conditionnel dans les e-mails](conditions.md).

## Vidéo pratique {#video}

Découvrez comment rendre le contenu du message dynamique à l’aide de l’éditeur d’expression pour personnaliser votre message ou ajouter du contenu conditionnel.

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)