# Chapitre 1 — Données de facturation transmises à l'administration

> **Navigation :** [← Retour au sommaire](#documentation)

Ce premier chapitre documente les données de facturation, de transaction et de paiement transmises à l'administration dans le cadre de la réforme française de la facturation électronique.

Ce dépôt a pour objectif de documenter, à partir de sources officielles, les données collectées, transmises et traitées dans le cadre de la réforme française de la facturation électronique.

L'objectif n'est pas de présenter comme établis des usages futurs qui ne le sont pas.

La méthode consiste à documenter séparément chaque composant du dispositif, puis à étudier les possibilités techniques et juridiques de croisement ou d'évolution de ces infrastructures.

Chaque élément est classé selon quatre niveaux :

- **AVÉRÉ** : explicitement établi par une source officielle.  
- **DÉDUCTIBLE TECHNIQUEMENT** : rendu possible par l'architecture ou les données disponibles, sans usage correspondant officiellement établi.  
- **HYPOTHÈSE** : scénario potentiel nécessitant des éléments supplémentaires pour être démontré.  
- **À ÉTABLIR** : question identifiée pour laquelle les sources étudiées ne permettent pas encore de tirer une conclusion suffisamment solide.

---

## Sommaire

- [1.1 — Le principe de transmission](#11-le-principe-de-transmission-est-officiellement-établi)  
- [1.2 — Rôle du Portail Public de Facturation](#12-rôle-du-portail-public-de-facturation)  
- [1.3 — Données B2B domestiques](#13-données-de-facturation-b2b-domestique-transmises-à-ladministration)  
- [1.4 — E-reporting B2B international](#14-e-reporting-b2b-international)  
- [1.5 — Cas particulier du B2C](#15-cas-particulier-du-b2c)  
- [1.6 — Données de paiement](#16-données-de-paiement)  
- [1.7 — Architecture de transmission](#17-architecture-de-transmission)  
- [1.8 — Conclusion du premier chapitre](#18-ce-que-ce-premier-chapitre-permet-détablir)

---

# 1. Transmission des données de facturation à l'administration

## 1.1 Le principe de transmission est officiellement établi

**Statut : AVÉRÉ**

La réforme française de la facturation électronique ne consiste pas uniquement à remplacer les factures papier ou PDF par des documents électroniques.

Elle organise également la transmission de données à l'administration fiscale.

La DGFiP distingue trois mécanismes :

1. la facturation électronique entre entreprises concernées ;  
2. la transmission électronique des données de transaction ;  
3. la transmission électronique des données de paiement ou d'encaissement.

Dans le cadre de la facturation électronique, les plateformes agréées extraient de la facture les données réglementaires destinées à l'administration [S1].

Pour les opérations relevant du e-reporting, des données de transaction ou de paiement sont également transmises à l'administration [S2][S3].

---

## 1.2 Rôle du Portail Public de Facturation

**Statut : AVÉRÉ**

À la suite du recentrage du Portail Public de Facturation (PPF), celui-ci conserve notamment une fonction de concentrateur pour la transmission à l'administration fiscale des données de facturation et de transaction [S4].

L'architecture peut donc être représentée, de manière simplifiée, ainsi :

```
Entreprise
   ↓
Plateforme agréée
   ↓
Extraction / transmission des données réglementaires
   ↓
Portail Public de Facturation
   ↓
Administration fiscale
```

Le PPF n'est donc pas uniquement un annuaire permettant le routage des factures.

Il constitue également un point de concentration des données destinées à l'administration [S4].

---

## 1.3 Données de facturation B2B domestique transmises à l'administration

**Statut : AVÉRÉ**

La DGFiP publie un tableau récapitulatif des données de facture devant être transmises à l'administration pour les opérations domestiques réalisées entre deux entreprises assujetties à la TVA établies en France [S1].

Ces données sont introduites progressivement en deux étapes.

### À compter du 1er septembre 2026

| Donnée                                                 | Granularité |
|--------------------------------------------------------|-------------|
| SIREN du fournisseur                                   | Facture     |
| Pays d'établissement du fournisseur                    | Facture     |
| SIREN du client                                        | Facture     |
| Pays d'établissement du client                         | Facture     |
| Catégorie de l'opération : biens, services ou les deux | Facture     |
| Date d'émission                                        | Facture     |
| Numéro unique de facture                               | Facture     |
| Montant HT par taux de TVA                             | Facture     |
| Montant de TVA par taux                                | Facture     |
| Taux de TVA applicable                                 | Facture     |
| Montant HT total                                       | Facture     |
| Montant total de TVA                                   | Facture     |
| Devise                                                 | Facture     |

Selon l'opération, d'autres informations doivent également être transmises :

- numéro de TVA intracommunautaire du fournisseur ;  
- numéro de TVA intracommunautaire du client ;  
- identification d'un éventuel représentant fiscal ;  
- référence de la facture initiale en cas de rectification ;  
- option pour le paiement de la TVA sur les débits ;  
- motif d'exonération de TVA ;  
- autofacturation ;  
- régime particulier de TVA ;  
- autoliquidation ;  
- appartenance à un assujetti unique ;  
- date effective de livraison du bien ou de réalisation de la prestation ;  
- date de versement d'un acompte dans les situations prévues.

### À compter du 1er septembre 2027

La granularité des données transmises augmente.

Deviennent notamment obligatoires :

| Donnée                                                      | Granularité                    |
|-------------------------------------------------------------|--------------------------------|
| Dénomination précise du bien livré ou du service rendu      | Ligne de facture               |
| Quantité de biens ou services                               | Ligne de facture               |
| Prix unitaire HT                                            | Ligne de facture               |
| Rabais, remises, ristournes et réductions                   | Ligne ou document selon le cas |
| Frais et charges, par exemple frais de transport            | Ligne ou document selon le cas |
| Adresse de livraison lorsqu'elle diffère de celle du client | Ligne ou document selon le cas |
| Date de la facture rectifiée                                | Facture                        |
| Mention d'escompte                                          | Facture                        |
| Éco-participation                                           | Ligne ou document selon le cas |

À partir du 1er septembre 2027, l'administration ne reçoit donc plus uniquement des totaux comptables et fiscaux pour les factures B2B domestiques.

La transmission réglementaire comprend également des informations permettant d'identifier la nature précise du bien ou du service facturé, sa quantité et son prix unitaire hors taxe [S1].

---

## 1.4 E-reporting B2B international

**Statut : AVÉRÉ**

Les transactions réalisées avec une entreprise assujettie à la TVA non établie en France sont également concernées par une transmission de données à l'administration [S2].

À compter du 1er septembre 2026, les informations transmises comprennent notamment :

- l'identification de l'entreprise française ;  
- l'identification de l'entreprise étrangère, notamment par son numéro de TVA intracommunautaire ou un identifiant étranger lorsqu'il existe ;  
- le pays du fournisseur ;  
- le pays du client ;  
- la catégorie de l'opération ;  
- la date de facture ;  
- le numéro de facture ;  
- le montant HT par taux de TVA ;  
- le montant de TVA par taux ;  
- les taux de TVA ;  
- le montant HT total ;  
- le montant total de TVA ;  
- la devise.

Selon l'opération, d'autres données fiscales ou relatives à la transaction sont également transmises.

À compter du 1er septembre 2027, sont notamment ajoutés :

- la dénomination précise du bien ou du service ;  
- la quantité ;  
- le prix unitaire HT ;  
- les réductions de prix ;  
- les frais et charges ;  
- l'adresse de livraison dans les cas prévus ;  
- certaines informations relatives aux factures rectificatives ;  
- l'éco-participation.

La granularité ligne par ligne prévue pour certaines données en 2027 concerne donc également les opérations B2B internationales entrant dans le champ du e-reporting.

---

## 1.5 Cas particulier du B2C

**Statut : AVÉRÉ**

Le traitement des transactions réalisées avec des personnes non assujetties, notamment les particuliers, doit être distingué du B2B.

Pour ces opérations, la DGFiP prévoit actuellement une transmission agrégée par jour.

Pour chaque catégorie de transactions concernée sont notamment transmis :

- la date du jour ;  
- la base d'imposition totale HT des opérations de la journée ;  
- le montant de TVA correspondant ;  
- une ventilation par taux de TVA lorsqu'il existe plusieurs taux.

Le dispositif réglementaire documenté ne permet donc pas d'affirmer que l'administration reçoit, dans le cadre général du e-reporting B2C, le détail individuel de chaque produit acheté par chaque particulier.

Cette distinction est essentielle :

**B2B : données pouvant atteindre la ligne de facture à compter de 2027.**

**B2C : données de transaction actuellement prévues sous forme agrégée par jour [S2].**

Cette différence devra être conservée dans toute analyse ultérieure.

---

## 1.6 Données de paiement

**Statut : AVÉRÉ**

La réforme comprend également un e-reporting des paiements pour les opérations dont la TVA est exigible à l'encaissement, notamment certaines prestations de services [S3].

Les données transmises comprennent :

- la date d'encaissement effectif ;  
- le montant encaissé ;  
- la ventilation du montant par taux de TVA lorsque nécessaire.

Lorsqu'une facture électronique existe, la transmission peut être rattachée à celle-ci par son statut « encaissée ».

Les informations comprennent alors notamment :

- le numéro de facture ;  
- la date de paiement ;  
- le montant encaissé par taux de TVA.

Pour certaines opérations B2B internationales sans dépôt de facture électronique, les données de paiement sont également transmises par facture.

Pour le B2C, les données de paiement suivent la logique du e-reporting de transaction : elles sont agrégées par jour.

---

## 1.7 Architecture de transmission

**Statut : AVÉRÉ**

Les spécifications externes version 3.2 décrivent le Portail Public de Facturation comme un concentrateur [S4].

Son rôle comprend la concentration :

- des données de facturation ;  
- des données de transaction ;  
- des données de paiement ;  
- de certaines informations relatives au cycle de vie des factures.

Ces données sont ensuite transmises à l'administration fiscale.

L'architecture peut donc être représentée de manière simplifiée ainsi :

```
Entreprise
   ↓
Plateforme agréée
   ↓
Données réglementaires
   ↓
Portail Public de Facturation
   ↓
Administration fiscale
```

La facture complète et les données réglementaires transmises à l'administration ne doivent pas être confondues.

L'administration reçoit les données prévues par les textes et les spécifications applicables.

---

## 1.8 Ce que ce premier chapitre permet d'établir

**Statut : AVÉRÉ**

À ce stade, les documents officiels permettent d'établir que la réforme met en place une infrastructure nationale permettant la collecte et la transmission automatisées de données économiques structurées à l'administration fiscale.

Ces données permettent notamment d'identifier :

- les entreprises participant à une transaction ;  
- la date et le numéro de la facture ;  
- la nature générale de l'opération ;  
- les montants HT ;  
- les taux et montants de TVA ;  
- certaines informations relatives à la livraison ;  
- certaines informations relatives au paiement.

À compter du 1er septembre 2027, pour les opérations B2B concernées, cette granularité comprend également :

- la dénomination précise du bien ou du service ;  
- sa quantité ;  
- son prix unitaire HT.

Il est donc établi que l'infrastructure permet, pour les transactions B2B concernées, de transmettre à l'administration des données structurées décrivant précisément le contenu économique de certaines lignes de facture.

En revanche, les documents étudiés à ce stade ne permettent pas d'établir :

- que chaque achat effectué par un particulier est individuellement transmis à l'administration ;  
- qu'un profil de consommation individuel est constitué ;  
- que ces données sont actuellement utilisées pour calculer une empreinte carbone individuelle ;  
- qu'elles sont croisées avec des données environnementales ;  
- qu'elles sont liées à un système de paiement ou à une monnaie numérique ;  
- qu'un mécanisme de restriction individuelle des achats est prévu.

Ces questions constituent les chapitres suivants de l'analyse.