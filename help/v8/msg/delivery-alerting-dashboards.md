---
audience: end-user
title: Alertes de diffusion
description: Découvrez comment utiliser les alertes de diffusion.
hidefromtoc: true
hide: true
robots: noindex
googlebot: noindex
exl-id: b91ef82b-f3e9-4704-87a2-0e3f75104572
source-git-commit: 19a7540af7502709b7eafdace038b5958e077173
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 87%

---

# Tableaux de bord des alertes de diffusion {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Tableaux de bord des alertes de diffusion"
>abstract="Les alertes de diffusion sont un système de gestion des alertes qui permet à des groupes d’utilisateurs et d’utilisatrices de recevoir automatiquement des notifications par e-mail contenant des informations sur l’exécution de leurs diffusions. Les tableaux de bord des alertes de diffusion permettent de spécifier qui recevra des alertes par e-mail, de choisir et de configurer les critères des alertes à utiliser pour envoyer ces alertes et d’accéder à l’historique de toutes les notifications envoyées."

Les tableaux de bord des alertes de diffusion permettent de spécifier qui recevra des alertes par e-mail, de choisir et de configurer les critères des alertes à utiliser pour envoyer ces alertes et d’accéder à l’historique de toutes les notifications envoyées. Ils sont accessibles à partir du menu **Alertes de diffusion** dans le volet de navigation de gauche, sous l’onglet **Tableaux de bord**.

![Capture d’écran affichant la liste des tableaux de bord des alertes dans le menu Alertes de diffusion.](assets/alerting-dashboard-list.png)

## Créer un tableau de bord de diffusion {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Créer un tableau de bord des alertes de diffusion"
>abstract="La création d’un tableau de bord des alertes de diffusion permet de spécifier qui recevra les alertes par e-mail, de choisir et de configurer les critères des alertes à utiliser pour envoyer ces alertes et d’accéder à l’historique de toutes les notifications envoyées."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Paramètres généraux des alertes de diffusion"
>abstract="Définissez les propriétés générales du tableau de bord des alertes de diffusion. Le champ **Sélectionner un groupe d’alertes** permet de spécifier le **groupe d’opérateurs et d’opératrices** qui recevra les alertes envoyées par ce tableau de bord."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Critères des alertes de diffusion"
>abstract="Dans cette section, ajoutez les critères que vous souhaitez utiliser pour envoyer des alertes à partir de ce tableau de bord. Faites votre choix parmi les critères prédéfinis ou créez vos propres critères pour répondre à des besoins spécifiques."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Paramètres des critères"
>abstract="Les critères comportent des valeurs de paramètres par défaut qui définissent la manière dont ils doivent être appliqués. Vous pouvez modifier ces valeurs en fonction de vos besoins dans cette section."

Pour créer un tableau de bord de diffusion, procédez comme suit :

1. Accédez au menu **Alertes de diffusion** dans le volet de navigation de gauche, puis cliquez sur **Créer un tableau de bord de diffusion**.

   ![Capture d’écran affichant l’option Créer un tableau de bord de diffusion dans le menu Alertes de diffusion](assets/alerting-dashboard.png).

1. Donnez un nom à votre tableau de bord dans le champ **Libellé**. Le champ **Nom interne** est renseigné automatiquement et en lecture seule.

1. Dans le champ **Sélectionner un groupe d’alertes**, spécifiez le **groupe d’opérateurs et d’opératrices** qui recevra les alertes envoyées par ce tableau de bord. Toutes les personnes membres du groupe d’opérateurs et d’opératrices sélectionné recevront les alertes.

   En savoir plus sur les autorisations et les groupes d’opérateurs dans la documentation d’[Adobe Campaign v8 (console)](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. Dans la section **Critères des alertes de diffusion**, ajoutez les critères que vous souhaitez utiliser pour envoyer des alertes. Faites votre choix parmi les critères prédéfinis ou créez vos propres critères pour répondre à des besoins spécifiques. [Découvrir comment utiliser les critères](../msg/delivery-alerting-criteria.md)

1. Les critères comportent des valeurs de paramètre par défaut qui définissent la manière dont ils doivent être appliqués. Vous pouvez modifier ces valeurs en fonction de vos besoins à partir de la section **Paramètres des critères**.

   ![Capture d’écran affichant la section Paramètres des critères dans le tableau de bord de la diffusion.](assets/alerting-criteria-parameters.png)

   Par exemple, par défaut, le paramètre de critère **Taille minimale de la cible de diffusion** est défini sur 50, ce qui signifie qu’une diffusion ne sera incluse dans l’alerte envoyée par ce tableau de bord que si elle cible au moins 50 profils. Vous pouvez modifier ce paramètre si vous souhaitez inclure des diffusions ciblant moins de 50 profils.

   Développez la section ci-dessous pour plus d’informations sur chaque paramètre de critère :

   +++Paramètres de critères disponibles

   * **Taille minimale de la cible de la diffusion** : si vous saisissez par exemple la valeur 100 dans ce champ, une notification est envoyée uniquement pour les diffusions dont la cible est supérieure ou égale à 100 destinataires. Ce paramètre s&#39;applique à tous les critères.
   * **Période de contrôle avant et après la date de contact (en heures)** : nombre d&#39;heures avant et après l&#39;heure actuelle. Seules les diffusions dont la date de contact est comprise dans cette plage sont prises en compte. Ce paramètre s&#39;applique à tous les critères. Par défaut, la valeur de ce champ est définie sur 24 heures.
   * **Taux maximal de rebonds temporaires** : une notification est envoyée pour toutes les diffusions dont le taux de rebonds temporaires est supérieur à la valeur spécifiée. Par défaut, la valeur de ce champ est définie sur 0,05 (5 %).
   * **Taux maximal de rebonds définitifs** : une notification est envoyée pour toutes les diffusions dont le taux de rebonds définitifs est supérieur à la valeur spécifiée. Par défaut, la valeur de ce champ est définie sur 0,05 (5 %).
   * **Limite de durée minimale pour une diffusion ayant le statut « Démarrage en attente » (en minutes)** : une notification est envoyée pour toutes les diffusions ayant le statut Démarrage en attente pendant une durée supérieure à celle spécifiée dans le champ. Le statut Démarrage en attente signifie que les messages n’ont pas encore été pris en compte par le système.
   * **Délai minimal (en minutes) nécessaire pour le calcul du débit** : seules les diffusions ayant démarré (avec le statut En cours) depuis plus longtemps que la durée spécifiée sont prises en compte pour le critère Diffusions avec faible débit.
   * **Pourcentage maximal des messages traités pour le calcul du débit** : seules les diffusions dont le pourcentage de messages traités est inférieur au pourcentage spécifié sont prises en compte pour le critère Diffusions avec faible débit.
   * **Débit minimal attendu (dans les messages envoyés par heure)** : seules les diffusions dont le débit est inférieur à la valeur spécifiée sont prises en compte pour le critère Diffusions avec faible débit.
   * **Taux de traitement minimal requis pour le critère « Diffusions en cours »** : seules les diffusions dont le pourcentage de messages traités est supérieur au pourcentage spécifié sont prises en compte.

+++

1. Par défaut, les tableaux de bord des alertes sont désactivés, ce qui signifie que les alertes par e-mail liées à ce tableau de bord ne sont pas envoyées. Pour activer immédiatement le tableau de bord, faites basculer l’option **Activé** dans la section **Général** en regard du champ de sélection du groupe d’alertes.

   Vous pouvez également enregistrer le tableau de bord et l’activer ultérieurement.

   ![Capture d’écran affichant l’option de basculement Activé dans les paramètres du tableau de bord de diffusion.](assets/alerting-dashboard-enable.png)

1. Pour enregistrer le tableau de bord des alertes, cliquez sur le bouton **Enregistrer**.

Le tableau de bord des alertes s’ouvre avec des données vides. Lorsque tout est prêt pour l’activer et envoyer des notifications, cliquez sur le bouton **Paramètres** et faites basculer l’option **Activé** si vous ne l’avez pas déjà fait.

Désormais, dès qu’une diffusion répond aux critères définis dans ce tableau de bord, une notification d’alerte est envoyée aux groupes d’opérateurs et d’opératrices spécifié.

## Gérer les tableaux de bord des alertes

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Alertes de diffusion envoyées"
>abstract="Cette section permet de visualiser des informations relatives aux dernières alertes envoyées."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Historique des alertes de diffusion"
>abstract="Le volet **Historique** contient toutes les alertes envoyées à partir de ce tableau de bord. Cliquez sur un élément pour accéder aux alertes correspondantes envoyées à ce moment précis."

Tous les tableaux de bord des alertes créés sont accessibles à partir du menu **Alertes de diffusion**, dans l’onglet **Tableaux de bord**.

![Capture d’écran affichant la liste des tableaux de bord des alertes dans le menu Alertes de diffusion.](assets/alerting-dashboard-list.png)

Vous pouvez dupliquer ou supprimer un tableau de bord à l’aide du bouton **Plus d’actions** situé en regard de son nom.

Pour accéder à la vue détaillée d’un tableau de bord, cliquez sur son nom dans la liste. Dans cet écran, vous pouvez visualiser la dernière alerte envoyée. Toutes les alertes envoyées sont répertoriées dans le volet de gauche. Cliquez sur un élément pour accéder aux alertes correspondantes envoyées à ce moment précis.

![Capture d’écran affichant la vue détaillée d’un tableau de bord d’alertes.](assets/alerting-dashboard-details.png)

Pour modifier le tableau de bord, cliquez sur le bouton **Paramètres** dans le coin supérieur droit et apportez les modifications souhaitées.