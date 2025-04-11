---
audience: end-user
title: À propos des workflows en lecture seule
description: Découvrez pourquoi les workflows sont en mode lecture seule.
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 21%

---

# À propos des workflows en lecture seule {#readonly-workflows}

>[!CONTEXTUALHELP]
>
Certains workflows sont en lecture seule. Les workflows techniques natifs sont toujours en lecture seule, mais cette restriction peut également s’appliquer à d’autres types de workflows.

Les utilisateurs de Campaign peuvent avoir un accès restreint aux données d’Adobe Campaign. Un administrateur Campaign peut lui accorder le droit d&#39;afficher certaines fonctionnalités, mais pas de les modifier. Les autorisations utilisateur/utilisatrice sur les données sont essentielles pour assurer la sécurité des données et des processus. En savoir plus sur la gestion des autorisations dans Campaign dans [cette section](../get-started/permissions.md).

Lorsqu’un workflow est en mode lecture seule :

* La mention **[!UICONTROL Lecture seule]** apparaît près du bouton **[!UICONTROL Paramètres]**.
* Les boutons d’action ne sont pas accessibles.

![Interface de workflow en lecture seule affichant le bouton des paramètres et les boutons d’action désactivés.](assets/readonly-workflow.png){zoomable="yes"}

Il est impossible de modifier quoi que ce soit dans un workflow en lecture seule. Ils ne sont pas autorisés à modifier les paramètres des activités.

![Interface du planificateur en mode lecture seule, affichant les options de paramètres désactivés.](assets/scheduler-readonly.png){zoomable="yes"}

Les utilisateurs ne peuvent pas supprimer le workflow.

![Interface affichant des droits restreints pour la suppression de workflows.](assets/readonly-rights.png){zoomable="yes"}

## Types de workflows en lecture seule {#readonly-workflow-types}

Selon le type de workflow, le mode lecture seule peut varier.

### Les workflows de campagne {#readonly-campaign-wf}

Dans un workflow de campagne en lecture seule, l’utilisateur ne peut pas accéder au bouton de surveillance.

![Interface des workflows Campaign en mode lecture seule, affichant les options de surveillance désactivées.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Workflows techniques {#readonly-tech-wf}

Les workflows techniques natifs sont en lecture seule pour tous les utilisateurs de Campaign, y compris les administrateurs. L’utilisateur ou l’utilisatrice peut toutefois les mettre en **pause** ou les **arrêter** si nécessaire. Il s’agit des seules actions autorisées.

![Interface de workflow technique en mode lecture seule, affichant les options permettant de suspendre ou d’arrêter les workflows.](assets/readonly-technical-workflow.png){zoomable="yes"}

En savoir plus sur les workflows techniques dans [cette section](https://experienceleague.adobe.com/fr/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).