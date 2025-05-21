---
audience: end-user
title: Utiliser l’activité de workflow Chargement de fichier
description: Découvrez comment utiliser l’activité de workflow Chargement de fichier.
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: b94c1263ea09c9537d1a33983ea78d41b5644fb7
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 97%

---

# Chargement de fichier {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Activité Chargement de fichier"
>abstract="L’activité **Chargement de fichier** est une activité de **Data Management**. Utilisez cette activité pour travailler sur des données stockées dans un fichier externe. Les profils et les données ne sont pas ajoutés à la base de données, mais tous les champs du fichier d’entrée peuvent être utilisés à des fins de personnalisation ou de mise à jour des profils ou de tout autre tableau."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Transition sortante de la gestion des rejets"
>abstract="Transition sortante de la gestion des rejets"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Transition sortante de la gestion des rejets (pour les rejets)"
>abstract="Transition sortante de la gestion des rejets (pour les rejets)"

L’activité **Chargement de fichier** est une activité de **Data Management**. Utilisez-la lorsque vous travaillez avec des profils et des données stockés dans un fichier externe. Les profils et les données ne sont pas ajoutés à la base de données, mais tous les champs du fichier d’entrée sont disponibles pour la [personnalisation](../../personalization/gs-personalization.md) ou la mise à jour des profils ou des tables.

>[!NOTE]
>Les formats de fichier pris en charge sont les suivants : texte (TXT) et valeur séparée par des virgules (CSV). Avec la console de l’interface utilisateur web, vous pouvez charger des fichiers jusqu’à une taille maximale de 50 Mo. Dans la console cliente, l’activité Chargement de données a une limite de 150MB. [En savoir plus](https://experienceleague.adobe.com/docs/campaign-web/v8/wf/design-workflows/load-file.html?lang=fr){target="_blank"}

Combinée avec l’activité [Réconciliation](reconciliation.md), elle permet de lier des données non identifiées à des ressources existantes. L’activité **Chargement de fichier** peut par exemple être placée après une activité de **Réconciliation** si vous importez des données non standard dans la base de données.

## Configurer l’activité Chargement de fichier {#load-configuration}

La configuration de l’activité **Charger un fichier** s’effectue en deux étapes. Définissez d’abord la structure attendue du fichier en chargeant un fichier d’exemple. Une fois cela effectué, spécifiez la provenance du fichier dont les données sont importées. Suivez les étapes ci-dessous pour configurer l’activité :

![Capture d’écran de configuration de l’activité de chargement de fichier du workflow](../assets/workflow-load-file.png)

### Configurer le fichier d’exemple {#sample}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Exemple de fichier"
>abstract="Sélectionnez la structure attendue du fichier en chargeant un fichier d’exemple."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Mise en forme de l’activité Chargement de fichier"
>abstract="Dans la section **Mise en forme**, spécifiez la mise en forme du fichier externe pour vous assurer que les données sont correctement importées."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Nouveau mappage des valeurs de l’activité Chargement de fichier"
>abstract="Utilisez cette option pour mapper des valeurs spécifiques des fichiers chargés à de nouvelles valeurs. Par exemple, si la colonne contient des valeurs « True » et « False », vous pouvez ajouter un mappage pour remplacer automatiquement ces valeurs par des caractères « 0 » et « 1 »."

Pour configurer le fichier d’exemple utilisé pour définir la structure de fichier attendue, procédez comme suit :

1. Ajoutez une activité **Charger un fichier** dans votre workflow.

1. Sélectionnez le fichier d’exemple à utiliser pour définir la structure de fichier attendue. Pour ce faire, cliquez sur le bouton **Sélectionner un fichier** dans la section **[!UICONTROL Exemple de fichier]** et sélectionnez le fichier local à utiliser.

   >[!NOTE]
   >
   >Les données du fichier d’exemple sont utilisées pour le paramétrage de l’activité mais ne sont pas importées. Utilisez un fichier d’exemple contenant peu de données. Le format de fichier doit correspondre à celui de l’[exemple de fichier](../../audience/file-audience.md#sample-file).

1. Un aperçu de l’exemple de fichier apparaît et affiche un maximum de 30 lignes.

1. Dans la liste déroulante **[!UICONTROL Type de fichier]**, indiquez si le fichier utilise des colonnes délimitées ou des colonnes à largeur fixe.

   ![Capture d’écran de configuration de fichier d’exemple](../assets/workflow-load-file-sample.png)

1. Pour les types de fichiers à colonnes délimitées, utilisez la section **Colonnes** pour configurer les propriétés de chaque colonne.

   +++Options disponibles pour les colonnes des fichiers

   * **[!UICONTROL Libellé]** : libellé à afficher de la colonne.
   * **[!UICONTROL Type de données]** : type de données que contient la colonne.
   * **[!UICONTROL Largeur]** (type de données chaîne) : nombre maximum de caractères à afficher dans la colonne.
   * **[!UICONTROL Transformation des données]** (type de données chaîne) : applique une transformation aux valeurs contenues dans la colonne.
   * **[!UICONTROL Gestion des espaces]** (type de données chaîne) : indiquez comment gérer les espaces contenus dans la colonne.
   * **[!UICONTROL Séparateurs]** (types de données date, heure, nombre entier et nombre) : spécifiez les caractères à utiliser comme séparateurs.
   * **[!UICONTROL Autoriser les valeurs NULL]** : indiquez comment gérer les valeurs vides dans la colonne. L’option « Paramètre par défaut d’Adobe Campaign » renvoie une erreur si une valeur vide est présente.
   * **[!UICONTROL Traitement des erreurs]** (type de données chaîne) : indiquez le comportement à suivre en cas d’erreur dans l’une des lignes.
   * **[!UICONTROL Remappage des valeurs]** : cette option vous permet de mapper des valeurs spécifiques à de nouvelles valeurs. Par exemple, si la colonne contient des valeurs de type « True » et « False », vous pouvez ajouter un mappage pour remplacer automatiquement ces valeurs par les caractères « 0 » et « 1 ».

   +++

1. Dans la section **Mise en forme**, indiquez la mise en forme du fichier externe pour vous assurer que les données sont correctement importées.

### Définir le fichier cible à charger {#target}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Fichier cible de l’activité Chargement de fichier"
>abstract="Dans la section **[!UICONTROL Fichier cible]**, spécifiez comment récupérer le fichier à charger sur le serveur."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nom du fichier"
>abstract="Spécifiez le nom du champ à charger sur le serveur. Cliquez sur l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]** afin d’utiliser l’éditeur d’expression, y compris les variables d’événement, pour calculer le nom du fichier."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Base de données cible"
>abstract="Si vous accédez à une activité **[!UICONTROL Charger un fichier]** qui a déjà été configurée dans la console cliente, une section supplémentaire **[!UICONTROL Base de données cible]** est disponible si vous avez configuré l’activité pour charger le fichier vers une base de données externe."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Commande de chargement de fichier"
>abstract="L’autorisation d’une instruction arbitraire pour le prétraitement pose un problème de sécurité. Désactivez l’option de sécurité XtkSecurity_Disable_Preproc pour forcer l’utilisation d’une liste prédéfinie d’instructions."

>[!CAUTION]
>
>Avant de charger le fichier cible, assurez-vous qu’il soit conforme à la mise en forme du fichier d’exemple. Toute incohérence concernant le format du fichier, la structure des colonnes ou le nombre de colonnes peut entraîner des erreurs lors de l’exécution du workflow.

Pour définir le fichier cible à charger, procédez comme suit :

1. Dans la section **[!UICONTROL Fichier cible]**, indiquez l’action à effectuer lors de la récupération du fichier à charger sur le serveur.

   * **[!UICONTROL Charger un fichier à partir d’un ordinateur local]** : sélectionnez le fichier à charger à partir de votre ordinateur.

   * **[!UICONTROL Spécifié dans la transition]** : chargez le fichier spécifié dans la transition entrante qui suit une activité antérieure, telle que **[!UICONTROL Transférer un fichier]**.

   * **[!UICONTROL Prétraiter le fichier]** : chargez le fichier spécifié dans la transition précédente et appliquez une commande de pré-traitement sur celui-ci, telle que **[!UICONTROL Décompression]** ou **[!UICONTROL Déchiffrer]**.

   * **[!UICONTROL Calculé]** : chargez le fichier dont le nom est spécifié dans le champ **[!UICONTROL Nom du fichier]**. Cliquez sur l’icône **[!UICONTROL Ouvrir la boîte de dialogue de personnalisation]** afin d’utiliser l’éditeur d’expression, y compris les variables d’événement, pour calculer le nom du fichier.

   ![Capture d’écran de la configuration du fichier cible](../assets/workflow-load-file-config.png)

   >[!NOTE]
   >
   >Si vous accédez à une activité **[!UICONTROL Charger un fichier]** qui a déjà été configurée dans la console cliente, une section supplémentaire appelée **[!UICONTROL Base de données cible]** s’affiche si vous avez configuré l’activité pour charger le fichier vers une base de données externe. Celle-ci vous permet de spécifier si vous souhaitez charger le fichier vers le serveur Campaign ou vers la base de données externe.

### Options additionnelles {#options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Gestion des rejets pour l’activité Chargement de fichier"
>abstract="Dans la section **Gestion des rejets**, spécifiez le comportement de l’activité en cas d’erreur. Vous pouvez définir le nombre maximal d’erreurs autorisées et activer l’option **[!UICONTROL Conserver les rejets dans un fichier]** pour télécharger sur le serveur un fichier contenant les erreurs qui se sont produites pendant l’import."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Supprimer le fichier après l’import"
>abstract="Activez le bouton **Supprimer le fichier après l’import** pour supprimer le fichier d’origine du serveur après son import."

1. Dans la section **Gestion des rejets**, spécifiez le comportement de l’activité en cas d’erreur :

   * Dans le champ **[!UICONTROL Nombre d’erreurs autorisées]**, spécifiez le nombre maximum d’erreurs autorisées lors du traitement du fichier à charger. Par exemple, si la valeur est définie sur « 20 », l’exécution du workflow échoue si plus de 20 erreurs se produisent lors du chargement du fichier.

   * Pour conserver les erreurs qui se sont produites lors du chargement du fichier, activez l’option **[!UICONTROL Conserver les rejets dans un fichier]** et saisissez le nom de votre choix pour le fichier dans le champ **[!UICONTROL Fichier de rejets]**.

     Après avoir activé cette option, une transition de sortie supplémentaire nommée « Complémentaire » est ajoutée après l’activité. Toute erreur qui se produit pendant l’import est stockée dans le fichier spécifié sur le serveur.

1. Pour supprimer le fichier chargé du serveur une fois le workflow exécuté, activez l’option **[!UICONTROL Supprimer le fichier après l’import]**.

   ![Capture d’écran de configuration des options supplémentaires](../assets/workflow-load-file-options.png)

1. Cliquez sur **Confirmer** une fois que les paramètres sont corrects.

## Exemple {#load-example}

Un exemple de chargement de fichier externe est disponible avec l’activité **Réconciliation** dans [cette section](reconciliation.md#reconciliation-example).
