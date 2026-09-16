<?xml version="1.0" encoding="UTF-8"?>
<xliff xmlns="urn:oasis:names:tc:xliff:document:1.2" xmlns:okp="okapi-framework:xliff-extensions" xmlns:its="http://www.w3.org/2005/11/its" xmlns:itsxlf="http://www.w3.org/ns/its-xliff/" version="1.2" its:version="2.0">
<file original="help/v8/workflows/activities/approval.md.mdsc" source-language="en-US" target-language="en-XX" datatype="x-text/markdown">
<body>
<trans-unit id="tu1" restype="x-YAML_METADATA_HEADER_VALUE" xml:space="preserve">
<source xml:lang="en-US">Approval workflow activity</source>
<target xml:lang="en-XX">Activité du workflow de validation</target>
</trans-unit>
<trans-unit id="tu2" restype="x-YAML_METADATA_HEADER_VALUE" xml:space="preserve">
<source xml:lang="en-US">Learn how to use the Approval workflow activity</source>
<target xml:lang="en-XX">Découvrez comment utiliser l’activité de workflow Validation.</target>
</trans-unit>
<trans-unit id="tu3" xml:space="preserve">
<source xml:lang="en-US">Approval</source>
<target xml:lang="en-XX">Validation</target>
</trans-unit>
<trans-unit id="tu4" xml:space="preserve">
<source xml:lang="en-US">Approval activity</source>
<target xml:lang="en-XX">Activité de validation</target>
</trans-unit>
<trans-unit id="tu5" xml:space="preserve">
<source xml:lang="en-US">The <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Approval<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph> activity requires the participation of an operator. Assign the task to a group or an individual operator, customize the notification title and message, and define the possible answers as output branches.</source>
<target xml:lang="en-XX">Une activité <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Validation<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph> requiert la participation d’un opérateur ou d’une opératrice. Attribuez la tâche à un groupe, à un opérateur individuel ou à une opératrice individuelle, personnalisez le titre et le message de la notification, puis définissez les réponses possibles comme branches de sortie.</target>
</trans-unit>
<trans-unit id="tu6" xml:space="preserve">
<source xml:lang="en-US">The <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Approval<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph> workflow activity allows you to assign a task to a group or an individual operator, customize the notification email title and message, and define the possible answers (for example Yes/No) as output branches.</source>
<target xml:lang="en-XX">L’activité de workflow <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Validation<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph> vous permet d’attribuer une tâche à un groupe, à un opérateur individuel ou à une opératrice individuelle, de personnaliser le titre et le message de l’e-mail de notification, puis de définir les réponses possibles (par exemple, Oui/Non) comme branches de sortie.</target>
</trans-unit>
<trans-unit id="tu7" xml:space="preserve">
<source xml:lang="en-US">Use this activity whenever a step in your workflow requires a human decision before continuing, for example to get sign-off on a budget, a target audience, or content, before the workflow proceeds.</source>
<target xml:lang="en-XX">Utilisez cette activité chaque fois qu’une étape de votre workflow nécessite une décision humaine pour pouvoir continuer, par exemple pour obtenir l’approbation d’un budget, d’une audience cible ou d’un contenu avant que le workflow ne se poursuive.</target>
</trans-unit>
<trans-unit id="tu8" xml:space="preserve">
<source xml:lang="en-US">How the approval process works</source>
<target xml:lang="en-XX">Fonctionnement du processus de validation</target>
</trans-unit>
<trans-unit id="tu9" xml:space="preserve">
<source xml:lang="en-US">It requires the participation of at least one operator. This activity does not block the workflow: other tasks can run while the workflow waits for a reply.</source>
<target xml:lang="en-XX">Il requiert la participation d’au moins un opérateur ou une opératrice. Cette activité ne bloque pas le workflow : d’autres tâches peuvent s’exécuter dans l’attente d’une réponse.</target>
</trans-unit>
<trans-unit id="tu10" xml:space="preserve">
<source xml:lang="en-US">While waiting for an answer, the activity is shown as pending on the canvas. The assignee responds using the link included in the notification message.</source>
<target xml:lang="en-XX">Dans l’attente d’une réponse, l’activité s’affiche comme étant en attente sur la zone de travail. La personne assignée répond en utilisant le lien contenu dans le message de notification.</target>
</trans-unit>
<trans-unit id="tu11" xml:space="preserve">
<source xml:lang="en-US">Here is the approval task process:</source>
<target xml:lang="en-XX">Le processus de tâche de validation est le suivant :</target>
</trans-unit>
<trans-unit id="tu12" xml:space="preserve">
<source xml:lang="en-US">Create a workflow and configure an <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Approval<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph> activity.</source>
<target xml:lang="en-XX">Créez un workflow et configurez une activité <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Validation<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph>.</target>
</trans-unit>
<trans-unit id="tu13" xml:space="preserve">
<source xml:lang="en-US">Start the workflow. When it reaches the <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Approval<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph> activity, a task is created for the assignee.</source>
<target xml:lang="en-XX">Démarrez le workflow. Lorsqu’il atteint l’activité <ph id="1" ctype="x-STRONG_EMPHASIS">**</ph>Validation<ph id="2" ctype="x-STRONG_EMPHASIS">**</ph>, une tâche est créée pour la personne assignée.</target>
</trans-unit>
<trans-unit id="tu14" xml:space="preserve">
<source xml:lang="en-US">The assignee receives the notification message, clicks on the link and selects an answer.</source>
<target xml:lang="en-XX">La personne assignée reçoit le message de notification, clique sur le lien et sélectionne une réponse.</target>
</trans-unit>
<trans-unit id="tu15" xml:space="preserve">
<source xml:lang="en-US">Once the assignee replies, the workflow continues through the transition matching their answer.</source>
<target xml:lang="en-XX">Une fois que la personne assignée a répondu, le workflow se poursuit via la transition correspondant à sa réponse.</target>
</trans-unit>
<trans-unit id="tu16" xml:space="preserve">
<source xml:lang="en-US">To configure this activity, follow these steps:</source>
<target xml:lang="en-XX">Pour configurer cette activité, procédez comme suit :</target>
</trans-unit>
<trans-unit id="tu17" xml:space="preserve">
<source xml:lang="en-US">Assign the task, <ph id="1" ctype="x-LINK">[</ph>read more<ph id="2" ctype="x-LINK">](#assignment)</ph></source>
<target xml:lang="en-XX">Attribuez la tâche, <ph id="1" ctype="x-LINK">[</ph>en savoir plus<ph id="2" ctype="x-LINK">](#assignment)</ph>.</target>
</trans-unit>
<trans-unit id="tu18" xml:space="preserve">
<source xml:lang="en-US">Define the notification message, <ph id="1" ctype="x-LINK">[</ph>read more<ph id="2" ctype="x-LINK">](#message)</ph></source>
<target xml:lang="en-XX">Définissez le message de notification, <ph id="1" ctype="x-LINK">[</ph>en savoir plus<ph id="2" ctype="x-LINK">](#message)</ph>.</target>
</trans-unit>
<trans-unit id="tu19" xml:space="preserve">
<source xml:lang="en-US">Define the possible answers, <ph id="1" ctype="x-LINK">[</ph>read more<ph id="2" ctype="x-LINK">](#answers)</ph></source>
<target xml:lang="en-XX">Définissez les réponses possibles, <ph id="1" ctype="x-LINK">[</ph>en savoir plus<ph id="2" ctype="x-LINK">](#answers)</ph>.</target>
</trans-unit>
<trans-unit id="tu20" xml:space="preserve">
<source xml:lang="en-US">Optionally, define an expiration, <ph id="1" ctype="x-LINK">[</ph>read more<ph id="2" ctype="x-LINK">](#expiration)</ph></source>
<target xml:lang="en-XX">Vous pouvez éventuellement définir une expiration, <ph id="1" ctype="x-LINK">[</ph>en savoir plus<ph id="2" ctype="x-LINK">](#expiration)</ph>.</target>
</trans-unit>
<trans-unit id="tu21" xml:space="preserve">
<source xml:lang="en-US">Assign the task</source>
<target xml:lang="en-XX">Affecter la tâche</target>
</trans-unit>
<trans-unit id="tu22" xml:space="preserve">
<source xml:lang="en-US">Assigning the task to a group or an operator is mandatory: a warning is displayed until you do so.</source>
<target xml:lang="en-XX">L’affectation de la tâche à un groupe, à un opérateur ou une opératrice, est obligatoire : un avertissement s’affiche jusqu’à ce que vous le fassiez.</target>
</trans-unit>
<trans-unit id="tu23" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-IMAGE">![</ph>Screenshot showing the Assignment section of the Approval activity<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval1.png){zoomable="yes"}</ph></source>
<target xml:lang="en-XX"><ph id="1" ctype="x-IMAGE">![</ph>Capture d’écran affichant la section Affectation de l’activité Validation<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval1.png){zoomable="yes"}</ph></target>
</trans-unit>
<trans-unit id="tu24" xml:space="preserve">
<source xml:lang="en-US">Follow these steps:</source>
<target xml:lang="en-XX">Procédez comme suit :</target>
</trans-unit>
<trans-unit id="tu25" xml:space="preserve">
<source xml:lang="en-US">In the <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Assignment type<ph id="3" ctype="x-LINK_REF">]**</ph> field, choose whether the task is assigned to a <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Group<ph id="7" ctype="x-LINK_REF">]**</ph> (default) or an <ph id="9" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Operator<ph id="11" ctype="x-LINK_REF">]**</ph>.</source>
<target xml:lang="en-XX">Dans le champ <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Type d’affectation<ph id="3" ctype="x-LINK_REF">]**</ph>, choisissez si la tâche est affectée à un <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Groupe<ph id="7" ctype="x-LINK_REF">]**</ph> (par défaut) ou à un <ph id="9" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Opérateur ou opératrice<ph id="11" ctype="x-LINK_REF">]**</ph>.</target>
</trans-unit>
<trans-unit id="tu26" xml:space="preserve">
<source xml:lang="en-US">Then select the <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Group<ph id="3" ctype="x-LINK_REF">]**</ph> (of operators) or an <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Operator<ph id="7" ctype="x-LINK_REF">]**</ph> (single operator).</source>
<target xml:lang="en-XX">Sélectionnez ensuite le <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Groupe<ph id="3" ctype="x-LINK_REF">]**</ph> (d’opérateurs et d’opératrices) ou un <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Opérateur ou opératrice<ph id="7" ctype="x-LINK_REF">]**</ph> (opérateur ou opératrice unique).</target>
</trans-unit>
<trans-unit id="tu27" xml:space="preserve">
<source xml:lang="en-US">Enable <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Multiple approval<ph id="3" ctype="x-LINK_REF">]**</ph> if you want every assignee to reply before the workflow continues. This option is available regardless of the assignment type. When disabled, the workflow continues as soon as any one assignee replies, and that reply is the one taken into account.</source>
<target xml:lang="en-XX">Activez l’option <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Validation multiple<ph id="3" ctype="x-LINK_REF">]**</ph> si vous souhaitez que chaque personne assignée réponde avant la poursuite du workflow. Cette option est disponible quel que soit le type d’affectation. Lorsqu’elle est désactivée, le workflow se poursuit dès qu’une personne assignée répond ; cette réponse est celle prise en compte.</target>
</trans-unit>
<trans-unit id="tu28" xml:space="preserve">
<source xml:lang="en-US">Click <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Advanced parameters<ph id="3" ctype="x-LINK_REF">]**</ph> to select the delivery template used for the notification. By default, a built-in template is used, but you can select any other delivery template.</source>
<target xml:lang="en-XX">Cliquez sur <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Paramètres avancés<ph id="3" ctype="x-LINK_REF">]**</ph> pour sélectionner le modèle de diffusion utilisé pour la notification. Par défaut, un modèle intégré est utilisé, mais vous pouvez sélectionner n’importe quel autre modèle de diffusion.</target>
</trans-unit>
<trans-unit id="tu29" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-IMAGE">![</ph>Screenshot showing the Advanced parameters of the Approval activity<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval1bis.png){zoomable="yes"}</ph></source>
<target xml:lang="en-XX"><ph id="1" ctype="x-IMAGE">![</ph>Capture d'écran affichant les paramètres avancés de l’activité Validation<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval1bis.png){zoomable="yes"}</ph></target>
</trans-unit>
<trans-unit id="tu30" xml:space="preserve">
<source xml:lang="en-US">Define the notification message</source>
<target xml:lang="en-XX">Définir le message de notification</target>
</trans-unit>
<trans-unit id="tu31" xml:space="preserve">
<source xml:lang="en-US">You can now define the notification message sent to the assignee.</source>
<target xml:lang="en-XX">Vous pouvez maintenant définir le message de notification envoyé à la personne assignée.</target>
</trans-unit>
<trans-unit id="tu32" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-IMAGE">![</ph>Screenshot showing the Message section of the Approval activity<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval2.png){zoomable="yes"}</ph></source>
<target xml:lang="en-XX"><ph id="1" ctype="x-IMAGE">![</ph>Capture d’écran affichant la section Message de l’activité Approbation<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval2.png){zoomable="yes"}</ph></target>
</trans-unit>
<trans-unit id="tu33" xml:space="preserve">
<source xml:lang="en-US">Follow these steps:</source>
<target xml:lang="en-XX">Procédez comme suit :</target>
</trans-unit>
<trans-unit id="tu34" xml:space="preserve">
<source xml:lang="en-US">Define the <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Title<ph id="3" ctype="x-LINK_REF">]**</ph> of the notification sent to the assignee.</source>
<target xml:lang="en-XX">Définissez le <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Titre<ph id="3" ctype="x-LINK_REF">]**</ph> de la notification envoyée à la personne assignée.</target>
</trans-unit>
<trans-unit id="tu35" xml:space="preserve">
<source xml:lang="en-US">Define the <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Message<ph id="3" ctype="x-LINK_REF">]**</ph> of the notification sent to the assignee.</source>
<target xml:lang="en-XX">Définissez le <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Message<ph id="3" ctype="x-LINK_REF">]**</ph> de la notification envoyée à la personne assignée.</target>
</trans-unit>
<trans-unit id="tu36" xml:space="preserve">
<source xml:lang="en-US">Both fields support personalization: click the personalization icon to insert event variables, such as the <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Operator who has replied<ph id="3" ctype="x-LINK_REF">]**</ph> and the <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Response<ph id="7" ctype="x-LINK_REF">]**</ph>, which you can reuse elsewhere in your workflow.</source>
<target xml:lang="en-XX">Les deux champs peuvent être personnalisés : cliquez sur l’icône de personnalisation pour insérer des variables d’événement, telles que l’<ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Opérateur ou opératrice ayant répondu<ph id="3" ctype="x-LINK_REF">]**</ph> et la <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Réponse<ph id="7" ctype="x-LINK_REF">]**</ph>, que vous pouvez réutiliser ailleurs dans votre workflow.</target>
</trans-unit>
<trans-unit id="tu37" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-IMAGE">![</ph>Screenshot showing message personalization<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval2bis.png){zoomable="yes"}</ph></source>
<target xml:lang="en-XX"><ph id="1" ctype="x-IMAGE">![</ph>Capture d’écran affichant la personnalisation du message<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval2bis.png){zoomable="yes"}</ph></target>
</trans-unit>
<trans-unit id="tu38" xml:space="preserve">
<source xml:lang="en-US">Define the possible answers</source>
<target xml:lang="en-XX">Définir les réponses possibles</target>
</trans-unit>
<trans-unit id="tu39" xml:space="preserve">
<source xml:lang="en-US">The activity comes with two default answers, <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Yes<ph id="3" ctype="x-LINK_REF">]**</ph> and <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>No<ph id="7" ctype="x-LINK_REF">]**</ph>. Each answer corresponds to an output transition on the canvas.</source>
<target xml:lang="en-XX">L’activité s’accompagne de deux réponses par défaut : <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Oui<ph id="3" ctype="x-LINK_REF">]**</ph> et <ph id="5" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Non<ph id="7" ctype="x-LINK_REF">]**</ph>. Chaque réponse correspond à une transition sortante sur la zone de travail.</target>
</trans-unit>
<trans-unit id="tu40" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-IMAGE">![</ph>Screenshot showing the Answers section of the Approval activity<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval3.png){zoomable="yes"}</ph></source>
<target xml:lang="en-XX"><ph id="1" ctype="x-IMAGE">![</ph>Capture d’écran affichant la section Réponses de l’activité Validation<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval3.png){zoomable="yes"}</ph></target>
</trans-unit>
<trans-unit id="tu41" xml:space="preserve">
<source xml:lang="en-US">Click <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Add answer<ph id="3" ctype="x-LINK_REF">]**</ph> to define additional choices.</source>
<target xml:lang="en-XX">Cliquez sur <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Ajouter une réponse<ph id="3" ctype="x-LINK_REF">]**</ph> pour définir des choix supplémentaires.</target>
</trans-unit>
<trans-unit id="tu42" xml:space="preserve">
<source xml:lang="en-US">When the assignee answers, the workflow continues through the transition matching their choice.</source>
<target xml:lang="en-XX">Lorsque la personne assignée répond, le workflow se poursuit via la transition correspondant à son choix.</target>
</trans-unit>
<trans-unit id="tu43" xml:space="preserve">
<source xml:lang="en-US">Define an expiration</source>
<target xml:lang="en-XX">Définir une expiration</target>
</trans-unit>
<trans-unit id="tu44" xml:space="preserve">
<source xml:lang="en-US">Finally, you can define an expiration for the approval task. Like an answer, an expiration triggers its own output transition if the assignee has not replied by the deadline.</source>
<target xml:lang="en-XX">Enfin, vous pouvez définir une expiration pour la tâche de validation. Comme une réponse, une expiration déclenche sa propre transition sortante si la personne assignée n’a pas répondu dans le délai.</target>
</trans-unit>
<trans-unit id="tu45" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-IMAGE">![</ph>Screenshot showing the Expiration section of the Approval activity<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval4.png){zoomable="yes"}</ph></source>
<target xml:lang="en-XX"><ph id="1" ctype="x-IMAGE">![</ph>Capture d’écran affichant la section Expiration de l’activité Validation<ph id="2" ctype="x-IMAGE">](../assets/workflow-approval4.png){zoomable="yes"}</ph></target>
</trans-unit>
<trans-unit id="tu46" xml:space="preserve">
<source xml:lang="en-US">Click <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Add expiration<ph id="3" ctype="x-LINK_REF">]**</ph>.</source>
<target xml:lang="en-XX">Cliquez sur <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Ajouter une expiration<ph id="3" ctype="x-LINK_REF">]**</ph>.</target>
</trans-unit>
<trans-unit id="tu47" xml:space="preserve">
<source xml:lang="en-US">Define a <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Label<ph id="3" ctype="x-LINK_REF">]**</ph> for the corresponding output transition.</source>
<target xml:lang="en-XX">Définissez un <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Libellé<ph id="3" ctype="x-LINK_REF">]**</ph> pour la transition sortante correspondante.</target>
</trans-unit>
<trans-unit id="tu48" xml:space="preserve">
<source xml:lang="en-US">In the <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Expiration type<ph id="3" ctype="x-LINK_REF">]**</ph> drop-down, choose one of the following options:</source>
<target xml:lang="en-XX">Dans le menu déroulant <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Type d’expiration<ph id="3" ctype="x-LINK_REF">]**</ph>, choisissez l’une des options suivantes :</target>
</trans-unit>
<trans-unit id="tu49" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Delay after task start<ph id="3" ctype="x-LINK_REF">]**</ph>: Define a delay to wait after the approval task starts.</source>
<target xml:lang="en-XX"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Délai après le début de la tâche<ph id="3" ctype="x-LINK_REF">]**</ph> : définissez un délai d’attente après le début de la tâche de validation.</target>
</trans-unit>
<trans-unit id="tu50" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Delay after a date<ph id="3" ctype="x-LINK_REF">]**</ph>: Define a delay to wait after a specific date.</source>
<target xml:lang="en-XX"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Délai après une date<ph id="3" ctype="x-LINK_REF">]**</ph> : définissez un délai d’attente après une date spécifique.</target>
</trans-unit>
<trans-unit id="tu51" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Delay before a date<ph id="3" ctype="x-LINK_REF">]**</ph>: Define a delay to wait before a specific date.</source>
<target xml:lang="en-XX"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Délai avant une date<ph id="3" ctype="x-LINK_REF">]**</ph> : définissez un délai d’attente avant une date spécifique.</target>
</trans-unit>
<trans-unit id="tu52" xml:space="preserve">
<source xml:lang="en-US"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Expiration calculated by script<ph id="3" ctype="x-LINK_REF">]**</ph>: Use a script to calculate the expiration.</source>
<target xml:lang="en-XX"><ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Expiration calculée par script<ph id="3" ctype="x-LINK_REF">]**</ph> : utilisez un script pour calculer l’expiration.</target>
</trans-unit>
<trans-unit id="tu53" xml:space="preserve">
<source xml:lang="en-US">Enable <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Do not terminate the task<ph id="3" ctype="x-LINK_REF">]**</ph> if you want the expiration transition to be activated without ending the approval task, so the assignee can still reply afterwards.</source>
<target xml:lang="en-XX">Activez l’option <ph id="1" ctype="x-STRONG_EMPHASIS">**[!UICONTROL </ph>Ne pas terminer la tâche<ph id="3" ctype="x-LINK_REF">]**</ph> si vous souhaitez que la transition d’expiration soit activée sans terminer la tâche de validation, de sorte que la personne assignée puisse toujours répondre par la suite.</target>
</trans-unit>
<trans-unit id="tu54" xml:space="preserve">
<source xml:lang="en-US">You can define multiple expirations for the same approval task.</source>
<target xml:lang="en-XX">Vous pouvez définir plusieurs expirations pour la même tâche de validation.</target>
</trans-unit>
<trans-unit id="tu55" xml:space="preserve">
<source xml:lang="en-US">You can then start the workflow. Once the assignee replies, the workflow continues through the transition matching their answer. <ph id="1" ctype="x-LINK">[</ph>Read more<ph id="2" ctype="x-LINK">](#process)</ph></source>
<target xml:lang="en-XX">Vous pouvez ensuite démarrer le workflow. Une fois que la personne assignée a répondu, le workflow se poursuit via la transition correspondant à sa réponse. <ph id="1" ctype="x-LINK">[</ph>En savoir plus<ph id="2" ctype="x-LINK">](#process)</ph></target>
</trans-unit>
<trans-unit id="tu56" xml:space="preserve">
<source xml:lang="en-US">Related topics</source>
<target xml:lang="en-XX">Rubriques connexes</target>
</trans-unit>
<trans-unit id="tu57" xml:space="preserve">
<source xml:lang="en-US">About workflow activities</source>
<target xml:lang="en-XX">À propos des activités de workflows</target>
</trans-unit>
<trans-unit id="tu58" xml:space="preserve">
<source xml:lang="en-US">Set up and manage the approval process</source>
<target xml:lang="en-XX">Configurer et gérer le processus de validation</target>
</trans-unit>
</body>
</file>
</xliff>