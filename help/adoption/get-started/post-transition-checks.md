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
source-git-commit: 11cf5f2a6e3e77d0747a0b88758ce3fe871e66fd
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 3%
---
# Vérifications et dépannage après la transition {#post-transition-checks}

Après la transition de Campaign Standard vers Campaign v8, certaines diffusions, certains workflows et certaines landing pages peuvent se comporter différemment de vos attentes. Le tableau ci-dessous répertorie les symptômes signalés par les utilisateurs en transition, avec leur cause et les mesures à prendre. Pour obtenir la liste complète des différences, voir [Différences entre Campaign Standard et Campaign v8](acs-v8-differences.md).

| Symptôme | Cause et procédure à suivre | En savoir plus |
|---|---|---|
| Les liens d’une diffusion sont des URL directes et aucune donnée de clic n’est collectée. | Le tracking est désactivé sur la diffusion ou sur le modèle de diffusion sur lequel il est basé. Vérifiez que l&#39;option **Activer le tracking** est activée, en particulier sur les modèles de vos diffusions récurrentes. | [Paramètres de tracking](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| Les destinataires désabonnés via la méthode List-Unsubscribe « mailto » ne sont pas en quarantaine. | Ceci est attendu. Ces destinataires ne sont pas mis en quarantaine. Ils sont désabonnés du service associé à la diffusion ou ajoutés à la place sur la liste bloquée si la diffusion n’a pas de service. Pour suivre ces désabonnements, vérifiez les abonnements du service ou la section **Ne plus contacter** du profil. | [Quarantaines](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Une landing page n’enregistre pas une valeur calculée par un script ou stockée dans un champ masqué. | Les landing pages créées dans l’interface utilisateur web de Campaign ne prennent pas en charge les champs de saisie masqués ou les JavaScript personnalisées. Créez plutôt le formulaire en tant qu’application web dans la console cliente. | [Landing pages](../../v8/landing-pages/get-started-lp.md) |
| **Le transfert de fichier** ne trouve pas le fichier généré par une activité courrier. | La transition sortante d’une activité de publipostage direct concerne la population ciblée, et non le fichier d’extraction. Ajoutez une activité **Extraction de données**, puis l’activité **Transfert de fichier**. | [Publipostage direct](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Plusieurs vagues d’une diffusion sont envoyées ensemble. | Les vagues sont planifiées à partir de la date de contact de la diffusion. Si la diffusion démarre après l’heure prévue de certaines vagues, ces vagues sont envoyées ensemble au lieu d’être espacées. | [Envoyer par vagues](../../v8/advanced-settings/send-using-waves.md) |
| Un masque de fichier avec des caractères après l’astérisque ne trouve aucun fichier dans le stockage Blob Azure. | Le stockage Blob d’Azure filtre les fichiers par préfixe de nom. Seul un astérisque de fin est pris en charge. | [Transférer le compte externe](../../v8/administration/transfer-external-account.md) |
| Une page miroir d’une diffusion envoyée avant que la transition ne s’ouvre pas. | Les pages miroir des diffusions envoyées depuis Campaign Standard avant la transition ne sont pas disponibles et il n’existe aucune solution de contournement. Les pages miroir des diffusions envoyées à partir de Campaign v8 fonctionnent comme d’habitude. | [Pages miroir](../../v8/email/mirror-page.md) |
| Une page de destination ou un bloc de contenu qui utilise un JavaScript personnalisé se comporte différemment. | Le JavaScript personnalisé est transformé lors de la migration, mais il doit être validé et ajusté, en particulier s’il utilise `queryDef`, les API JavaScript de Campaign, les écritures de session, la gestion des entités organisationnelles ou la génération d’URL personnalisée. | [Landing pages](../../v8/landing-pages/get-started-lp.md) |
