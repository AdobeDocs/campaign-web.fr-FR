---
audience: end-user
title: Configuration et gestion du processus de validation
description: Découvrez comment gérer les validations des campagnes marketing dans Campaign Web.
feature: Approvals, Campaigns
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 4%

---

# Gérer le processus de validation {#campaign-approvals}

>[!IMPORTANT]
>
>Les validations ne sont disponibles que pour les diffusions créées dans une campagne. Cela ne s’applique pas aux diffusions autonomes ou aux diffusions créées dans des workflows en dehors d’un contexte de campagne.

Le processus de validation permet de coordonner plusieurs parties prenantes et d’assurer un contrôle qualité avant l’envoi des diffusions. Utilisez les validations lorsque votre organisation nécessite la validation de différentes équipes, telles que les responsables marketing qui examinent le contenu ou les analystes de données qui valident les audiences cibles.

Lorsque les validations sont activées, vous devez soumettre le contenu ou la cible à la validation. Les réviseurs et réviseuses désignés reçoivent des notifications par e-mail demandant la validation et peuvent les approuver ou les refuser directement depuis l’interface utilisateur web. Les diffusions ne peuvent pas être envoyées tant que toutes les validations requises n’ont pas été accordées. Vous pouvez activer :

* **Validation du contenu** : validation du contenu, de la conception et de la personnalisation du message
* **Validation de la cible** : validez l&#39;audience et les critères de ciblage
* **Confirmation de diffusion** : demandez une confirmation finale avant l&#39;envoi.

## Configuration des paramètres d’approbation {#configure-approvals}

Les paramètres de validation sont hérités du modèle de campagne et peuvent être modifiés pour chaque campagne. Pour configurer les paramètres d’approbation, procédez comme suit :

1. Ouvrez votre campagne ou votre modèle de campagne, ou créez-en un, à partir du menu **[!UICONTROL Campagnes]**.

1. Cliquez sur le bouton **[!UICONTROL Paramètres]** en haut à droite du tableau de bord de la campagne.

1. Dans la section **[!UICONTROL Validations]**, configurez les options suivantes :

   ![Capture d’écran affichant les paramètres de validation de la campagne](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Activer la validation du contenu]** : lorsqu&#39;elle est activée, le contenu de la diffusion doit être validé avant envoi. Cliquez sur l’icône de dossier dans le champ **[!UICONTROL Réviseur]** pour sélectionner un opérateur ou un groupe d’opérateurs.

   * **[!UICONTROL Activer la validation de la cible]** : lorsqu&#39;elle est activée, l&#39;audience cible de la diffusion doit être validée. Cliquez sur l’icône de dossier dans le champ **[!UICONTROL Réviseur]** pour sélectionner un opérateur ou un groupe d’opérateurs.

   * **[!UICONTROL Confirmer la diffusion avant l&#39;envoi]** : nécessite une confirmation manuelle finale avant l&#39;envoi, même après toutes les autres validations.

>[!NOTE]
>
>* Si aucun réviseur n’est spécifié, le propriétaire de la campagne est affecté en tant que réviseur.
>* Les réviseurs ont besoin des autorisations appropriées pour approuver les diffusions. Seuls les utilisateurs identifiés dans la liste des réviseurs peuvent approuver.

## Soumettre à validation {#submit-approval}

Une fois votre diffusion créée, procédez comme suit pour envoyer le contenu et la cible pour validation.

>[!NOTE]
>Les validations sont disponibles à la fois dans les diffusions de workflow de campagne et dans les diffusions autonomes de campagne.

1. Dans le tableau de bord de la diffusion, cliquez sur le bouton **[!UICONTROL Soumettre le contenu]**. Les réviseurs et réviseuses désignés peuvent approuver ou refuser. Consultez cette [section](#approve-reject).

   ![Capture d’écran affichant le bouton Envoyer le contenu](assets/approvals2.png){zoomable="yes"}

   Le statut de validation passe à en attente dans la section **[!UICONTROL Propriétés]** du tableau de bord de la diffusion. Consultez cette [section](#rack-approvals).

1. Une fois le contenu validé, cliquez sur le bouton **[!UICONTROL Préparer]** pour préparer la cible de la diffusion. Le système prépare l’audience et les critères de ciblage.

1. Cliquez sur le bouton **[!UICONTROL Soumettre la cible]**. Les réviseurs et réviseuses désignés peuvent alors approuver ou rejeter le projet. Consultez cette [section](#approve-reject).

   ![Capture d’écran affichant le bouton Envoyer la cible](assets/approvals5.png){zoomable="yes"}

   Le statut d’approbation passe à en attente. Consultez cette [section](#rack-approvals).

1. Une fois la cible validée, la préparation reprend et la diffusion peut être envoyée.

>[!NOTE]
>Si une validation est refusée, le propriétaire de la diffusion doit apporter toutes les modifications nécessaires au contenu ou à la cible en fonction des commentaires du validant et effectuer une nouvelle soumission pour validation.

## Approuver ou rejeter {#approve-reject}

Les réviseurs et réviseuses désignés peuvent approuver ou rejeter les envois de contenu et de cible. Consultez cette [section](#submit-approval).

>[!NOTE]
>Pour que l’e-mail de notification soit envoyé, l’adresse du réviseur ou de la réviseuse doit être configurée dans l’instance .

1. Lorsque vous recevez l’e-mail de notification, ouvrez la diffusion qui nécessite une approbation directement depuis l’interface utilisateur web.

1. Examinez le contenu ou les informations sur la cible.

1. Cliquez sur le bouton **[!UICONTROL Approuver le contenu]** ou **[!UICONTROL Approuver la cible]**.

   ![Capture d’écran affichant le bouton Approuver le contenu dans le tableau de bord de la diffusion](assets/approvals3.png){zoomable="yes"}

1. Cliquez sur **[!UICONTROL Approuver]** ou **[!UICONTROL Rejeter]**.

1. Vous pouvez éventuellement ajouter un **[!UICONTROL Commentaire]** pour expliquer votre décision.

   ![ Capture d’écran affichant la boîte de dialogue d’approbation avec les boutons Approuver, Rejeter et le champ Commentaire ](assets/approvals4.png){zoomable="yes"}

1. Confirmez votre décision. Le statut de validation est immédiatement mis à jour dans le tableau de bord de la diffusion. Consultez cette [section](#rack-approvals).

## Suivi du statut de validation {#track-approvals}

Le statut de validation est visible dans la section **[!UICONTROL Propriétés]** du tableau de bord de la diffusion. Le statut affiche les validations en attente et leur statut actuel :

![Capture d’écran affichant le statut d’approbation](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL En édition]** : le contenu ou la cible n&#39;a pas encore été soumis à validation
* **[!UICONTROL En attente de validation]** : le contenu ou la cible est en attente de validation
* **[!UICONTROL Validé]** : le contenu ou la cible a été validé(e) par le validant
* **[!UICONTROL Rejeté]** : le contenu ou la cible a été rejeté par le validant

La section validation affiche toutes les validations et mises à jour activées en temps réel, à mesure que les réviseurs valident ou rejettent chaque étape.

## Rubriques connexes : {#related}

* [Créer des campagnes](create-campaigns.md)
* [Gérer les campagnes](manage-campaigns.md)
