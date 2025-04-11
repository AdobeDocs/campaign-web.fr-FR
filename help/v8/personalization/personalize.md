---
title: Personnaliser votre contenu dans Campaign
description: Découvrir comment personnaliser votre contenu dans Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 42%

---

# Personnaliser votre contenu {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="Ajouter la date actuelle"
>abstract="Ce menu fournit des fonctions liées à la mise en forme des dates que vous pouvez utiliser pour personnaliser votre contenu."

La personnalisation du contenu de la diffusion est une fonctionnalité clé qui vous permet d’adapter les messages à chaque personne destinataire, rendant ainsi la communication plus pertinente et attrayante.

Dans Adobe Campaign, en utilisant des [données de profil](#data-personalization) telles que le nom, l’emplacement ou les interactions passées du profil, ainsi que des [variables spécifiques de votre diffusion](#variables-personalization), vous personnalisez de manière dynamique des éléments tels que du texte, des images et des offres dans votre communication.

La personnalisation de la diffusion améliore l’expérience utilisateur et les taux d’engagement, ce qui entraîne une conversion et une satisfaction client plus élevées.

## Utiliser des données de profil pour la personnalisation {#data-personalization}

Vous personnalisez n’importe quelle diffusion avec des données de profil à l’aide de l’éditeur d’expression, accessible dans les champs de l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]**, comme l’objet, les liens d’e-mail et les composants de contenu texte/bouton. [Découvrez comment accéder à l’éditeur d’expression](gs-personalization.md/#access).

### Syntaxe de la personnalisation {#syntax}

Les balises de personnalisation suivent une syntaxe spécifique : `<%= table.field %>`. Par exemple, pour insérer le nom de la personne destinataire dans le tableau des destinataires, utilisez la syntaxe `<%= recipient.lastName %>`.

Au cours du processus de préparation de la diffusion, Adobe Campaign interprète ces balises et les remplace par les valeurs de champ correspondantes pour chaque destinataire. Vous pouvez afficher le remplacement réel en simulant votre contenu.

Lors du chargement de contacts depuis un fichier externe pour une diffusion e-mail autonome, tous les champs du fichier d’entrée peuvent être personnalisés. La syntaxe est la suivante : `<%= dataSource.field %>`.

### Ajouter des balises de personnalisation {#add}

Pour ajouter des balises de personnalisation dans une diffusion, procédez comme suit :

1. Ouvrez l’éditeur d’expression à l’aide de l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]**, accessible à partir des champs de modification de type texte, tels que l’objet ou le corps du SMS. [Découvrez comment accéder à l’éditeur d’expression](gs-personalization.md/#access).

   ![Capture d’écran montrant comment accéder à la boîte de dialogue de personnalisation](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. L’éditeur d’expression s’ouvre. Les champs de personnalisation disponibles dans la base de données d’Adobe Campaign sont organisés en plusieurs menus dans la partie gauche de l’écran :

   ![Capture d’écran affichant le menu du champ de personnalisation](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menu | Description |
   |------|-------------|
   | ![Icône du menu de l’application Abonnés](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Le menu **[!UICONTROL Application des abonnées et abonnés]** répertorie les champs liés aux abonnées et abonnés d’une application, tels que le terminal utilisé ou le système d’exploitation. *Ce menu est disponible uniquement pour les notifications push.* |
   | ![ Icône du menu Destinataires ](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Le menu **[!UICONTROL Destinataire]** répertorie les champs définis dans le tableau des destinataires, tels que les noms, âges ou adresses des destinataires. Lors du [chargement des contacts depuis un fichier externe](../audience/file-audience.md) pour une diffusion e-mail autonome, ce menu répertorie tous les champs disponibles dans le fichier d’entrée. |
   | ![Icône du menu Message](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Le menu **[!UICONTROL Message]** répertorie les champs liés aux logs de diffusion, y compris tous les messages envoyés aux destinataires ou aux appareils sur tous les canaux, comme la date du dernier événement avec un destinataire donné. |
   | ![ Icône du menu Diffusion ](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Le menu **[!UICONTROL Diffusion]** répertorie les champs liés aux paramètres requis pour effectuer des diffusions, tels que le canal ou le libellé de la diffusion. |

   >[!NOTE]
   >
   >Par défaut, chaque menu répertorie tous les champs du tableau sélectionné (Destinataires/Message/Diffusion). Si vous souhaitez inclure des champs issus de tableaux liées au tableau sélectionné, activez l’option **[!UICONTROL Afficher les attributs avancés]** située sous la liste.

1. Pour ajouter un champ de personnalisation, positionnez-vous à l’emplacement souhaité dans votre contenu, puis cliquez sur le bouton `+` pour l’insérer.

1. Une fois que votre contenu est prêt, enregistrez-le et testez le rendu de la personnalisation en simulant votre contenu. L’exemple ci-dessous illustre la personnalisation d’un SMS avec les prénoms des destinataires.

   ![Capture d’écran affichant l’aperçu de la personnalisation SMS avec le prénom du destinataire](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![Capture d’écran affichant l’aperçu de la personnalisation SMS avec le prénom du destinataire](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Utilisation de variables pour la personnalisation {#variables-personalization}

Vous utilisez également des variables pour personnaliser votre diffusion. En savoir plus sur l’[ajout de variables à une diffusion](../advanced-settings/delivery-settings.md#variables-delivery).

Par exemple, la variable `deliveryType` est définie comme illustré ci-dessous.

![Capture d’écran affichant la définition de la variable deliveryType](assets/variables-deliveryType.png){zoomable="yes"}

Cette variable est utilisée dans le contenu de la diffusion à l’aide de l’icône **[!UICONTROL Ajouter Personalization]** et de l’`<%= variables.deliveryType %>` d’expression pour cet exemple.

![Capture d’écran montrant l’utilisation de la variable deliveryType dans la personnalisation](assets/variables-perso.png){zoomable="yes"}

Vérifiez l’utilisation de votre variable à l’aide du bouton **[!UICONTROL Simuler du contenu]**.

![Capture d’écran montrant la simulation du contenu avec la variable deliveryType](assets/variables-simulate.png){zoomable="yes"}