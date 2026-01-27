---
audience: end-user
title: Créer des expériences de contenu
description: Découvrez comment créer des expériences de contenu dans Adobe Campaign Web
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 2%

---

# Créer des expériences de contenu {#content-experiment}

## À propos des expériences de contenu {#about-content-experiment}

Les expériences de contenu dans Adobe Campaign Web vous permettent de définir plusieurs variantes de diffusion de test A/B afin de mesurer celle qui fonctionne le mieux pour votre audience cible. Vous pouvez varier le contenu, l’objet ou l’expéditeur de la diffusion afin de tester différentes versions et de déterminer la variante produisant les meilleurs résultats.

Vous pouvez effectuer des tests A/B sur divers éléments d’e-mail, tels que :

* **Objet** : testez différentes lignes d’objet d’e-mail pour déterminer laquelle génère le taux d’ouverture le plus élevé
* **Nom expéditeur** : testez différentes combinaisons d’expéditeur
* **Contenu du corps de l’e-mail** : créez plusieurs versions de contenu pour identifier celles qui génèrent le meilleur taux de clic publicitaire

>[!NOTE]
>
>* Les expériences de contenu sont actuellement disponibles pour le canal e-mail uniquement.
>* Les tests A/B ne sont pas pris en charge pour les messages transactionnels.
>* Maximum de 3 traitements (variantes) par expérience.

## Créer une expérience de contenu {#create-content-experiment}

Pour ajouter une expérience de contenu à votre diffusion e-mail, procédez comme suit :

1. Créez une diffusion e-mail ou ouvrez un brouillon de diffusion existant. [Découvrez comment créer un email](create-email.md)

1. Sur la page des propriétés de la diffusion e-mail, cliquez sur le bouton **[!UICONTROL Créer une expérience]** situé dans la section **[!UICONTROL Contenu]**.

   ![Capture d’écran affichant le bouton Créer une expérience dans les propriétés d’e-mail](assets/ab-testing-1.png){zoomable="yes"}

## Configurer les paramètres de l’expérience {#configure-experiment}

Configurez votre expérience à l’aide des sections suivantes :

![Capture d’écran affichant les paramètres de l’expérience](assets/ab-testing-2.png){zoomable="yes"}

### Paramètres de l’audience {#audience-settings}

Définissez le pourcentage de votre population cible qui recevra les variantes de l’expérience.

Saisissez une valeur pour définir la taille de l’audience. Cela représente la proportion de destinataires qui recevront l’une des variantes de l’expérience pendant la phase de test.

* **Minimum** : 1 %
* **Maximum** : 100 %
* **Par défaut** : 10 %

L’audience restante (90 % par défaut) recevra la variante gagnante une fois l’expérience terminée et qu’un gagnant est déterminé.

Par exemple, avec une audience cible de 10 000 destinataires et une taille d’audience de 10 %, 1 000 destinataires seront sélectionnés de manière aléatoire pour participer à l’expérience. Les 9 000 destinataires restants recevront la variante gagnante une fois l’expérience terminée.

### Stratégie gagnante {#winning-strategy}

Sélectionnez la mesure qui sera utilisée pour déterminer la variante gagnante :

* **[!UICONTROL Meilleur taux d’ouverture]** (par défaut) : la variante ayant le pourcentage le plus élevé d’ouvertures d’e-mail est gagnante
* **[!UICONTROL Taux de meilleurs clics publicitaires]** : la variante qui a le pourcentage de clics le plus élevé dans l’e-mail gagne
* **[!UICONTROL Taux de désabonnement le plus faible]** : la variante ayant le pourcentage de désabonnements le plus faible gagne

Le système suit automatiquement ces mesures au cours de l’expérience et calcule la variante la plus performante en fonction du critère sélectionné.

### Méthode d&#39;envoi du gagnant {#sending-method}

Définissez la durée d’exécution de l’expérience et sélectionnez la méthode d’envoi :

1. Saisissez la valeur de la durée en heures. L’expérience s’exécutera pendant cette période avant de déterminer la variante gagnante.

   * **Minimum** : 3 heures
   * **Maximum** : 240 heures (10 jours)
   * **Par défaut** : 24 heures

   >[!NOTE]
   >
   >Assurez-vous que la durée de votre expérience est suffisamment longue pour collecter des données significatives. Une durée courte peut ne pas fournir une signification statistique suffisante, en particulier pour les mesures telles que le taux de clic publicitaire qui peuvent prendre plus de temps à s’accumuler.

1. Choisissez comment la variante gagnante doit être envoyée à la population restante :

   * **[!UICONTROL Envoi automatique]** activé : le système envoie automatiquement la variante gagnante à l’audience restante une fois l’expérience terminée.
   * **[!UICONTROL Envoi automatique]** désactivé : vous devez cliquer manuellement sur le bouton **[!UICONTROL Envoyer]** pour envoyer la variante gagnante après avoir consulté les résultats de l’expérience.

Si aucune variante n’obtient de résultats significativement meilleurs que les autres à la fin de l’expérience, le système envoie la première variante à la population restante. Consultez cette [section](#send-deliveries).

## Définition des traitements de contenu {#define-content}

Après avoir enregistré les paramètres de votre expérience, un premier traitement est créé par défaut. Vous devez maintenant ajouter vos autres traitements (jusqu’à trois) et définir leur contenu spécifique.

1. Dans les propriétés de la diffusion, cliquez sur **[!UICONTROL Modifier le contenu]**. Les traitements s’affichent sur le côté gauche.

   ![Capture d’écran affichant le panneau Expériences de contenu](assets/ab-testing-3.png){zoomable="yes"}

1. Cliquez sur le bouton **[!UICONTROL Ajouter un traitement]** et définissez son nom. Répétez cette opération pour tous les traitements que vous devez ajouter. Vous pouvez ensuite modifier leur nom, les dupliquer et les supprimer.

1. Cliquez sur chaque traitement et personnalisez les éléments suivants :

   * **Nom de l’expéditeur** : personnalisez l’expéditeur de l’e-mail
   * **Objet** : créez une ligne d’objet unique pour chaque traitement
   * **Corps de l’e-mail** : concevez différentes versions de contenu à l’aide du Designer d’e-mail

   ![Capture d’écran montrant plusieurs traitements](assets/ab-testing-4.png){zoomable="yes"}

1. Prévisualisez chaque traitement en cliquant dessus, puis sur **[!UICONTROL Simuler du contenu]**.

## Démarrer l’expérience et surveiller les résultats {#validate-start}

Une fois que vous avez défini tous vos traitements de contenu, vous pouvez valider et démarrer l’expérience.

1. Dans les propriétés de la diffusion, cliquez sur **[!UICONTROL Vérifier et envoyer]** puis sur **[!UICONTROL Préparer]**.

1. Cliquez ensuite sur **[!UICONTROL Démarrer l’expérimentation]** pour lancer le test A/B.

   ![Capture d’écran affichant le bouton Démarrer l’expérimentation](assets/ab-testing-5.png){zoomable="yes"}

1. Une fois votre expérience en cours d’exécution, surveillez les différentes mesures affichées dans le tableau de bord de la diffusion.

Pendant l’exécution de l’expérience, vous pouvez cliquer sur **[!UICONTROL Arrêter l’envoi]** pour terminer l’expérience. Vous pouvez également décider d’envoyer manuellement avant la fin de l’expérience en cliquant sur **[!UICONTROL Sélectionner et envoyer au gagnant]**.

>[!NOTE]
>
>Les résultats sont mis à jour en temps quasi réel lorsque les destinataires interagissent avec votre e-mail. Cependant, les premiers résultats peuvent ne pas avoir de signification statistique. Il est recommandé d’attendre que la durée de l’expérience soit terminée avant de prendre des décisions finales.

## Envoyer les diffusions {#send-deliveries}

L’envoi peut être effectué automatiquement ou manuellement, selon ce que vous avez choisi dans les paramètres **[!UICONTROL Méthode d’envoi gagnante]**. Consultez cette [section](#sending-method).

### Envoi automatique {#automatic-sending}

Pour l’envoi automatique, le système analyse les résultats en fonction de votre stratégie gagnante et détermine le traitement gagnant. Le traitement gagnant est automatiquement envoyé à l’audience restante. Si aucun gagnant n&#39;apparaît clairement, la première variante est choisie.

### Envoi manuel {#manual-sending}

Si vous avez configuré l’envoi manuel, passez en revue les résultats à la fin de l’expérience et cliquez sur **[!UICONTROL Envoyer]** pour envoyer le traitement gagnant. Si aucun gagnant n’est clairement apparu, le premier traitement est sélectionné par défaut, mais vous pouvez en choisir un autre.

## Afficher les résultats finaux {#final-results}

Une fois votre expérience terminée et la diffusion entièrement envoyée, vous pouvez accéder à des rapports complets :

1. Dans le tableau de bord de la diffusion, cliquez sur **[!UICONTROL Rapports]**.

1. Accédez à l’onglet rapport **[!UICONTROL Expériences]** pour afficher les mesures de performances clés de chaque traitement.

## Bonnes pratiques {#best-practices}

Lors de la création d’expériences de contenu, tenez compte des recommandations suivantes :

* **Tester un élément à la fois** : pour des résultats plus clairs, testez les variations d’un seul élément (par exemple, ligne d’objet uniquement ou contenu uniquement) plutôt que de plusieurs éléments simultanément.

* **Choisir la durée appropriée** : laisser suffisamment de temps pour la signification statistique :
   * Pour les tests à débit ouvert : 12 à 24 heures est habituellement suffisant
   * Pour les tests de taux de clic publicitaire : 24 à 48 heures ou plus peuvent être nécessaires
   * Les audiences plus volumineuses peuvent nécessiter moins de temps ; les audiences plus petites peuvent nécessiter plus de temps

* **Dimensionnez votre audience de manière appropriée** :
   * Assurez-vous que l’audience de l’expérience (le pourcentage alloué au test) est suffisamment grande pour produire des résultats significatifs
   * Règle générale : minimum de 1 000 destinataires par traitement pour des résultats fiables

* **Tester régulièrement, mais pas excessivement** : effectuez des expériences sur des campagnes importantes, mais évitez de tester chaque envoi pour concentrer les ressources sur des décisions importantes.

* **Documentez vos apprentissages** : conservez des enregistrements des résultats d’expérience pour éclairer les stratégies de campagne futures.

## Rubriques connexes : {#related-topics}

* [Créer votre premier e-mail](create-email.md)
* [Configurer le contenu des e-mails](edit-content.md)
* [Prévisualiser et envoyer un e-mail](../monitor/prepare-send.md)
* [Rapports de diffusion E-mail](../reporting/email-report.md)
