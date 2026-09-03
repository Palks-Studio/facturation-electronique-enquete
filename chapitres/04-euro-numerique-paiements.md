# Chapitre 4 — Euro numérique et infrastructures de paiement

> **Navigation :** [← Retour au sommaire](#documentation)

Ce chapitre examine l'architecture envisagée pour l'euro numérique, les acteurs intervenant dans son fonctionnement, les données nécessaires à l'exécution des paiements ainsi que les mécanismes techniques permettant d'automatiser certaines opérations.

L'objectif est notamment de déterminer ce que l'infrastructure de l'euro numérique permettrait techniquement, quelles données pourraient être traitées par les différents acteurs et quelles garanties sont prévues concernant la programmabilité de la monnaie, la protection des données et les possibilités de conditionnement des paiements.

Une distinction essentielle doit être faite entre :

- la programmabilité de la monnaie elle-même ;  
- les paiements conditionnels ;  
- l'automatisation de l'exécution d'un paiement ;  
- les données utilisées pour vérifier une condition ;  
- l'identification du payeur ou du bénéficiaire ;  
- l'utilisation éventuelle d'informations provenant d'autres systèmes numériques.

L'existence d'un mécanisme permettant de déclencher automatiquement un paiement lorsqu'une condition est satisfaite ne signifie pas que la monnaie elle-même est programmable.

---

## Sommaire

- [4.1 — Architecture générale de l'euro numérique](#41-architecture-générale-de-leuro-numérique)  
- [4.2 — Acteurs et infrastructures de paiement](#42-acteurs-et-infrastructures-de-paiement)  
- [4.3 — Données traitées lors des paiements](#43-données-traitées-lors-des-paiements)  
- [4.4 — Paiements en ligne et hors ligne](#44-paiements-en-ligne-et-hors-ligne)  
- [4.5 — Monnaie programmable et paiements conditionnels](#45-monnaie-programmable-et-paiements-conditionnels)  
- [4.6 — Conditions externes et automatisation des paiements](#46-conditions-externes-et-automatisation-des-paiements)  
- [4.7 — Identité numérique et infrastructures de paiement](#47-identité-numérique-et-infrastructures-de-paiement)  
- [4.8 — Limites et garanties prévues](#48-limites-et-garanties-prévues)  
- [4.9 — Ce que ce chapitre permet d'établir](#49-ce-que-ce-chapitre-permet-détablir)

---

## 4.1 Architecture générale de l'euro numérique

**Statut : AVÉRÉ / PROJET EN COURS**

L'euro numérique est un projet de monnaie numérique de banque centrale destiné à compléter les espèces et les autres moyens de paiement existants dans la zone euro [S22][S23].

Il ne s'agit pas d'un crypto-actif ou d'une monnaie émise par un établissement privé. Les unités d'euros numériques constitueraient une créance directe sur l'Eurosystème [S23].

À la date des sources étudiées, l'euro numérique n'est pas encore émis. Le projet poursuit son développement technique et reste dépendant de l'adoption du cadre législatif européen correspondant [S23].

---

### Une infrastructure centrale de règlement

L'architecture technique actuellement envisagée repose sur une plateforme centralisée de règlement exploitée par l'Eurosystème [S23].

L'Eurosystème traiterait et vérifierait les règlements ainsi que les avoirs en euros numériques enregistrés dans l'infrastructure [S23].

La BCE précise que cette architecture ne repose pas sur une blockchain ou une technologie de registre distribué comme infrastructure fondamentale du système [S23].

Elle reprend néanmoins certains principes techniques utilisés dans les systèmes distribués afin d'améliorer notamment la résilience et les performances.

**AVÉRÉ :**

> L'architecture actuellement envisagée pour l'euro numérique repose sur une infrastructure centrale de règlement contrôlée par l'Eurosystème [S23].

---

### Une distribution passant par des intermédiaires

L'existence d'une infrastructure centrale ne signifie pas que les utilisateurs disposeraient directement d'un compte auprès de la BCE pour leurs opérations quotidiennes.

La proposition de règlement prévoit que les services de paiement en euros numériques soient distribués par l'intermédiaire de prestataires de services de paiement [S22].

Ces intermédiaires permettraient notamment :

- l'accès et l'utilisation de l'euro numérique ;  
- l'initiation et la réception de paiements ;  
- la fourniture des instruments permettant d'effectuer ces paiements ;  
- la gestion des comptes de paiement en euros numériques ;  
- les opérations permettant de charger ou décharger les avoirs correspondants [S22].

La BCE indique également qu'un utilisateur pourrait accéder à l'euro numérique au moyen d'un compte mis en place auprès de sa banque ou d'un intermédiaire public [S23].

L'architecture distingue donc au moins deux niveaux :

```
Utilisateur
   ↓
Prestataire de services de paiement
   ↓
Infrastructure de l'Eurosystème
   ↓
Règlement en euros numériques
```

Cette séparation entre relation avec l'utilisateur et règlement central deviendra importante pour déterminer quelles données sont accessibles aux différents acteurs.

---

### Une monnaie inscrite au bilan de l'Eurosystème

Les euros numériques détenus par les utilisateurs constitueraient des engagements directs de l'Eurosystème [S23].

Cette caractéristique distingue l'euro numérique de la monnaie scripturale habituellement détenue sur un compte bancaire commercial.

Le prestataire de services de paiement assurerait donc la relation avec l'utilisateur et la fourniture du service, tandis que la valeur monétaire correspondante resterait une créance sur la banque centrale.

**AVÉRÉ :**

> L'intermédiation par une banque ou un prestataire de paiement ne transforme pas l'euro numérique en monnaie bancaire privée : les avoirs correspondants resteraient une créance directe sur l'Eurosystème [S23].

---

### Une infrastructure conçue pour fonctionner à grande échelle

La BCE prévoit une architecture répartie entre plusieurs régions géographiques, chacune disposant de plusieurs serveurs, afin d'assurer la continuité du service et la résilience de l'infrastructure [S23].

L'objectif est notamment de permettre au système de continuer à fonctionner en cas de défaillance affectant une partie de l'infrastructure.

L'euro numérique est donc envisagé comme une infrastructure européenne de paiement de détail destinée à fonctionner à grande échelle et non comme une expérimentation limitée à quelques acteurs.

---

### Paiements en ligne et hors ligne

L'architecture prévoit deux modalités principales d'utilisation :

- les paiements en ligne ;  
- les paiements hors ligne [S23].

La possibilité d'effectuer des paiements hors ligne constitue une caractéristique importante du projet.

Dans cette situation, la BCE indique que les détails de la transaction seraient connus uniquement du payeur et du bénéficiaire, afin de fournir un niveau de confidentialité proche de celui des espèces.

Les paiements en ligne utilisent en revanche l'infrastructure de paiement et impliquent les intermédiaires nécessaires à leur exécution.

La distinction entre ces deux modes devra donc être conservée lorsque seront examinées les données accessibles aux différents acteurs.

---

### Une architecture centralisée ne signifie pas une connaissance directe de l'identité par la BCE

La centralisation du règlement ne signifie pas que la BCE disposerait automatiquement de l'identité civile des utilisateurs correspondant à chaque transaction.

La BCE indique que les informations mises à disposition de l'Eurosystème seraient pseudonymisées et qu'elle ne devrait pas être en mesure d'identifier directement l'utilisateur à partir des données de paiement qu'elle reçoit [S23].

Les intermédiaires assurant la relation avec l'utilisateur disposeraient en revanche des informations nécessaires au respect de leurs obligations légales.

Cette distinction sera examinée plus précisément dans la section consacrée aux données de paiement.

---

### Une architecture encore en développement

L'euro numérique n'est pas actuellement une monnaie en circulation [S23].

La BCE poursuit le développement technique du dispositif et indique viser une préparation permettant une éventuelle première émission en 2029, sous réserve notamment de l'adoption du cadre législatif européen [S23].

Les spécifications techniques continuent donc d'évoluer.

Les éléments étudiés dans ce chapitre doivent être compris comme décrivant l'architecture actuellement proposée ou préparée et non comme le fonctionnement définitif d'un système déjà déployé.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> L'euro numérique est conçu comme une monnaie de banque centrale dont les avoirs constitueraient une créance directe sur l'Eurosystème [S22][S23].

**AVÉRÉ :**

> L'architecture actuellement envisagée repose sur une plateforme centralisée de règlement contrôlée par l'Eurosystème, tandis que la distribution et la relation avec les utilisateurs passent par des prestataires de services de paiement [S22][S23].

**AVÉRÉ :**

> L'infrastructure prévoit des paiements en ligne et hors ligne ainsi que des mécanismes techniques spécifiques destinés à assurer sa résilience [S23].

**AVÉRÉ :**

> La BCE indique que l'Eurosystème ne devrait pas pouvoir identifier directement les utilisateurs à partir des données de paiement auxquelles il aurait accès, tandis que les intermédiaires conserveraient les informations nécessaires à leurs obligations légales [S23].

**À ÉTABLIR :**

> Quelles données exactes circulent entre l'utilisateur, son prestataire de services de paiement et l'infrastructure centrale lors des différents types de transactions ?

**À ÉTABLIR :**

> Quels composants techniques disposent des informations permettant d'initier, vérifier, autoriser, régler ou éventuellement conditionner l'exécution d'un paiement ?

---

## 4.2 Acteurs et infrastructures de paiement

**Statut : AVÉRÉ / PROJET EN COURS**

L'architecture envisagée pour l'euro numérique ne repose pas sur une relation directe unique entre l'utilisateur et la Banque centrale européenne.

Elle fait intervenir plusieurs catégories d'acteurs assurant des fonctions distinctes dans l'accès au service, l'initiation des paiements, leur acceptation, leur contrôle et leur règlement [S22][S24].

Cette répartition des fonctions est importante pour déterminer quelles informations sont accessibles à chaque acteur et à quel moment d'une transaction.

---

### L'Eurosystème

L'Eurosystème constitue le niveau central de l'infrastructure.

Comme établi dans la section précédente, l'architecture actuellement envisagée prévoit une plateforme centrale permettant notamment le traitement et le règlement des opérations en euros numériques [S23].

L'Eurosystème définit également les règles et spécifications communes nécessaires au fonctionnement du dispositif.

Le rulebook de l'euro numérique décrit notamment :

- les acteurs participant au dispositif ;  
- les différents cas d'utilisation ;  
- les flux de paiement de bout en bout ;  
- les interfaces entre les différents composants ;  
- les exigences techniques applicables aux prestataires de services de paiement ;  
- les mécanismes de gestion des données ;  
- les échanges de données ;  
- les mécanismes de gestion du risque et de la fraude ;  
- le règlement des transactions [S24].

**AVÉRÉ :**

> L'Eurosystème ne constitue donc pas uniquement l'émetteur de la monnaie : il fournit également l'infrastructure centrale et définit les règles techniques communes permettant aux différents acteurs du système d'interagir [S23][S24].

---

### Les prestataires de services de paiement

La proposition de règlement prévoit que la distribution de l'euro numérique repose sur des prestataires de services de paiement [S22].

Les utilisateurs établissent une relation contractuelle avec ces prestataires et non directement avec la Banque centrale européenne [S22].

Les prestataires peuvent notamment permettre aux utilisateurs :

- d'accéder à l'euro numérique ;  
- d'initier et recevoir des paiements ;  
- de disposer d'instruments de paiement en euros numériques ;  
- de gérer leur compte de paiement en euros numériques ;  
- d'effectuer les opérations de chargement et de déchargement prévues par le dispositif [S22].

Les prestataires de services de paiement constituent donc une couche d'intermédiation entre l'utilisateur et l'infrastructure centrale.

---

### Le prestataire du payeur

Dans une transaction, le prestataire assurant la relation avec le payeur intervient dans l'initiation et le traitement du paiement [S24].

Il constitue notamment le point de contact entre l'utilisateur, son instrument de paiement et les services nécessaires à l'exécution de l'opération.

La documentation technique du dispositif distingue explicitement les fonctions et exigences applicables aux prestataires distribuant l'euro numérique [S24].

Ces prestataires doivent notamment interagir avec les services centraux nécessaires à l'accès au système, à la gestion de la liquidité et au traitement des transactions.

Ils restent également soumis aux obligations légales applicables aux prestataires de services de paiement.

Cette position est importante pour l'analyse des données : contrairement à l'Eurosystème, qui doit recevoir des informations pseudonymisées dans certaines situations, le prestataire assurant la relation avec l'utilisateur dispose des informations nécessaires pour fournir le service et satisfaire à ses obligations réglementaires.

---

### Le prestataire du bénéficiaire

Une transaction commerciale peut également faire intervenir un prestataire situé du côté du bénéficiaire du paiement.

Le rulebook distingue ainsi les prestataires distribuant l'euro numérique des prestataires assurant les fonctions d'acquisition nécessaires à l'acceptation des paiements [S24].

Dans une transaction commerciale, le prestataire acquéreur permet notamment l'interaction entre le dispositif d'acceptation du commerçant et l'infrastructure nécessaire au traitement du paiement.

L'architecture peut donc être représentée de manière simplifiée ainsi :

```
Payeur
   ↓
PSP du payeur
   ↓
Infrastructure de l'euro numérique
   ↓
PSP du bénéficiaire / acquéreur
   ↓
Commerçant ou bénéficiaire
```

Ce schéma est volontairement simplifié : les flux techniques peuvent faire intervenir plusieurs services communs supplémentaires.

---

### Les dispositifs d'acceptation

L'infrastructure ne se limite pas aux banques et à l'Eurosystème.

Le rulebook prévoit également des spécifications relatives aux dispositifs permettant d'accepter les paiements en euros numériques [S24].

Ces dispositifs peuvent notamment intervenir dans les paiements effectués auprès d'un commerçant.

Ils constituent le point technique où les informations nécessaires à la transaction sont présentées, échangées ou capturées avant leur transmission aux autres composants du système.

Le dispositif d'acceptation doit donc être distingué du système central de règlement : il intervient à proximité de l'acte commercial tandis que le règlement monétaire est réalisé dans une autre couche de l'infrastructure.

---

### Des services communs entre les différents acteurs

Le rulebook prévoit également une catégorie de services communs utilisables par différents participants au dispositif [S24].

Les spécifications techniques publiées par la BCE couvrent notamment :

- la gestion des accès ;
- la recherche et la résolution d'alias ;
- la gestion de la liquidité ;
- le traitement des paiements ;
- la gestion du risque et de la fraude ;
- les échanges de données ;
- le règlement des transactions [S24].

L'existence de ces services montre que l'exécution d'un paiement ne correspond pas simplement à un transfert direct entre deux portefeuilles.

Elle implique plusieurs fonctions techniques pouvant intervenir successivement ou simultanément dans le traitement d'une opération.

---

### Contrôle du risque, de la fraude et respect des obligations légales

Les prestataires de services de paiement restent responsables des contrôles qui leur sont imposés par la réglementation applicable.

La documentation technique du projet prévoit notamment des mécanismes relatifs à la gestion du risque et de la fraude [S24].

Les versions du rulebook préparant l'architecture indiquent également que le prestataire du payeur doit effectuer, avant l'exécution finale d'une transaction, les contrôles légalement requis en matière de fraude, de lutte contre le blanchiment et le financement du terrorisme ainsi que, lorsque cela est applicable, les contrôles relatifs aux sanctions et embargos.

Le prestataire conserve la responsabilité de l'exécution ou de la non-exécution de la transaction conformément au cadre juridique applicable.

**AVÉRÉ :**

> L'exécution d'un paiement en euros numériques n'est donc pas conçue comme une opération techniquement aveugle : des contrôles réglementaires et des mécanismes de gestion du risque et de la fraude interviennent dans le traitement des transactions [S24].

Ces contrôles correspondent à des obligations juridiques existantes et ne constituent pas, en eux-mêmes, une possibilité générale de conditionner les paiements selon n'importe quel critère.

---

### Plusieurs acteurs peuvent donc intervenir sur une même transaction

L'architecture permet de distinguer plusieurs fonctions :

```
Utilisateur
   ↓
Instrument ou interface de paiement
   ↓
PSP distributeur / PSP du payeur
   ↓
Services communs
   ↓
Infrastructure centrale
   ↓
PSP acquéreur / PSP du bénéficiaire
   ↓
Dispositif d'acceptation
   ↓
Bénéficiaire
```

Tous ces acteurs ou composants ne disposent pas nécessairement des mêmes informations.

La connaissance de l'identité du payeur, du bénéficiaire, du montant, de l'instrument utilisé, du contexte commercial ou des informations techniques nécessaires au règlement peut être répartie entre plusieurs composants.

Il est donc nécessaire de distinguer l'existence globale d'une information dans la chaîne de paiement de son accessibilité effective par un acteur déterminé.

---

### Une distinction essentielle entre connaissance et capacité d'action

La présence d'un acteur dans le traitement d'une transaction ne signifie pas automatiquement qu'il dispose de toutes les données relatives à cette transaction.

Inversement, un acteur n'a pas nécessairement besoin de connaître l'ensemble du contexte commercial pour effectuer une opération technique telle qu'une authentification, un contrôle, une autorisation ou un règlement.

Cette distinction sera particulièrement importante lorsque seront étudiés les paiements conditionnels.

Un système peut en effet recevoir le résultat d'une vérification externe sans nécessairement recevoir toutes les données ayant permis de produire ce résultat.

Une architecture de ce type peut être représentée ainsi :

```
Système externe
   ↓
Résultat d'une condition
   ↓
Composant de paiement
   ↓
Exécution ou absence d'exécution
```

**Cette représentation décrit uniquement un principe d'architecture informatique. Elle ne signifie pas qu'un système externe utilisant des données environnementales, fiscales ou individuelles soit actuellement relié à l'euro numérique.**

---

### Conclusion intermédiaire

**AVÉRÉ :**

> L'architecture envisagée pour l'euro numérique répartit les fonctions entre plusieurs catégories d'acteurs et de composants, notamment l'Eurosystème, les prestataires de services de paiement, les prestataires intervenant du côté du payeur ou du bénéficiaire, les dispositifs d'acceptation et différents services communs [S22][S24].

**AVÉRÉ :**

> Le rulebook prévoit des spécifications techniques distinctes concernant notamment les flux de bout en bout, les prestataires distributeurs et acquéreurs, les dispositifs d'acceptation, la gestion des données, les échanges de données, le risque et la fraude ainsi que le règlement [S24].

**AVÉRÉ :**

> Des contrôles réglementaires et des mécanismes de gestion du risque et de la fraude peuvent intervenir avant l'exécution finale d'une transaction, conformément aux obligations applicables aux prestataires de services de paiement [S24].

**DÉDUCTIBLE TECHNIQUEMENT :**

> La répartition des fonctions entre plusieurs composants permet qu'une décision ou une vérification nécessaire au traitement d'un paiement soit produite dans un système distinct puis communiquée au composant chargé de poursuivre ou non l'opération, sans que celui-ci ait nécessairement accès à l'ensemble des données ayant produit cette décision.

**À ÉTABLIR :**

> Quelles données exactes sont accessibles à chacun des acteurs intervenant dans une transaction en euros numériques et lesquelles sont échangées entre leurs différents systèmes ?

**À ÉTABLIR :**

> Quels services disposent techniquement de la capacité de bloquer, suspendre, différer ou déclencher une transaction, dans quelles situations et selon quelles règles ?

**À ÉTABLIR :**

> Des informations provenant de systèmes externes au paiement peuvent-elles être utilisées par certains composants de cette architecture pour déterminer l'exécution d'une opération, et si oui, dans quels cas ?

---

## 4.3 Données traitées lors des paiements

**Statut : AVÉRÉ / PROJET EN COURS**

La documentation technique publiée pour le projet d'euro numérique permet d'aller au-delà d'une description générale de l'architecture et d'examiner les catégories de données prévues pour assurer son fonctionnement [S24][S25].

Le rulebook v0.91 comporte notamment un modèle de données, un dictionnaire de données ainsi que des spécifications consacrées aux échanges de données entre les différents composants du système [S25].

Ces documents constituent encore des spécifications provisoires et non contraignantes. Ils décrivent néanmoins de manière détaillée les informations actuellement prévues dans la conception du dispositif.

---

### Un modèle structuré des utilisateurs, comptes, appareils et transactions

Le modèle de données distingue plusieurs catégories d'entités nécessaires au fonctionnement de l'euro numérique [S25].

Il comprend notamment :

- les utilisateurs ;  
- les utilisateurs professionnels ;  
- les comptes de paiement en euros numériques ;  
- certains comptes de paiement en euros non numériques liés au dispositif ;  
- les prestataires de services de paiement ;  
- les appareils utilisés ;  
- les alias ;  
- les points d'interaction avec les commerçants ;  
- les transactions ;  
- les payeurs ;  
- les bénéficiaires ;  
- les données relatives aux litiges ;  
- les données relatives au risque et à la fraude [S25].

Le document précise que ce modèle représente les entités, leurs attributs essentiels et les relations existant entre elles.

Il ne doit cependant pas être interprété comme la représentation complète de toutes les bases de données du système ni comme l'indication que chaque acteur conserve l'intégralité de ces informations.

**AVÉRÉ :**

> La conception actuelle de l'euro numérique repose sur un modèle de données structuré reliant notamment utilisateurs, comptes, appareils, prestataires de services de paiement et transactions [S25].

---

### Des identifiants propres aux utilisateurs et aux comptes

Le modèle prévoit un identifiant unique de l'utilisateur de l'euro numérique ainsi qu'un identifiant du compte de paiement en euros numériques, désigné notamment sous le terme DEAN dans les spécifications [S25].

Il prévoit également des alias pseudonymes.

Le rulebook définit l'alias comme un identifiant pseudonyme destiné à protéger l'identité de l'utilisateur lors du traitement des paiements. Selon la spécification, cet alias ne peut être rattaché à une personne physique ou morale identifiable que par le prestataire de services de paiement distribuant l'euro numérique ou par l'utilisateur concerné [S25].

L'alias est destiné à constituer un identifiant principal pouvant être partagé dans certaines transactions.

**AVÉRÉ :**

> L'architecture distingue donc l'identité connue du prestataire de services de paiement de l'identifiant pseudonyme susceptible de circuler dans certains traitements de transaction [S25].

Cette séparation constitue une mesure importante de protection de l'identité mais ne signifie pas que l'utilisateur soit anonyme vis-à-vis de son prestataire de services de paiement.

---

### Des données détaillées décrivant la transaction

Le modèle définit une transaction comme la représentation d'un échange financier entre acteurs.

Les exemples mentionnés comprennent notamment les opérations de chargement et de déchargement, les paiements récurrents, les réservations, les paiements, les achats, les retraits et d'autres opérations [S25].

Parmi les informations prévues figurent notamment :

- un identifiant de transaction ;  
- un identifiant de transaction de bout en bout connu des prestataires concernés ;  
- le montant de la transaction ;  
- la date et l'heure de création ;  
- la direction de la transaction ;  
- la devise ;  
- des informations complémentaires pouvant être renseignées par l'utilisateur lors de l'initiation ;  
- le type de transaction ;  
- la méthode d'initiation ;  
- le statut de la transaction ;  
- l'environnement dans lequel elle intervient [S25].

Les types et environnements prévus permettent notamment de distinguer achat, remboursement, réservation, paiement de compte à compte, transaction P2P, commerce électronique, commerce mobile, paiement récurrent ou ordre permanent [S25].

**AVÉRÉ :**

> Une transaction en euros numériques n'est donc pas représentée uniquement par un montant transféré : le modèle technique prévoit plusieurs attributs permettant de l'identifier, de la dater, de la catégoriser et d'en suivre le cycle de traitement [S25].

---

### Identification du payeur et du bénéficiaire

Le modèle prévoit des entités distinctes pour le payeur et le bénéficiaire [S25].

Le payeur peut être une personne physique, une entreprise, une administration ou une autre autorité publique.

Le bénéficiaire peut également appartenir à ces différentes catégories.

Les spécifications prévoient des identifiants uniques du payeur et du bénéficiaire dans le modèle de données [S25].

Cela ne signifie pas que leur identité civile complète soit communiquée à tous les composants du système.

Comme indiqué précédemment, l'architecture prévoit notamment l'utilisation d'alias pseudonymes et une répartition des informations entre les prestataires et l'infrastructure centrale.

**AVÉRÉ :**

> Le modèle de données permet techniquement de distinguer et d'identifier les parties participant à une transaction, tout en prévoyant des mécanismes destinés à limiter la circulation de leur identité directement identifiable [S25].

---

### Les appareils utilisés peuvent également être représentés

Le modèle prévoit des informations relatives aux appareils permettant d'interagir avec le système [S25].

Un appareil peut notamment correspondre à une application, une carte ou un accès par navigateur.

Parmi les attributs prévus figurent notamment :

- un identifiant de l'appareil ;  
- son type ;  
- son adresse IP lorsqu'elle est applicable [S25].

Ces informations peuvent notamment intervenir dans les processus techniques, de sécurité ou de gestion du risque.

Leur existence dans le modèle ne signifie pas nécessairement qu'elles sont transmises à tous les acteurs participant au règlement d'une transaction.

---

### Le contexte commercial peut être catégorisé

La documentation prévoit également des données relatives au commerçant et à son activité [S25].

Elle utilise notamment le **Merchant Category Code**, ou MCC, fondé sur la classification ISO 18245.

Ce code permet de classer un commerçant selon le type de biens ou de services correspondant à son activité, par exemple les transports, le commerce de détail ou la location de véhicules [S25].

Le modèle prévoit également un identifiant du commerçant ainsi que l'identifiant de son compte de paiement en euros numériques.

**AVÉRÉ :**

> L'architecture actuellement documentée permet donc de connaître, dans certains flux, non seulement le montant et les parties à une transaction mais également une catégorie correspondant à l'activité commerciale du bénéficiaire [S25].

Cette donnée ne décrit cependant pas le produit individuel acheté.

Un Merchant Category Code classe l'activité du commerçant ; il ne constitue pas un GTIN, un identifiant DPP ou un identifiant d'article.

Cette distinction est essentielle pour éviter de confondre **catégorie du commerçant** et **contenu détaillé du panier**.

---

### Le Merchant Category Code circule dans la requête de paiement

La documentation va plus loin concernant le MCC.

Elle indique que, parmi les informations relatives au type d'activité du commerçant, **seul le Merchant Category Code est transmis dans la requête de paiement au Digital Euro Service Platform (DESP) et au prestataire de services de paiement distributeur**, et qu'il est transmis sous forme chiffrée [S25].

**AVÉRÉ :**

> Dans l'architecture actuellement documentée, une information catégorisant l'activité du commerçant fait donc partie des données pouvant circuler dans la chaîne technique d'une requête de paiement [S25].

Le chiffrement de cette information doit être pris en compte : sa présence dans un message ne signifie pas que chaque composant intermédiaire puisse nécessairement la lire ou l'exploiter.

Il faudra donc distinguer, pour chaque traitement, la circulation technique d'une donnée de sa capacité effective à être déchiffrée et utilisée par un acteur déterminé.

---

### Des informations relatives au point d'interaction et à sa localisation

Le modèle décrit également le point d'interaction, ou POI, où une transaction peut être réalisée [S25].

Celui-ci peut correspondre à un emplacement physique, comme un terminal de paiement dans un commerce, ou à un emplacement virtuel, comme une page de paiement en ligne ou une application mobile.

Parmi les informations envisagées figurent notamment :

- un identifiant du point d'interaction ;  
- son type ;  
- un identifiant de l'entité juridique ;  
- un identifiant professionnel local, par exemple un SIRET en France ;  
- un identifiant en ligne tel qu'un nom de domaine ou une adresse IP ;  
- une adresse physique ;  
- une ville ;  
- un code postal ;  
- un pays [S25].

La documentation précise toutefois que plusieurs de ces informations doivent être gérées **en interne par le PSP acquéreur**, notamment à des fins de traçabilité, d'audit, de gestion des capacités d'acceptation et, pour certaines données, de gestion des pré-litiges ou litiges [S25].

**AVÉRÉ :**

> Des informations permettant de caractériser ou localiser un point d'interaction commercial existent dans le modèle, mais la documentation prévoit que plusieurs d'entre elles restent gérées au niveau du PSP acquéreur plutôt que d'être nécessairement transmises à l'ensemble de l'infrastructure [S25].

---

### Lien avec un compte bancaire non numérique

Le modèle prévoit également la possibilité de relier un compte de paiement en euros numériques à un compte de paiement non numérique [S25].

Pour ce dernier, la documentation mentionne notamment :

- l'IBAN ;  
- les dates d'ouverture et de fermeture ;  
- le solde ;  
- la date correspondant au solde [S25].

Cette relation intervient notamment dans les mécanismes permettant d'alimenter ou de désalimenter les avoirs en euros numériques.

**AVÉRÉ :**

> L'architecture prévoit donc une articulation technique possible entre le compte en euros numériques d'un utilisateur et un compte de paiement bancaire classique utilisé notamment pour les opérations de financement ou de déchargement [S25].

Cette articulation ne signifie pas que l'Eurosystème dispose librement de l'ensemble des données du compte bancaire traditionnel : la répartition des données entre PSP et DESP reste déterminante.

---

### Des données de risque et de fraude

Le modèle de paiement comprend également des données relatives à l'évaluation du risque et de la fraude [S25].

Il prévoit notamment une entité correspondant à un **fraud and risk score** ainsi qu'un type permettant de classifier ce score.

Ces informations doivent être replacées dans la fonction de prévention et de détection de la fraude prévue par l'architecture de paiement.

**AVÉRÉ :**

> L'architecture prévoit donc l'utilisation de scores ou indicateurs structurés destinés à l'évaluation du risque et de la fraude dans le traitement des paiements [S25].

La présence d'un score de risque ou de fraude ne démontre pas l'existence d'un score social, environnemental ou comportemental général.

Aucune des sources étudiées à ce stade ne permet d'affirmer qu'une donnée environnementale ou un profil environnemental entre dans le calcul de ces scores.

---

### Des données pouvant servir à des rapports, requêtes et analyses

Les spécifications du service d'échange de données prévoient que le DESP puisse fournir aux participants différents rapports et mécanismes de requête [S25].

La documentation indique explicitement que ces fonctions doivent répondre à des besoins **opérationnels, analytiques et statistiques** des participants.

Les rapports et requêtes prévus concernent notamment :

- les transactions ;  
- les comptes ;  
- certaines données de référentiel ;  
- les litiges ;  
- le calcul de certains frais ;  
- la gestion du risque et de la fraude [S25].

Certains rapports peuvent être détaillés, d'autres agrégés, et leur accès dépend du rôle du prestataire concerné.

La documentation prévoit par exemple des rapports détaillés de transactions pour les PSP éligibles ainsi qu'un rapport agrégé périodique relatif à la situation en matière de risque de fraude [S25].

**AVÉRÉ :**

> L'infrastructure prévoit donc non seulement le traitement transactionnel immédiat des données mais également des mécanismes structurés permettant à certains participants autorisés d'obtenir des rapports et d'effectuer des requêtes à des fins opérationnelles, analytiques ou statistiques [S25].

Cette capacité reste encadrée par les rôles et droits d'accès définis dans le système.

---

### Le modèle distingue les données existantes de leur accessibilité effective

Un point méthodologique est essentiel.

Le modèle de données décrit les informations nécessaires aux différents processus mais précise qu'il ne représente pas l'intégralité d'un système d'information et qu'il ne détermine pas automatiquement les informations déjà gérées dans les systèmes existants [S25].

De même, le service d'échange de données prévoit que les rapports et requêtes accessibles à un PSP dépendent de son rôle et des données auxquelles il est éligible.

Il faut donc distinguer trois niveaux :

```
Donnée prévue dans le modèle
   ↓
Donnée effectivement transmise dans un flux déterminé
   ↓
Donnée effectivement accessible et exploitable par un acteur déterminé
```

Ces trois niveaux ne doivent pas être confondus.

---

### Ce que les données de paiement ne permettent pas encore d'établir

Les éléments étudiés permettent de documenter une granularité importante des informations nécessaires au fonctionnement du système.

Ils ne permettent cependant pas d'affirmer que le système de paiement connaît systématiquement le produit individuel acheté.

À ce stade, les données identifiées comprennent notamment le montant, la date et l'heure, les parties, les comptes ou alias nécessaires, le type et l'environnement de la transaction, certains éléments techniques ainsi que la catégorie d'activité du commerçant.

Aucune des sources étudiées dans cette section ne permet d'établir que la requête de paiement contient systématiquement :

- le GTIN du produit acheté ;  
- l'identifiant de son passeport numérique de produit ;  
- sa désignation détaillée ;  
- son empreinte carbone ;  
- les différentes lignes composant le panier ;  
- les données fiscales détaillées d'une facture électronique.

**À ÉTABLIR :**

> Des données provenant du système commercial, d'une facture électronique, d'un DPP ou d'un autre système externe peuvent-elles être associées à l'identifiant de transaction ou utilisées par une autre couche de l'infrastructure sans être directement contenues dans le message de paiement ?

---

### Conclusion intermédiaire

**AVÉRÉ :**

> Le modèle technique actuellement publié pour l'euro numérique prévoit des données structurées relatives aux utilisateurs, comptes, appareils, prestataires, payeurs, bénéficiaires et transactions [S25].

**AVÉRÉ :**

> Les transactions disposent d'identifiants, dont un identifiant de bout en bout, et comportent notamment des informations relatives au montant, à la date et l'heure, au type, à l'environnement et au statut de l'opération [S25].

**AVÉRÉ :**

> L'architecture prévoit des identifiants pseudonymes permettant de limiter la circulation de l'identité directement identifiable de l'utilisateur, tandis que son prestataire de services de paiement conserve la capacité de rattacher certaines informations à son client [S25].

**AVÉRÉ :**

> Le Merchant Category Code permet de catégoriser l'activité commerciale du bénéficiaire et la documentation prévoit sa transmission chiffrée dans la requête de paiement au DESP et au PSP distributeur [S25].

**AVÉRÉ :**

> Le modèle comprend également des informations relatives aux points d'interaction, à certains éléments de localisation, aux appareils et à des scores de risque et de fraude, avec une répartition de leur gestion entre les différents acteurs [S25].

**AVÉRÉ :**

> Le DESP prévoit des rapports et mécanismes de requête destinés à certains PSP selon leurs droits et leurs rôles, notamment pour des besoins opérationnels, analytiques et statistiques [S25].

**NON ÉTABLI :**

> Les sources étudiées ne permettent pas d'affirmer que l'infrastructure de paiement reçoit systématiquement l'identifiant précis du produit acheté, son DPP, son GTIN, son empreinte environnementale ou le détail complet du panier.

**À ÉTABLIR :**

> Quelles informations supplémentaires peuvent être associées à une transaction par les PSP, commerçants ou systèmes externes grâce aux identifiants de transaction prévus dans l'architecture ?

**À ÉTABLIR :**

> Quelles données sont effectivement accessibles au DESP, aux PSP distributeurs, aux PSP acquéreurs et aux autres services techniques, sous quelle forme et pendant quelle durée ?

**À ÉTABLIR :**

> Dans quelles situations les informations décrivant le contexte d'une transaction peuvent-elles participer à une décision automatisée concernant son traitement ?

---

## 4.4 Paiements en ligne et hors ligne

**Statut : AVÉRÉ / PROJET EN COURS**

L'architecture envisagée pour l'euro numérique distingue deux modes de fonctionnement présentant des caractéristiques techniques et des niveaux d'accès aux données différents :

- le paiement en ligne ;  
- le paiement hors ligne [S23][S26].

Cette distinction est essentielle pour l'analyse des possibilités de traitement des données.

Un paiement en ligne utilise les infrastructures et intermédiaires nécessaires à son traitement et à son règlement.

Un paiement hors ligne est au contraire conçu pour permettre le transfert de valeur sans connexion à Internet et sans intervention en temps réel de l'infrastructure centrale [S26].

---

### Le paiement en ligne

Dans le fonctionnement en ligne, les différents composants étudiés dans les sections précédentes interviennent dans le traitement de la transaction.

Selon le type d'opération, cela peut notamment impliquer :

- le prestataire de services de paiement du payeur ;  
- le prestataire du bénéficiaire ;  
- les services communs du dispositif ;  
- le Digital Euro Service Platform ;  
- l'infrastructure de règlement de l'Eurosystème [S24][S25].

Les données nécessaires au traitement de la transaction peuvent alors circuler entre différents composants selon les règles, rôles et droits d'accès prévus par l'architecture.

Comme établi dans la section 4.3, ces données peuvent notamment comprendre des identifiants de transaction, le montant, la date et l'heure, le type et l'environnement de l'opération, les identifiants pseudonymes nécessaires au traitement ainsi que certaines informations relatives au contexte commercial [S25].

La BCE indique toutefois que l'Eurosystème ne devrait pas pouvoir identifier directement le payeur ou le bénéficiaire à partir des informations reçues pour les paiements en ligne [S23].

Le lien entre les identifiants pseudonymisés utilisés dans l'infrastructure et l'identité des utilisateurs resterait connu de leurs prestataires de services de paiement conformément aux obligations applicables [S23].

**AVÉRÉ :**

> Le fonctionnement en ligne implique donc une circulation structurée de données nécessaires au paiement, mais l'architecture prévoit une séparation entre les informations directement identifiantes détenues par les PSP et les informations pseudonymisées accessibles à l'Eurosystème [S23][S25].

---

### Le paiement hors ligne

Le fonctionnement hors ligne repose sur une architecture différente.

La BCE prévoit qu'un paiement puisse être réalisé directement entre les appareils du payeur et du bénéficiaire sans connexion à Internet au moment de la transaction [S26].

Dans les travaux techniques actuellement menés pour le pilote, les paiements hors ligne entre particuliers reposent notamment sur une communication de proximité utilisant le NFC.

La valeur nécessaire au paiement est conservée localement dans un environnement matériel sécurisé de l'appareil.

La BCE étudie notamment l'utilisation :

- d'éléments sécurisés intégrés, ou embedded Secure Elements ;  
- d'eSIM ;  
- d'autres composants matériels permettant de protéger les valeurs et opérations cryptographiques nécessaires au fonctionnement hors ligne [S26].

Ces composants sont destinés à empêcher notamment l'extraction des clés cryptographiques, la modification frauduleuse du solde ou l'altération des opérations réalisées dans l'environnement sécurisé.

---

### Un transfert direct entre appareils

Dans le mode hors ligne, le transfert ne nécessite pas l'intervention d'un système en ligne au moment du paiement [S26].

La BCE décrit le mécanisme comme un transfert direct entre deux appareils de valeurs cryptographiquement sécurisées.

Le fonctionnement peut être représenté simplement ainsi :

```
Appareil du payeur
   ↓
Communication locale sécurisée
   ↓
Appareil du bénéficiaire
```

L'infrastructure centrale n'intervient donc pas en temps réel dans le traitement individuel de cette transaction.

**AVÉRÉ :**

> Un paiement hors ligne en euros numériques est conçu pour pouvoir être exécuté directement entre les appareils du payeur et du bénéficiaire sans transmission de la transaction à un système en ligne au moment du paiement [S26].

---

### Les détails de la transaction restent sur les appareils

La différence avec le paiement en ligne est particulièrement importante concernant les données.

La BCE indique que, pour les paiements hors ligne, les informations sensibles relatives à la transaction restent dans l'environnement sécurisé des appareils et ne sont accessibles ni à l'Eurosystème ni aux prestataires de services de paiement [S26].

La documentation précise notamment que les informations relatives :

- aux biens achetés ou à l'objet du paiement ;  
- au lieu où les biens ont été achetés ;  
- au commerçant auprès duquel l'achat a été effectué ou à la personne ayant reçu le paiement,

ne sont pas accessibles à la BCE, aux banques ou aux PSP dans le cadre du paiement hors ligne [S26].

**AVÉRÉ :**

> Dans l'architecture actuellement annoncée, les détails personnels d'un paiement hors ligne sont conçus pour être connus uniquement du payeur et du bénéficiaire [S23][S26].

Cette caractéristique constitue une différence majeure avec le fonctionnement en ligne étudié précédemment.

---

### Un niveau de confidentialité comparable aux espèces

La BCE présente explicitement le paiement hors ligne comme devant offrir un niveau de confidentialité comparable à celui des espèces [S23][S26].

Le fonctionnement hors ligne empêche l'Eurosystème de relier directement la transaction à une personne.

Mais il va plus loin : contrairement au paiement en ligne, les PSP ne reçoivent pas non plus les détails personnels de la transaction elle-même pendant ou après son exécution [S26].

La différence peut être résumée ainsi :

**Paiement en ligne**

Transaction traitée par l'infrastructure numérique :

- données nécessaires réparties entre plusieurs composants  
- PSP capable d'identifier son client  
- Eurosystème recevant des informations conçues pour ne pas lui permettre d'identifier directement l'utilisateur

**Paiement hors ligne**

Transaction exécutée localement entre appareils :

- détails personnels conservés sur les appareils  
- PSP ne recevant pas les détails personnels de la transaction  
- Eurosystème ne recevant pas les détails personnels de la transaction

Cette distinction constitue une garantie architecturale importante dans l'analyse des possibilités de traçage des paiements.

---

### Les opérations de chargement et de déchargement restent distinctes

Le caractère privé du paiement hors ligne ne signifie cependant pas que l'utilisateur puisse acquérir ou convertir des euros numériques hors ligne sans aucune interaction avec son prestataire.

Les opérations permettant de charger des fonds dans la fonctionnalité hors ligne ou de les reconvertir vers d'autres formes de monnaie nécessitent l'intervention du prestataire de services de paiement [S26].

La BCE indique que les contrôles relatifs à la lutte contre le blanchiment sont effectués par le PSP au moment de ces opérations de chargement et de déchargement, selon une logique comparable aux contrôles applicables aux retraits et dépôts d'espèces [S23][S26].

Il faut donc distinguer :

**Chargement des fonds**   → interaction avec le PSP  
**Paiement hors ligne**    → transfert local entre appareils  
**Déchargement des fonds** → interaction avec le PSP

**AVÉRÉ :**

> La confidentialité du paiement hors ligne concerne la transaction réalisée entre les utilisateurs ; elle ne supprime pas les interactions réglementées avec le PSP nécessaires à l'entrée et à la sortie des fonds du dispositif hors ligne [S23][S26].

---

### Une valeur stockée localement implique des protections techniques spécifiques

La possibilité d'effectuer une transaction sans connexion nécessite que l'appareil puisse conserver et transférer de manière sécurisée la valeur correspondante.

Les travaux actuels de la BCE reposent notamment sur l'utilisation d'un élément matériel sécurisé [S26].

Ce composant protège notamment :

- les clés cryptographiques ;  
- la valeur disponible ;  
- les opérations de débit et de crédit ;  
- les informations critiques nécessaires au fonctionnement du mécanisme hors ligne [S26].

L'objectif est notamment d'empêcher qu'un utilisateur puisse modifier artificiellement son solde ou reproduire la même valeur pour effectuer plusieurs paiements.

Le mode hors ligne n'est donc pas simplement un mode en ligne temporairement déconnecté : il nécessite une architecture technique spécifiquement conçue pour permettre un transfert de valeur local et sécurisé.

---

### Une protection qui limite également certaines possibilités d'interconnexion

Les garanties du mode hors ligne ont une conséquence importante pour l'objet de cette enquête.

Si les détails d'une transaction restent exclusivement sur les appareils du payeur et du bénéficiaire et ne sont transmis ni au PSP ni à l'Eurosystème, les infrastructures externes ne disposent pas automatiquement des informations nécessaires pour rattacher ce paiement individuel à d'autres bases de données.

**DÉDUCTIBLE TECHNIQUEMENT :**

> L'architecture hors ligne actuellement décrite constitue donc un obstacle technique à un rapprochement centralisé systématique entre chaque paiement individuel et des informations provenant d'autres infrastructures, puisque les détails personnels de la transaction ne remontent pas dans l'infrastructure centrale.

Cette conclusion doit cependant rester limitée au fonctionnement hors ligne tel qu'il est actuellement conçu.

Elle ne permet pas de conclure que toutes les interactions entourant le paiement sont anonymes, puisque les opérations de chargement et de déchargement impliquent le PSP.

Elle ne permet pas non plus d'affirmer qu'aucune limite d'utilisation, règle de sécurité ou mécanisme antifraude ne puisse être appliqué au dispositif hors ligne.

Ces éléments doivent être examinés séparément.

---

### Une architecture actuellement testée

Le fonctionnement hors ligne ne constitue plus uniquement une hypothèse conceptuelle.

La BCE prépare un pilote de l'euro numérique prévu à partir du second semestre 2027 et poursuit actuellement les travaux nécessaires à la mise en œuvre de la fonctionnalité hors ligne [S26].

En août 2026, la BCE a notamment lancé une consultation technique concernant les standards nécessaires au déploiement du mode hors ligne dans les composants matériels sécurisés des smartphones.

Les travaux portent notamment sur les embedded Secure Elements et les eSIM.

**AVÉRÉ :**

> L'architecture hors ligne fait donc actuellement l'objet de travaux techniques concrets portant sur les composants matériels, les standards de sécurité et la préparation du pilote [S26].

Elle reste néanmoins une fonctionnalité d'un projet qui n'est pas encore déployé comme moyen de paiement en circulation générale.

---

### Ce que le mode hors ligne ne permet pas d'affirmer

L'existence d'une fonctionnalité hors ligne ne signifie pas que tous les paiements en euros numériques seront privés de la même manière.

Les paiements en ligne suivent une architecture différente.

Elle ne signifie pas non plus que le mode hors ligne sera nécessairement utilisable sans aucune limite de montant, de détention, de fréquence ou de sécurité.

Enfin, l'absence de remontée des détails personnels d'une transaction hors ligne ne permet pas de déduire que le commerçant ou le bénéficiaire ne dispose lui-même d'aucune information relative à l'achat dans ses propres systèmes commerciaux.

Un commerçant peut disposer séparément :

- d'un ticket de caisse ;  
- d'une commande ;  
- d'un compte client ;  
- d'une facture ;  
- d'un identifiant produit ;  
- ou d'autres données commerciales.

**NON ÉTABLI :**

> Les sources étudiées ne permettent donc pas de conclure que le mode hors ligne rend impossible tout rapprochement effectué indépendamment par le commerçant ou par un autre système disposant séparément des données commerciales nécessaires.

Cette distinction est essentielle : la confidentialité du **rail de paiement** ne signifie pas nécessairement l'absence de données dans le **système commercial** situé autour de ce paiement.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> L'euro numérique est conçu pour permettre des paiements en ligne et hors ligne reposant sur des architectures différentes [S23][S26].

**AVÉRÉ :**

> Le paiement hors ligne doit pouvoir être exécuté directement entre les appareils du payeur et du bénéficiaire sans connexion à Internet et sans intervention d'un système en ligne au moment de la transaction [S26].

**AVÉRÉ :**

> La valeur et les informations sensibles nécessaires au paiement hors ligne doivent être protégées dans un environnement matériel sécurisé de l'appareil [S26].

**AVÉRÉ :**

> Selon l'architecture annoncée par la BCE, les détails personnels des transactions hors ligne ne sont accessibles ni à l'Eurosystème ni aux PSP et restent connus du payeur et du bénéficiaire [S23][S26].

**AVÉRÉ :**

> Les opérations permettant de charger ou décharger les fonds restent en revanche liées au PSP, qui effectue les contrôles réglementaires correspondants [S23][S26].

**DÉDUCTIBLE TECHNIQUEMENT :**

> L'absence de transmission centrale des détails d'un paiement hors ligne limite fortement la possibilité d'effectuer, au niveau de l'infrastructure de paiement, un rapprochement centralisé systématique de cette transaction avec des données fiscales, commerciales ou environnementales externes.

**NON ÉTABLI :**

> Cette protection ne permet pas de conclure qu'aucun rapprochement ne puisse être réalisé indépendamment dans le système commercial du bénéficiaire lorsque celui-ci dispose de données permettant d'identifier la transaction, le produit ou le client.

**À ÉTABLIR :**

> Quelles limites de montant, de détention, de fréquence ou de fonctionnement seront finalement appliquées aux paiements hors ligne ?

**À ÉTABLIR :**

> Quelles informations relatives aux opérations de chargement et de déchargement seront conservées par les PSP et pendant quelle durée ?

**À ÉTABLIR :**

> Dans quelles conditions les mécanismes de sécurité, de lutte contre la fraude ou de gestion des limites peuvent-ils empêcher ou différer une opération hors ligne ?

**À ÉTABLIR :**

> Un paiement hors ligne peut-il participer à un mécanisme de paiement conditionnel ou les mécanismes conditionnels nécessitent-ils nécessairement une composante en ligne ?

---

## 4.5 Monnaie programmable et paiements conditionnels

**Statut : AVÉRÉ / DÉDUCTIBLE TECHNIQUEMENT / PROJET EN COURS**

La distinction entre monnaie programmable et paiement conditionnel constitue un élément central de l'architecture envisagée pour l'euro numérique.

La Banque centrale européenne exclut explicitement que l'euro numérique devienne une monnaie programmable [S22][S27].

Parallèlement, l'architecture est conçue pour permettre des paiements conditionnels, c'est-à-dire des paiements dont l'exécution peut être déclenchée automatiquement lorsque certaines conditions prédéfinies sont remplies [S27].

Ces deux mécanismes ne doivent pas être confondus.

---

### La monnaie programmable est explicitement exclue

La BCE définit la monnaie programmable comme une monnaie dont l'utilisation serait intrinsèquement limitée selon certaines règles.

Une telle monnaie pourrait, par exemple, être conçue pour :

- ne permettre l'achat que de certains biens ou services ;  
- ne pouvoir être utilisée que pendant une période déterminée ;  
- ne pouvoir être dépensée que dans une zone géographique particulière ;  
- ou imposer directement d'autres restrictions d'utilisation attachées aux unités monétaires [S27].

La BCE indique explicitement que ce fonctionnement est incompatible avec les principes retenus pour l'euro numérique.

Les unités d'euros numériques doivent rester fongibles et conserver la même valeur que les autres formes de l'euro.

**AVÉRÉ :**

> L'Eurosystème exclut explicitement que les unités d'euros numériques comportent elles-mêmes des règles limitant les biens, services, périodes, lieux ou bénéficiaires pour lesquels elles peuvent être utilisées [S22][S27].

La BCE présente cette garantie comme une différence fondamentale entre une monnaie et un bon ou voucher affecté à un usage déterminé.

---

### Un paiement peut néanmoins être conditionnel

L'exclusion de la monnaie programmable ne signifie pas que tous les paiements doivent être exécutés immédiatement et sans condition.

La BCE définit les paiements conditionnels comme des paiements exécutés automatiquement lorsque des conditions prédéfinies sont remplies [S27].

La condition ne modifie pas les propriétés des unités monétaires elles-mêmes.

Elle intervient dans le processus déterminant **quand un paiement déterminé doit être exécuté**.

La distinction peut être résumée ainsi :

**Monnaie programmable**

La règle est attachée à la monnaie elle-même.  
Exemple : cette unité monétaire ne peut servir qu'à acheter une catégorie déterminée de biens.

**Paiement conditionnel**

La monnaie reste librement utilisable, mais une transaction déterminée n'est exécutée que lorsque la condition convenue pour cette transaction est satisfaite.  
Exemple : le paiement d'un produit est libéré lorsque sa livraison est confirmée.

**AVÉRÉ :**

> La BCE distingue donc explicitement la restriction attachée à la monnaie, qu'elle exclut, de l'automatisation conditionnelle d'une transaction, qu'elle prévoit dans l'architecture de l'euro numérique [S27].

---

### La réservation des fonds constitue le mécanisme de base

L'architecture envisagée prévoit une fonctionnalité de réservation des fonds permettant de supporter les paiements conditionnels [S27].

Lorsqu'un paiement conditionnel est initié, le montant correspondant peut être temporairement réservé sur le compte du payeur.

Le montant réservé réduit alors le solde disponible pour d'autres dépenses, mais il n'est pas immédiatement transféré au bénéficiaire.

Les fonds restent disponibles pour exécuter le paiement lorsque la condition prévue est satisfaite.

Le mécanisme peut être représenté ainsi :

```
Paiement initié
   ↓
Montant réservé
   ↓
Vérification de la condition
   ↓
Condition satisfaite     → fonds transférés au bénéficiaire
Condition non satisfaite → réservation annulée ou expirée
```

**AVÉRÉ :**

> L'infrastructure centrale envisagée fournit donc une capacité technique de réservation de fonds permettant de différer leur transfert jusqu'à la vérification d'une condition [S27].

---

### Une couche de règlement distincte d'une couche de conditionnalité

Le rapport de clôture de la phase de préparation décrit explicitement une séparation entre deux couches [S27].

La première est la **couche de règlement**, située dans l'infrastructure back-end et fournie par l'Eurosystème.

La seconde est une **couche de conditionnalité**, développée par les acteurs du marché.

La couche de règlement assure le traitement monétaire.

La couche de conditionnalité détermine si les conditions prévues pour libérer les fonds sont satisfaites.

Le fonctionnement peut être représenté ainsi :

**Couche de conditionnalité — acteurs du marché**

```
Vérification d'un événement ou d'une condition
   ↓
Résultat de la vérification
   ↓
Fonction de réservation / infrastructure de paiement
   ↓
Couche de règlement — Eurosystème
   ↓
Transfert ou libération des fonds
```

**AVÉRÉ :**

> L'architecture actuellement décrite sépare donc techniquement la fonction monétaire de règlement et la logique permettant de déterminer si une condition associée à une transaction est remplie [S27].

Cette séparation est essentielle.

Elle signifie que l'Eurosystème n'a pas nécessairement besoin de connaître ou d'évaluer lui-même la donnée ayant servi à vérifier la condition.

---

### Une surveillance externe peut déclencher la condition

Le rapport de clôture de la BCE précise que cette architecture doit permettre une flexibilité pour un **monitoring externe capable de déclencher les conditions** [S27].

Dans l'exemple donné par la BCE, un système peut déterminer qu'un train est effectivement arrivé.

Lorsque cette information confirme la condition prévue, les fonds réservés sont transférés au bénéficiaire.

Si le train n'arrive pas ou si la condition définie n'est pas satisfaite, la réservation peut être annulée ou expirer et les fonds redeviennent disponibles pour le payeur [S27].

**AVÉRÉ :**

> Une information produite ou vérifiée en dehors de la couche de règlement peut donc techniquement participer au déclenchement ou à l'absence de déclenchement d'un paiement conditionnel [S27].

Il s'agit ici d'un premier lien explicitement documenté entre **une donnée ou un événement externe au règlement monétaire** et **l'exécution d'une transaction**.

---

### Des exemples déjà identifiés et expérimentés

Les travaux de la BCE et des acteurs du marché ont étudié plusieurs catégories de paiements conditionnels [S27].

Parmi les exemples documentés figurent notamment :

- le paiement à la livraison ;  
- le paiement à l'usage ;  
- les paiements déclenchés par étapes ou milestones ;  
- les remboursements automatiques ;  
- les abonnements ;  
- les paiements fractionnés ;  
- les paiements machine-to-machine ;  
- certains paiements liés à la consommation d'énergie [S27].

Dans le cas du paiement à la livraison, la transaction peut être finalisée lorsque la livraison du produit est confirmée.

Dans un paiement machine-to-machine, une machine peut participer automatiquement au déclenchement d'un paiement lorsqu'un événement prévu survient.

La BCE et des acteurs du marché ont déjà testé la faisabilité de plusieurs de ces mécanismes dans un environnement simulant le back-end de l'euro numérique [S27].

**AVÉRÉ :**

> Les paiements conditionnels ne constituent donc plus uniquement une possibilité abstraite décrite dans une proposition réglementaire : leur faisabilité technique a fait l'objet d'expérimentations avec des acteurs du marché dans l'environnement d'innovation de la BCE [S27].

Ces expérimentations n'ont cependant pas utilisé de véritables euros numériques et ne constituent pas le déploiement d'un système en production.

---

### La condition peut être vérifiée par un tiers

Les travaux antérieurs de la BCE fournissent également un exemple dans lequel le déclenchement d'un paiement à la livraison peut dépendre d'un tiers autre que le payeur ou le bénéficiaire, comme le service postal chargé de confirmer la livraison d'un produit [S27].

Cette architecture introduit donc potentiellement un troisième acteur dans la décision technique permettant de poursuivre le paiement.

```
Payeur + bénéficiaire définissent ou acceptent la condition
   ↓
Tiers ou système externe vérifie l'événement
   ↓
Confirmation de la condition
   ↓
Paiement exécuté automatiquement
```

**AVÉRÉ :**

> La vérification d'une condition peut donc être réalisée à partir d'une information provenant d'un acteur ou d'un système distinct du payeur, du bénéficiaire et de la couche centrale de règlement [S27].

---

### Les acteurs du marché développent la logique conditionnelle

La BCE considère que les intermédiaires supervisés et autres acteurs du marché sont les mieux placés pour développer les services de paiement conditionnel [S27].

L'infrastructure de l'euro numérique fournit notamment la fonctionnalité fondamentale de réservation des fonds.

Les acteurs du marché peuvent construire au-dessus de cette infrastructure des services à valeur ajoutée utilisant leurs propres logiques et les informations nécessaires aux cas d'usage concernés.

En juillet 2026, la BCE indiquait également que les banques pourraient utiliser l'infrastructure de l'euro numérique pour déclencher automatiquement des paiements lorsqu'une condition convenue est remplie et développer de nouveaux services en s'appuyant sur les données dont elles disposent [S27].

**AVÉRÉ :**

> La logique conditionnelle n'est donc pas conçue comme une fonction exclusivement définie et opérée par la Banque centrale européenne : des banques, PSP et autres acteurs du marché peuvent développer des services conditionnels au-dessus de l'infrastructure commune [S27].

---

### Le premier pont technique avec des données externes

Les sections précédentes ont établi que l'architecture de paiement peut traiter différentes informations relatives aux transactions et que les acteurs du marché disposent de leurs propres systèmes et données.

La présente section ajoute un élément supplémentaire : la couche de conditionnalité peut utiliser la vérification d'un événement externe afin de déterminer si les fonds réservés doivent être transférés [S27].

Le mécanisme général devient donc :

```
Donnée ou événement externe
   ↓
Vérification de la condition
   ↓
Couche de conditionnalité
   ↓
Instruction liée aux fonds réservés
   ↓
Exécution ou absence d'exécution du paiement
```

**AVÉRÉ :**

> Le principe selon lequel une information externe au règlement monétaire peut déclencher l'exécution d'un paiement conditionnel est explicitement prévu dans l'architecture étudiée [S27].

Cette constatation constitue un **pont technique entre une information externe et l'exécution d'un paiement**.

Elle ne permet cependant pas de conclure que n'importe quelle information peut être utilisée comme condition.

---

### Ce pont ne démontre pas l'utilisation de données environnementales

Aucune des sources étudiées dans cette section ne prévoit qu'un paiement soit conditionné par :

- l'empreinte carbone d'un produit ;  
- un passeport numérique de produit ;  
- un GTIN ;  
- une empreinte environnementale cumulée ;  
- un quota environnemental individuel ;  
- une donnée fiscale issue de la facturation électronique ;  
- ou un profil comportemental d'un utilisateur.

Les exemples actuellement documentés concernent principalement des événements directement liés à l'exécution d'un contrat ou d'un service : livraison, réalisation d'une prestation, utilisation d'un service, horaire, consommation ou événement vérifiable [S27].

**NON ÉTABLI :**

> L'existence d'une couche de conditionnalité capable d'utiliser des informations externes ne démontre pas qu'elle soit actuellement conçue pour recevoir ou utiliser des données environnementales, fiscales ou des profils individuels.

Cette distinction est fondamentale pour l'analyse.

---

### Mais la nature technique de la condition n'est pas intrinsèquement monétaire

La condition permettant de déclencher le paiement peut correspondre à un événement vérifié par un système distinct.

Le système de règlement n'a pas nécessairement besoin de connaître l'ensemble des informations ayant permis d'établir que cette condition est satisfaite.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une architecture de paiement conditionnel peut techniquement utiliser le résultat d'une vérification effectuée par un système externe sans que les données ayant servi à cette vérification soient directement intégrées dans l'infrastructure monétaire.

Par exemple, le système de paiement pourrait recevoir uniquement un résultat logique :

```
Condition vérifiée : OUI  
 ou  
Condition vérifiée : NON
```

sans recevoir nécessairement toutes les données ayant conduit à ce résultat.

Cette propriété technique signifie qu'une interconnexion n'exige pas nécessairement la fusion complète des bases de données concernées.

---

### Qui décide de la condition constitue une question juridique distincte

La possibilité technique de construire une condition ne signifie pas que n'importe quel acteur puisse imposer arbitrairement cette condition à un utilisateur.

La BCE indique que les paiements conditionnels reposent sur des conditions prédéfinies et convenues et affirme que les utilisateurs restent libres de choisir l'utilisation de ces services [S27].

Dans une communication de janvier 2026, la BCE a également précisé que les conditions d'un paiement ne pourraient être fixées que par le payeur et le bénéficiaire.

**AVÉRÉ :**

> Dans le cadre actuellement présenté par la BCE, les paiements conditionnels constituent des services volontaires reposant sur des conditions convenues entre les parties et ne donnent pas à l'Eurosystème un pouvoir général permettant de déterminer ce qu'un utilisateur peut acheter [S27].

Cette garantie doit être distinguée de la capacité technique du système à exécuter automatiquement une transaction lorsque la condition convenue est satisfaite.

---

### La frontière exacte avec une restriction externe doit rester surveillée

La distinction conceptuelle entre monnaie programmable et paiement conditionnel est claire :

- la monnaie programmable impose une restriction à l'unité monétaire elle-même ;  
- le paiement conditionnel applique une logique à une transaction déterminée.

Mais du point de vue de l'utilisateur, une condition peut néanmoins avoir pour effet pratique qu'un paiement déterminé ne soit pas exécuté tant que le critère prévu n'est pas satisfait.

Cette observation ne permet pas de qualifier le système de monnaie programmable.

Elle montre seulement que **l'absence de programmabilité de la monnaie n'implique pas l'absence de logique programmable autour de l'exécution des paiements**.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une infrastructure peut donc simultanément utiliser une monnaie totalement fongible et non programmable tout en permettant à des services externes d'appliquer des règles automatisées à l'exécution de transactions particulières.

La question déterminante devient alors celle de la gouvernance de ces règles : qui peut définir une condition, avec quel consentement, à partir de quelles données et dans quel cadre juridique ?

---

### Conclusion intermédiaire

**AVÉRÉ :**

> La BCE exclut explicitement que l'euro numérique soit une monnaie programmable limitant intrinsèquement les biens, services, périodes, lieux ou bénéficiaires pour lesquels les unités monétaires peuvent être utilisées [S22][S27].

**AVÉRÉ :**

> L'architecture prévoit néanmoins des paiements conditionnels exécutés automatiquement lorsque des conditions prédéfinies sont satisfaites [S27].

**AVÉRÉ :**

> Une fonctionnalité de réservation des fonds est prévue afin de conserver temporairement le montant nécessaire jusqu'à la vérification de la condition [S27].

**AVÉRÉ :**

> La BCE décrit une architecture séparant une couche de règlement fournie par l'Eurosystème et une couche de conditionnalité développée par les acteurs du marché, avec la possibilité qu'une vérification externe déclenche la condition [S27].

**AVÉRÉ :**

> Des paiements conditionnels ont déjà été expérimentés dans un environnement simulé avec des acteurs du marché, notamment pour des scénarios de paiement à la livraison, paiement à l'usage, paiements par étapes et autres services automatisés [S27].

**AVÉRÉ :**

> La BCE indique que les banques et autres prestataires pourront développer des services conditionnels au-dessus de l'infrastructure commune et s'appuyer sur les données dont ils disposent pour proposer des services innovants [S27].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une information provenant d'un système externe peut techniquement participer à l'exécution ou à la non-exécution d'une transaction sans que cette information soit nécessairement stockée dans la monnaie elle-même ni intégralement transmise à la couche de règlement.

**NON ÉTABLI :**

> Les sources étudiées ne permettent pas d'établir que des données environnementales, des DPP, des données fiscales ou un profil individuel soient utilisés comme conditions de paiement dans l'architecture actuellement prévue.

**AVÉRÉ :**

> Dans le cadre actuellement présenté par la BCE, les conditions sont conçues comme convenues par les parties et l'Eurosystème affirme ne pas disposer du pouvoir permettant de bloquer des catégories d'achats [S27].

**À ÉTABLIR :**

> Quelles catégories de données externes peuvent techniquement être utilisées par les services développant la couche de conditionnalité ?

**À ÉTABLIR :**

> Quels acteurs peuvent fournir la preuve ou le résultat permettant de considérer une condition comme satisfaite ?

**À ÉTABLIR :**

> Quelles garanties juridiques empêchent qu'une condition initialement conçue comme volontaire ou contractuelle soit imposée par un intermédiaire, une réglementation ou un autre acteur ?

**À ÉTABLIR :**

> Existe-t-il des projets ou expérimentations reliant les paiements conditionnels à des infrastructures de facturation, de traçabilité des produits ou de données environnementales ?

---

## 4.6 Conditions externes et automatisation des paiements

**Statut : AVÉRÉ / DÉDUCTIBLE TECHNIQUEMENT / À ÉTABLIR**

La section précédente a établi que l'architecture envisagée pour l'euro numérique distingue une couche de règlement fournie par l'Eurosystème et une couche de conditionnalité développée par les acteurs du marché [S27].

Les travaux menés dans le cadre de la plateforme d'innovation permettent d'aller plus loin : des acteurs du marché ont effectivement connecté leurs propres plateformes à un environnement simulant les interfaces de l'euro numérique afin d'expérimenter des paiements conditionnels [S28].

Il devient donc possible de distinguer trois composants :

```
système ou plateforme externe
   ↓
logique permettant de vérifier une condition
   ↓
infrastructure permettant de réserver puis de transférer les fonds
```
Cette architecture a fait l'objet d'expérimentations techniques, même si l'euro numérique lui-même n'est pas encore en circulation [S28].

---

### Les plateformes des participants ont été connectées aux interfaces simulées

Dans le cadre du groupe de travail des « pioneers », la BCE a fourni aux participants un environnement simulant le back-end de l'euro numérique ainsi que des spécifications techniques et des interfaces de programmation [S28].

Les participants ont pu connecter leurs propres plateformes à cet environnement au moyen d'API.

Ils agissaient, dans l'expérimentation, comme des prestataires développant leurs propres services au-dessus des fonctionnalités centrales fournies par l'Eurosystème.

**AVÉRÉ :**

> Des plateformes développées ou exploitées par des acteurs du marché ont donc effectivement été connectées, à titre expérimental, à des interfaces simulant l'infrastructure de l'euro numérique [S28].

Il ne s'agit pas encore d'une connexion au futur système de production.

Cette expérimentation démontre néanmoins que l'architecture est conçue pour permettre à des systèmes externes développés par les acteurs du marché d'utiliser les fonctionnalités fournies par l'infrastructure commune.

---

### L'Eurosystème fournit la fonction monétaire, le marché développe la condition

La répartition des responsabilités expérimentée reprend la séparation décrite précédemment [S27][S28].

L'Eurosystème fournit les fonctions fondamentales nécessaires au traitement monétaire, notamment la réservation des fonds.

Les PSP et autres acteurs du marché développent la couche déterminant les conditions nécessaires à leur libération.

Le mécanisme peut être représenté ainsi :

```
**Infrastructure de l'Eurosystème**
réservation des fonds
   ↓
**Plateforme du PSP ou de l'acteur du marché**
définition et gestion de la condition
   ↓
**Information permettant de vérifier la condition**
   ↓
condition satisfaite
   ↓
instruction permettant la libération des fonds
```

**AVÉRÉ :**

> Dans les expérimentations réalisées, la logique déterminant la condition n'était donc pas nécessairement située dans l'infrastructure centrale de l'Eurosystème : elle pouvait être développée et gérée par les plateformes des acteurs du marché [S28].

---

### La condition peut dépendre d'un événement extérieur au paiement

Plusieurs scénarios étudiés montrent que la condition n'a pas besoin d'être une information produite par le système monétaire lui-même [S27][S28].

Dans un paiement à la livraison, l'information déterminante est la confirmation de la livraison du produit.

Dans un remboursement lié à un transport, elle peut être liée à l'exécution, au retard ou à l'annulation du service.

Dans un paiement à l'usage, elle peut dépendre de l'utilisation effective d'un service ou d'un équipement.

Dans un paiement par étapes, elle peut dépendre de la réalisation successive d'objectifs ou de jalons prédéfinis [S28].

**AVÉRÉ :**

> Les conditions étudiées peuvent donc dépendre de faits ou d'événements produits en dehors de l'infrastructure monétaire et vérifiés par la couche conditionnelle développée par les acteurs du marché [S27][S28].

---

### Un système externe n'a pas nécessairement besoin de transmettre toutes ses données

La séparation entre couche conditionnelle et couche de règlement permet qu'un système externe effectue lui-même certaines vérifications.

La couche monétaire n'a alors pas nécessairement besoin de recevoir l'ensemble des informations ayant permis d'effectuer cette vérification.

Le mécanisme peut être résumé ainsi :

```
système externe dispose d'une information
   ↓
système externe vérifie une règle
   ↓
résultat : condition satisfaite ou non satisfaite
   ↓
couche conditionnelle traite ce résultat
   ↓
fonds libérés ou maintenus réservés
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une donnée utilisée pour déterminer l'exécution d'un paiement n'a donc pas nécessairement besoin d'être stockée dans l'infrastructure monétaire ni même transmise intégralement à celle-ci : un résultat de vérification peut techniquement suffire.

Cette propriété est importante pour l'étude des interconnexions.

L'absence d'une donnée dans le dictionnaire de données de l'euro numérique ne suffit pas, à elle seule, à démontrer que cette donnée ne puisse jamais participer indirectement à la logique d'un service de paiement développé autour de l'infrastructure.

---

### Les paiements machine-to-machine étendent l'automatisation

Les expérimentations ont également étudié des scénarios liés à l'Industrie 4.0 et aux paiements machine-to-machine [S28].

Dans ces scénarios, des équipements ou systèmes numériques peuvent participer automatiquement à l'initiation ou au déclenchement d'opérations financières.

Un exemple étudié concerne une machine détectant elle-même le besoin d'une pièce de remplacement et participant à l'automatisation du processus commercial correspondant.

Ces scénarios cherchent notamment à réduire les interventions manuelles et à permettre des règlements en temps réel ou fondés sur l'utilisation effective d'un service [S28].

**AVÉRÉ :**

> Les travaux d'expérimentation ne se limitent donc pas à des paiements déclenchés manuellement par une personne : ils examinent également des chaînes dans lesquelles des systèmes ou machines peuvent participer automatiquement à l'initiation et au traitement d'une transaction [S28].

Cette automatisation ne signifie pas qu'une machine puisse dépenser arbitrairement l'argent d'un utilisateur : elle intervient dans un cadre de service, de mandat, d'autorisation et de conditions préalablement définies.

---

### Des jalons peuvent déterminer progressivement la libération des fonds

Les expérimentations ont étudié des paiements fondés sur des étapes ou « milestones » [S28].

Dans ce type de scénario, la totalité des fonds n'est pas nécessairement libérée en une seule fois.

Le versement peut être effectué progressivement lorsque différents objectifs prédéfinis sont considérés comme atteints.

Un exemple étudié concerne une formation en ligne pour laquelle les fonds pourraient être libérés progressivement lorsque l'apprenant atteint certains objectifs.

Un autre exemple concerne le financement participatif, dans lequel des fonds pourraient être libérés selon l'avancement d'un projet [S28].

**AVÉRÉ :**

> Une condition externe peut donc non seulement déterminer si un paiement doit être exécuté, mais également participer à la détermination du moment ou de l'étape à laquelle une partie des fonds doit être libérée [S28].

---

### Les paiements à l'usage reposent sur une donnée mesurable

Le paiement à l'usage constitue une autre catégorie étudiée par la plateforme [S28].

Dans ce type de mécanisme, le montant ou le moment du paiement dépend de l'utilisation effective d'un bien ou d'un service.

La condition peut donc être alimentée par une information mesurant cette utilisation.

Cela peut concerner notamment des services de mobilité, des infrastructures ou certains équipements connectés.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Lorsqu'un système externe est capable de mesurer un événement ou une quantité et de communiquer le résultat correspondant à la couche conditionnelle, cette information peut techniquement participer à l'automatisation du paiement.

Il s'agit d'un principe général de fonctionnement des paiements conditionnels et non de la preuve que toute catégorie de donnée puisse être utilisée sans restriction.

---

### L'automatisation peut également concerner les remboursements

Les travaux de la BCE ne portent pas uniquement sur le déclenchement d'un paiement vers un commerçant [S27][S28].

Ils examinent également l'automatisation de remboursements lorsque certaines conditions sont satisfaites.

Dans le domaine des transports, par exemple, une annulation ou un retard peut conduire à l'automatisation d'un remboursement.

Le même principe général s'applique :

```
événement externe
   ↓
vérification de la situation
   ↓
déclenchement automatique
   ↓
paiement ou remboursement
```

**AVÉRÉ :**

> L'utilisation d'une condition externe peut donc agir sur différents flux financiers, notamment la libération d'un paiement ou le déclenchement d'un remboursement [S27][S28].

---

### Le paiement peut être associé à des informations commerciales complémentaires

La plateforme d'innovation a également étudié des services complémentaires tels que les reçus électroniques [S28].

La BCE présente les e-receipts comme une fonctionnalité susceptible d'être associée aux paiements en euros numériques afin de permettre notamment aux utilisateurs de suivre leurs dépenses et de gérer leurs garanties.

Cette fonctionnalité est distincte du règlement monétaire.

Elle montre cependant que les acteurs du marché envisagent des services dans lesquels une transaction de paiement peut être associée à des informations commerciales supplémentaires.

**AVÉRÉ :**

> Les travaux de la plateforme d'innovation envisagent donc également l'association d'un paiement en euros numériques avec des informations commerciales extérieures au strict transfert monétaire, notamment au moyen de reçus électroniques [S28].

**À ÉTABLIR :**

> Quelle granularité ces reçus électroniques pourraient-ils contenir et pourraient-ils notamment inclure des références de produits, des lignes d'achat ou des identifiants standardisés ?

---

### Le lien avec le produit devient techniquement concret dans certains scénarios

Le scénario de paiement à la livraison repose déjà sur une relation entre :

- une commande ;  
- un produit acheté ;  
- une livraison ;  
- une transaction ;  
- une condition ;  
- et la libération des fonds [S27][S28].

Le système doit être capable de déterminer que l'événement vérifié correspond à la transaction pour laquelle les fonds ont été réservés.

Il existe donc nécessairement, dans le service développé autour du paiement, un mécanisme permettant de rapprocher la condition vérifiée de la transaction concernée.

**AVÉRÉ :**

> Les scénarios expérimentés démontrent qu'une plateforme externe peut techniquement associer un événement commercial relatif à une commande ou à un service à la transaction dont l'exécution dépend de cet événement [S28].

Cela ne signifie pas que l'infrastructure centrale connaît le détail du produit.

Le rapprochement peut être effectué dans la plateforme externe, qui transmet ensuite uniquement l'information nécessaire à la poursuite du paiement.

---

### Le pont générique entre données externes et paiement est établi

À ce stade, plusieurs éléments peuvent être assemblés.

Le chapitre 4 a établi :

- qu'une transaction possède des identifiants structurés [S25] ;  
- qu'une architecture de réservation des fonds permet de différer leur transfert [S27] ;  
- qu'une couche de conditionnalité peut être développée par des acteurs du marché [S27][S28] ;  
- qu'un monitoring externe peut déclencher une condition [S27] ;  
- que les plateformes des participants ont effectivement été connectées aux interfaces simulées de l'euro numérique [S28] ;  
- que des événements commerciaux extérieurs au règlement ont été utilisés dans les scénarios de paiement conditionnel [S28].

La chaîne suivante est donc désormais documentée dans son principe :

```
événement ou donnée provenant d'un système externe
   ↓
plateforme ou service de l'acteur du marché
   ↓
vérification d'une condition
   ↓
association avec la transaction correspondante
   ↓
utilisation de la fonctionnalité de réservation des fonds
   ↓
exécution, libération, maintien ou restitution des fonds selon le scénario
```

**AVÉRÉ :**

> L'architecture et les expérimentations étudiées établissent donc qu'un système externe à la couche de règlement peut fournir ou vérifier une information utilisée par un service conditionnel afin de déterminer l'exécution d'une transaction déterminée [S27][S28].

Ce constat dépasse désormais la simple possibilité abstraite d'une architecture informatique : le mécanisme général a fait l'objet d'expérimentations techniques avec des plateformes d'acteurs du marché connectées à un environnement simulant l'euro numérique [S28].

---

### Le pont spécifique avec les données environnementales n'est pas établi

Cette conclusion ne doit cependant pas être étendue au-delà de ce que démontrent les sources.

Aucune des expérimentations étudiées ne permet d'établir qu'une condition de paiement a été alimentée par :

- un passeport numérique de produit ;  
- un identifiant DPP ;  
- un GTIN utilisé pour consulter un DPP ;  
- l'empreinte carbone d'un produit ;  
- une empreinte environnementale cumulée ;  
- une donnée issue du système français de facturation électronique ;  
- un profil environnemental individuel.

**NON ÉTABLI :**

> Le pont générique entre système externe et paiement conditionnel est documenté, mais le pont spécifique entre données environnementales ou fiscales et exécution d'un paiement ne l'est pas à ce stade.

Cette distinction constitue une limite essentielle de l'enquête.

---

### La combinaison avec le chapitre 3 devient néanmoins techniquement analysable

Le chapitre 3 a établi séparément qu'un produit peut être associé à un identifiant numérique et à des données environnementales structurées et que, lorsque des identifiants compatibles existent, ces informations peuvent techniquement être rapprochées d'une transaction commerciale.

Le présent chapitre établit maintenant qu'une information provenant d'un système externe peut être vérifiée dans une couche de conditionnalité et participer à l'exécution d'un paiement.

Ces deux constats ne démontrent pas leur interconnexion effective.

Ils permettent néanmoins d'identifier précisément le raccord technique qui serait nécessaire :

```
transaction ou commande
   ↓
produit identifiable
   ↓
système externe disposant d'une information relative au produit
   ↓
règle ou condition appliquée dans un service externe
   ↓
résultat de la vérification
   ↓
couche de conditionnalité du paiement
   ↓
exécution ou absence d'exécution selon la condition
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Si un acteur autorisé disposait d'une donnée environnementale relative à un produit et si cette donnée était utilisée comme critère d'une condition de paiement, l'architecture décrite pour les paiements conditionnels permettrait techniquement que le résultat de cette vérification participe à l'exécution de la transaction sans que la donnée environnementale soit intégrée à la monnaie elle-même.

Cette proposition décrit une possibilité technique résultant de la combinaison de composants documentés séparément.

**Elle ne démontre ni l'existence d'un tel service, ni son autorisation juridique, ni son utilisation par une administration, une banque ou un PSP.**

---

### Une interconnexion ne nécessite pas nécessairement une base de données unique

Les résultats obtenus dans les chapitres 3 et 4 montrent également qu'une éventuelle interconnexion n'aurait pas nécessairement besoin de centraliser toutes les informations dans un système unique.

Un service pourrait théoriquement :

```
recevoir l'identifiant nécessaire à une transaction
   ↓
interroger un système externe autorisé
   ↓
vérifier une condition
   ↓
obtenir un résultat
   ↓
transmettre uniquement ce résultat au système chargé du paiement
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> L'absence de fusion physique entre les bases de données environnementales, commerciales et monétaires ne suffit donc pas à exclure techniquement un mécanisme de décision reposant sur leur interopérabilité.

Cette déduction est cohérente avec les architectures étudiées : elles reposent précisément sur des identifiants, des API, des droits d'accès et des échanges entre composants spécialisés.

---

### Le consentement et la gouvernance restent déterminants

La capacité technique d'utiliser une condition externe ne détermine pas qui possède le droit de définir cette condition.

Dans les cas d'usage actuellement présentés par la BCE, les paiements conditionnels constituent des services destinés à répondre à un besoin du payeur et du bénéficiaire [S27].

Ils ne constituent pas un pouvoir général accordé à l'Eurosystème pour décider quels achats doivent être autorisés.

Une distinction doit donc être maintenue entre :

- une condition volontaire choisie dans un service ;  
- une condition contractuelle imposée par les conditions d'utilisation d'un service ;  
- une condition réglementaire imposée par le droit ;  
- une décision prise par un intermédiaire conformément à ses obligations légales ;  
- une restriction attachée à la monnaie elle-même.

Ces situations peuvent produire des effets techniques similaires sur une transaction mais reposent sur des bases juridiques et des acteurs décisionnaires différents.

**À ÉTABLIR :**

> Quelles garanties empêchent ou encadrent l'utilisation de la couche conditionnelle pour des critères autres que ceux volontairement acceptés par le payeur et le bénéficiaire ?

---

### Les expérimentations continuent en 2026

Les travaux de la plateforme d'innovation ne se sont pas arrêtés à la première expérimentation [S28].

La BCE a annoncé une nouvelle phase de collaboration avec les acteurs du marché en 2026.

Cette phase doit notamment approfondir les paiements conditionnels et d'autres services à valeur ajoutée, tels que les reçus électroniques, le partage de factures et les outils de gestion budgétaire.

La BCE indique également vouloir poursuivre l'exploration des paiements machine-to-machine, de l'intelligence artificielle appliquée aux paiements, des micropaiements et de différents cas d'usage B2B.

**AVÉRÉ :**

> L'intégration de services externes et l'automatisation des paiements constituent donc toujours un domaine actif de développement et d'expérimentation du projet en 2026 [S28].

Les caractéristiques définitives des services qui en résulteront ne sont cependant pas encore établies.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> Des acteurs du marché ont connecté leurs propres plateformes, au moyen d'API, à un environnement simulant les interfaces de l'euro numérique afin de tester des paiements conditionnels [S28].

**AVÉRÉ :**

> Dans l'architecture expérimentée, l'Eurosystème fournit les fonctionnalités monétaires fondamentales tandis que les PSP et autres acteurs du marché peuvent développer et gérer la logique déterminant les conditions de libération des fonds [S27][S28].

**AVÉRÉ :**

> Les conditions expérimentées peuvent dépendre d'événements externes au règlement monétaire, notamment une livraison, l'utilisation d'un service, l'accomplissement d'une étape ou d'autres événements vérifiables [S28].

**AVÉRÉ :**

> Des scénarios machine-to-machine ont également été étudiés, permettant à des systèmes ou équipements de participer automatiquement à certains processus commerciaux et de paiement [S28].

**AVÉRÉ :**

> Le mécanisme générique permettant à un système externe de fournir ou vérifier une information participant à l'exécution d'un paiement conditionnel a donc dépassé le stade de la simple hypothèse technique et a fait l'objet d'expérimentations dans un environnement simulé [S27][S28].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une donnée externe n'a pas nécessairement besoin d'être directement transmise ou stockée dans l'infrastructure monétaire : la couche conditionnelle peut techniquement effectuer ou recevoir une vérification et communiquer seulement le résultat nécessaire à l'exécution du paiement.

**DÉDUCTIBLE TECHNIQUEMENT :**

> La combinaison avec les infrastructures étudiées au chapitre 3 rend techniquement possible une architecture dans laquelle une caractéristique environnementale d'un produit serait vérifiée dans un système externe puis utilisée comme critère d'un service de paiement conditionnel.

**NON ÉTABLI :**

> Aucun élément étudié ne permet cependant d'établir qu'un DPP, un GTIN, une empreinte carbone, une donnée issue de la facturation électronique ou un profil environnemental individuel soit actuellement utilisé pour déclencher, empêcher ou modifier un paiement en euros numériques.

**À ÉTABLIR :**

> Existe-t-il des expérimentations, consortiums, marchés publics, spécifications ou partenariats reliant concrètement les infrastructures de traçabilité des produits, de facturation électronique ou de données environnementales aux services de paiement conditionnel ?

**À ÉTABLIR :**

> Les reçus électroniques envisagés avec l'euro numérique pourront-ils transporter des identifiants de produits ou d'autres informations permettant un rapprochement automatisé avec des systèmes commerciaux ou environnementaux ?

**À ÉTABLIR :**

> Quels acteurs sont présents simultanément dans les projets de DPP, de facturation électronique et d'euro numérique, et développent-ils des interfaces ou services permettant de relier ces infrastructures ?

---

## 4.7 Identité numérique et infrastructures de paiement

**Statut : AVÉRÉ / PROJET EN COURS**

L'identité numérique européenne constitue une infrastructure distincte de l'euro numérique.

Les sources officielles établissent cependant un raccord explicite entre l'European Digital Identity Wallet, ou EUDI Wallet, et les infrastructures de paiement [S29].

La Commission européenne documente un cas d'usage spécifiquement consacré à l'authentification des paiements au moyen de l'EUDI Wallet.

La Banque centrale européenne prévoit parallèlement que les prestataires participant au pilote de l'euro numérique puissent utiliser ce wallet comme méthode d'authentification forte pour certaines transactions en ligne [S29].

Le lien entre identité numérique et paiement n'est donc pas seulement techniquement déductible : il est explicitement prévu dans les architectures étudiées.

---

### L'EUDI Wallet constitue une infrastructure européenne d'identité numérique

Le cadre européen relatif à l'identité numérique prévoit la mise à disposition de wallets permettant aux personnes physiques et morales de s'identifier et de présenter différentes attestations numériques [S29].

Le wallet peut notamment contenir ou permettre de présenter :

- des données d'identité ;  
- des attestations électroniques ;  
- des justificatifs ou attributs vérifiables ;  
- des éléments nécessaires à l'authentification auprès de services publics ou privés.

L'architecture repose sur des formats et protocoles communs permettant aux émetteurs, wallets et parties utilisatrices de vérifier cryptographiquement les informations présentées.

Son utilisation est prévue comme volontaire pour l'utilisateur.

---

### L'EUDI Wallet est explicitement prévu pour les paiements

La Commission européenne documente un cas d'usage intitulé **Payment Authentication** permettant d'utiliser l'EUDI Wallet pour authentifier des paiements en ligne ou en magasin [S29].

Cette architecture est conçue pour fonctionner avec les infrastructures de paiement existantes, notamment les paiements par carte et les paiements de compte à compte.

Le wallet ne constitue donc pas lui-même nécessairement le système transférant les fonds.

Il intervient comme composant permettant notamment d'authentifier le payeur et de présenter les preuves nécessaires à la transaction.

Le fonctionnement général peut être résumé ainsi :

```
utilisateur
   ↓
EUDI Wallet
   ↓
présentation d'une preuve ou d'une attestation
   ↓
banque / PSP / acquéreur / commerçant
   ↓
authentification du paiement
```

**AVÉRÉ :**

> Une infrastructure européenne d'identité numérique est explicitement conçue pour pouvoir intervenir directement dans le processus d'authentification d'un paiement [S29].

---

### Le wallet peut être relié à un payeur et à un compte

La documentation prévoit notamment des attestations d'authentification forte émises par les prestataires de services de paiement [S29].

Ces attestations permettent d'établir un lien vérifiable entre :

- le wallet ;  
- un payeur déterminé ;  
- et un compte ou instrument de paiement déterminé.

Lorsqu'un paiement est initié, le wallet peut présenter l'attestation appropriée à la partie chargée de la vérifier, par exemple une banque, un acquéreur ou un commerçant.

**AVÉRÉ :**

> L'EUDI Wallet peut donc intervenir comme composant cryptographiquement vérifiable reliant l'utilisateur à l'authentification d'une opération de paiement et à l'instrument ou au compte concerné [S29].

Cela ne signifie pas que l'ensemble des informations d'identité contenues dans le wallet soit transmis avec chaque paiement.

---

### La divulgation sélective permet de présenter un attribut sans transmettre toute l'identité

L'architecture de l'EUDI Wallet repose notamment sur un principe de divulgation sélective [S29].

L'utilisateur peut présenter uniquement l'information nécessaire à une interaction donnée plutôt que l'intégralité de son identité ou du document contenant cette information.

La Commission fournit notamment comme exemples :

- l'âge ;  
- la résidence ;  
- certaines informations issues d'un permis de conduire [S29].

Dans un scénario d'achat soumis à une condition d'âge, le système peut ainsi vérifier que l'utilisateur remplit le critère requis sans nécessairement recevoir sa date de naissance complète.

Le principe peut être représenté ainsi :

```
wallet contenant une information vérifiable
   ↓
sélection de l'attribut nécessaire
   ↓
preuve du critère demandé
   ↓
service ou commerçant vérificateur
```

**AVÉRÉ :**

> L'infrastructure permet donc techniquement qu'un attribut relatif à une personne soit vérifié dans le contexte d'un paiement sans nécessiter la transmission de l'ensemble de son identité [S29].

---

### L'âge constitue déjà un exemple concret de critère associé à un achat

La documentation officielle fournit précisément l'exemple d'un achat nécessitant une vérification d'âge [S29].

Dans le parcours présenté par la Commission, l'utilisateur effectue un achat en ligne et utilise son EUDI Wallet dans le processus d'authentification.

Le wallet affiche notamment le commerçant, le montant et les attributs demandés.

L'utilisateur peut ensuite présenter la preuve nécessaire.

**AVÉRÉ :**

> Un attribut personnel vérifiable provenant de l'infrastructure d'identité numérique peut donc déjà être intégré au parcours technique entourant un paiement afin de vérifier une condition applicable à l'achat [S29].

Il est toutefois essentiel de distinguer ce mécanisme d'un paiement conditionnel au sens étudié dans les sections 4.5 et 4.6.

Dans cet exemple, la vérification d'âge répond à une exigence liée à l'accès ou à la vente du produit ; elle ne constitue pas la preuve que l'euro numérique lui-même applique une restriction d'achat.

---

### Le raccord avec l'euro numérique est explicitement prévu

La relation entre l'EUDI Wallet et l'euro numérique n'est pas seulement une possibilité résultant de l'existence de deux infrastructures européennes compatibles.

La documentation de la BCE relative au pilote de l'euro numérique l'indique explicitement [S29].

Les PSP participant au pilote pourront prendre en charge l'EUDI Wallet comme méthode d'authentification forte pour les transactions en ligne lorsque l'utilisateur utilise les instruments numériques du PSP.

Les PSP restent libres de choisir leurs méthodes d'authentification sous réserve du respect des exigences réglementaires applicables.

**AVÉRÉ :**

> L'utilisation de l'EUDI Wallet comme méthode d'authentification dans le pilote de l'euro numérique est explicitement prévue par la Banque centrale européenne [S29].

Le raccord suivant est donc officiellement documenté :

```
EUDI Wallet
   ↓
authentification forte
   ↓
PSP
   ↓
paiement en euro numérique
```

Ce raccord est plus solide que les rapprochements hypothétiques étudiés avec d'autres infrastructures : il est directement décrit par la BCE pour le pilote.

---

### Des pilotes européens ont déjà expérimenté identité et paiement

L'utilisation de l'EUDI Wallet dans les paiements a également fait l'objet de Large Scale Pilots européens [S29].

Les projets européens ont notamment testé :

- l'initiation de paiements ;  
- l'authentification forte ;  
- les paiements en ligne ;  
- les paiements en magasin ;  
- la vérification d'âge associée à un paiement.

**AVÉRÉ :**

> Le raccord entre identité numérique européenne et infrastructure de paiement a donc dépassé le stade d'une simple spécification conceptuelle : il a déjà fait l'objet de pilotes européens [S29].

Ces expérimentations ne constituent cependant pas la preuve d'un système généralisé reliant automatiquement toutes les informations d'identité à toutes les transactions.

---

### Une même infrastructure peut présenter différents types d'attestations

L'EUDI Wallet n'est pas limité à une identité civile élémentaire.

Son architecture permet de stocker et présenter différents types d'attestations émises par des sources de confiance.

Cela signifie qu'un même mécanisme technique peut être utilisé pour présenter différents attributs selon le service concerné.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une infrastructure de paiement utilisant l'EUDI Wallet pour une authentification ou une vérification n'a pas nécessairement besoin d'accéder à l'ensemble des données détenues par le wallet : elle peut demander et recevoir uniquement l'attestation ou l'attribut nécessaire au processus concerné.

Cette logique est comparable, sur le plan architectural, à celle étudiée pour les paiements conditionnels : le composant prenant une décision n'a pas nécessairement besoin de disposer de toutes les données sources lorsque le système peut lui présenter une preuve vérifiable.

---

### Le raccord identité → paiement est établi, mais sa portée doit être délimitée

À ce stade, la chaîne suivante peut être considérée comme documentée :

```
attribut ou identité vérifiable
   ↓
EUDI Wallet
   ↓
présentation d'une preuve
   ↓
PSP / banque / acquéreur / commerçant
   ↓
authentification ou vérification nécessaire au processus de paiement
```

Et, dans le cadre du pilote de l'euro numérique :

```
EUDI Wallet
   ↓
authentification forte
   ↓
PSP participant au pilote
   ↓
transaction en euro numérique
```

**AVÉRÉ :**

> Il existe donc un raccord institutionnel et technique explicitement prévu entre l'infrastructure européenne d'identité numérique et les infrastructures de paiement, y compris dans le cadre du pilote de l'euro numérique [S29].

---

### Ce raccord ne signifie pas qu'un profil complet accompagne chaque paiement

L'existence de ce lien ne doit pas conduire à considérer que l'ensemble des données détenues dans l'EUDI Wallet est automatiquement communiqué au PSP ou au commerçant.

La conception du wallet repose au contraire sur des principes de minimisation des données et de divulgation sélective [S29].

Une vérification peut, par exemple, porter uniquement sur le fait qu'une personne satisfait un critère d'âge.

**NON ÉTABLI :**

> Les sources étudiées ne permettent pas d'affirmer que l'ensemble des attributs détenus dans un EUDI Wallet puisse être consulté par une banque, un PSP, un commerçant ou l'Eurosystème lors d'un paiement.

**NON ÉTABLI :**

> Elles ne permettent pas non plus d'établir qu'un historique général des achats soit enregistré dans l'EUDI Wallet à des fins de profilage individuel.

---

### La combinaison avec les paiements conditionnels doit être distinguée de l'authentification

Les sections 4.5 et 4.6 ont établi qu'une donnée externe peut participer à la vérification d'une condition déclenchant un paiement conditionnel.

La présente section établit qu'un wallet d'identité peut fournir une preuve vérifiable dans le parcours d'un paiement.

Ces deux mécanismes sont techniquement compatibles dans leur principe, mais leur combinaison systématique n'est pas démontrée.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une attestation vérifiable fournie par une infrastructure d'identité peut techniquement constituer l'une des informations utilisées par un service externe pour vérifier qu'une condition nécessaire à une opération est satisfaite.

L'exemple de la vérification d'âge montre déjà qu'un attribut individuel peut intervenir dans un processus commercial associé à un paiement.

**NON ÉTABLI :**

> Cela ne démontre pas qu'un attribut environnemental, fiscal, social ou comportemental puisse actuellement être imposé comme condition générale d'utilisation de l'euro numérique.

---

### Le rapprochement avec les autres infrastructures reste à établir

Les chapitres précédents ont maintenant identifié séparément plusieurs mécanismes :

**Chapitre 1**  
données structurées relatives aux transactions et à la facturation

**Chapitre 3**  
produits identifiables et données environnementales structurées

**Chapitre 4.5–4.6**  
systèmes externes et conditions pouvant participer à l'exécution automatisée d'un paiement

**Chapitre 4.7**  
identité ou attribut vérifiable pouvant intervenir directement dans le processus de paiement

L'existence séparée de ces quatre éléments ne démontre toujours pas leur interconnexion globale.

Elle réduit cependant progressivement le nombre de raccords purement hypothétiques.

Le raccord :

> **identité numérique → infrastructure de paiement**

est désormais **AVÉRÉ** [S29].

Le raccord :

> **EUDI Wallet → authentification d'un paiement dans le pilote euro numérique**

est également **AVÉRÉ** [S29].

Le raccord :

> **système externe → condition → exécution automatisée d'un paiement**

a été établi dans les sections précédentes [S27][S28].

En revanche, le raccord :

> **données de facturation / DPP / données environnementales → attribut individuel → condition appliquée à un paiement**

reste **À ÉTABLIR**.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> L'EUDI Wallet est explicitement conçu pour être utilisé dans l'authentification de paiements en ligne et en magasin [S29].

**AVÉRÉ :**

> Des attestations émises notamment par les PSP peuvent établir un lien vérifiable entre un wallet, un payeur et un compte ou instrument de paiement [S29].

**AVÉRÉ :**

> L'architecture permet la présentation sélective de certains attributs personnels, notamment l'âge ou la résidence, sans nécessairement transmettre l'ensemble de l'identité de l'utilisateur [S29].

**AVÉRÉ :**

> Des pilotes européens ont déjà expérimenté des paiements utilisant l'EUDI Wallet, y compris des scénarios associant paiement et vérification d'âge [S29].

**AVÉRÉ :**

> La BCE prévoit explicitement que les PSP participant au pilote de l'euro numérique puissent utiliser l'EUDI Wallet comme méthode d'authentification forte pour les paiements en ligne [S29].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une preuve ou un attribut vérifiable provenant d'une infrastructure d'identité peut techniquement être utilisé dans un processus de vérification entourant une transaction sans que l'ensemble des données sources soit communiqué au système de paiement.

**NON ÉTABLI :**

> Aucun élément étudié ne permet d'établir que l'EUDI Wallet soit actuellement destiné à fournir un profil environnemental, fiscal ou comportemental utilisé pour autoriser ou refuser des paiements en euros numériques.

**À ÉTABLIR :**

> Quels attributs autres que ceux actuellement documentés pour l'authentification pourront être demandés dans les futurs services de paiement utilisant l'EUDI Wallet ?

**À ÉTABLIR :**

> Dans quelles conditions juridiques un commerçant, une banque, un PSP ou un autre service pourra demander la présentation d'un attribut avant l'exécution d'une transaction ?

**À ÉTABLIR :**

> Existe-t-il des infrastructures ou projets européens permettant de relier des attestations détenues dans un wallet d'identité à des données de facturation, de produit ou environnementales ?

---

## 4.8 Limites et garanties prévues

**Statut : AVÉRÉ / PROJET EN COURS / À ÉTABLIR**

Les sections précédentes ont établi que l'architecture envisagée pour l'euro numérique comporte des capacités techniques importantes : traitement structuré des transactions, intervention de plusieurs prestataires, réservation de fonds, paiements conditionnels, utilisation d'informations provenant de systèmes externes et possibilité d'utiliser une infrastructure d'identité numérique dans le processus de paiement [S22][S24][S25][S27][S28][S29].

Ces capacités ne peuvent cependant pas être analysées indépendamment des garanties juridiques et techniques prévues pour limiter leur utilisation.

Il faut notamment distinguer :

- ce qui est explicitement interdit ;  
- ce qui est rendu plus difficile par l'architecture ;  
- ce qui reste possible mais encadré par le droit ;  
- et ce qui dépendrait d'une modification future du cadre juridique.

---

### L'euro numérique ne doit pas être une monnaie programmable

La garantie la plus explicite concerne la programmabilité de la monnaie.

La proposition de règlement exclut que l'euro numérique soit conçu comme une monnaie comportant intrinsèquement des conditions limitant son utilisation à certains biens, services, lieux, personnes ou périodes [S22].

Cette interdiction est également constamment affirmée par la Banque centrale européenne [S23][S27].

**AVÉRÉ :**

> L'Eurosystème ne doit pas pouvoir attribuer à certaines unités d'euros numériques des règles déterminant les biens ou services pour lesquels elles peuvent être dépensées [S22][S23][S27].

Une unité d'euro numérique doit rester fongible avec les autres unités.

Cette garantie interdit donc un scénario dans lequel la monnaie elle-même porterait, par exemple, une règle du type :

« cette unité ne peut pas acheter tel produit ».

---

### Cette interdiction ne supprime pas les paiements conditionnels

Comme établi en 4.5 et 4.6, l'interdiction de la monnaie programmable ne supprime pas la possibilité de construire des services conditionnels autour du paiement [S27][S28].

La différence juridique et technique est fondamentale :

**restriction attachée à la monnaie** → explicitement exclue

**condition attachée à une transaction ou à un service** → prévue dans l'architecture

**AVÉRÉ :**

> La garantie contre la monnaie programmable n'interdit donc pas toute logique automatisée autour de l'exécution d'un paiement [S22][S27].

C'est précisément pour cette raison que la gouvernance de la couche de conditionnalité est importante.

---

### Les conditions sont présentées comme devant être convenues par les parties

Dans le modèle présenté par la BCE, les paiements conditionnels correspondent à des services dans lesquels les conditions sont déterminées ou acceptées par les parties à la transaction [S27].

L'Eurosystème fournit l'infrastructure monétaire nécessaire au règlement et à la réservation des fonds mais n'est pas présenté comme l'acteur définissant les critères commerciaux permettant leur libération.

**AVÉRÉ :**

> Dans le cadre actuellement présenté, l'Eurosystème ne dispose pas d'un pouvoir général lui permettant de définir les biens ou services qu'un utilisateur peut acheter au moyen de l'euro numérique [S22][S27].

Cette garantie est importante.

Elle ne répond cependant pas entièrement à une autre question :

**un critère peut-il devenir obligatoire parce qu'il résulte non de la BCE mais d'une obligation juridique ou réglementaire applicable au PSP, au commerçant ou à l'utilisateur ?**

Cette question relève alors moins de la conception monétaire que du droit applicable à l'acteur exécutant le paiement.

**À ÉTABLIR :**

> Dans quelles conditions une règle extérieure au système monétaire pourrait-elle légalement imposer à un PSP ou à un autre intermédiaire de vérifier un critère avant d'exécuter une transaction ?

---

### Les PSP disposent déjà de capacités de contrôle et de non-exécution

L'existence d'une monnaie non programmable ne signifie pas qu'un prestataire de services de paiement soit techniquement obligé d'exécuter toutes les transactions qui lui sont présentées.

Comme établi en 4.2, les PSP restent soumis à différentes obligations réglementaires concernant notamment :

- la lutte contre le blanchiment et le financement du terrorisme ;  
- les sanctions et embargos ;  
- la prévention de la fraude ;  
- la sécurité ;  
- certaines obligations fiscales [S22][S24].

Dans certaines circonstances prévues par le droit, ces obligations peuvent conduire à empêcher, suspendre ou refuser une opération.

**AVÉRÉ :**

> L'interdiction de la monnaie programmable n'équivaut donc pas à une impossibilité technique ou juridique absolue de bloquer une transaction : des mécanismes de contrôle et de non-exécution existent déjà lorsqu'une base juridique le prévoit [S22][S24].

La question centrale n'est donc pas uniquement :

« le paiement peut-il être bloqué ? »

mais également :

« qui possède le pouvoir de le bloquer, pour quel motif et sur quelle base juridique ? »

---

### Des limites de détention sont prévues

La proposition de règlement prévoit également la possibilité d'appliquer des limites au montant d'euros numériques qu'un utilisateur peut détenir [S22].

Ces limites doivent notamment permettre de préserver la stabilité financière et d'éviter une migration excessive des dépôts bancaires vers la monnaie de banque centrale.

Les PSP participent à l'application de ces limites.

Des mécanismes sont également prévus afin de vérifier qu'un utilisateur possédant plusieurs comptes en euros numériques ne puisse contourner la limite globale applicable [S22].

**AVÉRÉ :**

> L'architecture prévoit donc déjà des règles quantitatives pouvant être vérifiées et appliquées automatiquement au niveau des avoirs en euros numériques [S22].

Ces limites portent sur la **détention** d'euros numériques et non sur la nature des biens ou services achetés.

Elles ne constituent donc pas une restriction de consommation.

---

### L'infrastructure peut vérifier une règle sans connaître tout son contexte

La vérification des limites illustre néanmoins un principe technique déjà rencontré dans les sections précédentes.

Plusieurs composants peuvent coopérer pour déterminer qu'une règle est satisfaite sans que chacun dispose de toutes les informations relatives à l'utilisateur.

Cette logique rejoint celle des paiements conditionnels et de l'identité numérique :

```
donnée ou attribut
   ↓
vérification d'une règle
   ↓
résultat exploitable par un autre composant
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> L'architecture permet donc l'application automatisée de certaines règles sans nécessiter qu'un acteur unique centralise l'ensemble des données utilisées pour les vérifier.

Cette caractéristique constitue à la fois une possibilité technique et, lorsqu'elle repose sur la pseudonymisation ou la divulgation sélective, un mécanisme de protection des données.

---

### La BCE ne doit pas pouvoir identifier directement les utilisateurs à partir des données centrales

La proposition de règlement prévoit que les données communiquées à la BCE et aux banques centrales nationales soient organisées de manière à ne pas leur permettre d'identifier directement les utilisateurs [S22].

L'architecture prévoit notamment des mécanismes de séparation, de pseudonymisation et de protection cryptographique.

Comme établi en 4.3, les PSP conservent cependant la relation avec leurs clients et disposent des informations nécessaires à cette relation ainsi qu'au respect de leurs obligations réglementaires [S22][S25].

**AVÉRÉ :**

> La conception actuelle cherche donc à empêcher que l'infrastructure centrale de l'Eurosystème constitue directement une base nominative complète des paiements individuels [S22][S23].

Cela ne signifie pas qu'aucun acteur de la chaîne ne puisse identifier l'utilisateur.

La protection repose précisément sur une **répartition des informations entre différents acteurs**.

---

### La séparation des données constitue une garantie, mais pas une absence de traitement

La pseudonymisation ne signifie pas que les transactions deviennent inexistantes ou techniquement impossibles à traiter.

Elle signifie que certains composants utilisent des identifiants qui ne permettent pas directement d'identifier la personne concernée.

Les PSP disposent parallèlement de la relation permettant d'identifier leurs propres clients.

**AVÉRÉ :**

> L'architecture repose donc davantage sur une séparation des connaissances et des responsabilités que sur l'absence totale de données [S22][S25].

Cette distinction est importante pour l'analyse des interconnexions.

Un système distribué peut permettre plusieurs traitements sans qu'une base centrale unique contienne l'intégralité des informations.

---

### Le mode hors ligne constitue la protection architecturale la plus forte

Le mode hors ligne étudié en 4.4 constitue une situation différente [S23][S26].

Les détails personnels du paiement sont conçus pour rester sur les appareils du payeur et du bénéficiaire et ne pas être transmis aux PSP ou à l'Eurosystème.

**AVÉRÉ :**

> Dans l'architecture actuellement prévue, le mode hors ligne empêche donc l'infrastructure centrale d'exploiter systématiquement les détails individuels de chaque transaction hors ligne [S23][S26].

Cette protection constitue un obstacle technique beaucoup plus important à un rapprochement centralisé que la simple pseudonymisation d'une transaction en ligne.

Les opérations de chargement et de déchargement restent néanmoins visibles du PSP et soumises aux contrôles réglementaires correspondants.

---

### La minimisation des données est également prévue pour l'identité numérique

L'EUDI Wallet repose notamment sur la divulgation sélective [S29].

Lorsqu'un service doit vérifier un attribut, l'objectif est de ne transmettre que l'information nécessaire.

Par exemple :

« utilisateur âgé de plus de 18 ans : OUI »

peut être suffisant sans transmettre la date de naissance complète.

**AVÉRÉ :**

> L'interconnexion entre identité numérique et paiement n'implique donc pas nécessairement la transmission de l'ensemble du profil d'identité de l'utilisateur [S29].

Cette architecture limite la quantité de données exposées.

Elle confirme néanmoins également qu'une décision peut techniquement reposer sur un attribut personnel sans que le système prenant cette décision connaisse l'intégralité des données ayant permis de produire la preuve.

---

### Les garanties reposent en partie sur le droit et peuvent donc évoluer avec lui

Une distinction fondamentale doit être faite entre une impossibilité technique et une interdiction juridique.

Certaines garanties sont profondément intégrées à l'architecture, notamment la protection du mode hors ligne.

D'autres reposent sur les règles définissant les finalités autorisées, les droits d'accès, les obligations des PSP ou les catégories de traitements autorisés.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Lorsqu'une capacité technique existe mais que son utilisation est interdite ou limitée par le droit, la garantie dépend du maintien du cadre juridique qui encadre cette capacité.

Cela ne signifie pas que ce cadre soit destiné à être modifié.

Cela signifie simplement qu'une interdiction juridique ne doit pas être présentée comme une impossibilité technique.

Cette distinction est essentielle pour l'ensemble de cette enquête.

---

### Les garanties actuelles empêchent plusieurs conclusions excessives

À partir des sources étudiées, il serait incorrect d'affirmer que :

- la BCE pourra décider arbitrairement ce qu'un citoyen peut acheter ;  
- l'euro numérique comportera intrinsèquement un quota carbone ;  
- chaque unité monétaire pourra être limitée à certains produits ;  
- la BCE disposera nécessairement d'un historique nominatif complet des achats ;  
- les données du DPP seront automatiquement transmises avec chaque paiement ;  
- l'EUDI Wallet transmettra automatiquement l'ensemble des attributs personnels lors d'une transaction ;  
- les paiements hors ligne permettront un suivi centralisé identique aux paiements en ligne.

**NON ÉTABLI :**

> Aucun des éléments étudiés ne démontre l'existence actuelle d'un système permettant d'attribuer à une personne un quota environnemental puis de bloquer automatiquement ses achats lorsque ce quota est atteint.

---

### Mais les garanties ne suppriment pas les capacités techniques documentées

Inversement, il serait également incorrect de conclure que l'interdiction de la monnaie programmable rend techniquement impossible toute décision automatisée entourant un paiement.

Les sections précédentes ont établi séparément :

```
transactions structurées et identifiables [S25]
   ↓
réservation des fonds [S27]
   ↓
couche de conditionnalité externe à l'Eurosystème [S27][S28]
   ↓
vérification possible d'événements provenant de systèmes externes [S27][S28]
   ↓
plateformes d'acteurs du marché connectées par API dans les expérimentations [S28]
   ↓
identité et attributs vérifiables pouvant intervenir dans le parcours de paiement [S29]
```

**AVÉRÉ :**

> Les garanties entourant l'euro numérique limitent les usages autorisés de ces capacités mais ne suppriment pas l'existence des composants techniques permettant l'automatisation, la vérification de conditions et l'interaction avec des systèmes externes [S22][S27][S28][S29].

---

### La question centrale se déplace donc vers la gouvernance

Après examen des garanties, la question n'est plus seulement de savoir si l'infrastructure possède techniquement les composants permettant d'automatiser ou de conditionner certaines opérations.

Une partie de ces composants est désormais documentée.

La question devient :

```
qui peut définir la règle ?
   ↓
sur quelle base juridique ?
   ↓
à partir de quelles données ?
   ↓
avec quel consentement ou quelle obligation ?
   ↓
quel acteur vérifie la condition ?
   ↓
quel acteur possède la capacité d'agir sur la transaction ?
```

Cette distinction entre **capacité technique** et **autorité juridique** devra être centrale dans les chapitres consacrés aux interconnexions et aux garanties juridiques.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> La proposition relative à l'euro numérique interdit la monnaie programmable au sens d'unités monétaires comportant intrinsèquement des restrictions relatives aux biens, services, lieux, personnes ou périodes d'utilisation [S22][S27].

**AVÉRÉ :**

> Cette interdiction n'empêche pas les paiements conditionnels, qui reposent sur une logique appliquée à une transaction ou à un service plutôt qu'à la monnaie elle-même [S27][S28].

**AVÉRÉ :**

> Les PSP restent capables et, dans certaines situations, juridiquement tenus d'effectuer des contrôles pouvant conduire à la non-exécution d'une transaction, notamment dans les domaines de la fraude, des sanctions et de la lutte contre le blanchiment [S22][S24].

**AVÉRÉ :**

> Des limites de détention d'euros numériques peuvent être définies et appliquées automatiquement, mais elles concernent le montant détenu et non les catégories de biens pouvant être achetées [S22].

**AVÉRÉ :**

> L'architecture prévoit une séparation entre l'identité connue des PSP et les informations pseudonymisées traitées par l'infrastructure centrale, tandis que le mode hors ligne bénéficie d'une protection plus forte empêchant la remontée centrale des détails personnels de la transaction [S22][S23][S26].

**AVÉRÉ :**

> L'EUDI Wallet repose notamment sur la minimisation des données et la divulgation sélective des attributs nécessaires [S29].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les garanties juridiques encadrant une capacité technique ne doivent pas être confondues avec l'absence de cette capacité technique.

**NON ÉTABLI :**

> Aucun élément étudié ne permet d'établir l'existence d'un mécanisme actuel attribuant un quota environnemental individuel puis utilisant ce quota pour autoriser ou refuser des paiements.

**À ÉTABLIR :**

> Dans quelle mesure les règles encadrant les paiements conditionnels empêchent-elles juridiquement qu'une condition soit imposée autrement que par l'accord volontaire du payeur et du bénéficiaire ?

**À ÉTABLIR :**

> Une réglementation extérieure au cadre de l'euro numérique pourrait-elle légalement imposer à un PSP, à un commerçant ou à un autre intermédiaire de vérifier un attribut ou une condition avant l'exécution d'une transaction ?

**À ÉTABLIR :**

> Quelles garanties juridiques empêchent l'utilisation de données provenant d'autres infrastructures numériques comme critères décisionnels dans un service de paiement ?

**À ÉTABLIR :**

> Quelles garanties relèvent directement de l'architecture technique et lesquelles dépendent principalement du cadre juridique susceptible d'évoluer ?

---

## 4.9 Ce que ce chapitre permet d'établir

L'analyse de l'euro numérique montre qu'il ne s'agit pas uniquement d'un nouveau moyen de paiement reproduisant sous forme numérique le fonctionnement des espèces.

Le projet repose sur une infrastructure structurée faisant intervenir l'Eurosystème, des prestataires de services de paiement, des dispositifs d'acceptation, des services communs et différentes interfaces permettant aux acteurs du marché de développer des services complémentaires [S22][S23][S24].

Les documents techniques et les expérimentations étudiés permettent également d'établir plusieurs capacités importantes concernant les données, l'automatisation des paiements et l'interaction avec des systèmes externes.

Ces capacités doivent cependant être distinguées des usages effectivement autorisés ou actuellement déployés.

---

### Une infrastructure centralisée de règlement est prévue

**AVÉRÉ :**

> L'euro numérique est conçu comme une monnaie de banque centrale dont le règlement repose sur une infrastructure centralisée exploitée par l'Eurosystème et distribuée aux utilisateurs par l'intermédiaire de prestataires de services de paiement [S22][S23][S24].

Cette architecture ne repose pas sur une blockchain ou une infrastructure DLT comme fondement du système [S23].

L'utilisateur conserve principalement une relation avec son PSP, tandis que l'Eurosystème assure les fonctions centrales nécessaires au règlement et au fonctionnement de l'infrastructure.

---

### Les paiements en ligne produisent des données structurées

**AVÉRÉ :**

> Le modèle technique actuellement publié prévoit des données structurées relatives aux utilisateurs, comptes, appareils, prestataires, payeurs, bénéficiaires et transactions [S25].

Les transactions disposent notamment d'identifiants, d'un montant, d'une date et d'une heure, d'un type, d'un environnement et d'un statut.

Certaines informations permettent également de caractériser le contexte commercial.

Le Merchant Category Code permet notamment de catégoriser l'activité du commerçant et fait partie des informations prévues dans certains flux de paiement [S25].

Cela ne signifie pas que l'infrastructure connaît systématiquement le produit précis acheté ou le contenu détaillé du panier.

---

### Les données sont réparties entre plusieurs acteurs

**AVÉRÉ :**

> L'architecture ne prévoit pas qu'un acteur unique dispose nécessairement de l'ensemble des informations relatives à une transaction [S22][S24][S25].

Les PSP connaissent leurs clients conformément à leurs obligations.

L'infrastructure centrale utilise notamment des identifiants pseudonymisés et des mécanismes destinés à empêcher l'Eurosystème d'identifier directement les utilisateurs à partir des informations qu'il reçoit [S22][S23].

La présence d'une donnée quelque part dans la chaîne ne signifie donc pas qu'elle soit accessible à tous les participants.

---

### Le mode hors ligne constitue une architecture distincte

**AVÉRÉ :**

> L'euro numérique est conçu pour permettre également des paiements hors ligne exécutés directement entre les appareils du payeur et du bénéficiaire sans intervention en temps réel de l'infrastructure centrale [S23][S26].

Dans le modèle actuellement présenté, les détails personnels de ces transactions restent sur les appareils et ne sont accessibles ni à l'Eurosystème ni aux PSP.

Cette architecture constitue donc une limitation importante à la possibilité d'effectuer un rapprochement centralisé systématique des paiements hors ligne avec d'autres données.

---

### L'euro numérique ne doit pas être une monnaie programmable

**AVÉRÉ :**

> La proposition de règlement et la Banque centrale européenne excluent explicitement une monnaie dont les unités comporteraient intrinsèquement des restrictions déterminant les biens, services, lieux, bénéficiaires ou périodes pour lesquels elles peuvent être utilisées [S22][S23][S27].

L'euro numérique doit rester fongible.

Cette garantie exclut donc, dans le cadre actuellement proposé, un mécanisme dans lequel certaines unités monétaires seraient directement programmées pour interdire l'achat d'une catégorie de produits.

---

### Les paiements conditionnels sont en revanche explicitement prévus

**AVÉRÉ :**

> L'interdiction de la monnaie programmable n'empêche pas l'existence de paiements conditionnels dont l'exécution dépend de conditions prédéfinies [S27].

L'infrastructure prévoit notamment une fonctionnalité permettant de réserver des fonds puis de les transférer lorsque la condition correspondante est considérée comme satisfaite.

La BCE distingue ainsi :

**programmation de la monnaie** → exclue  
**programmation des conditions entourant une transaction** → prévue

Cette distinction constitue l'un des résultats centraux du chapitre.

---

### La logique conditionnelle peut être située en dehors de l'Eurosystème

**AVÉRÉ :**

> La BCE décrit une séparation entre une couche de règlement fournie par l'Eurosystème et une couche de conditionnalité pouvant être développée par des banques, PSP et autres acteurs du marché [S27][S28].

La couche externe peut vérifier qu'un événement ou une condition est satisfait puis utiliser les fonctions fournies par l'infrastructure pour poursuivre le traitement du paiement.

L'Eurosystème n'a donc pas nécessairement besoin de connaître lui-même l'ensemble des données ayant permis de vérifier cette condition.

---

### Un événement externe peut participer à l'exécution d'un paiement

**AVÉRÉ :**

> Les travaux de la BCE prévoient qu'un monitoring externe puisse déclencher une condition utilisée par un service de paiement conditionnel [S27].

Les exemples étudiés comprennent notamment :

- la confirmation d'une livraison ;  
- l'utilisation effective d'un service ;  
- l'accomplissement d'une étape ;  
- certains événements liés au transport ;  
- des interactions machine-to-machine [S27][S28].

Le principe général suivant est donc établi :

```
système ou événement externe
   ↓
vérification d'une condition
   ↓
service conditionnel
   ↓
action sur la transaction
```

---

### Ce mécanisme a fait l'objet d'expérimentations

**AVÉRÉ :**

> Des acteurs du marché ont connecté leurs propres plateformes par API à un environnement simulant les interfaces de l'euro numérique afin d'expérimenter des services et paiements conditionnels [S28].

Les PSP et autres participants pouvaient développer la logique conditionnelle au-dessus des fonctionnalités fondamentales fournies par l'environnement simulé.

Le pont générique entre **système externe** et **traitement conditionnel d'un paiement** ne relève donc plus uniquement d'une possibilité théorique d'architecture.

Il a fait l'objet d'expérimentations techniques.

---

### Une donnée externe n'a pas nécessairement besoin d'entrer dans l'infrastructure monétaire

**DÉDUCTIBLE TECHNIQUEMENT :**

> Un système externe peut effectuer une vérification à partir de ses propres données puis communiquer uniquement le résultat nécessaire au service conditionnel.

Le fonctionnement peut donc être :

```
données conservées dans un système externe
   ↓
vérification d'une règle
   ↓
résultat de la vérification
   ↓
service conditionnel
   ↓
exécution ou absence d'exécution de la transaction
```

Cette architecture signifie qu'une éventuelle interconnexion ne nécessite pas nécessairement la création d'une base centrale regroupant toutes les informations concernées.

---

### L'identité numérique possède également un raccord explicite avec le paiement

**AVÉRÉ :**

> L'EUDI Wallet est conçu pour pouvoir intervenir dans l'authentification de paiements et présenter des attestations ou attributs vérifiables aux acteurs concernés [S29].

L'architecture permet notamment la divulgation sélective d'un attribut sans transmettre nécessairement l'ensemble de l'identité de l'utilisateur.

La vérification d'âge constitue déjà un exemple documenté d'attribut pouvant intervenir dans un parcours commercial associé à un paiement.

---

### Le raccord entre EUDI Wallet et euro numérique est explicitement prévu

**AVÉRÉ :**

> La BCE prévoit que les PSP participant au pilote de l'euro numérique puissent utiliser l'EUDI Wallet comme méthode d'authentification forte pour les paiements en ligne [S29].

La chaîne suivante est donc directement documentée :

```
identité ou attestation numérique
   ↓
EUDI Wallet
   ↓
PSP
   ↓
authentification
   ↓
paiement en euro numérique
```

Le raccord entre identité numérique européenne et infrastructure de paiement ne constitue donc pas uniquement une possibilité théorique.

---

### Plusieurs capacités auparavant séparées peuvent maintenant être représentées ensemble

Les résultats du chapitre permettent de représenter l'architecture générale suivante :

```
Utilisateur
   ↓
identité / attribut vérifiable
   ↓
PSP ou service de paiement
   ↓
transaction structurée et identifiable
```

parallèlement :

```
système externe
   ↓
donnée ou événement vérifiable
   ↓
couche de conditionnalité
```

puis :

```
réservation des fonds
   ↓
condition satisfaite ou non satisfaite
   ↓
règlement ou absence de règlement
```

**AVÉRÉ :**

> Chacun des principaux composants de cette chaîne est documenté dans l'architecture ou dans les expérimentations étudiées [S22][S24][S25][S27][S28][S29].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Ces composants permettent techniquement de construire des services dans lesquels une information provenant d'un système externe participe à une décision automatisée concernant une transaction déterminée, sans rendre la monnaie elle-même programmable.

---

### Le rapprochement avec les données environnementales reste le maillon manquant

Le chapitre 3 a établi séparément :

- l'existence du Digital Product Passport ;  
- l'identification numérique de produits ;  
- la possibilité d'associer certaines données environnementales structurées à ces produits ;  
- l'existence de méthodes permettant de quantifier certaines empreintes environnementales ;  
- des mécanismes d'interopérabilité, d'API et de registres ;  
- la possibilité technique de rapprocher une transaction d'un produit identifiable lorsque les identifiants et droits d'accès nécessaires existent [S15][S18][S19][S20][S21].

Le chapitre 4 établit maintenant séparément :

- l'existence de transactions de paiement structurées ;  
- la réservation de fonds ;  
- les paiements conditionnels ;  
- une couche de conditionnalité externe ;  
- l'utilisation possible d'informations provenant de systèmes externes ;  
- des API permettant aux plateformes des acteurs du marché d'interagir avec l'environnement de paiement ;  
- et un raccord explicite entre identité numérique et paiement [S25][S27][S28][S29].

La combinaison technique peut donc être représentée ainsi :

```
produit identifiable
   ↓
donnée externe associée au produit
   ↓
système capable de vérifier une règle
   ↓
résultat de la vérification
   ↓
couche de conditionnalité
   ↓
transaction
   ↓
exécution ou absence d'exécution
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Si une donnée environnementale relative à un produit était rendue accessible à un service autorisé et si cette donnée devenait un critère valide d'une condition de paiement, l'architecture étudiée permettrait techniquement d'utiliser le résultat de cette vérification pour agir sur l'exécution d'une transaction sans programmer la monnaie elle-même.

---

### Ce raccord spécifique n'est cependant pas établi

**NON ÉTABLI :**

> Aucun élément étudié dans ce chapitre ne démontre qu'une donnée issue d'un Digital Product Passport, un GTIN, une empreinte carbone, une donnée de facturation électronique ou une empreinte environnementale individuelle soit actuellement utilisée comme condition permettant d'autoriser, refuser ou modifier un paiement en euros numériques.

Il n'est pas davantage établi qu'une administration française ou européenne dispose d'un mécanisme permettant d'appliquer automatiquement un quota environnemental individuel aux achats d'une personne.

La possibilité technique résultant de l'assemblage de plusieurs composants ne doit donc pas être présentée comme un usage existant ou officiellement prévu.

---

### Les garanties actuelles doivent être intégrées à cette conclusion

Plusieurs garanties s'opposent actuellement à une interprétation selon laquelle l'euro numérique constituerait directement un outil général de contrôle des achats :

- interdiction de la monnaie programmable [S22][S27] ;  
- conditions de paiement présentées comme convenues entre les parties [S27] ;  
- pseudonymisation et séparation des informations accessibles à l'Eurosystème [S22][S23] ;  
- minimisation et divulgation sélective dans l'EUDI Wallet [S29] ;  
- confidentialité renforcée des paiements hors ligne [S23][S26].

**AVÉRÉ :**

> Le cadre actuellement proposé ne donne donc pas à l'Eurosystème un pouvoir général lui permettant de déterminer arbitrairement les biens et services qu'un utilisateur est autorisé à acheter.

---

### Ces garanties ne doivent pas être confondues avec une impossibilité technique

Les mêmes sources établissent parallèlement l'existence :

- de contrôles pouvant conduire à la non-exécution de certaines transactions lorsqu'une base juridique le prévoit ;  
- de règles quantitatives appliquées automatiquement aux avoirs ;  
- de paiements conditionnels ;  
- de services externes pouvant vérifier des conditions ;  
- d'API permettant l'interaction avec des plateformes de marché ;  
- d'attributs d'identité vérifiables utilisables dans le parcours de paiement [S22][S24][S27][S28][S29].

**DÉDUCTIBLE TECHNIQUEMENT :**

> L'interdiction actuelle de certains usages ne signifie donc pas nécessairement que l'infrastructure serait techniquement incapable de mettre en œuvre une règle comparable si une base juridique et les droits d'accès correspondants existaient.

La distinction entre **capacité technique** et **autorité juridique** constitue ainsi l'une des conclusions principales de ce chapitre.

---

## Conclusion du Chapitre 4

L'analyse permet d'écarter deux conclusions opposées.

La première serait d'affirmer que l'euro numérique constitue déjà une monnaie programmable permettant à une autorité de contrôler les achats individuels.

**Les sources étudiées ne permettent pas de soutenir cette affirmation.**

La seconde serait d'affirmer que l'architecture rend techniquement impossible l'utilisation de données ou de conditions externes dans l'exécution d'un paiement.

**Les sources étudiées permettent au contraire d'établir que de tels mécanismes existent dans l'architecture envisagée et ont déjà fait l'objet d'expérimentations.**

Le résultat peut donc être formulé ainsi :

**AVÉRÉ :**

> L'euro numérique n'est pas conçu comme une monnaie programmable.

**AVÉRÉ :**

> L'infrastructure est néanmoins conçue pour supporter des paiements conditionnels.

**AVÉRÉ :**

> La logique déterminant une condition peut être développée en dehors de l'Eurosystème par des acteurs du marché.

**AVÉRÉ :**

> Une information ou un événement provenant d'un système externe peut participer à la vérification d'une condition.

**AVÉRÉ :**

> Des plateformes externes ont déjà été connectées par API à un environnement simulant l'euro numérique afin d'expérimenter ces mécanismes.

**AVÉRÉ :**

> L'identité numérique européenne dispose d'un raccord officiel avec les infrastructures de paiement et son utilisation est explicitement prévue dans le pilote de l'euro numérique.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une information provenant d'une infrastructure distincte peut être vérifiée extérieurement puis utilisée sous forme de résultat dans un service conditionnel sans que la donnée source soit nécessairement intégrée à l'infrastructure monétaire.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les composants étudiés permettraient donc techniquement qu'une donnée relative à un produit ou à une autre caractéristique externe soit utilisée comme critère d'une transaction conditionnelle si un acteur autorisé disposait de cette donnée et d'une base permettant de l'utiliser.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre actuellement l'utilisation d'un DPP, d'une donnée carbone, d'une donnée de facturation électronique ou d'un profil environnemental individuel comme critère d'autorisation ou de refus d'un paiement.

**À ÉTABLIR :**

> Existe-t-il des acteurs, projets, standards, infrastructures, appels d'offres ou expérimentations reliant concrètement les systèmes de facturation électronique, de Digital Product Passport, d'identité numérique et de paiement ?

**À ÉTABLIR :**

> Existe-t-il des identifiants, API ou infrastructures intermédiaires permettant de faire circuler ou vérifier une information entre ces différents systèmes ?

**À ÉTABLIR :**

> Des acteurs participant au développement de l'euro numérique interviennent-ils également dans les infrastructures de DPP, de facturation électronique ou de traitement des données environnementales ?

**À ÉTABLIR :**

> Les projets européens actuellement développés prévoient-ils explicitement une interopérabilité entre ces différentes infrastructures, même lorsque leurs finalités initiales restent distinctes ?

Ces questions constituent l'objet du chapitre suivant.