---
title: Branding
description: Découvrir tous les outils disponibles pour gérer les identités de branding
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: f6438303-5ae8-47c6-8c34-8e586f4b6fe7
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: ht
source-wordcount: '332'
ht-degree: 100%

---

# Commencer avec le branding {#branding-gs}

>[!AVAILABILITY]
>
>Cette fonctionnalité est uniquement disponible à la demande pour les nouvelles implémentations. Pour y accéder, contactez votre représentant ou représentante Adobe.


>[!IMPORTANT]
>
>Les marques ne peuvent pas être créées ni modifiées par des utilisateurs et utilisatrices finaux : ces opérations doivent être effectuées par l’administrateur ou administratrice technique Adobe Campaign. Pour toute demande, contactez l&#39;Assistance clientèle Adobe.

Chaque entreprise dispose de directives de marque qui définissent à la fois des éléments visuels et des détails techniques. Adobe Campaign vous aide à gérer ces directives de manière centralisée, afin que vous puissiez présenter à vos clientes et clients une image de marque cohérente dans tout ce que vous faites, des logos contenus dans les e-mails aux URL et domaines utilisés dans vos campagnes.

Les administrateurs et administratrices techniques peuvent créer et gérer plusieurs marques dans Adobe Campaign. Vous pouvez ainsi définir tous les éléments qui constituent votre identité de marque, y compris les logos et même les paramètres de tracking e-mail. Une fois créées, ces marques peuvent être facilement liées à vos diffusions.

Vous pouvez ajouter de nouvelles entités de votre organisation dans Campaign ou créer un nouveau type d’e-mail que vous devez envoyer sous un autre sous-domaine. Pour ce faire, suivez les étapes ci-après :

1. **Configurer un nouveau sous-domaine** - Pour tout nouveau sous-domaine utilisé par Adobe, la première étape consiste à le configurer. Vous pouvez effectuer cette opération via le [Panneau de contrôle Campaign](https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html?lang=fr) ou contacter votre contact technique Adobe. Pour en savoir plus sur la configuration de sous-domaine, consultez [cette page](https://experienceleague.adobe.com/fr/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/campaign/ac-domain-name-setup).

   >[!NOTE]
   >
   >Le Panneau de contrôle est accessible à tous les utilisateurs administrateurs. Les étapes permettant d&#39;octroyer un accès administrateur à un utilisateur sont présentées sur [cette page](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=fr#discover-control-panel).

1. **Créer un modèle de diffusion** - Une fois la nouvelle marque disponible, il est recommandé de créer au moins un modèle de diffusion vierge qui fait référence à cette nouvelle marque. [En savoir plus](branding-assign.md).

1. **Vérifier les instructions relatives à la délivrabilité** : avant de commencer à utiliser le nouveau domaine, la stratégie doit être discutée avec l&#39;équipe Adobe chargée de la délivrabilité Elle aidera à définir les bonnes pratiques, si une nouvelle affinité doit être créée pour fractionner les adresses IP entre les domaines par exemple, et/ou si un plan de propagation doit être défini.
