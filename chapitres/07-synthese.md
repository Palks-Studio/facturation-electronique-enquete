# Chapitre 7 — Synthèse générale

> **Navigation :** [← Retour au sommaire](#documentation)

Ce chapitre rassemble les principaux éléments établis au cours de l'enquête et met en perspective les résultats des différents chapitres.

L'objectif est de distinguer clairement :

- ce qui est **AVÉRÉ** par les sources étudiées ;  
- ce qui a été **EXPÉRIMENTÉ** dans des projets ou pilotes documentés ;  
- ce qui est **DÉDUCTIBLE TECHNIQUEMENT** à partir des architectures et raccords identifiés ;  
- ce qui demeure **NON ÉTABLI** ou **À ÉTABLIR**.

La synthèse ne cherche pas à transformer une possibilité technique en fait établi. Elle vise au contraire à déterminer jusqu'où les sources permettent de remonter la chaîne étudiée et à identifier précisément les points où la démonstration s'arrête.

---

## Sommaire

- [Chapitre 1 — Données de facturation transmises à l'administration](#chapitre-1--données-de-facturation-transmises-à-ladministration)  
- [Chapitre 2 — Conservation, accès et finalités des données](#chapitre-2--conservation-accès-et-finalités-des-données)  
- [Chapitre 3 — Données environnementales](#chapitre-3--données-environnementales)  
- [Chapitre 4 — Euro numérique et infrastructures de paiement](#chapitre-4--euro-numérique-et-infrastructures-de-paiement)  
- [Chapitre 5 — Interconnexions](#chapitre-5--interconnexions)  
- [Chapitre 6 — Garanties juridiques](#chapitre-6--garanties-juridiques)  
- [Conclusion générale](#conclusion-générale)

---

## Chapitre 1 — Données de facturation transmises à l'administration

**Statut : AVÉRÉ**

La réforme française de la facturation électronique met en place une infrastructure permettant la transmission automatisée à l'administration fiscale de données économiques structurées.

Ces données comprennent notamment l'identification des entreprises participant à une transaction, les dates et numéros de facture, les montants hors taxe, les taux et montants de TVA ainsi que certaines informations relatives aux livraisons et aux paiements.

À compter du 1er septembre 2027, pour les opérations B2B concernées, les données transmises comprennent également des informations au niveau des lignes de facture :

- la dénomination précise du bien ou du service ;  
- la quantité ;  
- le prix unitaire hors taxe.

Le dispositif permet donc, dans ces situations, de transmettre à l'administration des données structurées décrivant précisément le contenu économique d'une transaction B2B.

Pour les opérations B2C relevant du e-reporting, les données actuellement prévues sont en revanche agrégées par jour. Les éléments documentés ne permettent donc pas d'affirmer que le détail de chaque achat réalisé par un particulier est individuellement transmis à l'administration.

→ [Consulter les preuves et sources du Chapitre 1](01-donnees-facturation.md)

---

## Chapitre 2 — Conservation, accès et finalités des données

**Statut : AVÉRÉ / À ÉTABLIR**

Les textes étudiés établissent que la réforme ne se limite pas à la transmission technique des factures. Les données structurées issues des factures, des transactions et, dans les situations prévues, des paiements sont transmises à l'administration dans un cadre organisé faisant intervenir les plateformes agréées.

Les entreprises restent soumises à des obligations propres de conservation des documents fiscaux. Ces obligations ne permettent toutefois pas de déduire que l'administration conserve les données reçues pendant une durée identique.

La lutte contre la fraude à la TVA, le pré-remplissage des déclarations de TVA, la connaissance en temps réel de l'activité des entreprises et le pilotage des politiques publiques figurent parmi les objectifs officiellement annoncés de la réforme.

La documentation de la DGFiP indique également que la disponibilité et l'exploitation de données obtenues de façon automatique et continue doivent faciliter la connaissance de la conjoncture économique, notamment par secteur d'activité, ainsi que le pilotage de l'économie par la puissance publique.

Les travaux préparatoires de la réforme mentionnent en outre la possibilité d'enrichir des modèles d'analyse avec les données recueillies afin de faciliter notamment la détection et l'accompagnement des entreprises en difficulté.

Il est donc établi que les données recueillies ne répondent pas uniquement à une fonction de transmission des factures ou de détermination de la TVA : leur exploitation doit également contribuer à l'observation de l'activité économique et au pilotage des politiques publiques.

Plusieurs éléments restent cependant à établir, notamment la durée précise de conservation des différentes catégories de données par l'administration, les règles d'accès et d'habilitation, les traitements automatisés effectivement appliqués, les éventuels croisements avec d'autres bases de données et les conditions juridiques permettant leur réutilisation pour d'autres politiques publiques.

Les sources étudiées ne permettent pas d'établir l'existence d'une interconnexion avec des données environnementales, une infrastructure monétaire numérique ou des mécanismes permettant de conditionner certaines transactions. Ces possibilités doivent être étudiées séparément dans les chapitres suivants.

→ [Consulter les preuves et sources du Chapitre 2](02-conservation-acces-finalites.md)

---

## Chapitre 3 — Données environnementales

**Statut : AVÉRÉ / DÉDUCTIBLE TECHNIQUEMENT / À ÉTABLIR**

L'Union européenne a établi un cadre juridique et technique pour le passeport numérique de produit, ou Digital Product Passport (DPP), permettant d'associer des données numériques structurées, lisibles par machine et interopérables à des produits identifiables.

Selon les exigences applicables aux différentes catégories de produits, le passeport peut être défini au niveau du modèle, du lot ou de l'article individuel.

Les informations susceptibles d'être associées à certains produits comprennent notamment des données relatives à leur composition, leur durabilité, leur réparabilité, leur recyclabilité ainsi qu'à leur empreinte carbone ou environnementale.

L'Union européenne dispose également de méthodes permettant de quantifier certains impacts environnementaux des produits sur leur cycle de vie. Le règlement relatif aux batteries fournit déjà un exemple concret dans lequel une empreinte carbone quantitative est réglementairement associée à certaines catégories de produits.

Le DPP repose sur des identifiants structurés et peut notamment comporter un GTIN ou un identifiant équivalent. Les standards utilisés dans les échanges commerciaux électroniques permettent également de transporter des identifiants standardisés au niveau des articles.

Il est donc techniquement possible, lorsqu'un identifiant commun ou un mécanisme de correspondance existe et que les droits d'accès nécessaires sont réunis, de rapprocher une transaction commerciale des informations environnementales associées au produit correspondant.

La donnée environnementale n'a pas besoin d'être directement inscrite dans la facture pour qu'un tel rapprochement soit techniquement réalisable : l'identifiant du produit peut permettre de retrouver cette information dans un système distinct.

De même, l'identité de l'acheteur n'a pas besoin d'être stockée dans le DPP pour qu'un rapprochement soit techniquement possible si un autre système dispose séparément des informations permettant d'identifier la partie à la transaction et le produit concerné.

Lorsque plusieurs transactions comportent des produits identifiables auxquels sont associées des valeurs environnementales quantitatives, ces valeurs peuvent également, sur le plan technique, être rapprochées et agrégées par un système disposant des données et droits d'accès nécessaires.

L'architecture réglementaire du DPP prévoit par ailleurs des mécanismes d'interopérabilité, des échanges automatisés, une API, un registre européen et une interconnexion avec les systèmes douaniers. Des projets européens associent également traçabilité numérique, preuves de transactions commerciales et acteurs administratifs chargés notamment de la TVA et des douanes.

Ces éléments ne permettent cependant pas d'établir qu'une empreinte environnementale individuelle des achats est actuellement calculée par l'administration, que les données environnementales des produits sont automatiquement rapprochées des données françaises de facturation ou de e-reporting, ni qu'elles sont utilisées pour autoriser, refuser ou conditionner un paiement.

→ [Consulter les preuves et sources du Chapitre 3](03-donnees-environnementales.md)

---

## Chapitre 4 — Euro numérique et infrastructures de paiement

**Statut : AVÉRÉ / DÉDUCTIBLE TECHNIQUEMENT / À ÉTABLIR**

Le projet d'euro numérique repose sur une infrastructure centralisée de règlement exploitée par l'Eurosystème et distribuée aux utilisateurs par l'intermédiaire de prestataires de services de paiement.

Cette infrastructure ne repose pas sur une blockchain comme fondement du système. Les utilisateurs conserveraient principalement une relation avec leur banque ou leur prestataire de services de paiement, tandis que l'Eurosystème assurerait les fonctions centrales nécessaires au règlement et au fonctionnement de l'infrastructure.

Pour les paiements en ligne, le modèle technique publié prévoit le traitement de données structurées relatives aux utilisateurs, comptes, appareils, prestataires, payeurs, bénéficiaires et transactions.

Les transactions disposent notamment d'identifiants, d'un montant, d'une date et d'une heure, d'un type, d'un environnement et d'un statut. Le modèle comprend également différentes informations permettant l'identification ou la catégorisation des acteurs intervenant dans une transaction.

Certaines informations relatives au commerçant peuvent également intervenir dans le processus. Le Merchant Category Code, ou MCC, permet notamment de catégoriser le type d'activité commerciale du bénéficiaire et fait partie des informations transmises dans certaines étapes du processus de paiement documenté.

L'architecture distingue cependant les données présentes dans le modèle, les données effectivement transmises lors d'une transaction et les données auxquelles chaque acteur peut réellement accéder. L'existence d'une donnée dans le modèle technique ne signifie donc pas que tous les participants au système peuvent la consulter.

Le projet prévoit également un fonctionnement hors ligne permettant d'effectuer certains paiements directement entre appareils sans connexion à Internet. Dans ce mode, les détails personnels de la transaction ne sont pas transmis aux prestataires de services de paiement ni à l'Eurosystème pendant ou après le paiement. Cette architecture constitue une limitation importante aux possibilités de centralisation systématique des informations relatives aux transactions.

La proposition relative à l'euro numérique exclut explicitement la création d'une monnaie programmable au sens d'unités monétaires auxquelles seraient intrinsèquement attachées des restrictions déterminant les biens, services, lieux, personnes ou périodes pour lesquels elles pourraient être utilisées.

Cette interdiction ne signifie cependant pas l'absence de mécanismes automatisés autour des paiements.

La documentation de la Banque centrale européenne prévoit explicitement des paiements conditionnels dans lesquels l'exécution d'une transaction peut dépendre de la vérification préalable d'une condition.

L'Eurosystème peut fournir les fonctions monétaires fondamentales nécessaires à ces mécanismes, notamment la réservation des fonds, tandis que la logique permettant de déterminer si une condition est satisfaite peut être gérée par les prestataires de services de paiement ou d'autres acteurs du marché.

Les travaux techniques de la BCE indiquent également qu'un monitoring externe peut participer au déclenchement de ces conditions.

Ce mécanisme général ne constitue plus uniquement une possibilité théorique. Des acteurs du marché ont connecté leurs propres plateformes, au moyen d'API, à un environnement simulant le back-end de l'euro numérique afin d'expérimenter différents scénarios de paiements conditionnels.

Les scénarios étudiés comprennent notamment le paiement à la livraison, le paiement à l'usage, les paiements par étapes, certains remboursements automatisés et des paiements machine-to-machine.

Il est donc établi dans son principe qu'une information ou un événement provenant d'un système externe à la couche monétaire peut être vérifié par un service afin de participer à la décision d'exécuter, de libérer, de maintenir ou de restituer des fonds associés à une transaction déterminée.

L'information externe utilisée pour vérifier une condition n'a pas nécessairement besoin d'être intégralement stockée dans l'infrastructure monétaire : un système externe peut effectuer la vérification et transmettre uniquement le résultat nécessaire au processus conditionnel.

L'identité numérique européenne possède par ailleurs un raccord explicitement documenté avec les infrastructures de paiement.

L'European Digital Identity Wallet, ou EUDI Wallet, peut être utilisé dans des processus d'authentification de paiement. La BCE prévoit également son utilisation comme méthode d'authentification forte par les prestataires participant au pilote de l'euro numérique pour certaines transactions en ligne.

L'EUDI Wallet repose notamment sur des mécanismes d'attestations vérifiables, de minimisation des données et de divulgation sélective. L'existence de ce raccord ne signifie donc pas que l'ensemble des informations détenues dans le wallet soit communiqué au commerçant, au prestataire de paiement ou à l'Eurosystème.

Les éléments étudiés permettent ainsi d'établir séparément l'existence de transactions structurées et identifiables, de paiements conditionnels, d'une couche de conditionnalité pouvant utiliser des informations provenant de systèmes externes, d'interfaces permettant à des plateformes d'acteurs du marché d'interagir avec l'environnement de paiement et d'un raccord explicite entre identité numérique et paiement.

Ces éléments rendent techniquement possible la construction de services dans lesquels une information provenant d'une infrastructure externe participe à une décision automatisée concernant une transaction déterminée sans que la monnaie elle-même devienne programmable.

Ils ne permettent cependant pas d'établir qu'un passeport numérique de produit, un GTIN, une empreinte carbone, une donnée issue de la facturation électronique ou un profil environnemental individuel soit actuellement utilisé pour déclencher, empêcher ou modifier un paiement en euros numériques.

Le raccord générique entre système externe et paiement conditionnel est donc documenté. Le raccord spécifique entre données environnementales ou fiscales et exécution d'un paiement reste à établir.

→ [Consulter les preuves et sources du Chapitre 4](04-euro-numerique-paiements.md)

---

## Chapitre 5 — Interconnexions

**Statut : AVÉRÉ / EXPÉRIMENTÉ / DÉDUCTIBLE TECHNIQUEMENT / NON ÉTABLI**

Le Chapitre 5 a recherché les raccords existants, prévus, expérimentés ou techniquement possibles entre les infrastructures étudiées séparément dans les chapitres précédents.

Les recherches montrent que ces infrastructures ne constituent pas un système unique et centralisé, mais qu'elles ne sont pas non plus totalement indépendantes les unes des autres.

La Commission européenne inscrit explicitement plusieurs de ces dispositifs dans un même objectif d'interopérabilité et de création de synergies. Le Digital Product Passport, l'eInvoicing, les European Business Wallets et d'autres infrastructures européennes sont notamment présentés comme participant à un écosystème cohérent de solutions numériques.

La réutilisation des données de facturation électronique dépasse par ailleurs le seul traitement de la facture. Des travaux européens prévoient notamment leur réutilisation pour le reporting de durabilité et leur rapprochement avec certaines données douanières.

Les European Business Wallets constituent un autre point de convergence documenté. Le projet prévoit leur utilisation pour l'identification des opérateurs économiques, les attestations vérifiables, certaines informations fiscales et transactionnelles ainsi que des interactions avec le Digital Product Passport et les données relatives aux produits.

Les travaux de standardisation apportent également un raccord direct entre transaction et produit. Le modèle européen relatif aux eReceipts prévoit qu'un justificatif puisse contenir un identifiant permettant de relier le produit acheté à son Digital Product Passport et aux informations vérifiées correspondantes, comprenant notamment certaines informations relatives à sa durabilité et à ses impacts environnementaux.

La chaîne suivante dispose donc désormais de raccords documentés :

```
transaction
   ↓
eReceipt
   ↓
identifiant DPP
   ↓
Digital Product Passport
   ↓
informations produit / durabilité / environnement
```

Parallèlement, les expérimentations européennes étudiées ont permis de documenter une chaîne reliant identité d'entreprise, paiement, justificatif électronique détaillé, Business Wallet et traitement comptable ou fiscal expérimental.

```
identité / autorisation
   ↓
wallet
   ↓
paiement
   ↓
eReceipt détaillé
   ↓
Business Wallet
   ↓
comptabilité / traitement fiscal expérimental
```

Le raccord entre identité numérique et paiement est également documenté : l'EUDI Wallet peut intervenir dans l'authentification de paiements et son utilisation est prévue dans les travaux relatifs au pilote de l'euro numérique.

Enfin, les travaux de la BCE établissent qu'un système extérieur peut participer à la vérification d'une condition utilisée par un service de paiement conditionnel.

```
système externe
   ↓
vérification d'une condition
  ↓
couche de conditionnalité
   ↓
paiement
```

Ces différents éléments permettent techniquement de reconstruire une architecture dans laquelle une donnée relative à un produit pourrait être récupérée depuis une infrastructure externe, évaluée par un service et transformée en résultat utilisable par une logique automatisée entourant une transaction.

Il demeure cependant **NON ÉTABLI** qu'une donnée environnementale provenant du Digital Product Passport ou d'une infrastructure équivalente soit actuellement utilisée comme condition afin d'autoriser, refuser ou limiter un paiement.

Il demeure également **NON ÉTABLI** qu'un système centralisé réunisse identité individuelle, historique exhaustif des achats, données fiscales, données environnementales et données de paiement, ou qu'un profil carbone individuel généralisé soit calculé à partir de ces infrastructures.

Les travaux relatifs à l'euro numérique maintiennent en outre une distinction essentielle : la monnaie programmable, dont les unités comporteraient intrinsèquement des restrictions sur les biens ou services pouvant être achetés, est explicitement exclue, tandis que des services de paiement conditionnel distincts de la monnaie elle-même sont prévus et expérimentés.

Le résultat du Chapitre 5 est donc précis : **une part importante des infrastructures et des raccords permettant techniquement d'associer transaction, produit, environnement, identité et paiement est désormais documentée ; certains de ces raccords sont explicitement prévus, standardisés ou expérimentés ; mais le raccord transformant effectivement une donnée environnementale en règle imposée d'autorisation ou de refus d'un paiement n'a pas été établi.**

→ [Consulter les preuves et sources du Chapitre 5](05-interconnexions.md)

---

## Chapitre 6 — Garanties juridiques

**Statut : AVÉRÉ / GARANTIES JURIDIQUES / VULNÉRABILITÉS JURIDIQUES / ANGLES MORTS DOCUMENTAIRES**

Le Chapitre 6 a recherché si les capacités techniques et les interconnexions identifiées dans les chapitres précédents pouvaient être librement exploitées et combinées.

La réponse est négative.

L'existence d'une donnée, d'un identifiant, d'une interface ou d'une possibilité technique de rapprochement ne constitue pas en elle-même une autorisation juridique de l'utiliser pour une nouvelle finalité.

Le RGPD, le droit de l'Union européenne, le droit national et les garanties propres aux différentes infrastructures imposent notamment des exigences relatives :

- à la base juridique des traitements ;  
- à la détermination et à la compatibilité des finalités ;  
- à la nécessité et à la proportionnalité ;  
- à la minimisation des données ;  
- à la sécurité et au contrôle des accès ;  
- aux droits des personnes ;  
- au profilage et aux décisions automatisées ;  
- au contrôle par les autorités indépendantes et les juridictions.

L'enquête a néanmoins établi que ces protections ne constituent pas toutes des impossibilités techniques ou des garanties d'immuabilité.

L'exemple de CFVR est particulièrement important.

Ce traitement a vu son périmètre évoluer juridiquement à plusieurs reprises depuis sa création. En 2026, les données issues de la facturation électronique ont été intégrées parmi ses nouvelles sources, dans une architecture permettant leur exploitation algorithmique à grande échelle et leur rapprochement avec d'autres informations utilisées pour la détection d'anomalies et le ciblage du contrôle fiscal.

Cette évolution démontre concrètement qu'une infrastructure de données créée pour une fonction déterminée peut ultérieurement devenir une source juridiquement autorisée d'un autre traitement.

Elle ne démontre pas que toute interconnexion future sera autorisée.

Elle démontre que le périmètre juridique actuel des traitements ne doit pas être confondu avec une impossibilité permanente de faire évoluer leurs usages.

Le Chapitre 6 a également identifié une distinction essentielle entre centralisation physique et centralisation fonctionnelle.

Une architecture n'a pas besoin de réunir toutes les informations dans une base unique pour permettre leur rapprochement.

Des systèmes distincts peuvent échanger :

```
identifiant
   +
attribut
   +
preuve
   +
résultat
   +
condition vérifiée
```

sans nécessairement transférer l'intégralité de leurs données brutes.

Cette propriété est particulièrement importante pour l'analyse des infrastructures étudiées dans ce dossier, qui reposent largement sur des identifiants structurés, des registres, des interfaces, des attestations vérifiables et des mécanismes d'interopérabilité.

Le Chapitre 6 a également établi que certaines garanties importantes sont explicitement inscrites dans les cadres étudiés.

Le DPP prévoit notamment des restrictions concernant les données personnelles des clients.

Le portefeuille européen d'identité numérique prévoit des mécanismes de minimisation, de contrôle utilisateur et de divulgation sélective.

Le cadre actuellement proposé pour l'euro numérique exclut la monnaie programmable, c'est-à-dire une monnaie dont les unités comporteraient intrinsèquement des restrictions déterminant les biens, services, personnes, lieux ou périodes pour lesquels elles peuvent être utilisées.

Cette interdiction coexiste cependant avec la possibilité de développer des services de paiement conditionnel reposant sur des conditions vérifiées extérieurement.

La distinction est fondamentale :

```
monnaie programmable
   ≠
paiement conditionnel
```

Le premier mécanisme est exclu dans le cadre étudié.

Le second est prévu et a fait l'objet d'expérimentations.

Le Chapitre 6 n'a identifié aucun fondement permettant d'affirmer qu'une donnée environnementale relative à un produit est actuellement transformée en restriction individuelle de paiement.

Mais il confirme l'importance juridique de la frontière située entre :

```
information
   ↓
vérification
   ↓
profilage
   ↓
condition
   ↓
conséquence individuelle
```

Plus une donnée ou un résultat devient déterminant pour l'accès à un paiement, un service, un droit ou une autre possibilité importante, plus les exigences relatives à la base juridique, à la nécessité, à la proportionnalité, à l'exactitude, à la transparence, à la contestation et aux droits fondamentaux deviennent centrales.

**AVÉRÉ :**

> Les capacités techniques documentées dans les chapitres précédents sont juridiquement encadrées et ne peuvent pas être librement combinées pour n'importe quelle finalité.

**AVÉRÉ :**

> Les données issues de la facturation électronique ont rejoint en 2026 un traitement fiscal préexistant, CFVR, dont le périmètre avait déjà connu plusieurs évolutions successives.

**GARANTIE JURIDIQUE :**

> Une nouvelle capacité technique ou une nouvelle interconnexion ne constitue pas à elle seule une autorisation juridique de produire une conséquence individuelle.

**VULNÉRABILITÉ JURIDIQUE :**

> Le périmètre juridiquement autorisé d'une infrastructure peut évoluer, sous réserve du respect des normes supérieures applicables.

**VULNÉRABILITÉ JURIDIQUE :**

> Une augmentation des possibilités de rapprochement ne nécessite pas nécessairement la création d'une base centralisée réunissant physiquement toutes les données.

**ANGLE MORT DOCUMENTAIRE :**

> Les sources publiques étudiées permettent plus facilement d'évaluer chaque infrastructure et chaque extension séparément que l'effet cumulé de l'ensemble de leurs évolutions et interconnexions.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre actuellement l'existence d'un dispositif utilisant un profil environnemental individuel afin d'autoriser, refuser ou limiter les paiements, les achats, les services ou les droits d'une personne.

**NON ÉTABLI :**

> Aucun élément étudié ne démontre l'existence d'une infrastructure unique réunissant automatiquement facturation électronique, identité numérique, données environnementales, Digital Product Passport et euro numérique afin de contrôler les transactions individuelles.

→ [Consulter les preuves et sources du Chapitre 6](06-garanties-juridiques.md)

---

## Conclusion générale

Les six chapitres permettent désormais de suivre une chaîne qui n'était, au début de l'enquête, qu'une hypothèse à vérifier.

La réforme française de la facturation électronique transforme une partie importante de l'activité économique en données structurées, standardisées, transmissibles et exploitables automatiquement.

Ces données ne servent pas uniquement à transporter une facture.

Les sources étudiées établissent leur utilisation ou leur destination pour différentes finalités fiscales et économiques, notamment la lutte contre la fraude, le pré-remplissage de la TVA, la connaissance de l'activité économique et le pilotage des politiques publiques.

Depuis 2026, certaines données issues de la facturation électronique constituent également une source du traitement CFVR et de son infrastructure de traitement à grande échelle.

Parallèlement, l'Union européenne développe plusieurs autres infrastructures numériques.

Le Digital Product Passport permet d'associer à des produits identifiables des données structurées pouvant comprendre des informations relatives à leur durabilité et à leurs impacts environnementaux.

Les standards européens relatifs aux justificatifs électroniques permettent de relier une transaction et un produit à son Digital Product Passport.

Les infrastructures d'identité numérique permettent la présentation et la vérification d'attributs.

Le raccord entre identité numérique et paiement est documenté.

Des expérimentations ont relié identité, paiement, justificatif transactionnel et Business Wallet.

Enfin, les travaux relatifs à l'euro numérique ont établi qu'un système externe peut participer à la vérification d'une condition utilisée par un service de paiement conditionnel.

---

### Le pont recherché au début de l'enquête a donc bien été partiellement construit

L'enquête ne se termine pas au même point qu'elle a commencé.

Au départ, la question était de savoir si des infrastructures concernant :

```
facturation
   +
transaction
   +
produit
   +
environnement
   +
identité
   +
paiement
```

pouvaient réellement disposer de points de raccordement.

Plusieurs de ces raccords sont désormais **AVÉRÉS**, **STANDARDISÉS** ou **EXPÉRIMENTÉS**.

La chaîne documentaire obtenue peut être représentée ainsi :

```
FACTURATION / TRANSACTION
   ↓
DONNÉES STRUCTURÉES
   ↓
TRAITEMENTS ET RAPPROCHEMENTS

TRANSACTION
   ↓
eRECEIPT
   ↓
PRODUIT IDENTIFIABLE
   ↓
DIGITAL PRODUCT PASSPORT
   ↓
INFORMATIONS PRODUIT
   ↓
DURABILITÉ / ENVIRONNEMENT
```

Parallèlement :

```
IDENTITÉ / ATTRIBUTS
   ↓
WALLET
   ↓
AUTHENTIFICATION
   ↓
PAIEMENT
```

et :

```
SYSTÈME EXTERNE
   ↓
VÉRIFICATION
D'UNE CONDITION
  ↓
SERVICE DE
PAIEMENT CONDITIONNEL
   ↓
PAIEMENT
```

Une autre chaîne a en outre été expérimentée :

```
IDENTITÉ / AUTORISATION
   ↓
WALLET
   ↓
PAIEMENT
   ↓
eRECEIPT DÉTAILLÉ
   ↓
BUSINESS WALLET
   ↓
COMPTABILITÉ /
TRAITEMENT FISCAL
```

Le résultat est donc différent d'une simple juxtaposition d'infrastructures indépendantes.

> **Des ponts existent.**

Mais tous les segments ne possèdent ni le même statut ni le même niveau de preuve.

---

### Le dernier raccord déterminant n'est pas établi

L'enquête permet techniquement de reconstruire :

```
transaction
   ↓
produit identifiable
   ↓
DPP
   ↓
information environnementale
```

Elle permet également de reconstruire séparément :

```
système externe
   ↓
condition vérifiée
   ↓
paiement conditionnel
```

Elle documente encore :

```
identité numérique
   ↓
paiement
```

Mais elle n'a pas établi le raccord final :

```
IDENTITÉ
   +
HISTORIQUE DE TRANSACTIONS
   +
PRODUITS
   +
DONNÉES ENVIRONNEMENTALES
   ↓
PROFIL ENVIRONNEMENTAL
INDIVIDUEL
   ↓
CONDITION IMPOSÉE
   ↓
AUTORISATION / REFUS /
LIMITATION D'UN PAIEMENT
```

**NON ÉTABLI :**

> Aucun élément étudié ne démontre actuellement que cette chaîne complète soit déployée ou juridiquement organisée afin de contrôler les possibilités de paiement d'une personne.

Cette limite est fondamentale.

Elle empêche de présenter comme un fait ce qui demeure une possibilité construite à partir de capacités séparément documentées.

---

### Mais il serait également incorrect de conclure que le pont n'existe pas

L'absence du dernier raccord ne remet pas à zéro les résultats de l'enquête.

Les sources ont permis de passer de :

```
HYPOTHÈSE
« ces systèmes pourraient peut-être
un jour être reliés »
```

à :

```
CONSTAT
plusieurs raccords existent déjà,
sont standardisés,
prévus
ou ont été expérimentés
```

La frontière documentaire se situe désormais beaucoup plus loin dans la chaîne.

Ce qui reste **NON ÉTABLI** n'est plus la possibilité générale de relier transaction, produit, données environnementales, identité et paiement.

Ce qui reste **NON ÉTABLI** est leur utilisation combinée dans une finalité unique produisant une restriction individuelle.

Cette distinction constitue l'un des principaux résultats de l'enquête.

---

### Le Chapitre 6 apporte cependant une seconde frontière : la possibilité technique n'est pas l'autorisation juridique

Même lorsqu'un raccord est techniquement possible, il ne peut pas être librement exploité.

Les traitements demeurent soumis notamment :

```
base juridique
   +
finalité
   +
nécessité
   +
proportionnalité
   +
minimisation
   +
droits des personnes
   +
contrôle
   +
droits fondamentaux
```

Une infrastructure capable de rapprocher deux informations n'est donc pas automatiquement autorisée à le faire.

Et une infrastructure capable de produire une condition n'est pas automatiquement autorisée à utiliser cette condition pour restreindre un paiement, un service ou un droit.

Cette distinction constitue une véritable garantie.

---

### Mais le cadre juridique n'est pas immuable

L'enquête a également établi que les finalités, sources, catégories de données et destinataires d'un traitement peuvent évoluer juridiquement.

CFVR en fournit un exemple concret.

Depuis sa création, son périmètre a été modifié à plusieurs reprises.

En 2026, les données issues de la facturation électronique sont devenues une nouvelle source de ce traitement préexistant.

La frontière entre :

```
« techniquement possible
mais non utilisé »
```

et :

```
« juridiquement autorisé
et effectivement utilisé »
```

peut donc évoluer.

Cette constatation ne démontre aucune évolution future particulière.

Elle démontre que l'état juridique observé aujourd'hui ne doit pas être présenté comme une garantie d'immuabilité.

---

### La réforme de la facturation électronique doit donc être replacée dans un changement d'échelle plus large

L'enquête ne démontre pas que la facturation électronique constitue une base centrale réunissant l'ensemble des informations étudiées.

Une telle affirmation serait excessive.

Elle établit en revanche que cette réforme transforme une part importante de l'activité économique en données structurées pouvant être transmises et exploitées automatiquement.

Dans le domaine fiscal, leur intégration à CFVR fournit désormais un exemple concret de réutilisation dans une infrastructure algorithmique plus large.

La réforme constitue donc une **infrastructure structurante de données économiques**.

Son importance ne vient pas du fait qu'elle centraliserait déjà « tout ».

Elle vient du fait qu'elle rend une partie croissante de l'activité économique :

```
STRUCTURÉE
   ↓
STANDARDISÉE
   ↓
LISIBLE PAR MACHINE
   ↓
TRANSMISSIBLE
   ↓
CROISABLE
   ↓
ANALYSABLE
```

La question de ses interconnexions futures devient dès lors aussi importante que celle de ses finalités présentes.

---

### Le résultat final doit donc être formulé avec deux vérités simultanées

Première vérité :

> **l'enquête n'a pas démontré l'existence actuelle d'un système généralisé utilisant identité, achats, données environnementales et monnaie numérique pour contrôler les possibilités économiques individuelles.**

Deuxième vérité :

> **l'enquête a démontré qu'une partie importante des briques et des raccords techniques permettant de relier transaction, produit, informations environnementales, identité et paiement existe déjà, est prévue par des standards, intégrée à des architectures européennes ou a fait l'objet d'expérimentations.**

Ces deux affirmations ne sont pas contradictoires.

Elles définissent précisément le niveau de preuve atteint.

---

### Ce qui est établi

**AVÉRÉ :**

> La facturation électronique crée une infrastructure massive de données économiques structurées et exploitables automatiquement.

**AVÉRÉ :**

> Certaines données issues de cette infrastructure alimentent désormais CFVR, où elles peuvent être rapprochées d'autres informations dans le cadre de traitements algorithmiques destinés notamment à la détection d'anomalies et au ciblage fiscal.

**AVÉRÉ :**

> Des standards permettent de relier transaction, produit identifiable, Digital Product Passport et informations vérifiées relatives au produit, notamment certaines informations environnementales.

**AVÉRÉ / EXPÉRIMENTÉ :**

> L'identité numérique peut intervenir dans des processus de paiement et des expérimentations ont relié identité, paiement, justificatif électronique détaillé et Business Wallet.

**AVÉRÉ / EXPÉRIMENTÉ :**

> Un système externe peut vérifier une condition dont le résultat intervient dans un service de paiement conditionnel.

**DÉDUCTIBLE TECHNIQUEMENT :**

> Les raccords documentés permettent de construire techniquement une chaîne reliant une transaction identifiable à des informations relatives au produit et à son impact environnemental, puis de faire intervenir le résultat d'une vérification externe dans une logique conditionnelle entourant un paiement.

---

### Ce qui n'est pas établi

**NON ÉTABLI :**

> Il n'est pas démontré qu'un profil environnemental individuel généralisé soit actuellement calculé à partir des achats des citoyens.

**NON ÉTABLI :**

> Il n'est pas démontré que les informations environnementales du DPP soient actuellement utilisées comme condition pour autoriser, refuser ou limiter les paiements d'une personne.

**NON ÉTABLI :**

> Il n'est pas démontré que la facturation électronique, le DPP, l'identité numérique et l'euro numérique soient réunis dans une infrastructure unique destinée au contrôle des comportements individuels.

**NON ÉTABLI :**

> Il n'est pas démontré que l'euro numérique permettra de programmer intrinsèquement la monnaie afin d'interdire l'achat de certaines catégories de biens ; le cadre étudié exclut au contraire explicitement la monnaie programmable.

---

### La conclusion de l'enquête n'est donc ni une validation ni une accusation

Elle est une cartographie.

Elle montre :

```
ce qui existe
   +
ce qui communique
   +
ce qui a été expérimenté
   +
ce qui est techniquement possible
   +
ce que le droit autorise
   +
ce qu'il interdit ou encadre
   +
ce qui reste à démontrer
```

Le résultat essentiel est que **le pont a bien été construit sur une partie substantielle de son parcours**.

Il ne repose plus uniquement sur une succession d'hypothèses.

Plusieurs de ses piliers sont documentés par des règlements, des standards, des architectures techniques, des projets européens et des expérimentations.

Mais le dernier passage :

```
DONNÉE ENVIRONNEMENTALE
   ↓
PROFIL INDIVIDUEL
   ↓
RÈGLE IMPOSÉE
   ↓
RESTRICTION ÉCONOMIQUE
OU MONÉTAIRE
```

reste **NON ÉTABLI**.

C'est exactement là que les preuves disponibles s'arrêtent aujourd'hui.

---

### Conclusion finale

> **Cette enquête n'établit pas l'existence actuelle d'un système de contrôle environnemental des paiements ou des comportements économiques individuels.**

> **Elle établit en revanche qu'une partie substantielle de l'architecture technique qui rendrait certains rapprochements possibles existe déjà : données économiques structurées, identification des transactions et des produits, Digital Product Passport, données environnementales associées aux produits, identité numérique, infrastructures de paiement, vérification de conditions externes et paiements conditionnels.**

> **Plusieurs raccords entre ces briques sont avérés, standardisés ou expérimentés. Le pont technique n'est donc plus une hypothèse abstraite.**

> **Ce qui n'est pas établi est son activation intégrale dans une finalité unique permettant d'établir un profil environnemental individuel et d'en tirer une conséquence imposée sur un paiement, un achat, un service ou un droit.**

> **Le droit actuel oppose en outre plusieurs garanties à une telle évolution. Mais l'étude de CFVR démontre que le périmètre juridique des traitements peut évoluer dans le temps.**

> **La frontière à surveiller n'est donc plus seulement l'apparition de nouvelles bases de données. Elle se situe dans les nouveaux raccords, les nouvelles finalités, les nouveaux attributs, les nouvelles conditions et surtout les nouvelles conséquences que le droit pourrait progressivement autoriser à partir d'infrastructures déjà existantes.**

> **Le dossier s'arrête ainsi exactement à la limite des preuves disponibles : suffisamment loin pour établir que les briques et plusieurs ponts existent ; pas assez loin pour affirmer qu'elles constituent aujourd'hui le système intégré de contrôle que leur combinaison rendrait techniquement possible.**
