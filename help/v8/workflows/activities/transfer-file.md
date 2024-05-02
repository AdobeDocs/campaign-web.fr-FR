---
audience: end-user
title: Utilisation de l’activité Transfert de fichier
description: Découvrez comment utiliser l’activité de workflow Transfert de fichier
source-git-commit: 6fe8be5510e13cdb9e9e1bce44aadb80619275e4
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 13%

---

# Transfert de fichier {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="Transfert de fichier"
>abstract="La variable **Transfert de fichier** activité vous permet de recevoir ou d’envoyer des fichiers, de tester la présence de fichiers ou de lister les fichiers sur un serveur. Le protocole utilisé peut être soit un protocole serveur à serveur, soit un protocole HTTP."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="Options de transfert de fichier"
>abstract="Options de transfert de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="Activité de transfert de fichier"
>abstract="Activité de transfert de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="Serveur distant de transfert de fichier"
>abstract="Serveur distant de transfert de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Source de transfert de fichier"
>abstract="Source de transfert de fichier"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Effacer les fichiers source après leur transfert"
>abstract="Effacer les fichiers source après leur transfert"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Afficher les journaux de la session"
>abstract="Afficher les journaux de la session"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Répertorier tous les fichiers"
>abstract="Répertorier tous les fichiers"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Historisation des fichiers"
>abstract="Historisation des fichiers"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Traiter les fichiers absents"
>abstract="Traiter les fichiers absents"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Traiter les erreurs"
>abstract="Traiter les erreurs"

La variable **Transfert de fichier** est une activité **Data Management** activité. Il vous permet de recevoir ou d’envoyer des fichiers, de tester la présence de fichiers ou de lister les fichiers sur un serveur. Le protocole utilisé peut être soit un protocole serveur à serveur, soit un protocole HTTP.

>[!NOTE]
>
>Avec l&#39;interface utilisateur web de Campaign, nous avons consolidé deux activités en une seule en fusionnant les deux. **Transfert de fichier** et **Téléchargement web** fonctionnalités. Cette consolidation n&#39;a aucun impact sur les fonctionnalités de l&#39;activité.

Suivez les étapes détaillées ci-dessous pour configurer le **Transfert de fichier** activité.

## Choisir le protocole de transfert et l&#39;opération {#protocol}

1. Ajouter un **Transfert de fichier** dans votre workflow, puis indiquez le type de transfert à effectuer en fonction du protocole que vous souhaitez utiliser :

   * Pour le protocole HTTP, sélectionnez **[!UICONTROL Téléchargement Web]**. Vous pouvez ainsi effectuer le téléchargement d’un fichier par un GET ou un POST sur une URL explicite, un compte externe ou une instance Adobe Campaign.
   * Pour les autres protocoles serveur à serveur et actions connexes, sélectionnez **[!UICONTROL Transfert de fichier]**.

1. Sélectionnez l’action à exécuter avec l’activité. Les actions disponibles dépendent du type de transfert que vous avez sélectionné. Pour plus d’informations, développez les sections ci-dessous.

   +++Actions disponibles avec **Transfert de fichier** activités de type

   * **[!UICONTROL Téléchargement de fichier]**: téléchargez un fichier à partir du serveur.
   * **[!UICONTROL Chargement de fichier]**: téléchargez un fichier sur le serveur.
   * **[!UICONTROL Test d’existence de fichier]**: vérifiez si un fichier donné est présent sur le serveur. Génère deux transitions sortantes après l&#39;activité : &quot;Fichier présent&quot; et &quot;Fichier n&#39;existe pas&quot;.
   * **[!UICONTROL Listes de fichiers]**: répertorie tous les fichiers disponibles sur le serveur.

+++

   +++Actions disponibles avec **Téléchargement web** activités de type

   * **[!UICONTROL Transfert simple (GET)]**: récupérez un fichier.
   * **[!UICONTROL Transférer à l’aide d’un formulaire (POST)]**: téléchargez un fichier et des paramètres supplémentaires.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. Par défaut, pour les actions de téléchargement de fichiers, l’activité utilise le fichier spécifié dans l’activité précédente. Pour utiliser un autre fichier, faites basculer le **[!UICONTROL Utiliser le fichier de l’activité précédente]** puis cliquez sur l’option **[!UICONTROL Ajouter un fichier]** bouton .

   Dans le **[!UICONTROL Source]** , saisissez le nom de fichier souhaité ou utilisez l’éditeur d’expression pour calculer le nom du fichier à l’aide de variables d’événement. [Découvrez comment utiliser les variables d’événement et l’éditeur d’expression](../event-variables.md). Répétez l’opération pour ajouter autant de fichiers que nécessaire.

## Définition de la destination de transfert {#destination}

1. Dans le **[!UICONTROL Serveur distant]** , spécifiez le serveur auquel se connecter à l’aide de l’une des méthodes suivantes :

   * **[!UICONTROL Utiliser les paramètres de connexion définis dans un compte externe]**: connectez-vous à un serveur à l’aide des paramètres de connexion d’un compte externe. Dans le **[!UICONTROL Dossier du serveur]** , spécifiez le chemin d’accès au fichier (ou au dossier pour les actions de liste de fichiers).
   * **[!UICONTROL Configuration rapide]**: saisissez l’URL du fichier (ou dossier pour les actions de liste de fichiers).
   * **[!UICONTROL Instance Adobe Campaign]** (Activités de type Téléchargement Web) : téléchargez un fichier depuis un serveur d’instance Adobe Campaign.

   ![](../assets/workflow-transfer-file-server.png)

1. Pour les actions du POST de téléchargement Web, vous pouvez transmettre des paramètres supplémentaires avec l’opération. Pour ce faire, cliquez sur le bouton **[!UICONTROL Ajouter un paramètre]** puis indiquez le nom et la valeur des paramètres. Vous pouvez ajouter autant de paramètres que nécessaire.

1. Par défaut, pour le téléchargement de fichiers, les fichiers chargés sur un serveur sont automatiquement enregistrés. Si vous ne souhaitez pas conserver cet historique, activez la variable **[!UICONTROL Conserver l’historique des fichiers envoyés]** désactivée.

## Paramètres d’historisation   {#historization}

À chacune de ses exécutions, l’activité **[!UICONTROL Transfert de fichier]** stocke les fichiers transférés ou téléchargés dans un dossier dédié. Un dossier est créé pour chaque activité Transfert de fichier d’un workflow. Par défaut, les fichiers sont enregistrés dans le répertoire de stockage par défaut du dossier d’installation d’Adobe Campaign (`/vars`) avant d’être traité. Pour utiliser un dossier spécifique, faites basculer le **[!UICONTROL Utiliser un répertoire de stockage par défaut]** et saisissez le chemin du répertoire.

![](../assets/workflow-transfer-file-historization.png)

Il est important de pouvoir limiter la taille de ce dossier afin de préserver l’espace physique sur le serveur. Pour ce faire, vous pouvez définir un nombre maximum de fichiers ou la taille totale du dossier de l’activité. Par défaut, 100 fichiers et 50 Mo sont autorisés.

À chaque exécution de l’activité, le dossier est vérifié comme suit :

* Seuls les fichiers créés plus de 24 heures avant l’exécution de l’activité sont pris en compte.
* Si le nombre de fichiers pris en compte est supérieur à la valeur de la variable **[!UICONTROL Nombre de fichiers]** , les fichiers les plus anciens sont supprimés jusqu’à ce que le nombre maximal de fichiers autorisé soit atteint.
* Si la taille totale des fichiers pris en compte est supérieure à la valeur de la variable **[!UICONTROL Taille maximale (en Mo)]** , les fichiers les plus anciens sont supprimés jusqu’à ce que la Taille maximale (en Mo) soit atteinte.

>[!CAUTION]
>
>Si l’activité n’est pas exécutée à nouveau, son dossier ne sera pas vérifié ni purgé. Faites donc preuve de prudence lorsque vous transférez des fichiers de grande taille.

## Options avancées et de gestion des erreurs {#advanced}

1. Dans le **[!UICONTROL Options avancées]**, d’autres options sont disponibles en fonction du type d’activité que vous configurez. Pour plus d’informations, développez les sections ci-dessous.

   +++ Options supplémentaires pour **[!UICONTROL Transfert de fichier]** activités de type

   * **[!UICONTROL Supprimer les fichiers source après leur transfert]**: effacez les fichiers source après un transfert réussi.
   * **[!UICONTROL Affichage des journaux de session]**: lorsque cette option est activée, les informations relatives à l’opération de transfert s’affichent dans les logs du workflow une fois le workflow exécuté.
   * **[!UICONTROL Liste de tous les fichiers]** (Actions de liste de fichiers) : cette option indexe tous les fichiers présents sur le serveur dans la variable `vars.filenames` dans laquelle les noms de fichier sont séparés par la variable `n` caractères. [Découvrez comment utiliser des variables d’événement](../event-variables.md)

+++

   +++ Options supplémentaires pour **[!UICONTROL Téléchargement web]** activités de type

   * **[!UICONTROL Suivez les redirections]**: la redirection de fichier permet d&#39;utiliser des remplacements pour diriger la saisie ou la sortie de données vers un appareil d&#39;un autre type.
   * **[!UICONTROL Ajout des en-têtes HTTP au fichier]**: dans certains cas, vous pouvez ajouter des en-têtes HTTP supplémentaires à un fichier. Le plus souvent, ces en-têtes seront utilisés pour fournir des informations supplémentaires à des fins de dépannage, pour les [Partage des ressources cross-origin (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS)ou pour définir des directives de mise en cache spécifiques.
   * **[!UICONTROL Ignorer le code de retour HTTP]**: les codes retour HTTP, également appelés codes d’état HTTP, indiquent le résultat d’une requête HTTP.

1. La variable **[!UICONTROL Traiter les erreurs]** permet d&#39;activer une transition sortante &quot;Erreur&quot; après l&#39;activité si une erreur se produit pendant le transfert.

   En outre, pour **Transfert de fichier** les activités de type , **[!UICONTROL Traitement du fichier manquant]** permet d&#39;activer une transition sortante &quot;Aucun fichier&quot; après l&#39;activité si le fichier n&#39;est pas disponible sur le chemin spécifié.
