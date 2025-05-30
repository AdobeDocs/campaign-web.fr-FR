---
audience: end-user
title: Créer des workflows à l’aide d’Adobe Campaign Web
description: Découvrez comment créer des workflows à l’aide d’Adobe Campaign Web.
exl-id: 0c8e2158-518c-4620-9971-00ed2eccdd4f
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 100%

---

# Orchestrer les activités {#orchestrate}

Une fois que vous avez [créé un workflow](create-workflow.md), à partir du menu de workflow ou au sein d’une campagne, vous pouvez commencer à orchestrer les différentes tâches qu’il exécutera. Pour ce faire, une zone de travail visuelle dédiée vous permet de créer un diagramme de workflow. Dans ce diagramme, vous pouvez ajouter différentes activités et les enchaîner dans un ordre séquentiel.

## Ajouter des activités {#add}

À ce stade de la configuration, le diagramme comporte une icône de démarrage, qui représente le début de votre workflow. Pour ajouter votre première activité, cliquez sur le bouton **+** associé à l’icône de démarrage.

La liste des activités pouvant être ajoutées au diagramme s’affiche. Les activités disponibles dépendent de votre position dans le diagramme de workflow. Par exemple, lorsque vous ajoutez votre première activité pour démarrer votre workflow, vous pouvez cibler une audience, fractionner le chemin du workflow ou définir une activité **Attente** pour retarder l’exécution du workflow. Après une activité **Créer une audience**, vous pouvez affiner votre cible avec des activités de ciblage, envoyer une diffusion à votre audience avec des activités de canal ou organiser le processus du workflow avec des activités de contrôle de flux.

![Icône de démarrage du workflow et options d’activité](assets/workflow-start.png){zoomable="yes"}

Une fois qu’une activité a été ajoutée au diagramme, un volet s’affiche à droite. Il vous permet de configurer l’activité nouvellement ajoutée avec des paramètres spécifiques. Des informations détaillées sur la configuration de chacune des activités sont disponibles dans [cette section](activities/about-activities.md).

![Panneau de configuration des activités](assets/workflow-configure-activities.png){zoomable="yes"}

Répétez ce processus pour ajouter autant d’activités que vous le souhaitez en fonction des tâches que votre workflow exécute. Vous pouvez également insérer une nouvelle activité entre deux activités. Pour ce faire, cliquez sur le bouton **+** sur la transition entre les activités, puis sélectionnez l’activité souhaitée et configurez-la dans le volet de droite.

Pour supprimer une activité, sélectionnez-la dans la zone de travail et cliquez sur l’icône **Supprimer** dans les propriétés de l’activité.

>[!TIP]
>
>Vous pouvez personnaliser le nom des transitions entre chaque activité. Pour ce faire, sélectionnez la transition et modifiez son libellé dans le volet de droite.

## Barre d’outils {#toolbar}

La barre d’outils située dans le coin supérieur droit de la zone de travail fournit des options permettant de manipuler facilement les activités et de naviguer dans la zone de travail :

* **Mode de sélection multiple** : sélectionnez plusieurs activités pour les supprimer toutes en même temps ou pour les copier et les coller. Consultez [cette section](#copy).
* **Faire pivoter** : retournez la zone de travail verticalement.
* **Ajuster à l’écran** : adaptez le niveau de zoom de la zone de travail à votre écran.
* **Zoom arrière**/**Zoom avant** : effectuez un zoom arrière ou avant dans la zone de travail.
* **Afficher la carte** : ouvre un instantané de la zone de travail indiquant où vous vous trouvez.

![Options de la barre d’outils pour la zone de travail du workflow](assets/workflow-toolbar.png){zoomable="yes"}{width="50%"}

## Gérer des activités {#manage}

Lors de l’ajout d’activités, des boutons d’action sont disponibles dans le panneau des propriétés, vous permettant d’effectuer plusieurs opérations.

![Boutons d’action d’activité](assets/activity-action.png){zoomable="yes"}

Vous pouvez ainsi :

* **Supprimer** l’activité à partir de la zone de travail.
* **Désactivez/activez** l’activité. Lorsque le workflow est exécuté, les activités désactivées et les activités qui suivent sur le même chemin ne sont pas exécutées et le workflow est arrêté.
* **Mettez en pause/Reprenez** l’activité. Lorsque le workflow est exécuté, il s’arrête quand l’activité est en pause. La tâche correspondante, ainsi que toutes les suivantes dans le même chemin, ne sont pas exécutées.
* **Copiez** l’activité. Consultez [cette section](#copy).
* **Déplacez** une activité et tous ses nœuds enfant vers une autre transition. Consultez [cette section](#move).
* Accédez aux **Options d’exécution** de l’activité.
* Accédez aux **Journaux et tâches** de l’activité.

Plusieurs activités de **Ciblage**, telles que **Combiner** ou **Déduplication**, vous permettent de traiter la population restante et de l’inclure dans une transition de sortie supplémentaire. Par exemple, si vous utilisez une activité **Partage**, le complément est constitué de la population qui ne correspond à aucun des sous-ensembles définis précédemment. Pour utiliser cette fonctionnalité, activez l’option **Générer le complément**.

![Partager l’activité avec l’option complémentaire](assets/workflow-split-complement.png)

## Déplacer ou copier des activités {#move-copy}

### Activités de copier-coller {#copy}

Vous pouvez copier des activités de workflow et les coller dans n’importe quel workflow. Le workflow de destination peut se trouver dans un autre onglet du navigateur.

Pour copier des activités, vous avez deux possibilités :

* Copier une activité à l’aide du bouton d’action.

  ![Bouton Copier une seule activité](assets/workflow-copy.png){zoomable="yes"}{width="70%"}

* Copier plusieurs activités à l’aide du bouton de la barre d’outils.

  ![Bouton Copier plusieurs activités](assets/workflow-copy-2.png){zoomable="yes"}{width="70%"}

Pour coller les activités copiées, cliquez sur le bouton **+** sur une transition et sélectionnez « Coller l’activité X ».

![Option Coller les activités copiées](assets/workflow-copy-3.png){zoomable="yes"}{width="50%"}

### Déplacer des activités et leurs nœuds enfant {#move}

Journey Optimizer vous permet de déplacer une activité, ainsi que l’ensemble du contenu de ses nœuds enfant (y compris toutes les transitions et activités qu’elle contient), à la fin d’une autre transition au sein du même workflow.

Ce processus déconnecte l’activité et tout ce qui se trouve dans sa transition sortante de l’emplacement initial, en la déplaçant vers la nouvelle transition cible.

Pour déplacer une activité, procédez comme suit :

1. Sélectionnez l’activité que vous souhaitez déplacer.
1. Dans le volet des propriétés de l’activité, cliquez sur le bouton **Déplacer**.
1. Sélectionnez la transition où vous souhaitez placer l’activité et sa transition sortante, puis confirmez.

![Déplacer l’activité et les nœuds enfants](assets/activity-move.png)

## Options d’exécution {#execution}

Toutes les activités permettent de gérer les options d’exécution. Sélectionnez une activité et cliquez sur le bouton **Options d’exécution**. Vous pouvez ainsi définir le mode d’exécution et le comportement de l’activité en cas d’erreur.

![Panneau Options d’exécution](assets/workflow-execution-options.png){zoomable="yes"}{width="70%"}

### Propriétés

Le champ **Exécution** vous permet de définir l&#39;action à effectuer au moment du démarrage de la tâche.

Le champ **Durée d’exécution maximum** vous permet d’indiquer une durée de type « 30 s » ou « 1 h ». Si l’activité n’est pas terminée une fois la durée écoulée, une alerte est déclenchée, ce qui n’a par ailleurs aucun impact sur le fonctionnement du workflow.

Le champ **Fuseau horaire** vous permet de sélectionner le fuseau horaire de l’activité. Adobe Campaign gère les décalages horaires entre plusieurs pays sur par la même instance. La configuration appliquée est paramétrée lors de la création de l’instance.

Le champ **Affinité** vous permet de forcer l’exécution d’un workflow ou d’une activité de workflow sur une machine en particulier. Pour cela, vous devez définir une ou plusieurs affinités au niveau du workflow ou de l’activité concernée.

Le champ **Comportement** vous permet de définir la marche à suivre en cas de tâches asynchrones.

### Gestion des erreurs

Le champ **En cas d’erreur** vous permet de définir l’action à effectuer si l’activité rencontre une erreur.

### Script d’initialisation

Ce **script d’initialisation** vous permet d’initialiser des variables ou de modifier des propriétés d’activité. Cliquez sur le bouton **Modifier le code** et saisissez l’extrait de code à exécuter. Le script est appelé lors de l’exécution de l’activité. Consultez la section relative aux [variables d’événement](../workflows/event-variables.md).

## Exemple {#example}

Voici un exemple de workflow permettant d’envoyer un e-mail à l’ensemble de la clientèle (autres que les clientes et clients VIP) qui s’intéresse aux machines à café.

![Exemple de diagramme de workflow](assets/workflow-example.png){zoomable="yes"}

Pour y parvenir, les activités suivantes ont été ajoutées :

* une activité **[!UICONTROL Branchement]** qui divise le workflow en trois chemins (un pour chaque ensemble de clients et clientes)
* des activités **[!UICONTROL Créer une audience]** destinées à cibler les trois ensembles de clients et clientes :
   * les clients et clientes disposant d’une adresse e-mail
   * les clientes et clients appartenant à l’audience préexistante « Intéressés par la ou les machines à café »
   * les clientes et clients appartenant à l’audience préexistante « VIP ou récompense »
* une activité **[!UICONTROL Combiner]** qui regroupe les clients et clientes disposant d’une adresse e-mail et ceux ou celles intéressés par les machines à café
* une activité **[!UICONTROL Combiner]** qui exclut les clients et clientes VIP
* une activité **[!UICONTROL Diffusion e-mail]** qui envoie un e-mail aux clients et clientes correspondants

Une fois le workflow terminé, ajoutez l’activité **[!UICONTROL Fin]** à la fin du diagramme. Cette activité permet d’illustrer la fin d’un workflow et n’a aucun impact fonctionnel sur celui-ci.

Une fois le diagramme de workflow conçu, exécutez-le et suivez la progression de ses différentes tâches. [Découvrez comment démarrer un workflow et surveiller son exécution.](start-monitor-workflows.md)