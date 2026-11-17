---
title: Différences entre Campaign Standard et Campaign v8
description: Découvrez ce qui change lorsque vous passez de Campaign Standard à Campaign v8 et où trouver les détails
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
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 982fb1a5060db5b4eac6c6f68487116d9a72e109
workflow-type: tm+mt
source-wordcount: '1926'
ht-degree: 5%
---
# Différences entre Campaign Standard et Campaign v8 {#acs-v8-differences}

La plupart des concepts sont identiques dans Campaign Standard et Campaign v8. Cette page rassemble les différences qui vous affectent après la transition et fournit des liens vers la page qui explique chacune d’elles. Il complète les guides destinés aux [professionnels du marketing](marketers.md) et aux [administrateurs et développeurs](admin-developers.md).

* Pour les modifications terminologiques, voir [Terminologie](#terminology).
* Pour connaître les vérifications à exécuter et les problèmes signalés après une transition, voir [Vérifications et dépannage après la transition](post-transition-checks.md).
* Pour connaître les fonctionnalités disponibles uniquement dans la console cliente, voir [Console cliente Campaign Web et Campaign](../../v8/get-started/capability-matrix.md).

## Terminologie {#terminology}

La plupart des concepts sont similaires entre Adobe Campaign v8 et Adobe Campaign Standard. Cependant, il existe quelques différences, à commencer par la terminologie.

| Dans Campaign Standard | Dans Campaign v8 |
|---|---|
| Ressources personnalisées | **Schémas** |
| Messages | **Diffusions** |
| Utilisateurs du produit | **Opérateurs** |
| Rôles | Configuré avec **Droits nommés** |
| Groupes de sécurité | **Groupes d&#39;opérateurs** |
| Entités organisationnelles | Géré via **Autorisations de dossier** |

De plus, en tant que personne utilisant déjà Campaign, notez que certains concepts ont été renommés pour s’aligner sur les dernières normes terminologiques. Ces modifications s’appliquent uniquement à l’interface utilisateur web de Campaign et ne sont pas répercutées dans la console cliente.

| Dans Campaign Standard | Dans Campaign Web | En savoir plus |
|---|---|---|
| Destinataires | **Profils** | [Profils](../../v8/audience/gs-audiences-recipients.md) |
| Adresses de contrôle | **Profils de test** | [Tester les diffusions](../../v8/preview-test/test-deliveries.md) |
| Analyse des diffusions | **Préparation de la diffusion**. Pour lancer la préparation du message, cliquez sur le bouton **Préparer**. | [Préparer et envoyer](../../v8/monitor/prepare-send.md) |
| Aperçu de l’e-mail | Disponible via le bouton **Simuler du contenu**. | [Prévisualiser et tester](../../v8/preview-test/preview-test.md) |
| Listes | **Audiences** | [Audiences](../../v8/audience/gs-audiences-recipients.md) |

## Canaux et contenu {#channels}

Les étapes de création et d&#39;envoi des messages sont similaires dans les deux produits, comme décrit dans le [guide pour les professionnels du marketing](marketers.md). Les différences ci-dessous concernent la disponibilité du canal, les diffusions de test, les landing pages et les workflows de publipostage direct.

| Changements | En savoir plus |
|---|---|
| Le canal In-App n’est pas disponible dans Campaign v8. | [Canal In-App](marketers.md#acs-gs-marketers-in-app) |
| Pour effectuer la transition des workflows et des diffusions de notifications push existants, contactez votre gestionnaire de transition Adobe Campaign. | [Notifications push](marketers.md#acs-gs-marketers-push) |
| Dans Campaign Standard, un profil de test peut être marqué comme un **piège** pour recevoir l’envoi final. Dans Campaign v8, ajoutez un **groupe de pièges** dans les paramètres Audience de la diffusion. | [Groupe de pièges](../../v8/audience/trap-group.md) |
| Les landing pages créées dans l’interface utilisateur web de Campaign ne prennent pas en charge les champs de saisie masqués ou les JavaScript personnalisées. | [Landing pages](../../v8/landing-pages/get-started-lp.md) |
| Dans Campaign Standard, la transition sortante d’une activité de publipostage direct comportait également le fichier généré. Dans Campaign v8, elle ne transporte que la population ciblée. Pour envoyer le fichier à un serveur, ajoutez une activité **Extraction de données**, puis une activité **Transfert de fichier**. | [Publipostage direct](https://experienceleague.adobe.com/fr/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Audiences, workflows et diffusions {#data-and-workflows}

Ces différences affectent les audiences et les workflows migrés depuis Campaign Standard, certaines options de diffusions récurrentes et de l&#39;activité **Transfert de fichier**, ainsi que la portée des rapports dynamiques.

| Changements | En savoir plus |
|---|---|
| Les audiences créées avec l’activité Requête dans Campaign Standard deviennent des [filtres prédéfinis](../../v8/query/build-query.md) dans Campaign v8. Campaign v8 prend également en charge l’activité Requête . | [Gérer les audiences](marketers.md#acs-gs-marketers-audiences) |
| Une activité Lecture d’audience devient une activité Requête avec un filtre prédéfini. | [Gérer les audiences](marketers.md#acs-gs-marketers-audiences) |
| Un filtre prédéfini ne prend que la dernière valeur une fois l’audience migrée. | [Gérer les audiences](marketers.md#acs-gs-marketers-audiences) |
| Les audiences de type fichier deviennent des audiences de type liste sans dimensions. | [Gérer les audiences](marketers.md#acs-gs-marketers-audiences) |
| Les logs historiques des workflows exécutés dans Campaign Standard ne sont pas migrés. | [Créer un workflow](marketers.md#acs-gs-marketers-wf) |
| Dans Campaign Standard, vous pouvez sélectionner la période d’agrégation d’un e-mail récurrent. Cette option n’est pas disponible dans Campaign v8. | [Activités de canal](../../v8/workflows/activities/channels.md) |
| Les rapports dynamiques couvrent les diffusions par e-mail, les campagnes avec des diffusions par e-mail et les messages transactionnels. | [Reporting](marketers.md#acs-gs-marketers-reporting) |

## Accès et sécurité {#access}

Les groupes de sécurité, les rôles et les entités organisationnelles de Campaign Standard sont associés aux groupes d’opérateurs, aux droits nommés et aux autorisations de dossiers pendant la transition. Examinez les points ci-dessous, en particulier si certains utilisateurs disposent de droits plus larges ou plus étroits qu’auparavant.

| Changements | En savoir plus |
|---|---|
| Les groupes de sécurité, les rôles et les entités organisationnelles sont associés aux groupes d&#39;opérateurs, aux droits nommés et aux autorisations de dossiers. Les rôles personnalisés ne sont pas migrés. | [Gestion des accès utilisateur](user-management-acs.md) |
| Les utilisateurs dotés du rôle **Modèle de données** mais pas du rôle **Administration** obtiennent un accès **Administration**. | [Gestion des accès utilisateur](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Les utilisateurs affectés à des groupes de sécurité avec des entités organisationnelles parallèles peuvent bénéficier d&#39;un accès plus étendu dans Campaign v8. | [Affectation parallèle d’une entité organisationnelle](user-management-acs.md#parallel-assignments) |
| L&#39;accès aux API transactionnelles à partir de l&#39;instance d&#39;exécution nécessite un nouveau profil de produit. | [Mappage du profil de produit](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Les demandes d’accès à des informations personnelles peuvent arriver dans Campaign Standard et Campaign v8 pendant la période où votre environnement Campaign Standard reste actif. | [Informations personnelles et consentement](admin-developers.md#privacy-and-consent) |

## API et intégrations {#apis-and-integrations}

Ces différences affectent les intégrations qui appellent Campaign par le biais de son API REST, ainsi que les intégrations à d&#39;autres solutions et outils Adobe.

| Changements | En savoir plus |
|---|---|
| Les valeurs PKEY changent après la migration. Si vous stockez des PKEY en dehors de Campaign, suivez plutôt les arborescences renvoyées par l’API . | [Utilisation des clés](#key-usage) |
| Certains champs de profil migrés, tels que le fuseau horaire et `ccpaOptOut`, sont renvoyés uniquement par l’API `profileAndServicesExt/profile`. | [Fuseau horaire du profil et ccpaOptOut](#profile-timezone) |
| Adobe migre vos configurations Adobe Analytics et Audience Manager. Vous devez configurer à nouveau les intégrations Triggers et Adobe Target. | [Gestion des intégrations Adobe Campaign](admin-developers.md#acs-gs-integrations) |

## Recommandations et limitations de l’API REST {#rest-api-limitations}

Les recommandations et limitations ci-dessous s’appliquent aux API REST lorsque vous passez de Campaign Standard à Campaign v8.

### Autorisations et sécurité {#permissions}

#### Mappage des profils de produit {#rest-product-profiles}

Dans Campaign Standard, vous avez obtenu un accès élevé au rôle d’administrateur aux API, quel que soit le profil de produit qui vous a été attribué. Campaign v8 introduit un ensemble différent de profils de produit, ce qui nécessite de mapper les profils de produits Campaign Standard aux profils de produits Campaign v8.

Avec la migration, deux profils de produit sont ajoutés à vos comptes techniques existants ou précréés : Administrateur et Message Center (pour l’accès aux API transactionnelles). Vérifiez le mappage des profils de produit et attribuez le profil de produit nécessaire si vous ne souhaitez pas que le profil de produit Administrateur soit mappé à votre compte technique.

#### Identifiant du tenant

Après la migration, pour les intégrations futures, il est recommandé d’utiliser votre **identifiant client Campaign v8** dans les URL REST, en remplaçant votre identifiant client Campaign Standard précédent.

#### Utilisation des clés

La gestion des valeurs PKey diffère entre Campaign Standard et Campaign v8. Si vous stockiez des clés PKey avec Campaign Standard, assurez-vous que votre implémentation crée dynamiquement les appels API suivants à l’aide des clés PKey ou href obtenus à partir d’appels API précédents.

### API disponibles {#available-apis}

Pour l’instant, les API REST répertoriées ci-dessous peuvent être utilisées :

* **Profils**
* **Services et abonnements**
* **Ressources personnalisées**
* **Workflows**
* **Messages transactionnels**

>[!AVAILABILITY]
>
>Pour l’instant, l’API REST **Messages transactionnels** n’est pas disponible.
>
>Les API REST répertoriées ci-dessous sont obsolètes et ne peuvent pas être utilisées :
>* Historique marketing
>* Entités organisationnelles
>* Gestion de la confidentialité

### Filtrage {#rest-filtering}

* Pour utiliser vos filtres dans les payloads de l’API REST, vous devez les modifier dans Campaign v8 et fournir un nom à utiliser dans vos payloads. Pour ce faire, accédez aux paramètres supplémentaires du filtre à partir de l’onglet **[!UICONTROL Paramètres]** et indiquez le nom souhaité dans le champ **[!UICONTROL Nom du filtre dans l’API REST]**.

  ![](assets/api-filtering.png)


* Le préfixe « par » requis pour utiliser les filtres personnalisés n’est plus nécessaire. Le nom du filtre doit être utilisé tel quel dans vos requêtes.

  Exemple :

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### Champs de base de données supprimés {#dropped-fields}

Certains champs de la base de données sont supprimés lors de la migration. Lors de l’utilisation d’un champ déposé, les API REST renverront des valeurs vides. À l’avenir, tous les champs déposés seront abandonnés et supprimés.

### POST avec ressources liées {#post-linked}

Lors de l’utilisation du format de corps de requête suivant, avec « VehicleOwner » représentant le lien vers « nms:recipient » :

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

Les informations sur le lien sont ignorées. Par conséquent, un nouvel enregistrement est généré sous « cusVehicle » contenant uniquement les valeurs « VehicleNumber » et « VehicleName ». Cependant, le lien reste nul, ce qui entraîne la définition de « VehicleOwner » sur null.

Dans Campaign v8, lorsque la même structure de corps de requête est utilisée et que le « véhicule » est lié à un profil, une erreur se produit. Cette erreur se produit car la propriété « firstName » n&#39;est pas reconnue comme valide pour « cusVehicle ». Cependant, un corps de requête comprenant uniquement les attributs sans lien fonctionne sans aucun problème.

### Opérations de PATCH {#patch}

* Campaign v8 ne prend pas en charge PATCH avec un corps de requête vide : il renvoie un statut 204 Aucun contenu .
* Bien que Campaign Standard prenne en charge PATCH sur les éléments/attributs d’un schéma, notez que les opérations PATCH à l’emplacement ne sont pas prises en charge dans Campaign v8. Toute tentative de PATCH sur place entraînera une erreur de serveur interne 500 avec un message d’erreur indiquant que la propriété « zipCode » n’est pas valide pour la ressource « profile ».

### Réponses REST {#rest-responses}

La section ci-dessous répertorie les différences mineures entre les réponses REST de Campaign Standard et de v8.

* Pour les enregistrements GET uniques, la réponse inclut le href dans la réponse.
* Lorsqu’elle est interrogée avec l’attribut , Campaign v8 fournit Count et Pagination dans la réponse.
* Après les opérations POST, les valeurs des ressources liées sont renvoyées dans la réponse.

### Codes d’erreur et messages {#rest-errors}

La section ci-dessous répertorie les différences entre les codes d’erreur et les messages de Campaign Standard et de Campaign v8.

| Scénario | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| Utiliser une clé PKey non valide dans le corps de la requête | 500 - Attribut &#39;O5iRp40EGA&#39; inconnu (voir définition du schéma &#39;Profils (nms:recipient)&#39;). XTK-170036 Impossible d&#39;analyser l&#39;expression &#39;@id = @O5iRp40EGA&#39;. | 404 - Impossible de déchiffrer PKey. (PKey=@jksad) |
| Utiliser une clé PKey non valide dans l’URI | 500 - Attribut &#39;O5iRp40EGA&#39; inconnu (voir définition du schéma &#39;Profils (nms:recipient)&#39;). XTK-170036 Impossible d&#39;analyser l&#39;expression &#39;@id = @O5iRp40EGA&#39;. | 404 - Impossible de déchiffrer PKey. (PKey=@jksad) Point d’entrée non pris en charge. (endpoint=rest/profileAndServices/profile/@jksad) |
| Utilisation de deux Pkeys brutes différentes dans l’URI et le corps de la requête | 500 - RST-360011 Une erreur s&#39;est produite. Veuillez contacter votre administrateur. RST-360012 Opération incohérente sur la ressource &#39;service&#39; - Impossible de mettre à jour la clé &#39;SVC3&#39; vers &#39;SVC4&#39;. | 500 - Une erreur s’est produite. Contactez votre administrateur. |
| Utilisation de PKey dans l’URI et d’une PKey brute différente dans le corps de la requête | 500 - Un « Service » avec la même clé « SVC4 » existe déjà. Erreur PGS-220000 PostgreSQL : ERREUR : la valeur de clé dupliquée viole la contrainte unique « nmsservice_name » DÉTAIL : La clé (sname)=(SVC4) existe déjà. | 500 - Une erreur s’est produite. Contactez votre administrateur. |
| Utilisation d’un raw-id non existant dans l’URI | 404 - RST-360011 Une erreur s&#39;est produite. Veuillez contacter votre administrateur. Impossible de trouver le document de chemin &#39;Service&#39; à partir de la clé &#39;adobe_nl:0&#39; (document de schéma &#39;service&#39; et de nom &#39;adobe_nl&#39;) | 404 - Impossible de trouver le document de chemin &#39;Service&#39; à partir de la clé &#39;adobe_nl&#39; (document de schéma &#39;service&#39; et de nom &#39;adobe_nl&#39;) |
| Utilisation d’un raw-id non existant dans le corps de la requête | 404 - RST-360011 Une erreur s&#39;est produite. Veuillez contacter votre administrateur. Impossible de trouver le document de chemin &#39;Service&#39; à partir de la clé &#39;adobe_nl&#39; (document de schéma &#39;service&#39; et de nom &#39;adobe_nl&#39;) | 404 - Impossible de trouver le document de chemin &#39;Service&#39; à partir de la clé &#39;adobe_nl&#39; (document de schéma &#39;service&#39; et de nom &#39;adobe_nl&#39;) |
| - | 500 - RST-360011 Une erreur s&#39;est produite. Veuillez contacter votre administrateur. | 500 - Une erreur s’est produite. Contactez votre administrateur. |
| Insérer un profil/service avec une valeur d’énumération de genre (ou toute autre valeur) non valide | 500 - RST-360011 Une erreur s&#39;est produite. Veuillez contacter votre administrateur. La valeur &#39;invalid&#39; n&#39;est pas valide pour l&#39;énumération &#39;nms:recipient:gender&#39; du champ &#39;@gender&#39; | 500 - Une erreur s’est produite. Contactez votre administrateur. |

### Fuseau horaire du profil et ccpaOptOut {#profile-timezone}

Avec Campaign Standard, le fuseau horaire s’affiche dans le cadre de la réponse JSON des appels de l’API REST **profileAndServices/profile**.

Avec Campaign v8, le fuseau horaire n’est affiché que dans le cadre des appels API REST **profileAndServicesExt/profile**. Il ne fait pas partie des appels API REST **profileAndServices/profile**, car il est ajouté dans un schéma étendu.

Il en va de même pour le champ `ccpaOptOut` : il s’affiche uniquement dans le cadre des appels API REST **profileAndServicesExt/profile**, et non des appels API **profileAndServices/profile**, puisqu’il est ajouté dans un schéma étendu dans le cadre de la migration des données.

### Signaux externes de workflow {#workflow-signals}

L’API GET Workflow Campaign Standard renvoie des noms de paramètre tels que les variables d’instance de workflow et leurs types de données (booléen, chaîne, etc.). Il est utilisé pour créer un corps de requête JSON correctement formaté lors du déclenchement du signal via un appel de l’API POST.

Campaign v8 ne prend pas en charge les variables d’instance de workflow publicitaire, mais s’attend à ce que les développeurs et développeuses les connaissent. Ainsi, après la migration, les informations de paramètres dans le corps de la requête POST devront être construites sans que les informations de paramètres ne soient disponibles dans la réponse de l’API GET.
