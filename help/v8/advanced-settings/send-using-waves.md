---
audience: end-user
title: Envoyer par vagues
description: En savoir plus sur les paramètres de diffusion dans Campaign Web.
badge: label="Disponibilité limitée"
source-git-commit: 1d3e2ccbf4db5eb23531351572a4400754982e2d
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 53%

---


# Envoyer par vagues {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Définition des vagues"
>abstract="Définissez des vagues pour fractionner les diffusions en plusieurs lots au lieu d’envoyer de gros volumes de messages en même temps."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Taille de la vague"
>abstract="La taille de la vague est requise. Saisissez une valeur numérique (nombre de messages) ou un pourcentage (0 à 100 %) dans le champ Taille."

Pour équilibrer la charge, vous pouvez répartir les envois en plusieurs lots. Configurez le nombre de lots et leur proportion par rapport à l&#39;ensemble de la diffusion.

>[!NOTE]
>
>Vous pouvez uniquement définir la taille et le délai entre deux vagues consécutives. Le critère de sélection des destinataires pour chaque vague n&#39;est pas paramétrable.

1. Ouvrez le [paramètres de diffusion](delivery-settings.md#retries) et accédez au **[!UICONTROL Diffusion]** .
1. Sélectionnez l&#39;option **[!UICONTROL Envoyer en plusieurs vagues]**, puis cliquez sur le lien **[!UICONTROL Définition des vagues...]**.

1. Pour configurer des vagues, vous pouvez effectuer l&#39;une des opérations suivantes :

   * **[!UICONTROL Planification de plusieurs vagues de même taille]**. Par exemple, si vous saisissez **[!UICONTROL 30 %]** dans le champ correspondant, chaque vague représentera 30% des messages inclus dans la diffusion, à l&#39;exception de la dernière vague, qui représentera 10% des messages.

     Dans le **[!UICONTROL Intervalle]** , indiquez le délai entre le démarrage de deux vagues consécutives. Par exemple, si vous saisissez **[!UICONTROL 2d]**, la première vague démarrera immédiatement, la deuxième démarrera dans deux jours, la troisième dans quatre jours, etc.

   * **[!UICONTROL Planification des vagues selon un calendrier]**.

     Dans le **[!UICONTROL Début]** , indiquez le délai entre le démarrage de deux vagues consécutives. Dans le **[!UICONTROL Taille]** , saisissez un nombre fixe ou un pourcentage.

     Dans l&#39;exemple ci-dessous, la première vague représente 25 % du nombre total des messages inclus dans l&#39;envoi et démarre immédiatement. Les deux vagues suivantes terminent l&#39;envoi et sont définies pour démarrer à six heures d&#39;intervalle.

     une règle de contrôle de typologie spécifique, **[!UICONTROL Vérification de la planification des vagues]**, assure que la dernière vague est planifiée avant la limite de validité de la diffusion. Les typologies de campagne et leurs règles sont configurées dans la variable **[!UICONTROL Typologie]** de l’onglet des paramètres de diffusion. En savoir plus sur les règles de contrôle dans [Documentation de Campaign v8 (console cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html)

     >[!IMPORTANT]
     >
     >Veillez à ce que les dernières vagues ne dépassent pas la date limite de diffusion, définie dans la variable **[!UICONTROL Validité]** . Sinon, certains messages peuvent ne pas être envoyés. [En savoir plus](delivery-settings.md#validity)
     >
     >Lors de la configuration des dernières vagues, veillez également à prévoir assez de temps pour les reprises. [En savoir plus](delivery-settings.md#retries)

1. Pour surveiller vos envois, accédez à la [logs de diffusion](../monitor/delivery-logs.md).

Vous pouvez visualiser les diffusions qui ont déjà été envoyées dans les vagues traitées (statut **[!UICONTROL Envoyé]**) et celles à envoyer dans les vagues restantes (statut **[!UICONTROL En attente]**).

Les deux exemples ci-dessous constituent les cas d&#39;utilisation les plus fréquents de plusieurs vagues.

* **Lors de la phase de démarrage**

  Lorsque vous envoyez des emails à l&#39;aide d&#39;une nouvelle plateforme, rien n&#39;est plus suspect pour un FAI (fournisseur d&#39;accès internet) que les adresses IP qui ne sont pas reconnues. Si des emails sont subitement envoyés en masse, le FAI les range souvent dans le courrier indésirable.

  Pour éviter que les emails soient marqués comme spam, vous pouvez augmenter progressivement le volume envoyé à l&#39;aide de vagues. Cela permet d&#39;entamer la phase de démarrage en douceur et de réduire le nombre total d&#39;adresses invalides.

  Pour ce faire, utilisez l&#39;option **[!UICONTROL Planifier les vagues selon un calendrier]**. Par exemple, définissez la première vague sur 10 %, la deuxième sur 15 %, etc.

* **Campagnes impliquant un centre d&#39;appels**

  Lorsque vous gérez une campagne téléphonique de fidélisation, votre entreprise a une capacité de traitement des appels limitée pour contacter les abonnés.

  Grâce aux vagues, vous pouvez limiter le nombre des messages à 20 par jour, ce qui correspond à la capacité de traitement quotidien d&#39;un centre d&#39;appels.

  Pour ce faire, sélectionnez l’option **[!UICONTROL Planification de plusieurs vagues de même taille]** . Entrée **[!UICONTROL 20]** comme la taille de la vague et **[!UICONTROL 1d]** dans le **[!UICONTROL Période]** champ .