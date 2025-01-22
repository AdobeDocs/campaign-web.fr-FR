---
audience: end-user
title: À propos des workflows en lecture seule
description: Découvrez pourquoi les workflows sont en mode lecture seule.
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 58f25a6b41c89e97c0f721f4437b5245d16b3757
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 36%

---

# À propos des workflows en lecture seule {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Ce workflow est en lecture seule."
>abstract="Vous ne pouvez pas modifier ce workflow en raison de vos droits ou du type du workflow."

Certains workflows sont en lecture seule. Les workflows techniques natifs sont toujours en lecture seule, mais cette restriction peut également être activée sur d’autres types de workflows.

Les utilisateurs de Campaign peuvent avoir un accès restreint aux données d’Adobe Campaign. Un administrateur Campaign peut lui accorder le droit d&#39;afficher certaines fonctionnalités, mais pas de les modifier. Les autorisations utilisateur/utilisatrice sur les données sont essentielles pour assurer la sécurité des données et des processus. En savoir plus sur la gestion des autorisations dans Campaign dans [cette section](../get-started/permissions.md)

Lorsqu’un workflow est en mode lecture seule :

* La mention **[!UICONTROL Lecture seule]** à côté du bouton **[!UICONTROL Paramètres]**.
* Les boutons d’action ne sont pas accessibles.

![](assets/readonly-workflow.png){zoomable="yes"}

Les utilisateurs ne peuvent rien modifier dans un workflow en lecture seule. ils ne sont pas autorisés à modifier les paramètres des activités.

![](assets/scheduler-readonly.png){zoomable="yes"}

Les utilisateurs ne peuvent pas supprimer le workflow.

![](assets/readonly-rights.png){zoomable="yes"}


## Types de workflows en lecture seule {#readonly-workflow-types}

En fonction du type de workflow, le mode lecture seule peut être différent.

### Les workflows de campagne {#readonly-campaign-wf}

Dans le cas d’un workflow de campagne en lecture seule, l’utilisateur ou l’utilisatrice ne peut pas accéder au bouton de surveillance.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Workflows techniques {#readonly-tech-wf}

Les workflows techniques natifs sont en lecture seule pour tous les utilisateurs de Campaign, même pour l&#39;administrateur. Cependant, les utilisateurs peuvent les **mettre en pause** ou **arrêter** si nécessaire. Ce sont les seules actions autorisées.

![](assets/readonly-technical-workflow.png){zoomable="yes"}

En savoir plus sur les workflows techniques dans [cette section](https://experienceleague.adobe.com/fr/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)
