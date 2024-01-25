---
title: Créer un profil
description: Découvrez comment créer un profil sur le Web de Campaign.
badge: label="Disponibilité limitée"
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: 22b183a739dd92d7c4245fb4694034a247511d75
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 56%

---

# Créer un profil {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Détails de base"
>abstract="Cette section fournit des informations sur les détails de base du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Coordonnées"
>abstract="Cette section fournit des informations sur les coordonnées du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Adresse"
>abstract="Cette section fournit des informations sur l’adresse postale du profil et la qualité de l’adresse. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Détails du compte"
>abstract="Cette section fournit des informations sur les détails du compte du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Destinataires : ne plus contacter"
>abstract="Cette section fournit des informations sur les préférences de contact du profil. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Champs personnalisés"
>abstract="Les champs personnalisés sont des attributs spécifiques, adaptés à vos besoins, qui ont été configurés pour votre instance. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Autres"
>abstract="Cette section fournit des attributs intégrés supplémentaires. Pour modifier des informations, apportez vos modifications directement dans le champ correspondant, puis cliquez sur le bouton **Enregistrer** situé dans le coin supérieur droit de l’écran."

Pour créer un profil, procédez comme suit :

1. Accédez à **[!UICONTROL Gestion des clients]** > **[!UICONTROL Profils]** et cliquez sur le bouton **[!UICONTROL Créer un profil]** dans le coin supérieur droit de l’écran.

1. La liste des attributs disponibles pour l&#39;affichage du profil, organisée en différentes sections détaillées dans le tableau ci-dessous.

   ![](assets/create-profile.png)

   | Section Attributs | Description |
   |  ---  |  ---  |
   | **Détails de base** | Informations de base sur le profil, telles que le nom ou la date de naissance.<br/>Par défaut, les profils sont stockés dans la variable **[!UICONTROL Destinataires]** dossier. Vous pouvez le modifier en accédant à l’emplacement souhaité. [Découvrez comment utiliser les dossiers](../get-started/permissions.md#folders) |
   | **Coordonnées** | Les coordonnées du profil, telles que l’adresse électronique ou le numéro de téléphone. |
   | **Adresse** | Adresse postale du profil. Cette section fournit également une évaluation de la qualité des adresses. L&#39;adresse d&#39;un profil est considérée comme valide si les champs &#39;Nom&#39;, &#39;Ville&#39; et &#39;Code postal&#39; sont renseignés. |
   | **Détails du compte** | Informations sur le compte du profil, telles que son statut ou son numéro de compte. |
   | **Ne plus contacter** | Les préférences de contact du profil. Lorsque l’une de ces options est sélectionnée, le profil est en liste bloquée.<br/>Par exemple, si le destinataire a cliqué sur un lien de désinscription dans une newsletter, ces informations sont ajoutées aux données de contact. Cette personne n’est plus ciblée sur le ou les canaux sélectionnés. En savoir plus sur la gestion des quarantaines dans [Documentation d’Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=fr){target="_blank"} |
   | **Champs personnalisés** | Si des champs personnalisés ont été configurés, ils s’affichent dans cette section. Les champs personnalisés sont des attributs supplémentaires ajoutés au schéma **[!UICONTROL Profils]** via la console Adobe Campaign. En savoir plus dans la section [Documentation d’Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=fr){target="_blank"} |
   | **Autres** | Attributs intégrés supplémentaires. |

1. Une fois le profil configuré, cliquez sur **[!UICONTROL Créer]** pour l’enregistrer dans la base de données.

   Une fois terminé, vous pouvez modifier le profil à tout moment en l’ouvrant à partir de la liste des profils. [Découvrez comment explorer les détails des profils](profile-view.md)
