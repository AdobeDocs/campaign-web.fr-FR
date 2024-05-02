---
audience: end-user
title: Utilisation de l’activité Services d’abonnements
description: Découvrez comment utiliser l’activité de workflow de services d’abonnements
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 23%

---

# Services d’abonnements {#subscriptipon-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Activité de services d’abonnements"
>abstract="L&#39;activité Services d&#39;abonnements permet d&#39;abonner ou de désabonner plusieurs profils à un service en une seule action."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Paramètres généraux du service d’abonnement"
>abstract="Choisissez le service visé et choisissez l&#39;action à effectuer (inscription ou désinscription). Activez l’option **Envoyer un message de confirmation** l&#39;option sur pour notifier à la population qu&#39;elle est abonnée ou désabonnée au service sélectionné."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Générer une transition sortante"
>abstract="Activez l’option **Générer une transition sortante** pour ajouter une transition après l’activité."

La variable **Services d’inscriptions** est une activité **Data Management** activité. Il permet de créer ou supprimer un abonnement à un service d&#39;information pour la population spécifiée par la transition.

## Configuration de l’activité Services d’abonnements {#subscription-services-configuration}

Pour configurer la variable **Services d’inscriptions** activité :

1. Ajouter un **Services d’inscriptions** dans votre workflow. Vous pouvez utiliser cette activité après avoir ciblé des profils ou importé un fichier avec des données identifiées.

1. Sélectionnez le service pour lequel vous souhaitez gérer les abonnements à l&#39;aide de l&#39;une des options suivantes :

   * **[!UICONTROL Sélectionner un service spécifique]**: sélectionnez manuellement un service à l’aide du **[!UICONTROL Service]** champ .

   * **[!UICONTROL De la transition entrante]**: utilisez le service spécifié dans la transition entrante. Vous pouvez, par exemple, importer un fichier qui spécifie le service à gérer pour chaque ligne. Le service sur lequel effectuer l’opération est alors sélectionné dynamiquement pour chaque profil.

   ![](../assets/workflow-subscription-service.png)

1. Sélectionnez l’opération à effectuer : **Abonner** ou **Désabonner**.

   Si le service est défini dans la transition entrante, vous pouvez choisir comment récupérer cette opération :

   * **Sélection d’un type d’opération spécifique**: sélectionnez manuellement l’opération à effectuer (**Abonner** ou **Désabonner**)

   * **Sélectionner un type d’opération à partir d’un chemin de transition entrante**: sélectionnez la colonne des données entrantes spécifiant l’opération à effectuer pour chaque enregistrement. Par exemple, vous pouvez importer un fichier qui spécifie l’opération à effectuer pour chaque ligne dans une colonne &quot;operation&quot;.

     >[!NOTE]
     >
     >Seuls les champs booléens ou entiers peuvent être sélectionnés ici. Assurez-vous que les données contenant l’opération à effectuer correspondent à ce format. Par exemple, si vous chargez des données depuis une activité Chargement de fichier , vérifiez que vous avez correctement défini le format de la colonne contenant l’opération dans la variable **[!UICONTROL Chargement de fichier]** activité. Un exemple est présenté dans la section [cette section](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Pour informer les destinataires qu’ils sont abonnés ou désabonnés du service sélectionné, faites basculer le bouton **[!UICONTROL Envoyer un message de confirmation]** sur . Le contenu de cette notification est défini dans un modèle de diffusion associé au service d&#39;information.

1. Si vous utilisez des données d’une transition entrante, une **[!UICONTROL Informations supplémentaires]** s’affiche, vous permettant de spécifier les données et l’origine de l’abonnement pour chaque enregistrement. Vous pouvez laisser cette section vide, auquel cas aucune date ou origine ne sera définie lors de l’exécution du workflow.

   * Si les données entrantes contiennent une colonne indiquant la date d&#39;abonnement du profil au service, vous pouvez la sélectionner dans la **[!UICONTROL Date]** champ .

   * Dans le **[!UICONTROL Chemin d’origine]** , définissez l&#39;origine de l&#39;abonnement. Vous pouvez la définir sur l’un des champs des données entrantes ou sur une valeur constante de votre choix en cochant la case **[!UICONTROL Définir une constante comme origine]** .

   ![](../assets/workflow-subscription-service-additional.png)

1. Pour ajouter une transition sortante après l’activité, faites basculer le **[!UICONTROL Générer une transition sortante]** sur .

## Exemples {#example}

### Abonner une audience à un service spécifique {#uc1}

Ce workflow ci-dessous montre comment abonner une audience à un service existant.

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL Créer une audience]** activité cible une audience existante.

* A **[!UICONTROL Services d’inscriptions]** permet de sélectionner le service auquel les profils doivent s&#39;abonner.

### Mise à jour de plusieurs statuts d&#39;abonnement depuis un fichier {#uc2}

Le workflow ci-dessous montre comment importer un fichier contenant des profils et mettre à jour leur abonnement à plusieurs services spécifiés dans le fichier.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Chargement de fichier]** activité charge un fichier CSV contenant les données et définit la structure des colonnes importées. Les colonnes &quot;service&quot; et &quot;operation&quot; spécifient le service à mettre à jour et l&#39;opération à effectuer (abonnement ou désabonnement).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Comme vous l’avez peut-être remarqué, l’opération est spécifiée en tant que &quot;sub&quot; ou &quot;unsub&quot; dans le fichier. Le système attend une valeur de type **Booléen** ou **Entier** pour déterminer l’opération à réaliser : la valeur &quot;0&quot; pour désabonner et la valeur &quot;1&quot; pour abonner. Pour répondre à cette exigence, un recodification des valeurs doit être effectué dans le détail de la colonne &quot;operation&quot; de l&#39;écran de configuration du fichier d&#39;exemple.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Si le fichier utilise déjà les valeurs &quot;0&quot; et &quot;1&quot; pour identifier l’opération, il n’est pas nécessaire de recodifier ces valeurs. Veillez uniquement à ce que la colonne soit traitée comme une **Booléen** ou **Entier** dans les colonnes d’exemple de fichier.

* Une **[!UICONTROL Réconciliation]** permet d’identifier les données provenant du fichier comme appartenant à la dimension des profils de la base de données Adobe Campaign. La variable **email** du fichier est associé au champ **email** du champ de la ressource de profil.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* Un **[!UICONTROL Enrichissement]** crée un lien vers la table &quot;Services (nms)&quot; et crée une jointure simple entre la colonne &quot;service&quot; du fichier téléchargé et le champ &quot;nom interne&quot; des services dans la base de données.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Déduplication]** en fonction de la variable **email** identifie les doublons. Il est important de supprimer les doublons, car s’il en existe, l’abonnement à un service échouera pour l’ensemble des données.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)

* Une activité **[!UICONTROL Services d’inscription]** identifie les services à mettre à jour comme provenant de la transition, au travers du lien créé dans l’activité **[!UICONTROL Réconciliation]**.

  Le **[!UICONTROL Type d’opération]** est identifié comme provenant du champ **operation** du fichier. Seul un champ Booléen ou Entier peut être sélectionné ici. Si la colonne du fichier contenant l’opération à effectuer n’apparaît pas dans la liste, vérifiez que vous avez correctement défini le format de la colonne dans l’activité **[!UICONTROL Chargement de fichier]**, comme expliqué plus haut dans cet exemple.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
