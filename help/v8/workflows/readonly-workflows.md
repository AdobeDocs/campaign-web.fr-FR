---
audience: end-user
title: À propos des workflows en lecture seule
description: Découvrez pourquoi les workflows sont en mode lecture seule.
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 100%

---

# À propos des workflows en lecture seule {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Ce workflow est en lecture seule."
>abstract="Vous ne pouvez pas modifier ce workflow en raison de vos droits ou du type du workflow."

Certains workflows sont en lecture seule. Les workflows techniques natifs sont toujours en lecture seule, mais cette restriction peut également être appliquée à d’autres types de workflows.

Les personnes utilisant Campaign peuvent avoir un accès restreint aux données d’Adobe Campaign. L’équipe d’administration de Campaign peut leur accorder le droit d’afficher certaines fonctionnalités, mais pas de les modifier. Les autorisations d’utilisation sur les données sont essentielles pour assurer la sécurité des données et des processus. En savoir plus sur la gestion des autorisations de Campaign dans [cette section](../get-started/permissions.md).

Lorsqu’un workflow est en mode lecture seule :

* La mention **[!UICONTROL Lecture seule]** apparaît à côté du bouton **[!UICONTROL Paramètres]**.
* Les boutons d’action ne sont pas accessibles.

![Interface de workflow en lecture seule affichant le bouton des paramètres et les boutons d’action désactivés.](assets/readonly-workflow.png){zoomable="yes"}

Il est impossible de modifier quoi que ce soit dans un workflow en lecture seule. Il est impossible de modifier les paramètres des activités.

![Interface du planificateur en mode lecture seule, affichant les options de paramètres désactivés.](assets/scheduler-readonly.png){zoomable="yes"}

Le workflow ne peut pas être supprimé.

![Interface affichant des droits restreints pour la suppression de workflows.](assets/readonly-rights.png){zoomable="yes"}

## Types de workflows en lecture seule {#readonly-workflow-types}

Selon le type de workflow, le mode lecture seule peut varier.

### Les workflows de campagne {#readonly-campaign-wf}

Dans le cas d’un workflow de campagne en lecture seule, l’utilisateur ou l’utilisatrice ne peut pas accéder au bouton de surveillance.

![Interface de workflow d’une campagne en mode lecture seule, affichant les options de surveillance désactivées.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Workflows techniques {#readonly-tech-wf}

Les workflows techniques natifs sont en lecture seule pour toutes les personnes utilisant Campaign, même pour l’équipe d’administration. L’utilisateur ou l’utilisatrice peut toutefois les mettre en **pause** ou les **arrêter** si nécessaire. Ce sont les seules actions autorisées.

![Interface de workflow technique en mode lecture seule, affichant les options permettant de suspendre ou d’arrêter les workflows.](assets/readonly-technical-workflow.png){zoomable="yes"}

En savoir plus sur les workflows techniques dans [cette section](https://experienceleague.adobe.com/fr/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).