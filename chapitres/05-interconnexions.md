# Chapitre 5 — Interconnexions

> **Navigation :** [← Retour au sommaire](#documentation)

Ce chapitre recherche les interconnexions existantes, prévues ou expérimentées entre les infrastructures étudiées dans les chapitres précédents.

L'existence simultanée de plusieurs infrastructures numériques ne démontre pas leur interconnexion.

L'analyse recherche donc des éléments permettant d'identifier des liens concrets entre ces infrastructures :

- standards et identifiants communs ;  
- API et mécanismes d'interopérabilité ;  
- projets pilotes et expérimentations ;  
- consortiums et acteurs communs ;  
- partenariats ;  
- marchés publics et appels d'offres ;  
- références explicites à d'autres infrastructures dans les documentations techniques.

La présence d'un même acteur dans plusieurs projets est documentée comme telle mais ne constitue pas, à elle seule, la preuve d'un échange de données entre ces infrastructures.

Une interconnexion n'est classée **AVÉRÉE** que lorsqu'une source permet d'établir l'existence effective ou explicitement prévue du lien étudié.

---

## Sommaire

- [5.1 — Cartographie des raccords déjà établis](#51-cartographie-des-raccords-déjà-établis)  
- [5.2 — European Business Wallets : identité, facturation et données de transaction](#52-european-business-wallets--identité-facturation-et-données-de-transaction)  
- [5.3 — Business Wallets, Digital Product Passport et infrastructures européennes](#53-business-wallets-digital-product-passport-et-infrastructures-européennes)  
- [5.4 — Identifiants, standards et API communs](#54-identifiants-standards-et-api-communs)  
- [5.5 — Acteurs, consortiums et expérimentations communes](#55-acteurs-consortiums-et-expérimentations-communes)  
- [5.6 — Chaînes d'interconnexion documentées](#56-chaînes-dinterconnexion-documentées)  
- [5.7 — Le raccord environnement → paiement](#57-le-raccord-environnement--paiement)  
- [5.8 — Limites de la démonstration](#58-limites-de-la-démonstration)  
- [5.9 — Ce que ce chapitre permet d'établir](#59-ce-que-ce-chapitre-permet-détablir)

---

## 5.1 Cartographie des raccords déjà établis

**Statut : AVÉRÉ / DÉDUCTIBLE TECHNIQUEMENT / À ÉTABLIR**

Les quatre premiers chapitres ont étudié séparément plusieurs infrastructures numériques relatives aux transactions économiques, aux produits, à l'environnement, à l'identité et aux paiements.

Avant de rechercher de nouvelles interconnexions, il est nécessaire de distinguer les raccords déjà établis de ceux qui restent seulement techniquement possibles ou encore à démontrer.

---

### Facturation électronique → administration fiscale

**AVÉRÉ :**

> La réforme française de la facturation électronique organise la transmission automatisée à l'administration fiscale de données structurées relatives aux factures, aux transactions et, dans certaines situations, aux paiements [S1][S2][S3][S4].

Pour certaines opérations B2B, les données transmises atteignent le niveau des lignes de facture et comprennent notamment la désignation du bien ou du service, la quantité et le prix unitaire hors taxe.

Le premier raccord est donc directement établi :

```
facture / transaction
   ↓
plateforme agréée
   ↓
administration fiscale
```

---

### Données fiscales → analyse économique et pilotage public

**AVÉRÉ :**

> Les objectifs officiels de la réforme comprennent, au-delà de la lutte contre la fraude et du pré-remplissage de la TVA, l'amélioration de la connaissance en temps réel de l'activité économique et le pilotage des politiques publiques [S5][S6][S14].

Les travaux préparatoires mentionnent également l'utilisation des données recueillies afin d'enrichir certains modèles d'analyse.

Le raccord suivant est donc également documenté :

```
données économiques structurées
 ↓  
traitements et analyses
 ↓
connaissance de l'activité économique / pilotage public
```

Cela ne permet pas de déduire que toutes les utilisations possibles de ces données seraient autorisées.

---

### Produit → Digital Product Passport

**AVÉRÉ :**

> Le cadre européen du Digital Product Passport permet d'associer un produit, un modèle ou un lot à un ensemble structuré d'informations numériques au moyen d'identifiants uniques [S15][S20].

Ces informations peuvent, selon la catégorie de produit et la réglementation applicable, inclure différentes caractéristiques techniques et environnementales.

Le raccord suivant est donc établi :

```
produit identifiable
   ↓
identifiant unique
   ↓
Digital Product Passport
   ↓
données structurées relatives au produit
```

---

### Produit → données environnementales

**AVÉRÉ :**

> Certaines réglementations européennes permettent ou imposent déjà d'associer à certaines catégories de produits des informations environnementales quantitatives, notamment relatives à leur empreinte carbone [S15][S18][S19].

Le règlement relatif aux batteries constitue un exemple concret de cette association.

Le raccord :

```
produit identifiable
   ↓
donnée environnementale quantitative
```

est donc établi pour les catégories de produits auxquelles les obligations correspondantes s'appliquent.

Il ne doit pas être généralisé à l'ensemble des produits commercialisés.

---

### DPP → registre, API et systèmes externes

**AVÉRÉ :**

> L'architecture du Digital Product Passport prévoit un registre européen, des identifiants structurés, des mécanismes d'interopérabilité et des interfaces permettant l'échange automatisé de données [S15][S20].

Le registre DPP est désormais opérationnel et la Commission indique qu'il repose notamment sur des API documentées et un référentiel sémantique destiné à faciliter l'interopérabilité entre systèmes.

L'architecture ne constitue donc pas uniquement un ensemble de fiches numériques destinées à être consultées manuellement.

Elle est conçue pour permettre des échanges structurés entre systèmes informatiques.

---

### Transactions commerciales → DPP / traçabilité

**AVÉRÉ :**

> Des projets européens ont déjà rapproché des preuves de transactions commerciales, des acteurs administratifs chargés notamment de la TVA et des douanes et des mécanismes de traçabilité destinés à utiliser le Digital Product Passport [S21].

Le projet e-Origin permet notamment de stocker et partager des preuves de transactions commerciales et de les faire reconnaître par les autorités douanières.

Son évolution dans le cadre du projet EBSI-ELSA prévoit le développement de capacités de traçabilité utilisant le Digital Product Passport.

Cela établit l'existence d'un rapprochement institutionnel entre plusieurs domaines auparavant étudiés séparément :

```
transaction commerciale
   ↓
preuve numérique de transaction
   ↓
infrastructure de traçabilité
   ↓
acteurs administratifs / douaniers
```

parallèlement :

> développement de capacités de traçabilité utilisant le DPP

**NON ÉTABLI :**

> Ce projet ne démontre pas que les données du DPP sont transmises à l'administration fiscale française avec les données de facturation électronique.

---

### Système externe → condition de paiement

**AVÉRÉ :**

> L'architecture envisagée pour l'euro numérique prévoit une couche de conditionnalité développée par des acteurs du marché et capable d'utiliser la vérification d'un événement provenant d'un système externe [S27][S28].

La BCE indique explicitement que cette architecture permet un monitoring externe susceptible de déclencher les conditions utilisées dans un paiement conditionnel.

Le raccord générique suivant est donc établi :

```
système externe
   ↓
information ou événement
   ↓
vérification d'une condition
   ↓
couche de conditionnalité
   ↓
traitement de la transaction
```

---

### Plateforme externe → environnement euro numérique

**AVÉRÉ :**

> Des acteurs du marché ont connecté leurs propres plateformes au moyen d'API à un environnement simulant les interfaces de l'euro numérique afin d'expérimenter des paiements conditionnels [S28].

Les scénarios étudiés comprennent notamment les paiements à la livraison, à l'usage ou par étapes ainsi que certaines interactions machine-to-machine.

Le raccord entre une plateforme extérieure et la logique conditionnelle entourant un paiement ne constitue donc plus uniquement une possibilité théorique.

Il a déjà fait l'objet d'expérimentations techniques.

---

### Identité numérique → paiement

**AVÉRÉ :**

> L'European Digital Identity Wallet peut intervenir dans l'authentification de paiements et permettre la présentation d'attestations ou d'attributs vérifiables [S29].

Le wallet permet notamment de présenter sélectivement certains attributs sans communiquer nécessairement l'intégralité de l'identité de l'utilisateur.

Le raccord suivant est donc établi :

```
identité / attribut vérifiable
   ↓
EUDI Wallet
   ↓
banque / PSP / acquéreur / commerçant
   ↓
processus de paiement
```

---

### EUDI Wallet → euro numérique

**AVÉRÉ :**

> La Banque centrale européenne prévoit que les prestataires participant au pilote de l'euro numérique puissent utiliser l'EUDI Wallet comme méthode d'authentification forte pour certaines transactions en ligne [S29].

La chaîne suivante est donc explicitement prévue :

```
EUDI Wallet
   ↓
authentification forte
   ↓
PSP
   ↓
paiement en euro numérique
```

---

### Transaction → produit → donnée environnementale

Les chapitres précédents ont également identifié un raccord techniquement possible mais qui nécessite certaines conditions.

Une facture ou une transaction peut contenir un identifiant permettant de déterminer le produit concerné.

Le Digital Product Passport peut également utiliser un identifiant de produit tel qu'un GTIN ou un identifiant équivalent [S15][S17].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Lorsqu'un identifiant commun ou un mécanisme de correspondance existe et que les droits d'accès nécessaires sont réunis, une transaction commerciale peut techniquement être rapprochée des données environnementales associées au produit correspondant.

La chaîne devient alors :

```
transaction
   ↓
produit identifiable
   ↓
identifiant ou mécanisme de correspondance
   ↓
DPP ou autre source environnementale
   ↓
donnée environnementale
```

**NON ÉTABLI :**

> Les sources étudiées ne démontrent pas que l'administration fiscale française réalise actuellement ce rapprochement.

---

### Donnée externe → décision automatisée concernant un paiement

Les travaux relatifs aux paiements conditionnels permettent également d'établir qu'un système externe n'a pas nécessairement besoin de transférer toutes ses données au système de paiement.

Il peut vérifier lui-même une condition puis communiquer uniquement le résultat nécessaire au service conditionnel.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une information provenant d'une infrastructure extérieure peut donc participer à une décision automatisée concernant une transaction sans que la donnée source soit nécessairement intégrée à l'infrastructure monétaire.

Ce principe est important pour la recherche des interconnexions.

L'absence d'une base de données centrale réunissant toutes les informations ne suffit pas à démontrer l'absence d'un raccord entre plusieurs infrastructures.

---

### État de la chaîne après les quatre premiers chapitres

Les raccords établis peuvent désormais être représentés de manière simplifiée :

```
**Facturation électronique**
   ↓
données économiques structurées
   ↓
administration fiscale / analyse économique

**Produit identifiable**
   ↓
Digital Product Passport
   ↓
données structurées / données environnementales

**Identité numérique**
   ↓
EUDI Wallet
   ↓
authentification de paiement

**Système externe**
   ↓
vérification d'une condition
   ↓
service de paiement conditionnel

**Plateforme d'un acteur du marché**
   ↓
API
   ↓
environnement expérimental de l'euro numérique
```

Ces raccords ne forment pas encore, à eux seuls, une chaîne unique.

---

### Les raccords restant à rechercher

Après les quatre premiers chapitres, plusieurs questions deviennent donc beaucoup plus précises.

**À ÉTABLIR :**

> Existe-t-il une infrastructure explicitement destinée à relier les données de facturation ou de transaction aux autres infrastructures numériques européennes étudiées ?

**À ÉTABLIR :**

> Existe-t-il un raccord documenté entre le Digital Product Passport et une infrastructure d'identité ou de portefeuille numérique utilisée par les entreprises ?

**À ÉTABLIR :**

> Les infrastructures de facturation électronique et de DPP sont-elles explicitement envisagées comme les composants d'un même écosystème interopérable ?

**À ÉTABLIR :**

> Des identifiants, attestations, API ou services intermédiaires permettent-ils de transporter ou de vérifier une information entre ces différents systèmes ?

**À ÉTABLIR :**

> Des acteurs ou consortiums interviennent-ils simultanément dans le développement des infrastructures de produit, de facturation, d'identité et de paiement ?

**À ÉTABLIR :**

> Existe-t-il un raccord concret permettant à une donnée environnementale relative à un produit d'atteindre directement ou indirectement la couche de conditionnalité d'un service de paiement ?

---

### Conclusion intermédiaire

**AVÉRÉ :**

> Plusieurs raccords entre les infrastructures étudiées sont déjà explicitement documentés : facturation vers administration fiscale, produit vers DPP, DPP vers systèmes interopérables, identité numérique vers paiement, EUDI Wallet vers pilote de l'euro numérique et système externe vers paiement conditionnel.

**AVÉRÉ :**

> Des plateformes externes ont déjà interagi par API avec un environnement simulant l'euro numérique afin d'expérimenter des services conditionnels.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Lorsqu'un identifiant ou mécanisme de correspondance existe, une transaction comportant un produit identifiable peut techniquement être rapprochée des informations environnementales correspondantes.

**NON ÉTABLI :**

> Aucun élément étudié jusqu'ici ne démontre une chaîne opérationnelle reliant directement les données françaises de facturation électronique, le Digital Product Passport ou une donnée environnementale à la décision d'autoriser ou de refuser un paiement.

Le chapitre doit maintenant rechercher les infrastructures intermédiaires susceptibles de relier ces différents ensembles.

La première d'entre elles apparaît dans les travaux récents de la Commission européenne : **l'European Business Wallet**.

---

## 5.2 European Business Wallets : identité, facturation et données de transaction

**Statut : AVÉRÉ / PROJET EN COURS / À ÉTABLIR**

La Commission européenne a proposé en novembre 2025 la création des **European Business Wallets**, une infrastructure numérique destinée aux opérateurs économiques et aux organismes publics [S30].

Contrairement à l'EUDI Wallet étudié dans le chapitre 4, principalement orienté vers l'identité numérique des personnes physiques, le Business Wallet est conçu pour permettre aux entreprises et autres opérateurs économiques d'interagir numériquement avec d'autres entreprises et avec les administrations publiques.

Il constitue donc une nouvelle infrastructure intermédiaire entre plusieurs domaines étudiés séparément dans les chapitres précédents.

---

### Une infrastructure d'identification et d'échange de données pour les entreprises

**AVÉRÉ :**

> Les European Business Wallets doivent permettre aux opérateurs économiques de s'identifier, de s'authentifier et d'échanger de manière sécurisée des données, documents et attestations électroniques vérifiables avec d'autres acteurs économiques et avec les administrations publiques [S30].

Le dispositif ne constitue donc pas uniquement un portefeuille destiné à conserver des documents.

Il doit également fournir une couche d'échange numérique interopérable entre organisations.

La chaîne générale peut être représentée ainsi :

```
entreprise
   ↓
European Business Wallet
   ↓
identification / authentification / attestations vérifiables
   ↓
entreprise ou administration destinataire
```

---

### Business Wallet → EUDI Wallet

Le Business Wallet est construit à partir du cadre européen d'identité numérique.

La proposition prévoit notamment que les European Digital Identity Wallets et les attestations électroniques d'attributs puissent être utilisés pour l'onboarding et la gestion des accès aux European Business Wallets [S30].

**AVÉRÉ :**

> Un raccord explicite est donc prévu entre l'infrastructure EUDI étudiée dans le chapitre 4 et les European Business Wallets [S30].

La chaîne devient :

```
EUDI Wallet / attestation électronique
   ↓
authentification et gestion des accès
   ↓
European Business Wallet
```

Cette relation est particulièrement importante puisque le chapitre 4 a déjà établi séparément un raccord entre l'EUDI Wallet et les infrastructures de paiement.

Elle ne démontre cependant pas qu'une donnée contenue dans un Business Wallet soit automatiquement transmise à un système de paiement.

---

### Des identifiants fiscaux et économiques peuvent être utilisés comme attributs

La proposition mentionne plusieurs attributs pouvant être émis ou vérifiés au moyen des Business Wallets [S30].

Parmi les exemples figurent notamment :

- le numéro d'identification TVA ;  
- le numéro fiscal ;  
- le Legal Entity Identifier (LEI) ;  
- le numéro EORI utilisé dans le domaine douanier ;  
- le numéro d'accise.

**AVÉRÉ :**

> Le Business Wallet est donc explicitement conçu pour manipuler des attributs permettant d'identifier juridiquement, fiscalement ou économiquement une entreprise [S30].

Cela crée une infrastructure capable de faire circuler des preuves vérifiables concernant une même entité entre plusieurs contextes administratifs et économiques.

---

### Business Wallet → ViDA → facturation électronique

La proposition établit un raccord particulièrement important avec **VAT in the Digital Age (ViDA)** [S30].

ViDA modernise le système européen de TVA et prévoit notamment le développement de la facturation électronique et du reporting numérique.

La Commission indique que les European Business Wallets pourront permettre le stockage sécurisé et l'échange vérifiable d'attestations relatives à la TVA et de **données de transaction**, afin de soutenir le reporting en temps réel et la facturation de confiance [S30].

**AVÉRÉ :**

> La Commission prévoit donc explicitement une articulation entre European Business Wallets, données de transaction, TVA, reporting numérique et facturation électronique [S30].

La chaîne suivante n'est plus uniquement déductible :

```
entreprise
   ↓
European Business Wallet
   ↓
attestations TVA / données de transaction
   ↓
ViDA
   ↓
reporting numérique / facturation électronique
```

Il s'agit d'un raccord institutionnel explicitement décrit dans la proposition de la Commission.

---

### Le Business Wallet n'est pas limité aux relations avec l'administration

L'infrastructure doit pouvoir être utilisée dans les relations entre entreprises mais également dans les interactions entre entreprises et administrations [S30].

**AVÉRÉ :**

> Le même environnement de confiance est donc conçu pour permettre des échanges B2B et B2G.

Cette caractéristique est importante pour l'étude des interconnexions.

Une attestation ou une donnée vérifiable peut être utilisée dans plusieurs relations économiques sans nécessiter la création d'une infrastructure différente pour chaque administration ou partenaire commercial.

Cela ne signifie cependant pas qu'une donnée communiquée dans un contexte devienne automatiquement accessible dans tous les autres.

Les droits d'accès et les finalités restent déterminants.

---

### Le Business Wallet constitue une couche intermédiaire

Les infrastructures étudiées jusqu'ici pouvaient sembler appartenir à des domaines séparés :

- identité  
- fiscalité  
- facturation  
- douanes  
- produits  
- administrations  
- transactions commerciales

La proposition Business Wallet adopte précisément une logique transversale.

Elle fournit une infrastructure commune d'identification, d'attestations et d'échange sécurisé permettant à différents systèmes de communiquer avec un même opérateur économique [S30].

**AVÉRÉ :**

> L'Union européenne développe donc explicitement une infrastructure destinée à faciliter l'interopérabilité entre plusieurs systèmes administratifs et économiques auparavant distincts [S30].

---

### Un raccord important avec notre cartographie précédente

Après le chapitre 4, la chaîne suivante était déjà documentée :

```
EUDI Wallet
   ↓
authentification
   ↓
infrastructures de paiement
```

Le Business Wallet ajoute désormais une autre branche officiellement prévue :

```
EUDI Wallet / identité européenne
   ↓
European Business Wallet
   ↓
identité de l'entreprise / attributs vérifiables
   ↓
TVA / données de transaction / facturation / reporting
```

**AVÉRÉ :**

> L'infrastructure européenne d'identité constitue donc désormais un point commun documenté entre, d'une part, les mécanismes d'identification des opérateurs économiques et de facturation et, d'autre part, les infrastructures de paiement étudiées dans le chapitre précédent.

Cette constatation ne suffit pas à démontrer un échange direct de données entre facturation et paiement.

Elle établit cependant que ces domaines ne reposent plus nécessairement sur des infrastructures totalement indépendantes.

---

### Une interconnexion ne nécessite pas nécessairement une base centrale commune

Le fonctionnement envisagé repose sur des attestations, identifiants et échanges vérifiables entre acteurs.

Une entreprise peut donc prouver une information à un autre système sans qu'une base centrale unique regroupe nécessairement toutes les informations concernées.

Ce principe rejoint plusieurs architectures étudiées précédemment :

```
information détenue par un système
   ↓
attestation ou preuve vérifiable
   ↓
présentation à un autre système
   ↓
vérification  
   ↓
utilisation du résultat
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> L'interopérabilité entre plusieurs infrastructures peut donc reposer sur l'échange d'attestations et de preuves vérifiables plutôt que sur la centralisation de toutes les données dans une base commune.

---

### Ce que ce raccord ne démontre pas

L'existence des European Business Wallets ne permet pas d'affirmer que :

- les données françaises de facturation électronique seront automatiquement copiées dans un Business Wallet ;  
- toutes les données de transaction seront accessibles à toutes les administrations ;  
- les informations détenues dans un Business Wallet seront automatiquement transmises à une banque ou à l'Eurosystème ;  
- une donnée environnementale sera utilisée comme condition de paiement ;  
- l'EUDI Wallet permettra à lui seul de relier nominativement toutes les transactions économiques d'une entreprise ou d'une personne.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre à ce stade une transmission automatique des données de facturation ou de transaction contenues ou vérifiées par un Business Wallet vers la couche de conditionnalité d'un paiement en euro numérique.

---

### Mais la séparation institutionnelle entre plusieurs infrastructures se réduit

Le résultat de cette section est néanmoins important.

Avant l'étude des European Business Wallets, les infrastructures relatives à l'identité, à la facturation, aux données fiscales et aux paiements pouvaient encore être représentées comme plusieurs systèmes disposant essentiellement de raccords séparés.

La proposition de la Commission introduit une infrastructure transversale destinée précisément à permettre l'identification des opérateurs et l'échange sécurisé de données et d'attestations entre plusieurs de ces environnements.

**AVÉRÉ :**

> European Business Wallet ↔ EUDI Wallet [S30]

**AVÉRÉ :**

> European Business Wallet ↔ identité et attributs fiscaux de l'entreprise [S30]

**AVÉRÉ :**

> European Business Wallet ↔ ViDA [S30]

**AVÉRÉ :**

> European Business Wallet ↔ attestations TVA [S30]

**AVÉRÉ :**

> European Business Wallet ↔ données de transaction [S30]

**AVÉRÉ :**

> European Business Wallet ↔ reporting numérique / facturation de confiance [S30]

Ces raccords sont explicitement décrits dans les documents de la Commission.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> Les European Business Wallets sont conçus comme une infrastructure transversale permettant aux entreprises et administrations de s'identifier, s'authentifier et échanger des données et attestations vérifiables [S30].

**AVÉRÉ :**

> Leur architecture est explicitement articulée avec le cadre EUDI et permet l'utilisation d'attributs fiscaux et économiques vérifiables [S30].

**AVÉRÉ :**

> La Commission prévoit explicitement leur articulation avec ViDA ainsi que le stockage et l'échange vérifiable d'attestations TVA et de données de transaction afin de soutenir le reporting en temps réel et la facturation de confiance [S30].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Cette infrastructure fournit donc un mécanisme intermédiaire permettant à plusieurs systèmes économiques et administratifs de vérifier et réutiliser certaines informations relatives à une même entreprise sans nécessiter une base de données centrale commune.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre encore qu'une donnée issue de cette infrastructure soit utilisée pour conditionner un paiement en euro numérique.

Un autre raccord doit maintenant être examiné.

La Commission associe également explicitement les European Business Wallets au **Digital Product Passport**.

---

## 5.3 Business Wallets, Digital Product Passport et infrastructures européennes

**Statut : AVÉRÉ / PROJET EN COURS / DÉDUCTIBLE TECHNIQUEMENT / À ÉTABLIR**

L'analyse des European Business Wallets fait apparaître un raccord supplémentaire avec le Digital Product Passport étudié dans le chapitre 3.

Ce rapprochement ne résulte pas uniquement de la compatibilité technique des deux infrastructures.

La proposition relative aux European Business Wallets mentionne explicitement le Digital Product Passport parmi les dispositifs avec lesquels des synergies sont recherchées [S30].

La stratégie européenne pour le marché unique va plus loin en présentant le Digital Product Passport, l'eInvoicing, le futur European Business Wallet et plusieurs autres infrastructures comme les composants d'un même écosystème cohérent de solutions numériques destiné à créer des synergies [S31].

---

### Business Wallet → Digital Product Passport

La proposition de règlement relative aux European Business Wallets décrit explicitement leur articulation avec le Digital Product Passport [S30].

La Commission rappelle que le DPP dépend d'un accès fiable aux données relatives notamment à la conformité et à la durabilité des produits.

Elle indique que les Business Wallets peuvent notamment :

- prouver l'identité juridique d'un opérateur économique ;  
- prouver les droits d'accès qui lui ont été accordés ;  
- permettre la signature et le scellement de déclarations de conformité ;  
- permettre l'échange sécurisé et vérifiable de données relatives aux produits entre différents acteurs et États membres [S30].

**AVÉRÉ :**

> La Commission prévoit explicitement une articulation entre European Business Wallets et Digital Product Passport afin de permettre l'identification des opérateurs, la vérification des droits d'accès et l'échange sécurisé et vérifiable de données relatives aux produits [S30].

La chaîne suivante est donc documentée :

```
opérateur économique
   ↓
European Business Wallet
   ↓
identité juridique / droits d'accès
   ↓
Digital Product Passport
   ↓
données de conformité / durabilité / produit
```

---

### Le raccord concerne notamment les données de durabilité

Ce point est particulièrement important pour l'objet de cette enquête.

Le rapprochement entre Business Wallet et DPP n'est pas présenté uniquement comme un mécanisme permettant d'identifier une entreprise.

La Commission mentionne explicitement l'accès aux données de **conformité et de durabilité** associées au Digital Product Passport [S30].

**AVÉRÉ :**

> L'infrastructure Business Wallet est donc explicitement envisagée comme un mécanisme pouvant contribuer à l'accès sécurisé et vérifiable aux données de durabilité associées aux produits dans l'écosystème DPP [S30].

Cela ne signifie pas que toutes les données environnementales d'un produit soient automatiquement transférées dans le Business Wallet.

Le wallet peut notamment intervenir comme infrastructure permettant de prouver l'identité, les droits d'accès et l'authenticité des échanges.

---

### Business Wallet → DPP et Business Wallet → ViDA

La section précédente a établi séparément :

```
European Business Wallet
   ↓
ViDA
   ↓
attestations TVA / données de transaction / reporting / facturation
```

La présente section établit maintenant :

```
European Business Wallet
   ↓
Digital Product Passport
   ↓
données produit / conformité / durabilité
```

**AVÉRÉ :**

> Une même infrastructure européenne est donc explicitement articulée, d'une part, avec des données de transaction et de facturation et, d'autre part, avec le Digital Product Passport et ses données relatives aux produits [S30].

Ce constat constitue un rapprochement institutionnel entre deux ensembles étudiés séparément dans les chapitres précédents.

Il ne démontre pas encore qu'une donnée précise issue d'une facture soit automatiquement rapprochée d'une donnée précise issue d'un DPP.

---

### La Commission présente ces infrastructures comme un même écosystème numérique

La stratégie pour le marché unique adoptée en mai 2025 permet de dépasser la simple observation selon laquelle plusieurs projets européens évolueraient parallèlement [S31].

La Commission regroupe notamment :

- le Single Digital Gateway ;  
- le Once-Only Technical System ;  
- le Digital Product Passport ;  
- l'eInvoicing ;  
- le futur European Business Wallet ;  
- le Business Register Interconnection System ;  
- l'identifiant européen unique des entreprises ;  
- ainsi que d'autres initiatives destinées à simplifier l'échange de données et le reporting numérique [S31].

Elle indique que ces outils doivent collectivement constituer un **écosystème cohérent de solutions numériques** et créer des synergies facilitant les activités économiques dans l'Union européenne [S31].

**AVÉRÉ :**

> La Commission européenne ne présente donc pas le DPP, l'eInvoicing et le Business Wallet comme des infrastructures nécessairement isolées : elle les inscrit explicitement dans un même écosystème numérique destiné à créer des synergies [S31].

Ce point modifie la qualification de l'analyse.

L'existence d'une convergence entre ces infrastructures ne relève plus uniquement d'une déduction fondée sur leur compatibilité technique.

**AVÉRÉ :**

> Une stratégie institutionnelle d'interopérabilité et de création de synergies entre plusieurs de ces infrastructures est explicitement documentée [S31].

---

### eInvoicing → réutilisation des données

La stratégie identifie également un obstacle à l'automatisation complète des processus économiques : la faible réutilisation des données issues de la facturation électronique dans d'autres processus [S31].

La Commission cherche donc explicitement à augmenter cette réutilisation.

Sa documentation relative à l'eInvoicing indique que la facturation électronique doit permettre l'automatisation d'un ensemble plus large de processus comprenant notamment :

- le reporting TVA ;  
- certaines procédures douanières ;  
- le reporting environnemental, social et de gouvernance, ou ESG [S31].

**AVÉRÉ :**

> Les données de facturation électronique ne sont donc pas envisagées uniquement pour produire, transmettre et comptabiliser une facture : leur réutilisation dans d'autres processus numériques fait explicitement partie de la stratégie européenne [S31].

---

### eInvoicing → reporting de durabilité

La Commission prévoit plus précisément de tester la réutilisation des données issues de l'eInvoicing pour le **reporting de durabilité** [S31].

**AVÉRÉ / PROJET PRÉVU :**

> La stratégie européenne prévoit un pilote consacré à la réutilisation des données de facturation électronique pour le reporting de durabilité [S31].

Ce raccord est particulièrement important pour la cartographie étudiée dans cette enquête.

Jusqu'ici, la relation suivante était seulement techniquement déductible :

```
données de transaction
   ↓
produit
   ↓
donnée environnementale
```

La stratégie introduit désormais un raccord institutionnel supplémentaire :

```
données d'eInvoicing
   ↓
réutilisation
   ↓
reporting de durabilité
```

Cela ne signifie pas qu'une empreinte carbone individuelle soit calculée à partir des factures.

Cela établit en revanche que la réutilisation de données de facturation à des fins liées à la durabilité fait explicitement partie des travaux annoncés par la Commission.

---

### eInvoicing → données douanières

La même stratégie prévoit également d'améliorer la transparence douanière en reliant les données d'eInvoicing aux données douanières, en cohérence avec le développement de l'EU Customs Data Hub [S31].

**AVÉRÉ / PROJET PRÉVU :**

> La Commission prévoit explicitement un rapprochement entre données de facturation électronique et données douanières [S31].

La chaîne devient :

```
eInvoicing
   ↓
données structurées de transaction
   ↓
rapprochement avec les données douanières
   ↓
EU Customs Data Hub
```

Ce rapprochement rejoint les éléments du chapitre 3 relatifs aux infrastructures de traçabilité, au DPP et aux systèmes douaniers.

Il ne démontre cependant pas que toutes ces données soient déjà réunies dans un même système.

---

### Plusieurs raccords auparavant hypothétiques deviennent institutionnellement documentés

Après les sections 5.2 et 5.3, la cartographie peut désormais être complétée :

```
EUDI / identité numérique
   ↓
European Business Wallet
```
```
European Business Wallet
   ↓
ViDA / TVA / données de transaction / facturation
```
```
European Business Wallet
   ↓
Digital Product Passport / données produit / conformité / durabilité
```
```
eInvoicing
   ↓
réutilisation prévue pour le reporting de durabilité
```
```
eInvoicing
   ↓
rapprochement prévu avec les données douanières
```
```
DPP + eInvoicing + Business Wallet + autres infrastructures
   ↓
écosystème numérique cohérent et création de synergies
```

**AVÉRÉ :**

> Les documents de la Commission établissent donc désormais des liens institutionnels explicites entre plusieurs infrastructures étudiées séparément dans les chapitres précédents [S30][S31].

---

### Ce que cela change dans l'enquête

Au terme du chapitre 3, le rapprochement entre données de transaction et données environnementales reposait principalement sur une possibilité technique :

```
identifier le produit dans une transaction
   ↓
retrouver son DPP
   ↓
accéder à la donnée environnementale correspondante
```

Les éléments étudiés dans cette section ajoutent désormais trois faits distincts :

**AVÉRÉ :**

> La Commission prévoit une articulation entre Business Wallet et DPP pour l'identité, les droits d'accès et l'échange sécurisé de données produit, notamment de conformité et de durabilité [S30].

**AVÉRÉ :**

> La même infrastructure Business Wallet est articulée avec ViDA, les attestations TVA et les données de transaction [S30].

**AVÉRÉ / PROJET PRÉVU :**

> La Commission prévoit de tester directement la réutilisation des données d'eInvoicing pour le reporting de durabilité [S31].

La proximité entre données de transaction et données de durabilité n'est donc plus seulement le résultat d'un assemblage théorique réalisé dans cette enquête.

**AVÉRÉ :**

> La Commission européenne travaille explicitement sur la réutilisation et l'interopérabilité de ces catégories de données au sein d'un écosystème numérique commun [S30][S31].

---

### Ce que cela ne démontre toujours pas

Ces éléments ne permettent pas d'affirmer que :

- chaque ligne de facture sera automatiquement rapprochée d'un DPP ;  
- chaque produit acheté sera associé à son empreinte carbone dans une base centrale ;  
- une administration calculera une empreinte environnementale individuelle à partir des factures ;  
- les données de durabilité seront transmises aux banques ou à l'Eurosystème ;  
- une donnée environnementale issue d'un DPP sera utilisée comme condition d'un paiement ;  
- le reporting de durabilité envisagé concerne un profil environnemental individuel des consommateurs.

**NON ÉTABLI :**

> Le raccord spécifique entre donnée environnementale d'un produit et couche de conditionnalité d'un paiement reste à démontrer.

---

### Une chaîne institutionnelle apparaît néanmoins

Sans transformer les éléments précédents en preuve d'un usage qui n'est pas documenté, une chaîne institutionnelle plus précise peut désormais être représentée :

```
eInvoicing / données de transaction*
   ↓
réutilisation prévue des données
   ↘ reporting de durabilité
     ↘ **données douanières / EU Customs Data Hub
```

parallèlement :

```
     European Business Wallet
   ↙                         ↘  
ViDA / transaction     DPP / produit / durabilité
```

le tout inscrit par la Commission dans :

**un écosystème cohérent de solutions numériques destiné à créer des synergies**

**AVÉRÉ :**

> L'existence d'une stratégie de rapprochement et de réutilisation des données entre plusieurs de ces infrastructures est désormais explicitement documentée [S30][S31].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une infrastructure capable d'identifier l'opérateur, de vérifier ses droits d'accès et d'échanger des données produit peut servir de couche d'interopérabilité entre des systèmes de transaction et des systèmes contenant des informations de durabilité, lorsque les règles applicables autorisent cet échange.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> Les European Business Wallets sont explicitement articulés avec le Digital Product Passport et peuvent intervenir dans l'identification des opérateurs, la vérification des droits d'accès et l'échange sécurisé et vérifiable de données relatives aux produits, notamment de conformité et de durabilité [S30].

**AVÉRÉ :**

> Les European Business Wallets sont parallèlement articulés avec ViDA, les attestations TVA et les données de transaction [S30].

**AVÉRÉ :**

> La Commission inscrit le DPP, l'eInvoicing, le Business Wallet et plusieurs autres infrastructures dans un même écosystème cohérent de solutions numériques destiné à créer des synergies [S31].

**AVÉRÉ / PROJET PRÉVU :**

> La Commission prévoit de tester la réutilisation des données d'eInvoicing pour le reporting de durabilité [S31].

**AVÉRÉ / PROJET PRÉVU :**

> La Commission prévoit également de rapprocher les données d'eInvoicing des données douanières en lien avec l'EU Customs Data Hub [S31].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Ces mécanismes réduisent la distance technique et institutionnelle entre données décrivant une transaction, données décrivant un produit et données relatives à sa durabilité.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre encore qu'une donnée environnementale provenant d'un DPP soit transmise à une infrastructure de paiement afin d'autoriser ou de refuser une transaction.

La question n'est désormais plus seulement de savoir si ces infrastructures peuvent communiquer.

La Commission documente elle-même leur interopérabilité, leur réutilisation et les synergies recherchées.

Il reste à déterminer **par quels identifiants, standards et API ces rapprochements peuvent concrètement être réalisés**.

---

## 5.4 Identifiants, standards et API communs

**Statut : AVÉRÉ / DÉDUCTIBLE TECHNIQUEMENT / À ÉTABLIR**

Les sections précédentes ont établi que la Commission européenne recherche explicitement des synergies entre plusieurs infrastructures numériques relatives à la facturation, aux entreprises, aux produits et à leur durabilité.

L'existence d'une volonté d'interopérabilité ne suffit cependant pas à démontrer qu'un rapprochement de données peut effectivement être réalisé.

Pour qu'une interconnexion fonctionne, plusieurs conditions techniques doivent généralement être réunies : les systèmes doivent pouvoir identifier les objets ou acteurs concernés, comprendre les données échangées, vérifier les droits d'accès et disposer d'interfaces permettant les échanges automatisés.

Les infrastructures étudiées disposent déjà de plusieurs de ces composants.

---

### eInvoicing → modèle sémantique commun

**AVÉRÉ :**

> Le standard européen EN 16931 définit un modèle sémantique commun permettant aux systèmes émetteurs et récepteurs de comprendre et traiter automatiquement les informations contenues dans une facture électronique [S32].

L'objectif du standard est précisément de réduire les différences entre formats et systèmes nationaux afin de permettre l'interopérabilité.

La chaîne technique générale est donc :

```
système de facturation A
   ↓
données structurées selon un modèle sémantique commun
   ↓
système de facturation B
```

La donnée n'est plus seulement destinée à être lue par une personne.

Elle est structurée afin de pouvoir être interprétée automatiquement par différents systèmes.

---

### EN 16931 évolue vers d'autres usages de données

Les travaux européens de standardisation ne concernent plus uniquement l'échange traditionnel d'une facture entre fournisseur et client.

Le plan européen de standardisation 2026 prévoit de maintenir EN 16931 en cohérence avec ViDA et d'intégrer les besoins résultant de différentes politiques européennes.

Parmi les domaines explicitement mentionnés figurent :

- le reporting fiscal ;  
- le reporting de durabilité ;  
- les douanes ;  
- d'autres processus automatisés.

**AVÉRÉ :**

> L'évolution du standard européen de facturation prend explicitement en compte des besoins provenant du reporting fiscal, du reporting de durabilité et des procédures douanières [S32].

Cette évolution est cohérente avec les projets de réutilisation des données d'eInvoicing identifiés dans la section précédente.

Elle ne signifie pas que toutes les données nécessaires à ces usages soient déjà présentes dans chaque facture.

---

### DPP → identifiant unique et persistant du produit

Le règlement européen relatif à l'écoconception impose qu'un Digital Product Passport soit relié à un **identifiant unique persistant du produit** [S15][S32].

Cet identifiant est associé à un support de données permettant d'accéder au passeport.

**AVÉRÉ :**

> Le DPP repose donc sur un mécanisme permettant à différents systèmes de désigner de manière persistante le même produit, modèle ou lot selon les règles applicables [S15][S32].

La chaîne est :

```
produit
   ↓
identifiant unique persistant
   ↓
Digital Product Passport
```

Ce mécanisme constitue une condition essentielle à tout rapprochement automatisé entre un produit physique et ses informations numériques.

---

### DPP → standards ouverts et données interopérables

Le règlement impose également que les données du Digital Product Passport reposent sur des standards ouverts et soient, selon les cas :

- lisibles par machine ;  
- structurées ;  
- recherchables ;  
- transférables ;
- accessibles au moyen d'un réseau ouvert et interopérable d'échange de données [S15][S32].

**AVÉRÉ :**

> L'interopérabilité du DPP constitue donc une exigence réglementaire de son architecture et non une simple fonctionnalité facultative [S15][S32].

Le système est conçu pour permettre l'utilisation automatisée des données par différents acteurs autorisés.

---

### Le registre DPP dispose d'une API

Le règlement d'exécution (UE) 2026/1778 précise l'architecture du registre européen du Digital Product Passport [S20][S32].

Le registre comprend notamment :

- une interface utilisateur sécurisée ;  
- une API permettant l'enregistrement des Digital Product Passports et la réception d'informations provenant du registre ;  
- une plateforme de vérification ;  
- un mécanisme d'identification et d'autorisation des utilisateurs ;  
- un système générant des identifiants uniques d'enregistrement ;  
- un référentiel sémantique ;  
- un système de journalisation [S20][S32].

**AVÉRÉ :**

> Le registre DPP dispose donc d'une interface machine-to-machine explicitement conçue pour permettre des interactions automatisées avec d'autres systèmes [S20][S32].

La chaîne suivante est directement prévue :

```
système externe autorisé
   ↓
API
   ↓
registre DPP
   ↓
enregistrement / vérification / informations
```

---

### Le référentiel sémantique facilite la compréhension entre systèmes

Le registre DPP comprend également un référentiel sémantique destiné à définir de manière autoritative la signification, la structure, les versions et les exigences d'interopérabilité des données du passeport [S20][S32].

**AVÉRÉ :**

> Le dispositif ne fournit donc pas seulement une interface technique permettant de transmettre des données ; il prévoit également une couche sémantique permettant aux systèmes de comprendre de manière cohérente les informations échangées [S20][S32].

Deux conditions nécessaires à une interconnexion automatisée sont ainsi réunies :

```
interface technique commune
   +
compréhension sémantique commune
```

---

### Le registre associe produit et opérateur économique vérifié

Le règlement d'exécution impose également la vérification des opérateurs économiques et des autres acteurs de la chaîne de valeur intervenant dans le registre [S20][S32].

Lorsqu'un DPP est enregistré, le registre peut notamment associer :

- l'identifiant unique du produit ;  
- l'identité de l'opérateur économique vérifié responsable ;  
- certaines informations nécessaires à l'enregistrement ;  
- un identifiant unique d'enregistrement [S20][S32].

Une preuve électronique d'enregistrement peut également être générée.

**AVÉRÉ :**

> Le registre DPP établit donc une relation vérifiable entre un produit identifiable et un opérateur économique identifiable [S20][S32].

La chaîne devient :

```
opérateur économique vérifié
   ↓
produit identifiable
   ↓
DPP
   ↓
identifiant d'enregistrement / preuve vérifiable
```

---

### Les mécanismes d'identité numérique peuvent participer à la vérification des opérateurs

Le règlement d'exécution prévoit plusieurs mécanismes permettant de vérifier l'identité des opérateurs économiques.

Ils comprennent notamment, selon les situations, des moyens d'identification électronique conformes au cadre eIDAS ainsi que des attestations électroniques d'attributs [S20][S32].

**AVÉRÉ :**

> L'infrastructure DPP et l'infrastructure européenne d'identité numérique partagent donc des mécanismes permettant l'identification ou la vérification des opérateurs économiques [S20][S32].

Il ne s'agit pas encore nécessairement d'un raccord direct avec l'EUDI Wallet dans toutes les situations.

Mais l'utilisation du même cadre européen d'identité et d'attestations facilite l'interopérabilité entre ces environnements.

---

### Business Wallet → attestations vérifiables

Les European Business Wallets reposent également sur des données et attestations électroniques vérifiables [S30][S32].

Ces attestations peuvent représenter différents attributs relatifs à l'entreprise, à ses représentants, à ses rôles ou à ses autorisations.

L'architecture prévoit notamment :

- des formats structurés d'attributs ;  
- des mécanismes de vérification ;  
- la gestion des mandats et délégations ;  
- des contrôles d'accès ;  
- la traçabilité des autorisations ;  
- des preuves cryptographiquement vérifiables [S30][S32].

**AVÉRÉ :**

> Les échanges entre infrastructures ne reposent donc pas uniquement sur la transmission de données brutes mais peuvent également reposer sur la présentation et la vérification d'attestations numériques [S30][S32].

---

### Business Wallet → contrôle d'accès interopérable

La proposition prévoit des mécanismes permettant de déterminer en temps réel si un acteur possède les droits nécessaires pour accéder à une donnée ou exécuter une procédure [S30][S32].

Les autorisations doivent notamment pouvoir être :

- vérifiées ;  
- auditées ;  
- révoquées ;  
- tracées jusqu'à leur émetteur ;  
- utilisées de manière interopérable entre États membres.

**AVÉRÉ :**

> L'interopérabilité recherchée concerne donc également les droits permettant d'accéder aux données et services, et pas uniquement les formats de données [S30][S32].

Ce point est essentiel pour l'analyse des interconnexions.

Un système peut techniquement disposer d'une API permettant d'accéder à une donnée tout en empêchant cet accès lorsque l'acteur ne possède pas l'autorisation correspondante.

---

### Business Wallet → European Digital Directory → API

La proposition relative aux European Business Wallets prévoit également la création d'un **European Digital Directory** [S30][S32].

Ce répertoire doit comporter deux interfaces :

- un portail destiné aux utilisateurs ;  
- une interface lisible par machine exposée au moyen d'une API pour les communications automatisées entre systèmes.

**AVÉRÉ :**

> L'écosystème Business Wallet prévoit donc lui aussi une interface machine-to-machine permettant la découverte et l'interaction automatisée entre acteurs et systèmes [S30][S32].

La structure générale devient :

```
acteur / système
   ↓
European Digital Directory
   ↓
API
   ↓
identification / découverte / interaction avec l'acteur concerné
```

---

### Les mêmes principes techniques apparaissent dans plusieurs infrastructures

Les systèmes étudiés ne reposent pas nécessairement sur les mêmes bases de données ni sur un identifiant universel unique.

Ils utilisent cependant des principes techniques convergents :

| Infrastructure  | Identification                          | Données structurées | Sémantique                  | API / échange automatisé | Autorisation   |
| ----------------| ----------------------------------------|---------------------|-----------------------------| -------------------------| ---------------|
| eInvoicing      | entreprises / références de transaction | oui                 | EN 16931                    | échanges électroniques   | selon systèmes |
| DPP             | produit / opérateur                     | oui                 | référentiel sémantique      | API du registre          | oui            |
| Business Wallet | entreprise / rôles / mandats            | oui                 | attestations / vocabulaires | API / interfaces         | oui            |
| EUDI            | personne / attributs                    | oui                 | attestations vérifiables    | protocoles d'échange     | oui            |
| euro numérique  | utilisateurs / PSP / transactions       | oui                 | modèle de données           | interfaces de paiement   | oui            |

**AVÉRÉ :**

> Plusieurs infrastructures européennes utilisent donc simultanément des identifiants structurés, des modèles de données interprétables automatiquement, des mécanismes d'autorisation et des interfaces destinées aux échanges machine-to-machine [S20][S25][S29][S30][S32].

---

### L'Union européenne recherche explicitement l'interopérabilité entre ces systèmes

Cette convergence technique n'est pas uniquement accidentelle.

La Commission indique plus largement vouloir assurer une interopérabilité transfrontalière entre les solutions numériques publiques telles que :

- l'eInvoicing ;  
- la signature électronique ;  
- les soumissions électroniques ;  
- le Digital Product Passport.

Elle présente parallèlement le European Business Wallet comme un élément central permettant aux entreprises d'interagir numériquement avec les administrations.

**AVÉRÉ :**

> La stratégie européenne recherche explicitement une interopérabilité entre plusieurs catégories de systèmes étudiées dans cette enquête [S30][S31][S32].

---

### Une convergence sémantique est également en cours pour les Business Wallets

Les travaux techniques relatifs aux European Business Wallets comprennent désormais le développement d'un vocabulaire sémantique destiné aux attestations électroniques utilisées dans les différents cas d'usage.

Ces travaux s'appuient notamment sur des standards de credentials vérifiables et sur des formats destinés à permettre l'interopérabilité des attributs.

**AVÉRÉ / TRAVAUX EN COURS :**

> La construction de l'écosystème Business Wallet comprend donc également une couche destinée à harmoniser la signification des données et attributs échangés entre systèmes.

Cette évolution rapproche son fonctionnement du principe déjà observé dans EN 16931 et dans le référentiel sémantique du DPP.

---

### Existe-t-il un identifiant universel reliant automatiquement toutes les infrastructures ?

À ce stade, les sources étudiées ne permettent pas d'établir l'existence d'un identifiant unique universel qui serait présent simultanément dans :

```
facture
   +
DPP
   +
Business Wallet
   +
identité
   +
paiement
```

**NON ÉTABLI :**

> Aucun identifiant universel permettant de joindre automatiquement toutes les infrastructures étudiées n'a été identifié.

Cette absence est importante.

Elle empêche d'affirmer qu'un rapprochement complet serait automatique ou systématique.

---

### Un identifiant universel n'est cependant pas techniquement indispensable

Une interconnexion entre systèmes ne nécessite pas obligatoirement qu'ils utilisent tous exactement le même identifiant.

Des mécanismes de correspondance peuvent relier plusieurs identifiants.

Par exemple :

```
identifiant entreprise dans le système A
   ↓
identité ou attestation vérifiable
   ↓
correspondance avec l'entreprise dans le système B
```
ou :

```
référence de produit dans une transaction
   ↓
mécanisme de correspondance
   ↓
identifiant unique du DPP
   ↓
informations relatives au produit
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Des attestations, référentiels ou services intermédiaires peuvent permettre de résoudre les correspondances entre plusieurs systèmes sans imposer un identifiant universel commun à l'ensemble de l'architecture.

C'est précisément l'une des fonctions que peuvent remplir des infrastructures d'identité, des registres ou des services d'interopérabilité.

---

### Une API commune unique n'est pas davantage nécessaire

La même distinction s'applique aux interfaces.

Il n'est pas nécessaire qu'une seule API relie directement :

> facturation → DPP → Business Wallet → paiement

Une architecture distribuée peut fonctionner sous la forme :

```
système A
   ↓ API
service intermédiaire
   ↓ API
système B
   ↓ résultat vérifiable
système C
```

Cette logique est déjà observée dans les architectures étudiées précédemment.

**DÉDUCTIBLE TECHNIQUEMENT :**

> L'absence d'une API unique reliant directement toutes les infrastructures ne permet donc pas, à elle seule, de conclure à l'absence d'interconnexion.

---

### La question des droits d'accès reste déterminante

La possibilité technique de rapprocher plusieurs données ne signifie pas que ce rapprochement soit juridiquement ou opérationnellement autorisé.

Les architectures DPP, EUDI et Business Wallet comprennent précisément des mécanismes destinés à contrôler les droits d'accès et les informations pouvant être communiquées.

**AVÉRÉ :**

> L'interopérabilité technique et l'autorisation d'accéder aux données constituent deux questions distinctes [S20][S29][S30][S32].

Une chaîne peut donc être techniquement réalisable tout en restant juridiquement interdite ou inaccessible à certains acteurs.

---

### Ce que cette section permet désormais d'établir

Après les sections précédentes, il était établi que la Commission recherchait des synergies entre plusieurs infrastructures.

Cette section montre que les principaux composants techniques permettant de réaliser de telles synergies existent également :

```
**identifiants**
   ↓
désigner les acteurs, produits et transactions

**modèles sémantiques**  
   ↓
comprendre automatiquement les données

**attestations vérifiables**
   ↓
prouver une information sans nécessairement transférer toutes les données sources

**mécanismes d'autorisation**
   ↓
déterminer qui peut accéder à quoi

**API et interfaces machine-to-machine**
   ↓
permettre les échanges automatisés

**registres et répertoires**
   ↓
retrouver et vérifier les acteurs, produits ou services
```
**AVÉRÉ :**

> Ces composants existent dans plusieurs des infrastructures étudiées et sont explicitement développés dans une logique d'interopérabilité [S20][S30][S32].

---

### Conclusion intermédiaire

**AVÉRÉ :**

> L'eInvoicing repose sur un modèle sémantique européen commun destiné à permettre le traitement automatisé et interopérable des factures [S32].

**AVÉRÉ :**

> Le DPP repose sur des identifiants uniques persistants, des données structurées et interopérables, une API, un référentiel sémantique et des mécanismes d'identification et d'autorisation [S15][S20][S32].

**AVÉRÉ :**

> Les European Business Wallets reposent sur des attestations vérifiables, des mécanismes d'autorisation interopérables et des interfaces destinées aux communications automatisées entre systèmes [S30][S32].

**AVÉRÉ :**

> Les politiques européennes de standardisation cherchent explicitement à rapprocher l'eInvoicing des besoins liés notamment au reporting fiscal, au reporting de durabilité et aux douanes [S32].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les composants nécessaires à la construction de passerelles automatisées entre plusieurs infrastructures existent donc : identification, résolution de correspondances, sémantique commune, contrôle d'accès, attestations vérifiables et API.

**NON ÉTABLI :**

> Aucun identifiant universel ou API unique reliant automatiquement facturation, DPP, identité et paiement n'est établi par les sources étudiées.

La recherche d'une interconnexion ne peut donc pas se limiter à chercher une base de données, un identifiant ou une API unique.

Une architecture distribuée peut relier plusieurs systèmes au moyen de services intermédiaires, d'attestations, de correspondances d'identifiants et d'interfaces successives.

La prochaine étape consiste donc à rechercher si **les mêmes acteurs, consortiums et projets pilotes interviennent effectivement dans plusieurs de ces infrastructures**.

---

## 5.5 Acteurs, consortiums et expérimentations communes

**Statut : AVÉRÉ / INDICE D'INTERCONNEXION / À ÉTABLIR**

L'existence d'acteurs communs à plusieurs infrastructures ne démontre pas, à elle seule, que des données circulent entre ces infrastructures.

Elle constitue cependant un élément pertinent lorsque ces acteurs participent concrètement à la conception, à l'intégration ou à l'expérimentation de plusieurs systèmes étudiés dans cette enquête.

L'analyse des projets européens relatifs à l'euro numérique, à l'identité numérique et aux Business Wallets montre que ces travaux ne sont pas conduits uniquement par des institutions publiques indépendantes les unes des autres.

Ils associent également des banques, prestataires de paiement, entreprises technologiques, opérateurs économiques, fournisseurs de wallets et intégrateurs intervenant dans plusieurs écosystèmes [S33].

---

### Digital Euro Innovation Platform → acteurs privés

En 2025, la Banque centrale européenne a créé une plateforme d'innovation réunissant environ 70 participants du marché afin d'expérimenter des fonctionnalités et cas d'usage relatifs à l'euro numérique [S28][S33].

Les participants comprennent notamment :

- des banques ;  
- des prestataires de services de paiement ;  
- des fintechs ;  
- des entreprises technologiques ;  
- des acteurs du commerce ;  
- des fournisseurs d'infrastructures et de services numériques.

**AVÉRÉ :**

> La conception et l'expérimentation des services pouvant être développés autour de l'euro numérique associent directement des acteurs privés provenant de plusieurs secteurs économiques [S28][S33].

Ces acteurs ne se limitent donc pas à observer le projet.

Dans le cadre du volet « pioneers », ils ont pu connecter leurs propres plateformes à l'environnement simulé fourni par la BCE afin d'expérimenter différentes fonctionnalités [S28].

---

### Plusieurs grands acteurs financiers et technologiques participent à l'expérimentation de l'euro numérique

La liste publiée par la BCE comprend notamment :

- Accenture ;  
- CaixaBank ;  
- equensWorldline ;  
- KPMG ;  
- SAP Fioneer ;  
- Tata Consultancy Services ;  
- Infineon ;  
- plusieurs banques et prestataires européens de paiement [S33].

Un consortium appelé **Digi-Trade** participe également aux deux volets de l'Innovation Platform.

Il réunit :

- Amazon ;  
- CargoX ;  
- Deutsche Bank ;  
- Stripe ;  
- Swift [S33].

**AVÉRÉ :**

> Des acteurs majeurs du commerce électronique, de la banque, du paiement, de la messagerie financière et des infrastructures technologiques participent donc conjointement à l'expérimentation de services reposant sur l'environnement de l'euro numérique [S33].

Cette participation ne démontre pas que leurs infrastructures commerciales existantes seront automatiquement reliées à l'euro numérique.

Elle établit en revanche qu'ils disposent d'un accès direct aux travaux expérimentaux permettant d'évaluer et de développer de futurs services autour de cette infrastructure.

---

### WE BUILD → un consortium transversal

Le Large Scale Pilot **WE BUILD** constitue un autre élément important [S33].

Ce projet européen rassemble plus de 200 organisations issues de plusieurs dizaines de pays.

Il comprend notamment :

- des autorités publiques ;  
- des registres d'entreprises ;  
- des administrations fiscales ;  
- des banques et institutions financières ;  
- des fournisseurs de wallets et services de confiance ;  
- des entreprises technologiques ;  
- des PME ;  
- des organismes de recherche [S33].

**AVÉRÉ :**

> Un même consortium européen réunit donc des acteurs publics, fiscaux, financiers, technologiques et économiques afin de développer et tester des infrastructures interopérables reposant sur l'EUDI Wallet et les European Business Wallets [S33].

---

### WE BUILD ne traite pas uniquement d'identité

La documentation officielle relative aux Large Scale Pilots présente WE BUILD comme un projet consacré à des cas d'usage relatifs aux entreprises **et aux paiements** [S33].

Son architecture répartit les travaux entre plusieurs domaines.

Parmi eux figurent notamment :

**Business**  
identité d'entreprise / représentation / partage de données

**Supply Chain**  
processus relatifs aux chaînes d'approvisionnement et à la facturation électronique

**Payments & Banking**  
paiements sécurisés / services bancaires / onboarding financier [S33]

**AVÉRÉ :**

> Des cas d'usage relatifs à la facturation électronique et des cas d'usage relatifs aux paiements et services bancaires sont donc développés au sein d'un même Large Scale Pilot européen et d'une même architecture générale d'interopérabilité [S33].

Ce constat ne démontre pas qu'une facture soit utilisée comme condition d'un paiement.

Il établit cependant que les deux domaines sont expérimentés au sein du même programme technique.

---

### Business Wallet → supply chain → eInvoicing

Le blueprint d'architecture de WE BUILD mentionne explicitement la facturation électronique parmi les processus couverts dans le domaine Supply Chain [S33].

Le même projet développe parallèlement des mécanismes relatifs :

- à l'identité des entreprises ;  
- aux mandats et représentations ;  
- au partage de données ;  
- aux relations entre acheteurs et fournisseurs ;  
- aux paiements et services bancaires.

**AVÉRÉ :**

> La facturation électronique, l'identité des entreprises, le partage de données et les paiements ne sont donc plus étudiés uniquement dans des programmes européens séparés : ils apparaissent également comme différents cas d'usage d'un même environnement expérimental [S33].

---

### WE BUILD → administrations fiscales

La composition du consortium comprend également des administrations fiscales [S33].

L'administration fiscale finlandaise indique par exemple participer directement à WE BUILD afin d'expérimenter :

- la transmission d'informations fiscales au moyen de wallets ;  
- les déclarations de TVA transfrontalières ;  
- l'émission et la réception de documents fiscaux numériques ;  
- différents processus nécessitant des attestations fiscales.

**AVÉRÉ :**

> Des administrations fiscales participent donc directement à l'expérimentation des Business Wallets et à l'utilisation de données fiscales et d'attestations numériques dans cet environnement [S33].

La chaîne expérimentale comprend ainsi :

```
entreprise
   ↓
Business Wallet
   ↓
donnée / attestation fiscale
   ↓
administration fiscale
```

---

### WE BUILD → paiements

WE BUILD dispose également de travaux spécifiquement consacrés aux paiements.

Le consortium a créé en 2026 une communauté dédiée aux paiements afin de présenter et discuter les solutions techniques expérimentées autour des EUDI Wallets et Business Wallets pour les paiements et les services bancaires [S33].

**AVÉRÉ :**

> Les EUDI Wallets et Business Wallets sont donc effectivement expérimentés dans des cas d'usage relatifs aux paiements et aux services bancaires au sein du consortium [S33].

Les travaux portent notamment sur les exigences réglementaires, les standards, les architectures techniques et les interactions avec les institutions financières et prestataires de paiement.

---

### Certains acteurs apparaissent dans plusieurs environnements

L'analyse des participants permet d'identifier plusieurs recoupements entre les écosystèmes.

**CaixaBank** participe à la Digital Euro Innovation Platform de la BCE [S33].

La banque apparaît également dans les travaux et événements du consortium WE BUILD consacrés aux wallets et aux paiements.

**Worldline**, via equensWorldline, participe à la Digital Euro Innovation Platform [S33].

Le groupe participe également aux Large Scale Pilots relatifs à l'EUDI Wallet, notamment WE BUILD, dans des travaux liés aux paiements.

Ces recoupements peuvent être représentés ainsi :

```
Digital Euro Innovation Platform
   ↕
acteurs bancaires / PSP / intégrateurs
   ↕
EUDI / WE BUILD
   ↕
Business Wallet / paiements / services bancaires
```

**AVÉRÉ :**

> Certains acteurs financiers et technologiques interviennent donc effectivement dans plusieurs initiatives européennes relatives à l'identité numérique, aux wallets et aux paiements [S33].

---

### Un même acteur dans deux projets ne prouve pas un échange de données

Cette distinction est essentielle.

Une entreprise peut participer simultanément à plusieurs projets européens pour des raisons différentes :

- expertise technique ;  
- préparation réglementaire ;  
- développement commercial ;  
- recherche ;  
- standardisation ;  
- expérimentation.

**NON ÉTABLI :**

> La présence d'un acteur dans plusieurs projets ne permet pas d'affirmer que cet acteur transfère des données d'une infrastructure vers une autre.

Par exemple :

```
acteur A participe au projet X
   +
acteur A participe au projet Y
```

ne signifie pas automatiquement :

données du projet X → acteur A → projet Y

Pour établir un tel raccord, il faut identifier un cas d'usage, une interface, un flux, une architecture ou une documentation décrivant effectivement cet échange.

---

### Le cas WE BUILD est plus fort qu'un simple recoupement d'acteurs

WE BUILD présente cependant une différence importante.

Il ne s'agit pas uniquement de constater que les mêmes entreprises participent séparément à plusieurs projets.

Les domaines étudiés sont réunis **dans un même consortium et dans une même architecture d'intégration**.

Le blueprint du projet distingue explicitement :

```
Business
   +
Supply Chain
   +
Payments & Banking [S33]
```

et prévoit une architecture commune destinée à assurer l'interopérabilité entre les différents cas d'usage.

**AVÉRÉ :**

> L'identité d'entreprise, le partage de données, les chaînes d'approvisionnement, la facturation électronique et les paiements sont donc testés comme différents composants d'un même écosystème de wallets interopérables [S33].

Cette constatation constitue un élément d'interconnexion plus fort que la simple présence d'un acteur commun dans plusieurs programmes.

---

### Un projet européen relie désormais explicitement Business Wallet et paiements

Les European Business Wallets étudiés en 5.2 étaient principalement apparus comme une infrastructure d'identité, d'attestations et d'échange de données pour les entreprises.

WE BUILD montre que cette infrastructure est également expérimentée dans des cas d'usage bancaires et de paiement [S33].

La chaîne devient donc :

```
identité de l'entreprise
   ↓
European Business Wallet
   ↓
attestations / données d'entreprise
   ↓
services bancaires / paiements
```

**AVÉRÉ :**

> Le raccord fonctionnel entre Business Wallet et environnement bancaire ou de paiement fait donc déjà l'objet d'expérimentations dans un Large Scale Pilot financé par l'Union européenne [S33].

---

### La facturation et le paiement se trouvent désormais dans le même environnement expérimental

En combinant uniquement les éléments explicitement documentés dans WE BUILD :

```
European Business Wallet
   ↓
identité / représentation / partage de données
```

parallèlement :

```
Supply Chain
   ↓
facturation électronique
```

parallèlement :

```
Payments & Banking
   ↓
paiements / services financiers
```

**AVÉRÉ :**

> La facturation électronique et les paiements apparaissent donc désormais dans le même programme européen d'expérimentation des wallets [S33].

**NON ÉTABLI :**

> Aucun élément étudié ne permet encore d'affirmer qu'une donnée provenant directement d'une facture électronique est utilisée comme critère d'autorisation ou de refus d'un paiement dans WE BUILD.

---

### Des travaux rapprochent encore davantage identité et paiement

Les expérimentations relatives à l'EUDI Wallet ne sont pas uniquement conceptuelles.

Des travaux menés dans les Large Scale Pilots ont déjà porté sur l'authentification de paiements au moyen du wallet.

WE BUILD poursuit désormais cette trajectoire avec des cas d'usage consacrés aux paiements et services bancaires.

**AVÉRÉ :**

> L'identité numérique et les infrastructures de paiement font donc l'objet d'expérimentations conjointes impliquant banques, prestataires de paiement, fournisseurs de wallets et entreprises technologiques [S29][S33].

---

### La cartographie des acteurs devient transversale

Les projets étudiés font apparaître plusieurs catégories d'acteurs présentes à différents niveaux de l'écosystème :

```
**institutions européennes**
Commission européenne / BCE
   ↓
**administrations nationales**
registres / administrations fiscales / autorités publiques
   ↓
**banques et PSP**
   ↓
**fournisseurs de wallets et services de confiance**
   ↓
**intégrateurs et entreprises technologiques**
   ↓
**entreprises et commerçants**
```

**AVÉRÉ :**

> Les infrastructures étudiées sont donc développées dans un environnement institutionnel et industriel commun faisant intervenir simultanément acteurs publics, administrations fiscales, banques, prestataires de paiement et entreprises technologiques [S33].

Cela ne démontre toujours pas une centralisation des données entre tous ces acteurs.

Cela établit cependant l'existence d'un espace commun de conception, de standardisation et d'expérimentation.

---

### Ce que cela change dans l'enquête

Au début du chapitre 5, plusieurs infrastructures étaient encore reliées principalement par leurs caractéristiques techniques.

Les sections précédentes ont progressivement établi :

```
DPP + eInvoicing + Business Wallet
→ même stratégie européenne d'interopérabilité

eInvoicing
→ réutilisation prévue pour le reporting de durabilité

Business Wallet
→ DPP / données produit / durabilité

Business Wallet
→ ViDA / données de transaction

EUDI Wallet
→ paiement

système externe
→ paiement conditionnel

WE BUILD
→ Business + Supply Chain + eInvoicing + Payments & Banking
```

**AVÉRÉ :**

> Plusieurs domaines précédemment étudiés séparément se retrouvent désormais au sein de stratégies, architectures et programmes expérimentaux communs [S30][S31][S32][S33].

---

### Ce que cela ne permet toujours pas d'affirmer

Même avec ces nouveaux éléments, il n'est pas établi que :

- les données françaises de facturation électronique soient transmises aux infrastructures de paiement ;  
- les données d'un DPP soient transmises à une banque ;  
- une empreinte carbone soit utilisée dans une décision de paiement ;  
- une administration fiscale puisse ordonner automatiquement le refus d'un achat sur la base d'une donnée environnementale ;  
- les participants communs aux différents projets organisent un échange de données entre ces infrastructures.

**NON ÉTABLI :**

> Le raccord opérationnel spécifique environnement → condition de paiement reste à démontrer.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> La Digital Euro Innovation Platform associe banques, PSP, entreprises technologiques, fintechs et acteurs commerciaux à l'expérimentation de services pouvant être développés autour de l'euro numérique [S28][S33].

**AVÉRÉ :**

> Certains acteurs financiers et technologiques participent à plusieurs initiatives relatives à l'identité numérique, aux wallets et aux paiements [S33].

**AVÉRÉ :**

> WE BUILD réunit plus de 200 organisations publiques et privées et développe dans un même programme des cas d'usage relatifs aux entreprises, aux chaînes d'approvisionnement et aux paiements [S33].

**AVÉRÉ :**

> La facturation électronique figure dans les cas d'usage Supply Chain tandis que les paiements et services bancaires disposent de leur propre domaine au sein du même projet [S33].

**AVÉRÉ :**

> Des administrations fiscales, banques, institutions financières, fournisseurs de wallets et entreprises technologiques participent au même environnement expérimental [S33].

**AVÉRÉ :**

> Le raccord fonctionnel entre Business Wallet, identité d'entreprise et services bancaires ou de paiement fait l'objet d'expérimentations [S33].

**INDICE D'INTERCONNEXION :**

> La présence de plusieurs infrastructures et catégories d'acteurs dans un même programme réduit encore la séparation institutionnelle et technique entre les domaines étudiés, sans démontrer à elle seule qu'une donnée circule effectivement de l'un à l'autre.

**NON ÉTABLI :**

> Aucun flux opérationnel reliant directement une donnée environnementale issue d'un produit à une condition déterminant l'exécution d'un paiement n'est encore établi.

Les acteurs communs existent.

Les programmes communs existent.

Les architectures d'intégration existent.

Les cas d'usage relatifs à la facturation et aux paiements se trouvent désormais dans le même environnement expérimental.

La prochaine étape consiste donc à ne plus étudier séparément les composants, mais à reconstruire les **chaînes d'interconnexion effectivement documentées de bout en bout**.

---

## 5.6 Chaînes d'interconnexion documentées

**Statut : AVÉRÉ / EXPÉRIMENTÉ / DÉDUCTIBLE TECHNIQUEMENT / À ÉTABLIR**

Les sections précédentes ont identifié séparément des infrastructures interopérables, des identifiants, des API, des wallets, des acteurs communs et des programmes expérimentaux réunissant facturation, identité et paiement.

Il est désormais possible de rechercher non plus seulement des composants compatibles, mais des chaînes dans lesquelles plusieurs de ces composants interviennent effectivement au cours d'une même transaction ou d'un même processus.

Les travaux de WE BUILD permettent d'en documenter plusieurs.

---

### Identité d'entreprise → compte bancaire → paiement → preuve de transaction

Le consortium WE BUILD présente en septembre 2026 une chaîne B2B utilisant l'European Business Wallet comme infrastructure de confiance commune [S34].

Le parcours décrit suit une entreprise depuis son identification jusqu'à la preuve de la transaction.

Il comprend notamment :

```
entreprise
   ↓
identité / KYC / KYB transfrontalier
   ↓
European Business Wallet
   ↓  
ouverture ou identification du compte bancaire
   ↓
attestation vérifiable d'IBAN
   ↓
paiement utilisant l'IBAN vérifié
   ↓
eReceipt
   ↓
preuve de la transaction
```

**AVÉRÉ / EXPÉRIMENTÉ :**

> WE BUILD documente donc une chaîne dans laquelle identité numérique d'entreprise, donnée bancaire vérifiée, paiement et justificatif électronique de transaction interviennent dans un même parcours B2B [S34].

Ce raccord dépasse la simple présence de cas d'usage distincts dans un même consortium.

Les composants sont ici utilisés successivement dans le même processus transactionnel.

---

### EUDI Wallet → authentification du paiement

Le cas PA4 documenté par un participant au consortium apporte un niveau de détail supplémentaire [S34].

Un salarié agit pour le compte d'une entreprise.

Son EUDI Wallet permet de présenter les éléments nécessaires à son authentification et à son autorisation.

Le paiement peut être réalisé depuis un compte ou une carte associés au parcours.

La transaction contient notamment :

- le montant ;  
- la devise ;  
- le bénéficiaire ;  
- le moyen de paiement sélectionné.

L'utilisateur confirme les données de transaction et la banque procède au règlement.

La chaîne expérimentée devient :

```
personne autorisée
   ↓
EUDI Wallet
   ↓
authentification forte
   ↓
données de transaction
   ↓
banque
   ↓
règlement du paiement
```

**EXPÉRIMENTÉ :**

> Le raccord entre identité numérique, autorisation de la personne agissant pour l'entreprise et paiement est donc matérialisé dans un parcours technique de démonstration [S34].

---

### Paiement → émission automatique d'un justificatif vérifiable

Une fois le paiement confirmé, le vendeur émet un eReceipt sous la forme d'un credential vérifiable [S34].

Ce justificatif est envoyé directement vers le European Business Wallet de l'entreprise acheteuse.

La chaîne devient :

```
paiement confirmé
   ↓
vendeur / Business Wallet
   ↓
génération du eReceipt
   ↓
credential vérifiable
   ↓
European Business Wallet de l'acheteur
```

**EXPÉRIMENTÉ :**

> Un événement provenant directement du processus de paiement peut donc déclencher l'émission et le transfert automatisé d'un document transactionnel structuré vers le wallet de l'entreprise [S34].

Le lien paiement → donnée transactionnelle structurée n'est donc plus seulement théorique dans ce cas d'usage.

---

### Le justificatif contient le détail économique de la transaction

Le eReceipt utilisé dans la démonstration ne constitue pas uniquement une preuve indiquant qu'un montant global a été payé.

Selon la documentation technique publiée par le participant au projet, il contient notamment :

- l'identité du vendeur ;  
- son numéro de TVA ;  
- les lignes d'achat ;  
- les montants hors taxe et toutes taxes comprises ;  
- les sous-totaux de TVA par taux ;  
- la référence du paiement [S34].

**EXPÉRIMENTÉ :**

> Le même objet numérique peut donc établir un lien vérifiable entre le paiement et le contenu économique détaillé de la transaction [S34].

La chaîne devient :

```
paiement
   ↓
référence de paiement
   ↓
eReceipt vérifiable
   ↓
lignes d'achat + montants + TVA + vendeur
```

Ce point est important pour l'enquête.

Dans ce cas expérimental, la couche transactionnelle et le détail des biens ou services achetés ne sont plus nécessairement deux ensembles dépourvus de relation technique.

Un justificatif vérifiable peut servir de pont entre eux.

---

### Justificatif → comptabilité

Le Business Wallet peut également être relié aux systèmes utilisés par l'entreprise.

Dans la démonstration PA4, un connecteur transmet les eReceipts vers le système comptable afin de comptabiliser automatiquement les dépenses [S34].

La chaîne devient :

```
paiement
   ↓
eReceipt vérifiable
   ↓
Business Wallet
   ↓
connecteur
   ↓
comptabilité
```

**EXPÉRIMENTÉ :**

> Les données issues de la transaction peuvent donc être réutilisées automatiquement par un système extérieur au wallet sans ressaisie manuelle [S34].

Ce mécanisme confirme le rôle de couche d'interopérabilité attribué aux wallets dans les sections précédentes.

---

### Justificatif → administration fiscale

Le cas expérimental décrit par le participant va encore plus loin.

Les justificatifs vérifiés peuvent être communiqués à un service fiscal de démonstration.

Celui-ci vérifie notamment :

- la signature du justificatif ;  
- la confiance accordée à son émetteur ;  
- son statut de révocation.

Le système peut ensuite utiliser les informations de TVA contenues dans les justificatifs pour effectuer un rapprochement de TVA [S34].

La chaîne expérimentale complète devient :

```
achat B2B
   ↓
paiement
   ↓
eReceipt vérifiable
   ↓
European Business Wallet
   ↓
données détaillées de transaction
   ↓
système comptable
```

et :

```
eReceipt vérifiable
   ↓
service fiscal de démonstration
   ↓
vérification
   ↓
rapprochement de TVA
```

**EXPÉRIMENTÉ — SOURCE PARTICIPANT :**

> Un participant de WE BUILD documente donc une démonstration technique reliant de bout en bout paiement, justificatif structuré, wallet d'entreprise, comptabilité et traitement fiscal [S34].

**LIMITE :**

> Cette démonstration ne constitue pas la preuve qu'une administration fiscale nationale utilise actuellement cette chaîne en production.

---

### Paiement et fiscalité peuvent donc appartenir à une même chaîne technique

Cette distinction est importante par rapport aux chapitres précédents.

Jusqu'ici, l'enquête avait établi séparément :

```
paiement
→ données de paiement

facturation / transaction
→ données fiscales

Business Wallet
→ attestations et données d'entreprise
```

Le pilote permet désormais de représenter une chaîne expérimentale unique :

```
identité de l'entreprise
   ↓
identité / délégation de la personne
   ↓
EUDI Wallet
   ↓
compte ou carte
   ↓
paiement
   ↓
eReceipt vérifiable
   ↓
European Business Wallet
   ↓
détail de transaction / TVA
   ↓
comptabilité
   ↓
traitement fiscal expérimental
```

**EXPÉRIMENTÉ :**

> Le raccord technique paiement → justificatif structuré → données fiscales → traitement fiscal a donc fait l'objet d'une démonstration de bout en bout dans l'écosystème WE BUILD [S34].

---

### Ce raccord ne dépend pas d'une base centrale unique

Le parcours confirme également un principe identifié précédemment.

Les informations n'ont pas besoin d'être regroupées dans une base de données centrale unique.

Les différents composants peuvent échanger successivement des preuves ou credentials vérifiables.

Par exemple :

```
banque
→ confirmation du paiement

vendeur
→ émission du justificatif

wallet
→ conservation / présentation du credential

comptabilité 
→ exploitation du justificatif

service fiscal
→ vérification du justificatif
```

**AVÉRÉ / EXPÉRIMENTÉ :**

> Une chaîne d'interconnexion peut donc fonctionner de bout en bout au moyen de plusieurs systèmes distribués sans nécessiter qu'un acteur central détienne l'intégralité des données de chaque étape [S34].

Cette architecture distribuée rend particulièrement importante l'analyse des interfaces et des droits d'accès plutôt que la seule recherche d'une base de données centrale.

---

### Facturation électronique et paiement : autre chaîne étudiée dans le même programme

WE BUILD ne limite pas ses travaux aux eReceipts.

La documentation du programme fait également apparaître parmi ses cas d'usage :

- Business Payments ;  
- eInvoicing ;  
- Foreign Tax Declaration [S33][S34].

Des ateliers d'interopérabilité ont en outre porté sur les paiements professionnels, la facturation et les justificatifs numériques dans l'environnement des EUDI Wallets et Business Wallets.

**AVÉRÉ :**

> Paiement professionnel, facturation électronique et traitement fiscal font donc partie des domaines effectivement expérimentés dans le même programme européen [S33][S34].

**NON ÉTABLI :**

> Les éléments étudiés ne permettent pas encore d'affirmer que la chaîne PA4 relative aux eReceipts constitue directement le futur mécanisme ViDA de facturation électronique ou le mécanisme français de facturation électronique.

---

### Un pont important est désormais fermé

Au début du chapitre 5, plusieurs raccords restaient séparés :

- identité        → paiement  
- transaction     → fiscalité  
- Business Wallet → données d'entreprise

Le cas WE BUILD permet désormais de les réunir expérimentalement :

```
identité
   ↓
paiement
   ↓
preuve structurée de transaction
   ↓
Business Wallet
   ↓
données fiscales
   ↓
traitement fiscal
```

**EXPÉRIMENTÉ :**

> Il existe donc au moins un cas d'usage européen dans lequel ces domaines sont techniquement reliés de bout en bout.

Cela ne démontre aucune finalité de contrôle des achats.

Cela démontre en revanche que leur interconnexion technique ne constitue plus seulement une possibilité abstraite.

---

### Il reste le raccord environnemental

Le chapitre 3 a établi séparément :

```
produit identifiable
   ↓
DPP
   ↓
données produit
   ↓
données de durabilité / environnementales
```

Les sections 5.2 et 5.3 ont ensuite établi :

```
Business Wallet
   ↔
DPP / données produit / durabilité
```

et :

```
Business Wallet
   ↔
transaction / TVA / facturation
```

La présente section établit désormais expérimentalement :

```
paiement
   ↓
justificatif comportant les lignes d'achat
   ↓
Business Wallet
   ↓
traitement comptable / fiscal
```

Il devient donc possible de juxtaposer les deux chaînes documentées :

```
DPP / données de durabilité
   ↕  
European Business Wallet
```

et :

```
paiement
   ↓
eReceipt / lignes d'achat
   ↓
European Business Wallet
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Lorsqu'une ligne d'achat permet d'identifier le produit correspondant et que les droits d'accès nécessaires existent, le Business Wallet ou un service interconnecté dispose techniquement des composants permettant de rapprocher la preuve de transaction des informations correspondantes contenues dans l'écosystème DPP.

Ce rapprochement n'est plus déduit uniquement de la compatibilité théorique de deux formats.

Il repose désormais sur l'existence documentée d'un environnement wallet relié, d'un côté, aux données produit et de durabilité et, de l'autre, à des justificatifs détaillés issus d'un paiement.

---

### Le dernier raccord vers le paiement conditionnel reste distinct

Le chapitre 4 a établi une autre chaîne :

```
système externe
   ↓
vérification d'une condition
   ↓
couche de conditionnalité
   ↓
paiement
```

Les travaux de la BCE ont également démontré expérimentalement que des plateformes d'acteurs du marché pouvaient communiquer par API avec un environnement simulant l'euro numérique [S27][S28].

Nous disposons donc désormais de deux ensembles :

**Ensemble A**

```
produit / DPP / durabilité
   ↕
Business Wallet
   ↕
transaction détaillée / eReceipt
   ↕
paiement
```

**Ensemble B**

```
système externe
   ↓
condition externe
   ↓
couche de conditionnalité
   ↓
paiement
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les architectures documentées contiennent donc les composants nécessaires pour qu'une information provenant d'un système extérieur soit vérifiée et utilisée dans un processus entourant l'exécution d'un paiement.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre cependant que les données environnementales du DPP soient actuellement utilisées comme condition dans un paiement en euro numérique ou dans un autre système de paiement.

---

### La différence entre « possible », « expérimenté » et « prévu »

À ce stade de l'enquête, trois niveaux doivent être strictement distingués.

**EXPÉRIMENTÉ :**

> identité → paiement → justificatif structuré → Business Wallet → comptabilité / traitement fiscal.

**AVÉRÉ / PRÉVU :**

> Business Wallet ↔ DPP / données produit et de durabilité.

**AVÉRÉ / EXPÉRIMENTÉ :**

> système externe → vérification d'une condition → paiement conditionnel.

Mais :

**NON ÉTABLI :**

> donnée environnementale → condition déterminant l'exécution d'un paiement.

Cette dernière flèche ne doit pas être ajoutée artificiellement à la chaîne tant qu'aucune source ne la documente.

---

### Ce que cette section change dans la démonstration

Au début de l'enquête, il aurait été possible d'objecter que les différents systèmes étudiés n'avaient aucun lien entre eux :

« la facture est fiscale » ;

« le DPP est environnemental » ;

« le wallet sert à l'identité » ;

« le paiement appartient aux banques » ;

« l'euro numérique est une infrastructure monétaire distincte ».

Les sources étudiées permettent désormais d'écarter une version aussi absolue de cette séparation.

**AVÉRÉ :**

> La Commission recherche explicitement des synergies entre plusieurs de ces infrastructures [S30][S31].

**AVÉRÉ :**

> Des standards, API, attestations et mécanismes d'interopérabilité permettent leurs interactions [S20][S30][S32].

**AVÉRÉ :**

> Des programmes européens réunissent identité, facturation, fiscalité et paiement dans les mêmes environnements expérimentaux [S33][S34].

**EXPÉRIMENTÉ :**

> Une chaîne de bout en bout reliant identité, paiement, justificatif détaillé, Business Wallet, comptabilité et traitement fiscal a été démontrée par des participants de WE BUILD [S34].

**NON ÉTABLI :**

> L'utilisation d'une donnée environnementale comme critère de paiement reste, elle, non démontrée.

---

### Conclusion intermédiaire

**AVÉRÉ / EXPÉRIMENTÉ :**

> Une infrastructure de wallet peut participer à une chaîne reliant l'identité d'une entreprise et de son représentant, un compte ou une carte, un paiement et une preuve structurée de la transaction [S34].

**EXPÉRIMENTÉ :**

> Cette preuve peut contenir les lignes d'achat, les montants, les informations de TVA et une référence au paiement puis être transmise automatiquement au European Business Wallet de l'entreprise [S34].

**EXPÉRIMENTÉ :**

> Des connecteurs permettent ensuite la réutilisation du justificatif par un système comptable et, dans le cas de démonstration étudié, par un service fiscal effectuant un rapprochement de TVA [S34].

**AVÉRÉ :**

> Le même écosystème Business Wallet est parallèlement articulé avec le Digital Product Passport et ses données relatives aux produits et à leur durabilité [S30].

**AVÉRÉ / EXPÉRIMENTÉ :**

> Une architecture distincte de paiement conditionnel permet par ailleurs à une condition vérifiée par un système externe d'intervenir dans l'exécution d'une transaction [S27][S28].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les infrastructures étudiées permettent donc de construire une chaîne technique dans laquelle une transaction détaillée peut être reliée à un produit identifiable, le produit à des données externes et le résultat d'une vérification externe à une logique conditionnelle entourant un paiement.

**NON ÉTABLI :**

> Aucun document étudié ne démontre cependant que cette chaîne soit actuellement assemblée afin d'utiliser une donnée environnementale pour autoriser, refuser ou limiter un paiement.

Le nombre de raccords manquants s'est donc considérablement réduit.

Il reste maintenant à examiner précisément **le dernier raccord de la chaîne : environnement → paiement**, en recherchant non plus seulement s'il est techniquement possible, mais s'il existe un projet, un pilote, un standard ou une documentation qui l'expérimente ou le prévoit explicitement.

---

## [S35] CEN/TS 16931-8:2024 — eReceipts, identifiant DPP et informations environnementales du produit

**Organisme :** Comité européen de normalisation (CEN)

**Document :** CEN/TS 16931-8:2024 — Electronic invoicing — Part 8: Semantic data model of the elements of an e-receipt

**Date :** 2024

**Utilisé dans :** Chapitre 5

**Éléments établis :** modèle sémantique européen relatif aux justificatifs électroniques ; description d'un processus dans lequel l'acheteur sélectionne un moyen de paiement, effectue ou initie le paiement puis reçoit un eReceipt généré par le vendeur ; possibilité d'inclure dans certains environnements des informations spécifiques relatives au produit ; mention explicite du Digital Product Passport pour les catégories de produits concernées ; utilisation d'un identifiant DPP permettant de relier le justificatif aux informations vérifiées relatives au produit ; mention parmi ces informations de la durabilité des matériaux ainsi que des impacts sociaux et environnementaux liés aux matériaux, à la production, à l'utilisation et à la fin de vie du produit.

**Précaution méthodologique :** l'existence d'un champ ou mécanisme permettant de relier un eReceipt au DPP démontre la possibilité normalisée d'établir ce raccord. Elle ne démontre pas que chaque eReceipt contiendra un identifiant DPP, ni que les données environnementales correspondantes seront systématiquement récupérées, ni qu'elles seront utilisées par un système de paiement.

**Référence :** CEN/TS 16931-8:2024

---

## 5.7 Le raccord environnement → paiement

**Statut : AVÉRÉ / EXPÉRIMENTÉ / DÉDUCTIBLE TECHNIQUEMENT / NON ÉTABLI**

Les sections précédentes ont progressivement réduit le nombre de raccords manquants entre les infrastructures étudiées.

À l'issue de la section 5.6, deux chaînes distinctes étaient établies.

La première relie désormais expérimentalement le paiement au détail économique de la transaction :

```
paiement
   ↓
eReceipt
   ↓
lignes d'achat
   ↓
European Business Wallet
```

La seconde relie une information provenant d'un système extérieur à l'exécution d'un paiement conditionnel :

```
système externe
   ↓
vérification d'une condition
   ↓
couche de conditionnalité
   ↓
paiement
```

La question de cette section est donc volontairement limitée à une seule flèche :

> **Existe-t-il un mécanisme documenté permettant de relier une information environnementale relative au produit à la transaction ou à la condition déterminant l'exécution du paiement ?**

---

### eReceipt → Digital Product Passport

Un élément supplémentaire apparaît dans les travaux européens de normalisation relatifs aux justificatifs électroniques [S35].

Le modèle CEN/TS 16931-8:2024 décrit le processus économique dans lequel l'acheteur sélectionne un moyen de paiement, effectue ou initie le paiement, puis reçoit un eReceipt généré par le vendeur.

Le même document prévoit que, dans certains environnements, des informations spécifiques relatives au produit puissent être associées au justificatif.

Pour les catégories de produits soumises au Digital Product Passport, le standard mentionne explicitement l'utilisation d'un **identifiant DPP permettant de relier le justificatif aux informations vérifiées relatives au produit** [S35].

**AVÉRÉ :**

> Un standard européen relatif aux eReceipts prévoit donc explicitement un raccord entre le justificatif d'une transaction et le Digital Product Passport du produit correspondant [S35].

La chaîne devient :

```
achat
   ↓
paiement
   ↓
eReceipt
   ↓
identifiant DPP
   ↓
Digital Product Passport
```

Ce raccord est plus précis que la simple possibilité de faire correspondre ultérieurement une référence commerciale avec un identifiant produit.

Le mécanisme de liaison au DPP est directement envisagé dans le modèle du justificatif.

---

### Le raccord donne accès à des informations environnementales

Le même standard explique l'intérêt de cette relation avec le DPP.

L'identifiant permet de relier le produit aux informations vérifiées concernant son cycle de vie.

Parmi les informations explicitement mentionnées figurent notamment :

- la durabilité de l'approvisionnement en matériaux ;  
- les impacts sociaux des matériaux utilisés ;  
- les impacts environnementaux des matériaux utilisés ;  
- la production ;  
- l'utilisation ;  
- la fin de vie du produit [S35].

**AVÉRÉ :**

> Le raccord eReceipt → identifiant DPP ne conduit donc pas uniquement vers une référence administrative du produit : il peut conduire vers des informations vérifiées comprenant des caractéristiques relatives à sa durabilité et à ses impacts environnementaux [S35].

La chaîne suivante est ainsi explicitement documentée au niveau du modèle sémantique :
```
transaction
   ↓
eReceipt
   ↓
identifiant DPP
   ↓
produit
   ↓
informations vérifiées
   ↓
durabilité / impacts environnementaux
```

---

### Paiement → eReceipt → DPP → environnement

Ce nouvel élément peut être rapproché de la chaîne expérimentée dans WE BUILD.

La section 5.6 a établi :

```
paiement
   ↓
eReceipt vérifiable
   ↓
lignes d'achat / informations de transaction
```

Le standard CEN/TS 16931-8 ajoute :

```
eReceipt
   ↓
identifiant DPP
   ↓
informations vérifiées du produit
   ↓
informations environnementales
```

**AVÉRÉ / EXPÉRIMENTÉ SELON LES MAILLONS :**

> Les composants documentés permettent donc désormais de construire une chaîne dans laquelle un paiement est relié à un justificatif électronique et dans laquelle un justificatif électronique peut lui-même être relié, au moyen d'un identifiant DPP, aux informations environnementales vérifiées du produit [S34][S35].

La chaîne complète peut être représentée ainsi :

```
paiement
   ↓
eReceipt
   ↓
produit identifiable
   ↓
identifiant DPP
   ↓
Digital Product Passport
   ↓
données de durabilité / environnementales
```

**LIMITE :**

> Cette représentation assemble deux raccords documentés dans des contextes différents. Elle ne démontre pas qu'un même système opérationnel utilise actuellement l'intégralité de cette chaîne de bout en bout.

---

### Le rapprochement transaction → environnement n'est donc plus uniquement hypothétique

Au début de l'enquête, le lien entre un achat et les caractéristiques environnementales du produit reposait sur une déduction :

```
transaction
   ↓
identifier le produit
   ↓
rechercher son DPP
   ↓
retrouver la donnée environnementale
```

Le standard relatif aux eReceipts apporte un élément supplémentaire.

**AVÉRÉ :**

> Le modèle européen prévoit directement qu'un identifiant DPP puisse être associé au justificatif afin de relier l'achat aux informations vérifiées relatives au produit [S35].

Il n'est donc plus nécessaire de supposer qu'un rapprochement devrait obligatoirement être réalisé après la transaction à partir de bases indépendantes.

Le justificatif peut lui-même transporter le mécanisme permettant d'accéder au passeport du produit.

---

### Une autre convergence existe avec la facturation électronique

Cette relation doit également être rapprochée des éléments établis en 5.3 et 5.4.

La Commission prévoit :

```
eInvoicing
   ↓
réutilisation des données
   ↓
reporting de durabilité
```

et les travaux de standardisation relatifs à EN 16931 prennent explicitement en compte les besoins provenant du reporting de durabilité [S31][S32].

Le standard relatif aux eReceipts ajoute désormais :

```
eReceipt
   ↓
identifiant DPP
   ↓
informations environnementales du produit
```

**AVÉRÉ :**

> Plusieurs travaux européens distincts organisent donc le rapprochement entre données décrivant une transaction et informations relatives à la durabilité ou à l'environnement [S31][S32][S35].

Cela ne démontre toujours pas l'établissement d'un profil environnemental individuel.

---

### Le paiement conditionnel accepte une condition provenant de l'extérieur

De l'autre côté de la chaîne, les travaux de la BCE établissent que la logique conditionnelle n'a pas besoin d'être intégrée à la monnaie elle-même.

Le dispositif étudié sépare :

```
infrastructure de règlement
   +
couche de conditionnalité développée par le marché
```

Cette couche peut utiliser un monitoring extérieur afin de vérifier qu'une condition est satisfaite [S27][S28].

Une fois cette condition vérifiée :

```
condition satisfaite
   ↓
libération des fonds
```

ou, si elle ne l'est pas :

```
condition non satisfaite
   ↓
annulation / expiration de la réservation
```

**AVÉRÉ / EXPÉRIMENTÉ :**

> La conception actuelle permet donc à une information vérifiée à l'extérieur de l'infrastructure de règlement d'intervenir dans la décision d'exécuter un paiement conditionnel [S27][S28].

---

### La nature de la condition n'est pas techniquement limitée à la livraison

Les exemples les plus fréquemment présentés par la BCE concernent la livraison d'un produit, l'arrivée d'un train, l'utilisation d'un service ou l'accomplissement d'une étape.

Ces exemples décrivent des cas d'usage.

Ils ne constituent pas une liste technique exhaustive des seules informations pouvant être vérifiées par une couche de conditionnalité.

Les travaux expérimentaux montrent que les prestataires peuvent développer la logique conditionnelle et que des plateformes externes peuvent intervenir dans sa vérification [S27][S28].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une condition provenant d'une infrastructure environnementale pourrait techniquement être traitée selon le même principe si un prestataire développait un tel service, si la donnée correspondante était accessible et si cet usage était juridiquement autorisé.

Par exemple :

```
identifiant DPP
   ↓
service externe
   ↓
lecture d'une caractéristique environnementale
   ↓
évaluation d'une règle
   ↓
résultat de la vérification
```

Le système de paiement n'aurait pas nécessairement besoin de recevoir l'intégralité du DPP.

Il pourrait techniquement recevoir uniquement un résultat :

```
condition remplie
   ou
condition non remplie
```

---

### Le dernier raccord technique peut donc être représenté

En assemblant uniquement les capacités documentées :

```
produit acheté
   ↓
eReceipt
   ↓
identifiant DPP
   ↓
Digital Product Passport
   ↓
donnée environnementale
   ↓
service externe de vérification
   ↓
résultat d'une condition
   ↓
couche de conditionnalité
   ↓
paiement
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Aucun obstacle architectural identifié dans les sources étudiées n'impose que la donnée vérifiée par le système externe soit une donnée de livraison plutôt qu'une autre donnée accessible à ce système.

Mais cette déduction doit immédiatement être séparée de la preuve d'un usage réel.

---

### La recherche du cas environnemental dans les travaux de la BCE

Les documents de la Digital Euro Innovation Platform permettent de vérifier si cette possibilité a déjà été transformée en cas d'usage environnemental.

Les scénarios documentés portent notamment sur :

- la livraison ;  
- les paiements à l'usage ;  
- les paiements par étapes ;  
- la mobilité et le transport ;  
- le commerce électronique ;  
- les services financiers ;  
- certaines applications industrielles ;  
- les interactions machine-to-machine [S28].

Les travaux relatifs aux eReceipts mentionnent également un bénéfice environnemental résultant de la réduction de l'utilisation du papier.

**NON ÉTABLI :**

> Les documents étudiés de la Digital Euro Innovation Platform ne décrivent cependant pas de scénario dans lequel l'empreinte carbone, la performance environnementale, le DPP ou une autre donnée de durabilité d'un produit constitue la condition déclenchant ou empêchant un paiement [S28].

Ce résultat négatif est important.

Il empêche de transformer la possibilité technique en affirmation d'un projet actuellement documenté.

---

### L'euro numérique ne peut pas être utilisé comme monnaie programmable

Une autre limite doit rester explicitement présente.

La proposition de règlement relative à l'euro numérique exclut la **monnaie programmable** [S22].

Cela signifie que les unités d'euro numérique ne doivent pas comporter intrinsèquement des restrictions déterminant :

- les catégories de biens pouvant être achetées ;  
- les commerçants auprès desquels elles peuvent être utilisées ;  
- la période pendant laquelle elles peuvent être dépensées ;  
- ou d'autres limitations remettant en cause leur pleine fongibilité.

**AVÉRÉ :**

> L'Eurosystème ne prévoit donc pas de coder dans les unités monétaires elles-mêmes une règle du type « cet euro ne peut pas acheter un produit dont l'empreinte carbone dépasse X » [S22][S27].

---

### Paiement conditionnel et monnaie programmable restent cependant deux mécanismes différents

L'exclusion de la monnaie programmable ne supprime pas les paiements conditionnels.

La proposition européenne définit séparément l'opération de paiement conditionnelle comme une opération exécutée automatiquement lorsque des conditions prédéfinies convenues entre le payeur et le bénéficiaire sont remplies [S22].

La BCE prévoit parallèlement que les prestataires de paiement puissent développer la couche de conditionnalité [S27][S28].

La distinction est donc :

```
**MONNAIE PROGRAMMABLE**
règle intégrée dans l'unité monétaire
→ exclue

contre :

**PAIEMENT CONDITIONNEL**
règle appliquée au processus de transaction
→ prévu / expérimenté
```

**AVÉRÉ :**

> L'interdiction de la monnaie programmable ne constitue donc pas une interdiction générale de toute logique automatisée entourant l'exécution d'un paiement [S22][S27][S28].

---

### Les conditions sont présentées comme convenues entre les parties

Cette limite est également essentielle.

Dans la proposition législative, les conditions d'un paiement conditionnel sont définies comme des conditions prédéfinies **convenues par le payeur et le bénéficiaire** [S22].

Les services supplémentaires étudiés par la BCE sont par ailleurs présentés comme des services développés par les acteurs du marché et utilisés volontairement par les utilisateurs.

**AVÉRÉ :**

> Les documents étudiés ne donnent donc pas à la BCE ou à l'Eurosystème un pouvoir général permettant d'imposer unilatéralement une condition environnementale aux achats des utilisateurs.

**NON ÉTABLI :**

> Aucun mécanisme permettant à une administration de transformer directement une donnée environnementale individuelle en interdiction de paiement imposée au payeur n'a été identifié.

---

### La chaîne technique et la chaîne juridique doivent être séparées

Le résultat de l'analyse peut donc être représenté de deux manières différentes.

**CAPACITÉ TECHNIQUE :**

```
transaction
   ↓
eReceipt
   ↓
identifiant DPP
   ↓
donnée environnementale
   ↓
service externe
   ↓
condition
   ↓
paiement conditionnel
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les composants permettant de construire cette chaîne existent séparément et les interfaces nécessaires à plusieurs de ses raccords sont documentées.

Mais :

**USAGE ÉTABLI :**

```
donnée environnementale
   ↓
condition environnementale imposée
   ↓
autorisation / refus du paiement
```

**NON ÉTABLI :**

> Aucun projet institutionnel, règlement, pilote ou documentation technique étudié ne démontre actuellement l'utilisation d'une donnée environnementale relative à un produit afin d'autoriser, refuser ou limiter un paiement.

---

### Une différence importante apparaît néanmoins par rapport au début de l'enquête

Au début de l'analyse, presque toute la chaîne devait être reconstruite par hypothèse :

```
facture
   ?
produit
   ?
environnement
   ?
identité
   ?
paiement
```

À ce stade, les raccords documentés sont beaucoup plus nombreux :

```
facturation / transaction
   ↓
données structurées

produit
   ↓
DPP
   ↓
données environnementales

eReceipt
   ↓
identifiant DPP

Business Wallet
   ↔
DPP / durabilité

Business Wallet
   ↔
transaction / fiscalité

identité
   ↓
wallet
   ↓
paiement

paiement
   ↓
eReceipt détaillé

système externe
   ↓
condition
   ↓
paiement conditionnel
```

Le point restant non démontré n'est donc plus l'existence des infrastructures nécessaires.

Il est désormais beaucoup plus précis :

> **l'existence d'une règle ou d'un cas d'usage utilisant effectivement une donnée environnementale comme condition déterminant l'exécution d'un paiement.**

---

### La frontière documentaire actuelle

La frontière entre ce qui est établi et ce qui ne l'est pas peut désormais être placée précisément.

**AVÉRÉ :**

> Un produit peut être relié à des données environnementales au moyen du Digital Product Passport [S15][S19].

**AVÉRÉ :**

> Un eReceipt peut comporter un identifiant permettant de relier l'achat au DPP et à ses informations vérifiées relatives au produit [S35].

**EXPÉRIMENTÉ :**

> Un paiement peut être relié à un eReceipt contenant le détail économique de la transaction [S34].

**AVÉRÉ / EXPÉRIMENTÉ :**

> Un système extérieur peut vérifier une condition utilisée par une couche de conditionnalité entourant un paiement [S27][S28].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une donnée environnementale accessible depuis le DPP pourrait être vérifiée par un service extérieur et son résultat utilisé comme condition technique selon la même architecture.

**NON ÉTABLI :**

> Les sources étudiées ne démontrent pas qu'un tel service environnemental soit actuellement prévu ou expérimenté pour déterminer l'exécution d'un paiement.

---

### Conclusion intermédiaire

**AVÉRÉ :**

> Le standard européen relatif aux eReceipts prévoit explicitement qu'un identifiant DPP puisse relier un justificatif de transaction aux informations vérifiées du produit, comprenant notamment des informations relatives à sa durabilité et à ses impacts environnementaux [S35].

**EXPÉRIMENTÉ :**

> Des travaux européens ont parallèlement démontré une chaîne reliant paiement, eReceipt détaillé et Business Wallet [S34].

**AVÉRÉ / EXPÉRIMENTÉ :**

> L'architecture des paiements conditionnels permet à un système externe de vérifier une condition dont le résultat intervient dans l'exécution du paiement [S27][S28].

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les composants documentés permettent donc techniquement de construire une chaîne paiement ↔ transaction identifiable ↔ produit ↔ DPP ↔ donnée environnementale ainsi qu'une chaîne donnée externe → condition → paiement.

**NON ÉTABLI :**

> Aucun élément identifié ne démontre toutefois que ces deux chaînes soient actuellement raccordées afin qu'une donnée environnementale détermine l'autorisation, le refus ou la limitation d'un paiement.

**AVÉRÉ :**

> Dans le cadre juridique proposé pour l'euro numérique, les conditions d'un paiement conditionnel sont présentées comme prédéfinies et convenues entre le payeur et le bénéficiaire, tandis que la monnaie programmable limitant intrinsèquement les biens ou services pouvant être achetés est explicitement exclue [S22].

La recherche du raccord environnement → paiement aboutit donc à un résultat nuancé mais précis :

> **la chaîne technique est reconstructible avec des composants et raccords désormais largement documentés ; son utilisation environnementale comme mécanisme de décision de paiement reste, elle, non établie.**

Cette frontière doit être conservée dans la conclusion de l'enquête.

La section suivante doit maintenant examiner les **limites de la démonstration**, afin de distinguer définitivement ce que l'architecture permet, ce qui a été expérimenté et ce qu'aucune source ne permet encore d'affirmer.

---

## 5.8 Limites de la démonstration

**Statut : LIMITES ÉTABLIES / NON ÉTABLI**

Les sections précédentes ont permis d'identifier de nombreux raccords entre les infrastructures étudiées.

Ces raccords ne doivent cependant pas être interprétés au-delà de ce que démontrent effectivement les sources.

Cette section fixe donc les limites de la démonstration avant d'en établir la synthèse.

---

### Interopérabilité ne signifie pas échange systématique de données

Les infrastructures étudiées utilisent des identifiants, standards, API, attestations vérifiables et mécanismes d'autorisation permettant leur interopérabilité [S20][S30][S32].

**AVÉRÉ :**

> Plusieurs de ces systèmes sont techniquement conçus pour pouvoir échanger ou vérifier des informations provenant d'autres systèmes.

Mais :

**NON ÉTABLI :**

> Cette interopérabilité ne signifie pas que toutes leurs données soient automatiquement mises en commun, transmises ou centralisées.

Une possibilité d'interconnexion doit donc être distinguée d'un flux réellement activé.

---

### Un raccord entre deux systèmes ne démontre pas une chaîne complète

Plusieurs raccords ont été documentés séparément :

- transaction     → eReceipt  
- eReceipt        → DPP  
- DPP             → données environnementales  
- identité        → paiement  
- système externe → condition → paiement

L'existence de chacun de ces raccords ne suffit pas à démontrer qu'ils sont tous utilisés simultanément dans un même processus.

**NON ÉTABLI :**

> Aucun système opérationnel identifié dans les sources étudiées ne relie actuellement de bout en bout une donnée environnementale provenant du DPP à une décision autorisant ou refusant un paiement.

---

### Standard prévu ne signifie pas utilisation systématique

Le standard relatif aux eReceipts prévoit la possibilité de relier un justificatif au Digital Product Passport au moyen d'un identifiant DPP [S35].

Cela démontre l'existence d'un mécanisme normalisé permettant ce raccord.

Mais :

**NON ÉTABLI :**

> Tous les eReceipts ne contiendront pas nécessairement un identifiant DPP et tous les produits ne seront pas nécessairement soumis aux mêmes exigences de passeport numérique.

La possibilité normalisée d'inclure une donnée ne démontre donc pas son utilisation systématique.

---

### Projet pilote ne signifie pas système déployé

Les expérimentations WE BUILD et celles de la Digital Euro Innovation Platform permettent de démontrer la faisabilité de plusieurs chaînes techniques [S28][S33][S34].

Elles constituent des preuves d'expérimentation.

Elles ne constituent pas nécessairement des preuves de déploiement opérationnel.

**NON ÉTABLI :**

> Les processus expérimentés dans ces pilotes ne doivent pas être présentés comme des mécanismes déjà généralisés à l'ensemble des entreprises, administrations, banques ou utilisateurs européens.

Cette distinction est particulièrement importante pour les démonstrations utilisant des services fiscaux simulés ou des environnements de paiement expérimentaux.

---

### Proposition législative ne signifie pas droit définitivement adopté

Les European Business Wallets étudiés dans ce chapitre reposent notamment sur une proposition de règlement présentée par la Commission européenne [S30].

À la date de l'analyse, cette proposition suit encore la procédure législative européenne.

**AVÉRÉ :**

> Le projet permet d'établir l'orientation proposée, les fonctionnalités envisagées et l'architecture recherchée.

Mais :

**NON ÉTABLI :**

> Toutes les dispositions étudiées ne peuvent pas être présentées comme constituant déjà le droit définitif applicable dans leur rédaction actuelle.

Le texte final peut encore évoluer au cours de la procédure législative.

---

### Possibilité technique ne signifie pas autorisation juridique

Une infrastructure peut techniquement permettre à deux systèmes de communiquer sans que tous les acteurs soient juridiquement autorisés à accéder aux données correspondantes.

Le DPP prévoit notamment des droits d'accès différenciés selon les données et catégories de produits [S15][S20].

Les architectures EUDI et Business Wallet reposent également sur des mécanismes d'autorisation et de présentation sélective des informations [S29][S30].

**AVÉRÉ :**

> L'accès technique à une infrastructure et le droit d'accéder à une donnée particulière constituent deux questions différentes.

Par conséquent :

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une chaîne peut être architecturalement réalisable.

sans que cela permette d'affirmer :

> qu'un acteur déterminé possède juridiquement le droit de l'utiliser pour une finalité déterminée.

---

### Le DPP n'est pas un profil individuel de consommation

Le Digital Product Passport décrit le produit, son modèle, son lot ou son article selon les règles applicables [S15].

Le règlement prévoit en outre que les données personnelles relatives aux clients ne soient pas stockées dans le DPP sans leur consentement explicite [S15].

**AVÉRÉ :**

> Le DPP constitue une infrastructure relative au produit et non, par nature, une base de données destinée à établir le profil individuel de son acheteur.

**NON ÉTABLI :**

> L'existence du DPP ne démontre donc pas l'existence d'un registre européen centralisé associant chaque individu à l'ensemble des produits qu'il achète.

Un rapprochement avec une transaction ou une identité nécessiterait des mécanismes supplémentaires ainsi qu'une base juridique ou un consentement approprié selon le cas.

---

### Business Wallet ne signifie pas wallet individuel du consommateur

Les European Business Wallets sont destinés aux opérateurs économiques et aux interactions professionnelles ou administratives [S30].

Ils doivent être distingués de l'EUDI Wallet destiné aux personnes physiques.

**AVÉRÉ :**

> Les chaînes B2B documentées dans WE BUILD ne démontrent pas qu'un mécanisme identique soit automatiquement appliqué aux achats personnels de chaque consommateur.

Cette distinction empêche de transposer directement un pilote B2B à un scénario de contrôle individuel de la consommation.

---

### Données fiscales ne signifie pas connaissance exhaustive des achats individuels

Le chapitre 1 a montré que les données transmises dans le cadre français de la facturation électronique et du e-reporting diffèrent selon les opérations.

Les transactions B2C ne conduisent pas nécessairement à la transmission à l'administration fiscale du détail individualisé de chaque produit acheté par chaque consommateur [S1][S2][S3][S4].

**NON ÉTABLI :**

> La réforme française de la facturation électronique ne peut donc pas être présentée, sur la base des sources étudiées, comme créant à elle seule un registre nominatif exhaustif des achats de chaque particulier.

Cette limite demeure même si d'autres infrastructures disposent séparément d'informations plus détaillées sur certains produits ou transactions.

---

### Donnée environnementale disponible ne signifie pas profil carbone individuel

Le DPP et d'autres réglementations européennes permettent ou imposent, selon les produits concernés, la disponibilité de données relatives à la durabilité ou à certains impacts environnementaux [S15][S18][S19].

Le rapprochement technique entre une transaction et ces informations peut également être envisagé ou normalisé [S31][S35].

Mais :

**NON ÉTABLI :**

> Aucun mécanisme général établissant automatiquement un bilan carbone individuel à partir de l'ensemble des achats d'une personne n'a été identifié dans les sources étudiées.

Une telle finalité nécessiterait notamment l'identification des transactions pertinentes, leur attribution à une personne, la récupération des données environnementales correspondantes et une méthode permettant leur agrégation.

---

### Paiement conditionnel ne signifie pas monnaie programmable

Le chapitre 4 a établi une distinction fondamentale [S22][S27][S28].

L'euro numérique ne doit pas être conçu comme une monnaie programmable dont les unités seraient limitées à certains biens, commerçants, lieux ou périodes.

En revanche, des services de paiement conditionnel sont prévus et expérimentés.

La distinction est :

**monnaie programmable**  
règle intégrée à l'unité monétaire  
→ exclue

et :

**paiement conditionnel**  
règle appliquée au processus entourant la transaction  
→ prévu / expérimenté

**AVÉRÉ :**

> L'existence de paiements conditionnels ne permet donc pas d'affirmer que l'euro numérique lui-même pourra être programmé afin d'interdire certaines catégories d'achats [S22][S27][S28].

---

### Une condition technique possible ne signifie pas condition imposée

Les paiements conditionnels sont présentés comme reposant sur des conditions prédéfinies intervenant dans le processus de transaction [S22][S27][S28].

Les acteurs du marché peuvent développer des services utilisant cette couche de conditionnalité.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une donnée accessible à un système extérieur pourrait techniquement servir à vérifier une condition si un service correspondant était développé.

Mais :

**NON ÉTABLI :**

> Aucun pouvoir général permettant à une administration d'imposer une condition environnementale à l'ensemble des paiements des utilisateurs n'a été identifié dans les sources étudiées.

---

### La BCE n'a pas documenté de condition environnementale de paiement

Les expérimentations de la Digital Euro Innovation Platform comprennent différents scénarios de paiements conditionnels [S28].

Les cas étudiés concernent notamment la livraison, l'utilisation d'un service, des étapes contractuelles, le transport ou des processus machine-to-machine.

**NON ÉTABLI :**

> Les documents étudiés ne présentent pas l'empreinte carbone, le DPP ou une autre caractéristique environnementale du produit comme condition déterminant l'exécution d'un paiement.

Cette absence constitue actuellement la principale limite documentaire de la chaîne étudiée.

---

### Acteur commun ne signifie pas échange de données

Plusieurs banques, prestataires de paiement, entreprises technologiques et intégrateurs participent à différents projets européens [S33].

Ces recoupements permettent d'identifier un environnement industriel commun.

Mais :

**NON ÉTABLI :**

> La participation d'une même organisation à plusieurs projets ne démontre pas qu'elle transfère des données entre ces projets ou leurs infrastructures.

Une interconnexion doit être établie à partir d'un flux, d'une interface, d'un cas d'usage ou d'une documentation décrivant effectivement le raccord.

---

### Infrastructure distribuée ne signifie pas base centrale de surveillance

Les chaînes étudiées peuvent fonctionner au moyen :

- d'API ;  
- d'attestations vérifiables ;  
- de wallets ;  
- de registres ;  
- de services intermédiaires ;  
- de mécanismes de vérification externes.

Une information peut donc être vérifiée sans nécessairement être copiée intégralement dans tous les systèmes intervenant dans le processus.

**NON ÉTABLI :**

> Les sources étudiées ne démontrent pas l'existence d'une base européenne centrale réunissant simultanément identité individuelle, historique complet des achats, données environnementales, données fiscales et données de paiement.

La possibilité d'interconnexion distribuée doit donc être distinguée de l'hypothèse d'une centralisation intégrale des données.

---

### Finalité annoncée et capacité technique sont deux niveaux différents

L'enquête documente deux catégories d'éléments qu'il convient de ne pas confondre.

D'une part :

> **les finalités explicitement annoncées**

Par exemple :

- lutte contre la fraude ;  
- simplification administrative ;  
- reporting fiscal ;  
- information sur les produits ;  
- durabilité ;  
- identité numérique ;  
- interopérabilité ;  
- innovation dans les paiements.

D'autre part :

> **les capacités techniques résultant de l'architecture**

Par exemple :

- rapprocher plusieurs identifiants ;  
- interroger un registre ;  
- vérifier une attestation ;  
- relier un justificatif à un produit ;  
- récupérer une information environnementale ;  
- vérifier une condition externe ;  
- automatiser certaines étapes d'une transaction.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Une capacité peut exister avant qu'une finalité particulière ne lui soit attribuée.

Mais :

**NON ÉTABLI :**

> L'existence de cette capacité ne constitue pas une preuve que les institutions européennes ou nationales ont l'intention de l'utiliser pour une finalité non documentée.

Cette distinction constitue l'une des limites méthodologiques centrales de l'enquête.

---

### La frontière de la démonstration

Après l'ensemble des recherches du chapitre 5, la frontière peut être placée précisément.

**ÉTABLI OU EXPÉRIMENTÉ :**

> facturation / transaction → données structurées

> produit → DPP → données environnementales

> eReceipt → identifiant DPP → informations du produit

> identité → wallet → paiement

> paiement → eReceipt détaillé

> Business Wallet ↔ données de transaction / fiscalité

> Business Wallet ↔ écosystème produit / durabilité

> système externe → vérification d'une condition → paiement conditionnel

Mais :

**NON ÉTABLI :**

> donnée environnementale → règle imposée → autorisation / refus d'un paiement

et :

**NON ÉTABLI :**

> ensemble de ces infrastructures → système centralisé de contrôle individuel de la consommation

---

### Conclusion intermédiaire

Les recherches menées dans ce chapitre permettent donc d'aller beaucoup plus loin que le simple constat de l'existence parallèle de plusieurs infrastructures numériques.

Des raccords institutionnels, normatifs et techniques existent réellement.

Certains sont déjà prévus par les textes.

D'autres sont standardisés.

D'autres encore ont été expérimentés dans des pilotes européens.

Mais plusieurs limites demeurent essentielles :

> **interopérable** ne signifie pas **interconnecté en permanence** ;

> **interconnecté** ne signifie pas **centralisé** ;

> **techniquement possible** ne signifie pas **juridiquement autorisé** ;

> **expérimenté** ne signifie pas **déployé** ;

> **donnée environnementale accessible** ne signifie pas **profil carbone individuel** ;

> **paiement conditionnel** ne signifie pas **monnaie programmable** ;

> **capacité technique** ne signifie pas **intention politique**.

Enfin, la principale frontière documentaire reste inchangée :

> **les infrastructures permettant de relier transaction, produit, donnée environnementale et mécanisme de conditionnalité existent ou peuvent être raccordées techniquement, mais aucune source étudiée ne démontre actuellement qu'une donnée environnementale soit utilisée afin d'autoriser, refuser ou limiter le paiement d'un utilisateur.**

---

## 5.9 Ce que ce chapitre permet d'établir

Le chapitre 5 avait pour objectif de déterminer si les infrastructures étudiées précédemment devaient être considérées comme des systèmes indépendants ou si des interconnexions concrètes pouvaient être documentées entre elles.

Les recherches permettent désormais d'apporter une réponse plus précise.

Les systèmes ne forment pas une infrastructure unique et centralisée.

Ils ne sont cependant pas non plus totalement indépendants les uns des autres.

Des raccords institutionnels, normatifs et techniques existent entre plusieurs d'entre eux. Certains sont prévus par les textes, certains sont standardisés et d'autres ont déjà été expérimentés.

---

### Un écosystème européen commun est explicitement recherché

La Commission européenne ne présente plus certaines de ces infrastructures uniquement comme des projets isolés.

Sa stratégie pour le marché unique rassemble notamment :

- le Digital Product Passport ;  
- l'eInvoicing ;  
- les European Business Wallets ;  
- le Single Digital Gateway ;  
- le Once Only Technical System ;  
- les systèmes européens d'identification et d'échange de données.

La Commission indique que ces outils doivent collectivement former un **écosystème cohérent de solutions numériques** destiné à créer des synergies entre les différents systèmes [S30][S31].

**AVÉRÉ :**

> L'existence d'une stratégie européenne visant l'interopérabilité et la création de synergies entre plusieurs infrastructures étudiées dans cette enquête est explicitement documentée.

Cette convergence institutionnelle ne démontre cependant pas que toutes les données de ces systèmes soient échangées entre elles.

---

### Facturation électronique → autres usages de la donnée

La facturation électronique ne constitue pas uniquement un mécanisme de transmission d'un document entre vendeur et acheteur.

En France, les données structurées alimentent notamment l'administration fiscale [S1][S2][S3][S4].

Au niveau européen, la Commission prévoit également de développer la réutilisation des données d'eInvoicing pour d'autres fonctions [S31].

Parmi les orientations explicitement documentées figurent :

```
eInvoicing
   ↓
reporting TVA
```

mais également :

```
eInvoicing
   ↓
reporting de durabilité
```

et :

```
eInvoicing
   ↓
données douanières / EU Customs Data Hub
```

**AVÉRÉ :**

> La réutilisation des données de facturation électronique au-delà de la seule production de la facture fait partie des orientations européennes documentées [S31].

---

### Transaction → produit → environnement

Le chapitre 3 avait établi l'existence d'une infrastructure permettant d'associer un produit à un Digital Product Passport contenant, selon les catégories concernées, des informations relatives à sa durabilité ou à ses caractéristiques environnementales [S15][S18][S19][S20].

Le chapitre 5 a identifié un raccord supplémentaire.

Le modèle européen relatif aux eReceipts prévoit qu'un justificatif puisse comporter un identifiant permettant de relier le produit acheté à son Digital Product Passport [S35].

La chaîne devient :

```
transaction
   ↓
eReceipt
   ↓
identifiant DPP
   ↓
produit
   ↓
données de durabilité / environnementales
```

**AVÉRÉ :**

> Un mécanisme normalisé permettant de relier un justificatif transactionnel au Digital Product Passport et aux informations vérifiées du produit est documenté [S35].

**LIMITE :**

> Cela ne signifie pas que tous les produits ou tous les justificatifs utiliseront systématiquement ce mécanisme.

---

### Business Wallet → identité, transaction et données produit

Les European Business Wallets constituent un autre point de raccord important.

Les documents étudiés prévoient leur utilisation pour :

- identifier et authentifier les opérateurs économiques ;  
- gérer des attestations vérifiables ;  
- échanger des informations relatives à la TVA et aux transactions ;  
- soutenir des processus liés à la facturation ;  
- interagir avec le Digital Product Passport et certaines données relatives aux produits et à leur durabilité [S30].

La chaîne institutionnelle peut donc être représentée ainsi :

```
identité de l'entreprise
   ↕
Business Wallet
   ↔ données fiscales / transactionnelles
   ↔ facturation
   ↔ DPP / données produit
```

**AVÉRÉ :**

> Le Business Wallet est conçu comme une infrastructure transversale permettant à plusieurs catégories de données d'entreprise d'être présentées, vérifiées ou échangées dans un environnement interopérable [S30][S32].

**LIMITE :**

> Le projet législatif relatif aux European Business Wallets n'est pas encore un texte définitivement adopté dans sa rédaction actuelle.

---

### Identité → paiement

Le raccord entre identité numérique et paiement est également explicitement documenté.

L'EUDI Wallet peut être utilisé pour l'authentification de paiements et la présentation sélective de certaines attestations [S29].

Les travaux relatifs à l'euro numérique prévoient également son utilisation comme mécanisme possible d'authentification pour certaines transactions [S22][S29].

La chaîne :

```
identité numérique
   ↓
EUDI Wallet
   ↓
authentification
   ↓
paiement
```

est donc :

**AVÉRÉ / EXPÉRIMENTÉ :**

> L'identité numérique européenne et les infrastructures de paiement font déjà l'objet de raccords et d'expérimentations communes [S29].

---

### Paiement → transaction détaillée → Business Wallet

Les expérimentations étudiées dans WE BUILD apportent un raccord supplémentaire.

Un parcours B2B relie :

```
identité de l'entreprise
   ↓
personne autorisée
   ↓
wallet
   ↓
compte ou carte
   ↓
paiement
   ↓
eReceipt vérifiable
   ↓
lignes d'achat / TVA / référence du paiement
   ↓
European Business Wallet
```

Le justificatif peut ensuite être réutilisé par des systèmes comptables et, dans la démonstration étudiée, par un service fiscal de rapprochement de TVA [S34].

**EXPÉRIMENTÉ :**

> Une chaîne reliant identité, paiement, justificatif transactionnel détaillé, wallet d'entreprise et traitement comptable ou fiscal a donc fait l'objet d'une démonstration technique [S34].

Cette chaîne ne doit cependant pas être présentée comme un système déjà généralisé ou déployé par les administrations fiscales européennes.

---

### Système externe → condition → paiement

Les travaux relatifs à l'euro numérique établissent parallèlement qu'un paiement conditionnel peut dépendre d'une condition vérifiée à l'extérieur de l'infrastructure de règlement [S22][S27][S28].

L'architecture peut être représentée ainsi :

```
événement ou information externe
   ↓
service de vérification
   ↓
condition satisfaite / non satisfaite
   ↓
couche de conditionnalité
   ↓
exécution du paiement
```

**AVÉRÉ / EXPÉRIMENTÉ :**

> Des systèmes externes peuvent intervenir dans la vérification d'une condition utilisée par un service de paiement conditionnel [S27][S28].

La logique conditionnelle peut être développée par les acteurs du marché sans être intégrée à l'unité monétaire elle-même.

---

### Les principales chaînes documentées

À l'issue du chapitre 5, les raccords peuvent être synthétisés ainsi :

```
**FACTURATION / TRANSACTION**
données structurées
   ↓
fiscalité
   ↓
réutilisation prévue pour d'autres reportings
```

---

```
**TRANSACTION / PRODUIT**
eReceipt
   ↓
identifiant DPP
   ↓
Digital Product Passport
   ↓
informations produit / durabilité / environnement
```

---

```
**ENTREPRISE**
identité
   ↓
European Business Wallet
   ↔ attestations
   ↔ transaction / TVA / facturation
   ↔ environnement produit / DPP
```

---

```
**IDENTITÉ / PAIEMENT**
EUDI Wallet
   ↓  
authentification
   ↓
paiement
```

---

```
**PAIEMENT / JUSTIFICATIF**
paiement
   ↓
eReceipt vérifiable
   ↓
détail de transaction
   ↓
Business Wallet
   ↓
comptabilité / traitement fiscal expérimental
```

---

```
**PAIEMENT CONDITIONNEL**
système externe
   ↓
vérification d'une condition
   ↓
couche de conditionnalité
   ↓
paiement
```

---

### La chaîne techniquement reconstructible

Ces raccords permettent désormais de reconstruire une chaîne beaucoup plus complète que celle disponible au début de l'enquête :

```
identité
   ↓
wallet
   ↓
transaction / paiement
   ↓
justificatif structuré
   ↓
produit identifiable
   ↓
Digital Product Passport
   ↓
donnée environnementale
```

Parallèlement :

```
donnée externe
   ↓
service de vérification
   ↓
résultat d'une condition
   ↓
paiement conditionnel
```

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les architectures documentées permettent techniquement qu'une information relative à un produit soit récupérée depuis une infrastructure externe, évaluée par un service et transformée en résultat utilisable par une logique automatisée entourant une transaction.

Cette conclusion ne nécessite pas l'existence d'une base centrale réunissant toutes les informations.

Les différents systèmes peuvent fonctionner au moyen d'identifiants, API, wallets, attestations vérifiables et services intermédiaires [S20][S30][S32].

---

### Le raccord qui n'a pas été trouvé

Malgré les recherches menées dans les différentes infrastructures, aucun document étudié ne permet d'ajouter la flèche suivante comme élément avéré :

```
donnée environnementale
   ↓
condition environnementale
   ↓
autorisation / refus / limitation du paiement
```

**NON ÉTABLI :**

> Aucun règlement, projet institutionnel, standard ou pilote identifié dans cette enquête ne démontre actuellement qu'une donnée environnementale issue du DPP ou d'une infrastructure équivalente soit utilisée afin de déterminer l'exécution d'un paiement.

Les exemples de paiements conditionnels étudiés portent sur d'autres événements ou conditions [S27][S28].

La présence des composants nécessaires ne constitue donc pas la preuve de leur assemblage pour cette finalité.

---

### Ce qui change néanmoins par rapport à l'hypothèse initiale

Au début de l'enquête, une représentation possible aurait été :

```
facturation
   ?
produit
   ?
environnement
   ?
identité
   ?
paiement
```

Après analyse des sources officielles, la situation est différente.

Plusieurs points d'interrogation peuvent être remplacés par des raccords documentés :

```
transaction
   → eReceipt
   → DPP
   → données environnementales
```

et :

```
identité
   → wallet
   → paiement
```

ainsi que :

```
paiement
   → eReceipt détaillé
   → Business Wallet
```

et :

```
système externe
   → condition
   → paiement conditionnel
```

Enfin, la Commission documente elle-même une stratégie visant à créer des synergies entre plusieurs infrastructures numériques étudiées dans cette enquête [S30][S31].

**AVÉRÉ :**

> L'hypothèse selon laquelle toutes ces infrastructures seraient nécessairement conçues et exploitées comme des systèmes totalement indépendants n'est donc pas compatible avec l'ensemble des documents étudiés.

Mais l'affirmation inverse serait également excessive.

**NON ÉTABLI :**

> Les sources ne démontrent pas l'existence d'une infrastructure unique réunissant toutes ces données ni d'un système européen de contrôle environnemental individuel des paiements.

---

### Tableau de synthèse

| Raccord étudié                                                                                  | Statut                                                |
|-------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| Facturation électronique → administration fiscale                                               | **AVÉRÉ**                                             |
| Données fiscales → analyse économique / politiques publiques                                    | **AVÉRÉ**                                             |
| Produit → Digital Product Passport                                                              | **AVÉRÉ**                                             |
| DPP → données de durabilité / environnementales                                                 | **AVÉRÉ**                                             |
| DPP → registre / API / systèmes externes                                                        | **AVÉRÉ**                                             |
| eReceipt → identifiant DPP                                                                      | **AVÉRÉ**                                             |
| eReceipt → informations environnementales via DPP                                               | **AVÉRÉ**                                             |
| eInvoicing → réutilisation pour reporting de durabilité                                         | **PRÉVU / AVÉRÉ**                                     |
| eInvoicing → rapprochement avec données douanières                                              | **PRÉVU / AVÉRÉ**                                     |
| Business Wallet → identité d'entreprise                                                         | **AVÉRÉ DANS LE PROJET**                              |
| Business Wallet → données TVA / transaction / facturation                                       | **AVÉRÉ DANS LE PROJET**                              |
| Business Wallet → DPP / données produit                                                         | **AVÉRÉ DANS LE PROJET**                              |
| EUDI Wallet → authentification de paiement                                                      | **AVÉRÉ / EXPÉRIMENTÉ**                               |
| EUDI Wallet → euro numérique                                                                    | **PRÉVU / EXPÉRIMENTÉ**                               |
| Paiement → eReceipt détaillé → Business Wallet                                                  | **EXPÉRIMENTÉ**                                       |
| eReceipt → comptabilité / traitement fiscal                                                     | **EXPÉRIMENTÉ**                                       |
| Système externe → condition → paiement                                                          | **AVÉRÉ / EXPÉRIMENTÉ**                               |
| Transaction → produit → donnée environnementale                                                 | **AVÉRÉ / DÉDUCTIBLE SELON LE RACCORDEMENT EFFECTIF** |
| Donnée environnementale → service externe de vérification                                       | **DÉDUCTIBLE TECHNIQUEMENT**                          |
| Donnée environnementale → condition de paiement                                                 | **DÉDUCTIBLE TECHNIQUEMENT**                          |
| Donnée environnementale → refus ou limitation effective du paiement                             | **NON ÉTABLI**                                        |
| Profil carbone individuel généralisé à partir des achats                                        | **NON ÉTABLI**                                        |
| Base centrale réunissant identité + achats + fiscalité + environnement + paiement               | **NON ÉTABLI**                                        |
| Contrôle institutionnel des achats selon leur impact environnemental                            | **NON ÉTABLI**                                        |

---

### Conclusion du chapitre 5

Le chapitre 5 permet d'écarter deux conclusions opposées.

La première serait d'affirmer :

> **« Ces infrastructures n'ont aucun lien entre elles. »**

Cette affirmation est contredite par les sources.

Des raccords existent entre facturation, données transactionnelles, identité numérique, Business Wallets, Digital Product Passport, données de durabilité, fiscalité et paiement.

Certains raccords sont inscrits dans les textes ou standards.

D'autres font partie de stratégies européennes explicitement consacrées à l'interopérabilité.

D'autres ont déjà été matérialisés dans des expérimentations.

La seconde conclusion excessive serait d'affirmer :

> **« Un système européen utilise déjà toutes ces infrastructures pour surveiller l'empreinte environnementale individuelle et autoriser ou bloquer les achats. »**

Les sources étudiées ne permettent pas de soutenir cette affirmation.

Le résultat documentaire se situe entre ces deux positions.

**AVÉRÉ :**

> L'Union européenne développe plusieurs infrastructures numériques interopérables capables de relier identité, entreprises, transactions, produits, données fiscales et, selon les systèmes concernés, informations environnementales.

**AVÉRÉ :**

> La Commission européenne recherche explicitement des synergies et la réutilisation de données entre plusieurs de ces infrastructures.

**AVÉRÉ / EXPÉRIMENTÉ :**

> Des chaînes reliant identité, paiement, justificatif détaillé, wallet d'entreprise et traitement fiscal ont déjà été expérimentées.

**AVÉRÉ :**

> Un standard européen prévoit qu'un justificatif électronique puisse être relié au Digital Product Passport et aux informations environnementales vérifiées du produit.

**AVÉRÉ / EXPÉRIMENTÉ :**

> Des architectures de paiement conditionnel permettent qu'un événement ou une information vérifiée par un système externe intervienne dans l'exécution d'une transaction.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Ces composants permettent de construire une architecture dans laquelle une donnée environnementale relative à un produit pourrait être interrogée par un service externe et son résultat utilisé dans une logique conditionnelle entourant un paiement.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre que cette utilisation environnementale du paiement conditionnel soit actuellement prévue, expérimentée ou déployée.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre l'existence d'un système centralisé attribuant à chaque individu un profil environnemental exhaustif de consommation utilisé pour contrôler ses paiements.

La conclusion du chapitre n'est donc pas que le scénario étudié existe.

Elle est plus précise :

> **une part importante de l'architecture qui rendrait techniquement possible l'interconnexion de données transactionnelles, produit, environnementales, identitaires et de paiement est désormais documentée ; plusieurs raccords sont explicitement prévus ou expérimentés ; mais le raccord décisif transformant une donnée environnementale en règle imposée d'autorisation ou de refus d'un paiement n'a pas été établi.**

Cette distinction entre **infrastructure existante**, **interopérabilité documentée**, **capacité technique** et **usage effectivement démontré** constitue le principal résultat du chapitre 5.