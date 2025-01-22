---
audience: end-user
title: À propos des workflows en lecture seule
description: Découvrez pourquoi les workflows sont en mode lecture seule.
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 62d4733b9dc6bf3edf06d172069b5f8b1d0ee4a7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 100%

---

# À propos des workflows en lecture seule {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Ce workflow est en lecture seule."
>abstract="Vous ne pouvez pas modifier ce workflow en raison de vos droits ou du type du workflow."

Certains workflows peuvent être en lecture seule. Dans ce cas, ils s’affichent comme suit :

- La mention **[!UICONTROL Lecture seule]** à côté du bouton **[!UICONTROL Paramètres]**.
- Les boutons d’action ne sont pas accessibles.

![](assets/readonly-workflow.png){zoomable="yes"}

Vous ne pouvez rien modifier dans un workflow en lecture seule. Vous n’êtes pas autorisé à modifier les paramètres des activités.


![](assets/scheduler-readonly.png){zoomable="yes"}


Vous n’avez pas non plus les droits nécessaires pour supprimer le workflow.

![](assets/readonly-rights.png){zoomable="yes"}

## Finalité des workflows en lecture seule

Le mode Lecture seule est destiné aux utilisateurs et utilisatrices qui ne disposent pas de droits d’accès et d’autorisation pour modifier ces workflows. [En savoir plus ici](../get-started/permissions.md)

Un utilisateur ou une utilisatrice de Campaign peut avoir des restrictions sur les données qui lui sont accessibles dans Adobe Campaign. L’administrateur ou l’administratrice peut lui offrir la possibilité d’afficher certaines fonctionnalités mais de ne pas les utiliser.

## Types de workflows en lecture seule

En fonction du type de workflow, le mode lecture seule peut être différent.

### Les workflows de campagne

Dans le cas d’un workflow de campagne en lecture seule, l’utilisateur ou l’utilisatrice ne peut pas accéder au bouton de surveillance.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Workflows techniques

Les workflows techniques sont en lecture seule pour les utilisateurs et utilisatrices de Campaign.
Les workflows techniques intégrés sont en lecture seule pour toutes les personnes, même pour celles disposant d’un accès administratif. L’utilisateur ou l’utilisatrice peut toutefois les mettre en **pause** ou les **arrêter** si nécessaire. Ce sont les seules actions autorisées. [En savoir plus ici](https://experienceleague.adobe.com/fr/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}
