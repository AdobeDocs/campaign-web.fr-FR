---
audience: end-user
title: Gestion des modèles de campagne avec Adobe Campaign Web
description: Découvrez comment gérer les modèles de campagne avec Adobe Campaign Web
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 91%

---


# Gestion des modèles de campagne{#manage-campaign-templates}

Toutes les campagnes marketing sont basées sur un modèle qui stocke les principales caractéristiques et fonctionnalités. Campaign est fourni avec un ensemble de modèles intégrés pour vous aider à démarrer. Vous pouvez créer et configurer des modèles d&#39;opération, puis créer des opérations à partir de ces modèles.

## Création d’un modèle d’opération

Pour créer un modèle de campagne, procédez comme suit :

Ouvrez l&#39;Explorateur Campaign et accédez à Ressources > Modèles > Modèles de campagne.
Cliquez sur Nouveau dans la barre d&#39;outils située au-dessus de la liste des modèles.


Vous pouvez également dupliquer le modèle par intégré afin de le réutiliser et d&#39;adapter sa configuration à vos besoins. Pour cela, faites un clic droit sur le modèle et sélectionnez Dupliquer.

Saisissez le libellé du nouveau modèle d&#39;opération.

Cliquez sur Enregistrer, puis rouvrez le modèle.

Dans l&#39;onglet Modifier, définissez les propriétés du modèle.

Sélectionnez le lien Paramètres avancés de l&#39;opération... pour ajouter un workflow à votre modèle d&#39;opération.



Remplacez la valeur Ciblage et workflows par Oui, puis confirmez. Découvrez comment ajouter des fonctionnalités dans cette section.

L&#39;onglet Ciblage et workflows est ajouté au modèle. Cliquez sur Ajouter un workflow..., saisissez un Libellé et cliquez sur Ok.

Créez votre workflow selon vos besoins.



Cliquez sur Enregistrer. Votre modèle est maintenant prêt à être utilisé pour créer une nouvelle campagne.

Les divers onglets et sous-onglets du modèle de campagne vous permettent d&#39;accéder à ses paramètres, qui sont décrits dans la section Configuration générale.

Sélectionnez les modules Le lien Paramètres avancés de l&#39;opération... permet d&#39;activer et désactiver les traitements pour les opérations basées sur ce modèle. Sélectionnez les fonctionnalités à activer dans les campagnes créées à partir de ce modèle.



Si une fonctionnalité n&#39;est pas sélectionnée, les éléments relatifs au processus (menus, icônes, options, onglets, sous-onglets, etc.) n&#39;apparaîtront pas dans l&#39;interface du modèle ou dans les campagnes basées sur celui-ci. Les onglets situés à gauche des détails de la campagne, ainsi que ceux disponibles, coïncident généralement avec les processus sélectionnés dans le modèle. Par exemple, si la fonctionnalité Dépenses et objectifs n&#39;est pas sélectionnée, l&#39;onglet Budget correspondant n&#39;apparaîtra pas dans les campagnes basées sur ce modèle.

De plus, des raccourcis vers les fenêtres de configuration sont ajoutés dans le tableau de bord de la campagne : lorsqu&#39;une fonctionnalité est activée, un lien direct permet d&#39;y accéder depuis le tableau de bord de la campagne.

Modèles de configuration
Par exemple, avec les paramètres suivants :



Le tableau de bord de la campagne affiche :



Notez que l&#39;onglet Ciblage et workflows est manquant.

Les fonctionnalités suivantes sont disponibles :



Notez que l&#39;onglet Budget est manquant.

Les paramètres avancés de la campagne reflètent également cette configuration.



Notez que l&#39;onglet Validations n&#39;est pas disponible.

Avec cette configuration :


Le tableau de bord de la campagne affiche :



Notez que l&#39;onglet Ciblage et workflows est disponible, mais le lien Ajouter un document est manquant.

Les fonctionnalités suivantes sont disponibles :



Notez que l&#39;onglet Budget est disponible.

Les paramètres avancés de la campagne reflètent également cette configuration.



Notez que l&#39;onglet Validations est disponible, mais les onglets Population témoin et Adresses de contrôle ne sont pas activés.

Typologie des modules Population témoin

Lorsque ce module est sélectionné, un onglet supplémentaire est ajouté dans les paramètres avancés du modèle et des opérations basées sur ce modèle. La configuration peut être définie à partir du modèle ou individuellement, au niveau de chaque opération. En savoir plus sur les populations témoins dans cette section.



Adresses de contrôle

Lorsque ce module est sélectionné, un onglet supplémentaire est ajouté dans les paramètres avancés du modèle et des opérations basées sur ce modèle. La configuration peut être définie à partir du modèle ou individuellement, au niveau de chaque opération.



Documents

Lorsque ce module est sélectionné, un onglet supplémentaire est ajouté à l&#39;onglet Modifier du modèle et des campagnes basées sur ce modèle. Les documents attachés peuvent être ajoutés à partir du modèle ou individuellement au niveau de chaque campagne. En savoir plus sur les documents dans cette section.



Composition de diffusion

Lorsque ce module est sélectionné, un sous-onglet Compositions de diffusion est ajouté à l’onglet Documents afin de définir des compositions de diffusion pour l’opération. En savoir plus sur les compositions de diffusion dans cette section.



Ciblages et workflows

Lorsque vous sélectionnez le module Ciblages et workflows, un onglet est ajouté pour vous permettre de créer un ou plusieurs workflows pour les opérations basées sur ce modèle. Les workflows peuvent également être configurés individuellement pour chaque opération en fonction de ce modèle. En savoir plus sur les workflows des opérations dans cette section.



Lorsque ce module est activé, un onglet Traitements est ajouté dans les paramètres avancés de la campagne afin de définir la séquence d&#39;exécution du processus.

Validations

Si vous sélectionnez le module Validations, vous pouvez sélectionner les processus à valider et choisir les opérateurs chargés de leur validation. En savoir plus sur les validations dans cette section.



Vous pouvez choisir d&#39;activer ou non la validation du processus dans l&#39;onglet Validations de la section des paramètres avancés des modèles.

Dépenses et objectifs

Lorsque ce module est sélectionné, un onglet Budget est ajouté dans les détails du modèle et des opérations basées sur ce modèle afin de sélectionner le budget associé.



Propriétés des modèles


Lorsque vous créez un modèle de campagne, vous devez indiquer les informations suivantes :

Saisissez le libellé du modèle : le libellé est obligatoire et constitue le libellé par défaut pour toutes les campagnes basées sur ce modèle.
Sélectionnez la nature de la campagne dans la liste déroulante. Les valeurs proposées dans cette liste correspondent à celles enregistrées dans l&#39;énumération natureOp.
Découvrez comment accéder à vos énumérations et la manière de les configurer sur cette page.

Sélectionnez le type de campagne : unique, récurrente ou périodique. Par défaut, les modèles de campagne s&#39;appliquent aux campagnes uniques. Les opérations périodiques et récurrentes sont décrites dans cette section.

Indiquez la durée de l&#39;opération, c&#39;est-à-dire la période sur laquelle s&#39;étalera l&#39;opération. Lors de la création d&#39;une opération basée sur ce modèle, les dates de début et de fin de l&#39;opération seront alors automatiquement renseignées.

S&#39;il s&#39;agit d&#39;une opération récurrente, vous devez indiquer les dates de début et de fin de l&#39;opération directement dans le modèle.

Indiquez le programme d&#39;appartenance du modèle : les campagnes basées sur le modèle seront associées au programme sélectionné.

