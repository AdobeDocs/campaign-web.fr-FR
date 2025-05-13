---
audience: end-user
title: Utiliser l’activité de workflow Test
description: Découvrez comment utiliser l’activité de workflow Test
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: ht
source-wordcount: '382'
ht-degree: 100%

---


# Test {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="Activité Test"
>abstract="L’activité **Test** est une activité de **contrôle de flux**. Il permet d’activer des transitions en fonction de conditions spécifiées."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="Conditions"
>abstract="L’activité **Test** peut avoir plusieurs transitions sortantes. Lors de l’exécution du workflow, chaque condition est testée de manière séquentielle jusqu’à ce que l’une d’elles soit remplie. Si aucune des conditions n’est remplie, le workflow se poursuit sur la voie de la **[!UICONTROL condition par défaut]**. Si aucune condition par défaut n’est activée, le workflow s’arrête à ce stade."

L’activité **Test** est une activité de **contrôle de flux**. Il permet d’activer des transitions en fonction de conditions spécifiées.

## Configurer l’activité Test {#test-configuration}

Pour configurer l’activité **Test**, procédez comme suit :

1. Ajoutez une activité **Test** à votre workflow.

1. Par défaut, l’activité **[!UICONTROL Test]** présente un test booléen simple. Si la condition définie dans la transition « True » est remplie, cette transition sera activée. Sinon, une transition « False » par défaut sera activée.

1. Pour configurer la condition associée à une transition, cliquez sur l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]**. Utilisez l’éditeur d’expression pour définir les règles d’activation de cette transition. Vous pouvez également utiliser des variables d’événement, des conditions et des fonctions de date/heure. [Découvrez comment travailler avec les variables d’événement et l’éditeur d’expression](../event-variables.md).

   En outre, modifiez le champ **[!UICONTROL Libellé]** pour personnaliser le nom de la transition dans la zone de travail du workflow.

   ![Configuration par défaut de l’activité Test](../assets/workflow-test-default.png)

1. Ajoutez plusieurs transitions de sortie à une activité **[!UICONTROL Test]**. Pour ce faire, cliquez sur le bouton **[!UICONTROL Ajouter une condition]** et configurez le libellé et la condition associée pour chaque transition.

1. Lors de l’exécution du workflow, chaque condition est testée de manière séquentielle jusqu’à ce que l’une d’elles soit remplie. Si aucune des conditions n’est remplie, le workflow se poursuit sur la voie de la **[!UICONTROL condition par défaut]**. Si aucune condition par défaut n’est activée, le workflow s’arrête à ce stade.

## Exemple {#example}

Dans cet exemple, différentes transitions sont activées en fonction du nombre de profils ciblés par une activité **[!UICONTROL Créer une audience]** :
* Si plus de 10 000 profils sont ciblés, un e-mail est envoyé.
* Pour 1 000 à 10 000 profils, un SMS est envoyé.
* Si les profils ciblés sont inférieurs à 1 000, ils sont dirigés vers une transition « Ne pas contacter ».

![Exemple de transitions d’activité Test](../assets/workflow-test-example.png)

Pour ce faire, la variable d’événement `vars.recCount` est utilisée dans les conditions « E-mail » et « SMS » pour comptabiliser le nombre de profils ciblés et activer la transition appropriée.

![Exemple de configuration d’une activité de test](../assets/workflow-test-example-config.png)
