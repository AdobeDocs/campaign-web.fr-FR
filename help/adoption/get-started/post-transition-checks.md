---
title: Vérifications et dépannage après la transition vers Campaign v8
description: Découvrez les éléments à vérifier et comment résoudre les problèmes courants après la transition de Campaign Standard vers Campaign v8
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 8b78a8494223fbcd3def29c955e6171cbb643fef
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 2%
---
# Vérifications et dépannage après la transition {#post-transition-checks}

Après la transition de Campaign Standard vers Campaign v8, certaines diffusions, certains workflows et certaines landing pages peuvent se comporter différemment de vos attentes. Le tableau ci-dessous répertorie les symptômes signalés par les utilisateurs en transition, avec leur cause et les mesures à prendre. Pour obtenir la liste complète des différences, voir [Différences entre Campaign Standard et Campaign v8](acs-v8-differences.md).

| Symptôme | Cause et procédure à suivre | En savoir plus |
|---|---|---|
| Les liens d’une diffusion sont des URL directes et aucune donnée de clic n’est collectée. | Le tracking est désactivé sur la diffusion ou sur le modèle de diffusion sur lequel il est basé. Vérifiez que l&#39;option **Activer le tracking** est activée, en particulier sur les modèles de vos diffusions récurrentes. | [Paramètres de tracking](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| Les destinataires désabonnés via la méthode List-Unsubscribe « mailto » ne sont pas en quarantaine. | Ceci est attendu. Ces destinataires ne sont pas mis en quarantaine. Ils sont désabonnés du service associé à la diffusion ou ajoutés à la place sur la liste bloquée si la diffusion n’a pas de service. Pour suivre ces désabonnements, vérifiez les abonnements du service ou la section **Ne plus contacter** du profil. | [Quarantaines](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Une landing page n’enregistre pas une valeur calculée par un script ou stockée dans un champ masqué. | Les landing pages créées dans l’interface utilisateur web de Campaign ne prennent pas en charge les champs de saisie masqués ou les JavaScript personnalisées. Créez plutôt le formulaire en tant qu’application web dans la console cliente. | [Landing pages](../../v8/landing-pages/get-started-lp.md) |
| **Le transfert de fichier** ne trouve pas le fichier généré par une activité courrier. | La transition sortante d’une activité de publipostage direct concerne la population ciblée, et non le fichier d’extraction. Ajoutez une activité **Extraction de données**, puis l’activité **Transfert de fichier**. | [Publipostage direct](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Plusieurs vagues d’une diffusion sont envoyées ensemble. | Les vagues sont planifiées à partir de la date de contact de la diffusion. Si la diffusion démarre après l’heure prévue de certaines vagues, ces vagues sont envoyées ensemble au lieu d’être espacées. | [Envoyer par vagues](../../v8/advanced-settings/send-using-waves.md) |
| Un masque de fichier avec des caractères après l’astérisque ne trouve aucun fichier dans le stockage Blob Azure. | Le stockage Blob d’Azure filtre les fichiers par préfixe de nom. Seul un astérisque de fin est pris en charge. | [Transférer le compte externe](../../v8/administration/transfer-external-account.md) |
| Une page de destination ou un bloc de contenu qui utilise un JavaScript personnalisé se comporte différemment. | Le JavaScript personnalisé est transformé lors de la migration, mais il doit être validé et ajusté, en particulier s’il utilise `queryDef`, les API JavaScript de Campaign, les écritures de session, la gestion des entités organisationnelles ou la génération d’URL personnalisée. | [Landing pages](../../v8/landing-pages/get-started-lp.md) |
| Un appel de l’API REST renvoie une valeur vide, une erreur ou une réponse inattendue. | Certains champs de la base de données sont ignorés lors de la migration et renvoient des valeurs vides. Un PATCH vide renvoie 204, et un PATCH sur l’emplacement renvoie 500. Une requête POST avec une ressource liée ignore le lien ou renvoie une erreur. Une PKEY non valide renvoie 404. | [Limites de l’API REST](acs-v8-differences.md#rest-api-limitations) |
| Une PKEY stockée ne fonctionne plus dans les appels API. | Les valeurs PKEY changent après la migration. Ne les stockez pas en dehors de Campaign. À partir de chaque appel des arborescences renvoyées par l’appel précédent. | [Utilisation des clés](acs-v8-differences.md#key-usage) |
| Le fuseau horaire ou `ccpaOptOut` est absent d&#39;une réponse de profil. | Ces champs sont renvoyés uniquement par `profileAndServicesExt/profile`, et non par `profileAndServices/profile`. Appelez le point d’entrée étendu. | [Fuseau horaire du profil et ccpaOptOut](acs-v8-differences.md#profile-timezone) |
| Un filtre personnalisé renvoie une erreur dans un appel de l’API REST. | Dans Campaign v8, attribuez un nom au filtre dans le champ **Nom du filtre dans l’API REST** et utilisez ce nom tel quel dans la requête, sans le préfixe « par ». | [Filtrage](acs-v8-differences.md#rest-filtering) |
| Un appel qui déclenche un signal externe de workflow ne peut pas créer son corps de requête. | L’API GET de workflow ne renvoie plus les variables de workflow. Créez les paramètres du corps de la requête POST à partir de vos propres connaissances du workflow. | [Signaux externes de workflow](acs-v8-differences.md#workflow-signals) |
| L&#39;accès aux API transactionnelles est refusé. | L&#39;accès aux API transactionnelles à partir de l&#39;instance d&#39;exécution nécessite un nouveau profil de produit. Examinez le mappage des profils de produit de vos comptes techniques. | [Mappage du profil de produit](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Une audience migrée affiche uniquement la dernière valeur ou une audience de fichier n’a pas de dimensions. | Ceci est attendu. Un filtre prédéfini prend uniquement la dernière valeur après la migration de l’audience et les audiences de type fichier deviennent des audiences de type Liste sans dimensions. | [Gérer les audiences](marketers.md#acs-gs-marketers-audiences) |
| L&#39;historique des workflows exécutés dans Campaign Standard est vide. | Les logs historiques des workflows exécutés dans Campaign Standard ne sont pas migrés. Les workflows exécutés dans Campaign v8 ont leur propre historique et leurs propres journaux. | [Créer un workflow](marketers.md#acs-gs-marketers-wf) |
| Certains utilisateurs peuvent voir ou faire plus qu’auparavant. | Les utilisateurs dotés du rôle **Modèle de données** mais pas du rôle **Administration** obtiennent un accès **Administration** et les groupes de sécurité dotés d’entités organisationnelles parallèles peuvent bénéficier d’un accès plus étendu. Vérifiez les groupes d’opérateurs, les droits nommés et les autorisations de dossiers. | [Gestion des accès utilisateur](user-management-acs.md) |
| Un profil de test marqué comme **Interruption** ne reçoit pas l’envoi final. | Dans Campaign v8, ajoutez un **groupe de pièges** dans les paramètres Audience de la diffusion. | [Groupe de pièges](../../v8/audience/trap-group.md) |
| Un email récurrent n’a pas d’option de période d’agrégation. | Cette option n’est pas disponible dans Campaign v8. | [Activités de canal](../../v8/workflows/activities/channels.md) |
| Les rapports dynamiques n’affichent aucune donnée pour une diffusion. | Les rapports dynamiques couvrent les diffusions par e-mail, les campagnes avec des diffusions par e-mail et les messages transactionnels. | [Reporting](marketers.md#acs-gs-marketers-reporting) |
