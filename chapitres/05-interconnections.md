# Chapter 5 — Interconnections

> **Navigation:** [← Back to the table of contents](#documentation)

This chapter examines existing, planned or experimented interconnections between the infrastructures studied in the previous chapters.

The simultaneous existence of several digital infrastructures does not demonstrate their interconnection.

The analysis therefore looks for elements enabling concrete links between these infrastructures to be identified:

- common standards and identifiers;  
- APIs and interoperability mechanisms;  
- pilot projects and experiments;  
- common consortia and actors;  
- partnerships;  
- public procurement contracts and calls for tenders;  
- explicit references to other infrastructures in technical documentation.

The presence of the same actor in several projects is documented as such but does not, by itself, constitute proof of data exchange between these infrastructures.

An interconnection is classified as **ESTABLISHED** only when a source makes it possible to establish the actual or explicitly planned existence of the connection examined.

---

## Table of contents

- [5.1 — Mapping of already established connections](#51-mapping-of-already-established-connections)  
- [5.2 — European Business Wallets: identity, invoicing and transaction data](#52-european-business-wallets-identity-invoicing-and-transaction-data)  
- [5.3 — Business Wallets, Digital Product Passport and European infrastructures](#53-business-wallets-digital-product-passport-and-european-infrastructures)  
- [5.4 — Common identifiers, standards and APIs](#54-common-identifiers-standards-and-apis)  
- [5.5 — Common actors, consortia and experiments](#55-common-actors-consortia-and-experiments)  
- [5.6 — Documented interconnection chains](#56-documented-interconnection-chains)  
- [5.7 — The environmental data → payment connection](#57-the-environmental-data--payment-connection)  
- [5.8 — Limits of the demonstration](#58-limits-of-the-demonstration)  
- [5.9 — What this chapter establishes](#59-what-this-chapter-establishes)

---

## 5.1 Mapping of already established connections

**Status: ESTABLISHED / TECHNICALLY DEDUCIBLE / TO BE ESTABLISHED**

The first four chapters separately examined several digital infrastructures relating to economic transactions, products, the environment, identity and payments.

Before looking for new interconnections, it is necessary to distinguish connections that are already established from those that remain only technically possible or still need to be demonstrated.

---

### Electronic invoicing → tax administration

**ESTABLISHED:**

> The French electronic invoicing reform organizes the automated transmission to the tax administration of structured data relating to invoices, transactions and, in certain situations, payments [S1][S2][S3][S4].

For certain B2B transactions, the data transmitted reaches invoice-line level and notably includes the description of the good or service, the quantity and the unit price excluding VAT.

The first connection is therefore directly established:

```
invoice / transaction
   ↓
approved platform
   ↓
tax administration
```

---

### Tax data → economic analysis and public policy management

**ESTABLISHED:**

> The official objectives of the reform include, beyond combating fraud and pre-filling VAT returns, improving real-time knowledge of economic activity and the management of public policies [S5][S6][S14].

The preparatory work also mentions the use of collected data to enrich certain analytical models.

The following connection is therefore also documented:

```
structured economic data
   ↓
processing and analysis
   ↓
knowledge of economic activity / public policy management
```

This does not make it possible to infer that all possible uses of these data would be authorized.

---

### Product → Digital Product Passport

**ESTABLISHED:**

> The European Digital Product Passport framework makes it possible to associate a product, model or batch with a structured set of digital information through unique identifiers [S15][S20].

This information may, depending on the product category and the applicable regulation, include various technical and environmental characteristics.

The following connection is therefore established:

```
identifiable product
   ↓
unique identifier
   ↓
Digital Product Passport
   ↓
structured data relating to the product
```

---

### Product → environmental data

**ESTABLISHED:**

> Certain European regulations already allow or require quantitative environmental information, notably relating to carbon footprint, to be associated with certain categories of products [S15][S18][S19].

The Batteries Regulation constitutes a concrete example of this association.

The connection:

```
identifiable product
   ↓
quantitative environmental data
```

is therefore established for the product categories to which the corresponding obligations apply.

It must not be generalized to all products placed on the market.

---

### DPP → registry, APIs and external systems

**ESTABLISHED:**

> The Digital Product Passport architecture provides for a European registry, structured identifiers, interoperability mechanisms and interfaces enabling automated data exchange [S15][S20].

The DPP registry is now operational and the Commission indicates that it notably relies on documented APIs and a semantic repository intended to facilitate interoperability between systems.

The architecture therefore does not merely constitute a set of digital records intended to be consulted manually.

It is designed to enable structured exchanges between information systems.

---

### Commercial transactions → DPP / traceability

**ESTABLISHED:**

> European projects have already brought together evidence of commercial transactions, administrative actors responsible notably for VAT and customs, and traceability mechanisms intended to use the Digital Product Passport [S21].

The e-Origin project notably makes it possible to store and share evidence of commercial transactions and have it recognized by customs authorities.

Its evolution within the EBSI-ELSA project provides for the development of traceability capabilities using the Digital Product Passport.

This establishes the existence of an institutional connection between several areas previously examined separately:

```
commercial transaction
   ↓
digital evidence of transaction
   ↓
traceability infrastructure
   ↓
administrative / customs actors
```

in parallel:

> development of traceability capabilities using the DPP

**NOT ESTABLISHED:**

> This project does not demonstrate that DPP data are transmitted to the French tax administration together with electronic invoicing data.

---

### External system → payment condition

**ESTABLISHED:**

> The envisaged architecture for the digital euro provides for a conditionality layer developed by market actors and capable of using the verification of an event originating from an external system [S27][S28].

The ECB explicitly indicates that this architecture enables external monitoring capable of triggering the conditions used in a conditional payment.

The following generic connection is therefore established:

```
external system
   ↓
information or event
   ↓
verification of a condition
   ↓
conditionality layer
   ↓
transaction processing
```

---

### External platform → digital euro environment

**ESTABLISHED:**

> Market actors have connected their own platforms through APIs to an environment simulating the digital euro interfaces in order to experiment with conditional payments [S28].

The scenarios examined notably include payment on delivery, pay-per-use or milestone payments, as well as certain machine-to-machine interactions.

The connection between an external platform and the conditional logic surrounding a payment therefore no longer constitutes merely a theoretical possibility.

It has already been the subject of technical experiments.

---

### Digital identity → payment

**ESTABLISHED:**

> The European Digital Identity Wallet can contribute to payment authentication and enable the presentation of verifiable attestations or attributes [S29].

The wallet notably makes it possible to selectively present certain attributes without necessarily communicating the user's entire identity.

The following connection is therefore established:

```
verifiable identity / attribute
   ↓
EUDI Wallet
   ↓
bank / PSP / acquirer / merchant
   ↓
payment process
```

---

### EUDI Wallet → digital euro

**ESTABLISHED:**

> The European Central Bank provides for providers participating in the digital euro pilot to be able to use the EUDI Wallet as a strong authentication method for certain online transactions [S29].

The following chain is therefore explicitly provided for:

```
EUDI Wallet
   ↓
strong authentication
   ↓
PSP
   ↓
digital euro payment
```

---

### Transaction → product → environmental data

The previous chapters also identified a technically possible connection that requires certain conditions.

An invoice or transaction may contain an identifier enabling the product concerned to be determined.

The Digital Product Passport may also use a product identifier such as a GTIN or equivalent identifier [S15][S17].

**TECHNICALLY DEDUCIBLE:**

> When a common identifier or matching mechanism exists and the necessary access rights are in place, a commercial transaction can technically be matched with the environmental data associated with the corresponding product.

The chain then becomes:

```
transaction
   ↓
identifiable product
   ↓
identifier or matching mechanism
   ↓
DPP or other environmental source
   ↓
environmental data
```

**NOT ESTABLISHED:**

> The sources examined do not demonstrate that the French tax administration currently performs this matching.

---

### External data → automated decision concerning a payment

The work relating to conditional payments also establishes that an external system does not necessarily need to transfer all its data to the payment system.

It can itself verify a condition and then communicate only the result necessary for the conditional service.

**TECHNICALLY DEDUCIBLE:**

> Information originating from an external infrastructure can therefore contribute to an automated decision concerning a transaction without the source data necessarily being integrated into the monetary infrastructure.

This principle is important for the investigation of interconnections.

The absence of a central database bringing together all the information is not sufficient to demonstrate the absence of a connection between several infrastructures.

---

### State of the chain after the first four chapters

The established connections can now be represented in simplified form:

```
**Electronic invoicing**
   ↓
structured economic data
   ↓
tax administration / economic analysis

**Identifiable product**
   ↓
Digital Product Passport
   ↓
structured data / environmental data

**Digital identity**
   ↓
EUDI Wallet
   ↓
payment authentication

**External system**
   ↓
verification of a condition
   ↓
conditional payment service

**Market actor platform**
   ↓
API
   ↓
experimental digital euro environment
```

These connections do not yet, by themselves, form a single chain.

---

### Connections that remain to be investigated

After the first four chapters, several questions therefore become much more precise.

**TO BE ESTABLISHED:**

> Is there an infrastructure explicitly intended to connect invoicing or transaction data with the other European digital infrastructures examined?

**TO BE ESTABLISHED:**

> Is there a documented connection between the Digital Product Passport and a digital identity or wallet infrastructure used by businesses?

**TO BE ESTABLISHED:**

> Are electronic invoicing and DPP infrastructures explicitly envisaged as components of the same interoperable ecosystem?

**TO BE ESTABLISHED:**

> Do identifiers, attestations, APIs or intermediary services enable information to be transported or verified between these different systems?

**TO BE ESTABLISHED:**

> Are actors or consortia simultaneously involved in the development of product, invoicing, identity and payment infrastructures?

**TO BE ESTABLISHED:**

> Is there a concrete connection enabling environmental data relating to a product to reach, directly or indirectly, the conditionality layer of a payment service?

---

### Interim conclusion

**ESTABLISHED:**

> Several connections between the infrastructures examined are already explicitly documented: invoicing to tax administration, product to DPP, DPP to interoperable systems, digital identity to payment, EUDI Wallet to the digital euro pilot, and external system to conditional payment.

**ESTABLISHED:**

> External platforms have already interacted through APIs with an environment simulating the digital euro in order to experiment with conditional services.

**TECHNICALLY DEDUCIBLE:**

> When an identifier or matching mechanism exists, a transaction involving an identifiable product can technically be matched with the corresponding environmental information.

**NOT ESTABLISHED:**

> None of the elements examined so far demonstrate an operational chain directly connecting French electronic invoicing data, the Digital Product Passport or environmental data to the decision to authorize or refuse a payment.

The chapter must now investigate the intermediary infrastructures capable of connecting these different systems.

The first of these appears in the European Commission's recent work: the **European Business Wallet**.

---

## 5.2 European Business Wallets: identity, invoicing and transaction data

**Status: ESTABLISHED / ONGOING PROJECT / TO BE ESTABLISHED**

In November 2025, the European Commission proposed the creation of **European Business Wallets**, a digital infrastructure intended for economic operators and public bodies [S30].

Unlike the EUDI Wallet examined in Chapter 4, which is primarily oriented toward the digital identity of natural persons, the Business Wallet is designed to enable businesses and other economic operators to interact digitally with other businesses and public administrations.

It therefore constitutes a new intermediary infrastructure between several areas examined separately in the previous chapters.

---

### An identification and data exchange infrastructure for businesses

**ESTABLISHED:**

> European Business Wallets are intended to enable economic operators to identify and authenticate themselves and securely exchange verifiable electronic data, documents and attestations with other economic actors and public administrations [S30].

The system therefore does not merely constitute a wallet intended to store documents.

It is also intended to provide an interoperable digital exchange layer between organizations.

The general chain can be represented as follows:

```
business
   ↓
European Business Wallet
   ↓
identification / authentication / verifiable attestations
   ↓
recipient business or administration
```

---

### Business Wallet → EUDI Wallet

The Business Wallet is built on the European digital identity framework.

The proposal notably provides for European Digital Identity Wallets and electronic attestations of attributes to be used for onboarding and access management for European Business Wallets [S30].

**ESTABLISHED:**

> An explicit connection is therefore provided for between the EUDI infrastructure examined in Chapter 4 and European Business Wallets [S30].

The chain becomes:

```
EUDI Wallet / electronic attestation
   ↓
authentication and access management
   ↓
European Business Wallet
```

This relationship is particularly important since Chapter 4 has already separately established a connection between the EUDI Wallet and payment infrastructures.

It does not, however, demonstrate that data contained in a Business Wallet are automatically transmitted to a payment system.

---

### Tax and economic identifiers can be used as attributes

The proposal mentions several attributes that can be issued or verified through Business Wallets [S30].

Examples notably include:

- VAT identification number;  
- tax identification number;  
- Legal Entity Identifier (LEI);  
- EORI number used in the customs field;  
- excise number.

**ESTABLISHED:**

> The Business Wallet is therefore explicitly designed to handle attributes enabling a business to be legally, fiscally or economically identified [S30].

This creates an infrastructure capable of circulating verifiable evidence concerning the same entity across several administrative and economic contexts.

---

### Business Wallet → ViDA → electronic invoicing

The proposal establishes a particularly important connection with **VAT in the Digital Age (ViDA)** [S30].

ViDA modernizes the European VAT system and notably provides for the development of electronic invoicing and digital reporting.

The Commission indicates that European Business Wallets could enable the secure storage and verifiable exchange of VAT-related attestations and **transaction data**, in order to support real-time reporting and trusted invoicing [S30].

**ESTABLISHED:**

> The Commission therefore explicitly provides for a connection between European Business Wallets, transaction data, VAT, digital reporting and electronic invoicing [S30].

The following chain is no longer merely deducible:

```
business
   ↓
European Business Wallet
   ↓
VAT attestations / transaction data
   ↓
ViDA
   ↓
digital reporting / electronic invoicing
```

This is an institutional connection explicitly described in the Commission's proposal.

---

### The Business Wallet is not limited to interactions with public administrations

The infrastructure must be usable in relationships between businesses as well as in interactions between businesses and public administrations [S30].

**ESTABLISHED:**

> The same trusted environment is therefore designed to enable B2B and B2G exchanges.

This characteristic is important for the study of interconnections.

A verifiable attestation or data item can be used in several economic relationships without requiring the creation of a different infrastructure for each administration or business partner.

This does not, however, mean that data communicated in one context automatically become accessible in all others.

Access rights and purposes remain decisive.

---

### The Business Wallet constitutes an intermediary layer

The infrastructures examined so far could appear to belong to separate domains:

- identity  
- taxation  
- invoicing  
- customs  
- products  
- public administrations  
- commercial transactions

The Business Wallet proposal specifically adopts a cross-cutting approach.

It provides a common infrastructure for identification, attestations and secure exchange, enabling different systems to communicate with the same economic operator [S30].

**ESTABLISHED:**

> The European Union is therefore explicitly developing an infrastructure intended to facilitate interoperability between several previously distinct administrative and economic systems [S30].

---

### An important connection with our previous mapping

After Chapter 4, the following chain was already documented:

```
EUDI Wallet
   ↓
authentication
   ↓
payment infrastructures
```

The Business Wallet now adds another officially planned branch:

```
EUDI Wallet / European identity
   ↓
European Business Wallet
   ↓
business identity / verifiable attributes
   ↓
VAT / transaction data / invoicing / reporting
```

**ESTABLISHED:**

> The European identity infrastructure therefore now constitutes a documented common point between, on the one hand, mechanisms for identifying economic operators and invoicing and, on the other hand, the payment infrastructures examined in the previous chapter.

This finding is not sufficient to demonstrate a direct exchange of data between invoicing and payment.

It does, however, establish that these domains no longer necessarily rely on completely independent infrastructures.

---

### An interconnection does not necessarily require a common central database

The envisaged operation relies on attestations, identifiers and verifiable exchanges between actors.

A business can therefore prove information to another system without a single central database necessarily bringing together all the information concerned.

This principle is consistent with several architectures examined previously:

```
information held by one system
   ↓
attestation or verifiable proof
   ↓
presentation to another system
   ↓
verification
   ↓
use of the result
```

**TECHNICALLY DEDUCIBLE:**

> Interoperability between several infrastructures can therefore rely on the exchange of attestations and verifiable proofs rather than on the centralization of all data in a common database.

---

### What this connection does not demonstrate

The existence of European Business Wallets does not make it possible to claim that:

- French electronic invoicing data will automatically be copied into a Business Wallet;  
- all transaction data will be accessible to all public administrations;  
- information held in a Business Wallet will automatically be transmitted to a bank or the Eurosystem;  
- environmental data will be used as a payment condition;  
- the EUDI Wallet alone will make it possible to nominally link all economic transactions of a business or person.

**NOT ESTABLISHED:**

> None of the elements examined demonstrate at this stage an automatic transmission of invoicing or transaction data contained in or verified by a Business Wallet to the conditionality layer of a digital euro payment.

---

### But the institutional separation between several infrastructures is narrowing

The result of this section is nevertheless important.

Before examining European Business Wallets, the infrastructures relating to identity, invoicing, tax data and payments could still be represented as several systems with essentially separate connections.

The Commission's proposal introduces a cross-cutting infrastructure specifically intended to enable the identification of operators and the secure exchange of data and attestations between several of these environments.

**ESTABLISHED:**

> European Business Wallet ↔ EUDI Wallet [S30]

**ESTABLISHED:**

> European Business Wallet ↔ business identity and tax attributes [S30]

**ESTABLISHED:**

> European Business Wallet ↔ ViDA [S30]

**ESTABLISHED:**

> European Business Wallet ↔ VAT attestations [S30]

**ESTABLISHED:**

> European Business Wallet ↔ transaction data [S30]

**ESTABLISHED:**

> European Business Wallet ↔ digital reporting / trusted invoicing [S30]

These connections are explicitly described in the Commission's documents.

---

### Interim conclusion

**ESTABLISHED:**

> European Business Wallets are designed as a cross-cutting infrastructure enabling businesses and public administrations to identify and authenticate themselves and exchange verifiable data and attestations [S30].

**ESTABLISHED:**

> Their architecture is explicitly connected to the EUDI framework and enables the use of verifiable tax and economic attributes [S30].

**ESTABLISHED:**

> The Commission explicitly provides for their connection with ViDA as well as the storage and verifiable exchange of VAT attestations and transaction data in order to support real-time reporting and trusted invoicing [S30].

**TECHNICALLY DEDUCIBLE:**

> This infrastructure therefore provides an intermediary mechanism enabling several economic and administrative systems to verify and reuse certain information relating to the same business without requiring a common central database.

**NOT ESTABLISHED:**

> None of the elements examined yet demonstrate that data originating from this infrastructure are used to condition a digital euro payment.

Another connection must now be examined.

The Commission also explicitly associates European Business Wallets with the **Digital Product Passport**.

---

## 5.3 Business Wallets, Digital Product Passport and European infrastructures

**Status: ESTABLISHED / ONGOING PROJECT / TECHNICALLY DEDUCIBLE / TO BE ESTABLISHED**

The analysis of European Business Wallets reveals an additional connection with the Digital Product Passport examined in Chapter 3.

This connection does not result solely from the technical compatibility of the two infrastructures.

The European Business Wallets proposal explicitly mentions the Digital Product Passport among the systems with which synergies are sought [S30].

The European Single Market Strategy goes further by presenting the Digital Product Passport, eInvoicing, the future European Business Wallet and several other infrastructures as components of the same coherent ecosystem of digital solutions intended to create synergies [S31].

---

### Business Wallet → Digital Product Passport

The proposed regulation on European Business Wallets explicitly describes their connection with the Digital Product Passport [S30].

The Commission notes that the DPP depends on reliable access to data relating notably to product compliance and sustainability.

It indicates that Business Wallets can notably:

- prove the legal identity of an economic operator;  
- prove the access rights granted to it;  
- enable the signing and sealing of declarations of conformity;  
- enable the secure and verifiable exchange of product-related data between different actors and Member States [S30].

**ESTABLISHED:**

> The Commission explicitly provides for a connection between European Business Wallets and the Digital Product Passport in order to enable the identification of operators, the verification of access rights and the secure and verifiable exchange of product-related data [S30].

The following chain is therefore documented:

```
economic operator
   ↓
European Business Wallet
   ↓
legal identity / access rights
   ↓
Digital Product Passport
   ↓
compliance / sustainability / product data
```

---

### The connection notably concerns sustainability data

This point is particularly important for the purpose of this investigation.

The connection between the Business Wallet and the DPP is not presented solely as a mechanism for identifying a business.

The Commission explicitly mentions access to **compliance and sustainability data** associated with the Digital Product Passport [S30].

**ESTABLISHED:**

> The Business Wallet infrastructure is therefore explicitly envisaged as a mechanism that can contribute to secure and verifiable access to sustainability data associated with products in the DPP ecosystem [S30].

This does not mean that all environmental data relating to a product are automatically transferred into the Business Wallet.

The wallet can notably act as an infrastructure enabling identity, access rights and the authenticity of exchanges to be proven.

---

### Business Wallet → DPP and Business Wallet → ViDA

The previous section separately established:

```
European Business Wallet
   ↓
ViDA
   ↓
VAT attestations / transaction data / reporting / invoicing
```

The present section now establishes:

```
European Business Wallet
   ↓
Digital Product Passport
   ↓
product / compliance / sustainability data
```

**ESTABLISHED:**

> The same European infrastructure is therefore explicitly connected, on the one hand, with transaction and invoicing data and, on the other hand, with the Digital Product Passport and its product-related data [S30].

This finding constitutes an institutional connection between two sets of systems examined separately in the previous chapters.

It does not yet demonstrate that a specific data item from an invoice is automatically matched with a specific data item from a DPP.

---

### The Commission presents these infrastructures as part of the same digital ecosystem

The Single Market Strategy adopted in May 2025 makes it possible to go beyond the mere observation that several European projects are developing in parallel [S31].

The Commission notably groups together:

- the Single Digital Gateway;  
- the Once-Only Technical System;  
- the Digital Product Passport;  
- eInvoicing;  
- the future European Business Wallet;  
- the Business Register Interconnection System;  
- the European Unique Identifier for companies;  
- as well as other initiatives intended to simplify data exchange and digital reporting [S31].

It indicates that these tools should collectively constitute a **coherent ecosystem of digital solutions** and create synergies facilitating economic activities within the European Union [S31].

**ESTABLISHED:**

> The European Commission therefore does not present the DPP, eInvoicing and the Business Wallet as necessarily isolated infrastructures: it explicitly places them within the same digital ecosystem intended to create synergies [S31].

This point changes the qualification of the analysis.

The existence of convergence between these infrastructures is no longer merely a deduction based on their technical compatibility.

**ESTABLISHED:**

> An institutional strategy of interoperability and the creation of synergies between several of these infrastructures is explicitly documented [S31].

---

### eInvoicing → data reuse

The strategy also identifies an obstacle to the full automation of economic processes: the limited reuse of data from electronic invoicing in other processes [S31].

The Commission is therefore explicitly seeking to increase this reuse.

Its documentation relating to eInvoicing indicates that electronic invoicing should enable the automation of a broader set of processes, notably including:

- VAT reporting;  
- certain customs procedures;  
- environmental, social and governance, or ESG, reporting [S31].

**ESTABLISHED:**

> Electronic invoicing data are therefore not envisaged solely for producing, transmitting and recording an invoice: their reuse in other digital processes is explicitly part of the European strategy [S31].

---

### eInvoicing → sustainability reporting

More specifically, the Commission plans to test the reuse of data from eInvoicing for **sustainability reporting** [S31].

**ESTABLISHED / PLANNED PROJECT:**

> The European strategy provides for a pilot dedicated to the reuse of electronic invoicing data for sustainability reporting [S31].

This connection is particularly important for the mapping examined in this investigation.

Until now, the following relationship was only technically deducible:

```
transaction data
   ↓
product
   ↓
environmental data
```

The strategy now introduces an additional institutional connection:

```
eInvoicing data
   ↓
reuse
   ↓
sustainability reporting
```

This does not mean that an individual carbon footprint is calculated from invoices.

It does, however, establish that the reuse of invoicing data for sustainability-related purposes is explicitly part of the work announced by the Commission.

---

### eInvoicing → customs data

The same strategy also provides for improving customs transparency by linking eInvoicing data with customs data, in line with the development of the EU Customs Data Hub [S31].

**ESTABLISHED / PLANNED PROJECT:**

> The Commission explicitly provides for a connection between electronic invoicing data and customs data [S31].

The chain becomes:

```
eInvoicing
   ↓
structured transaction data
   ↓
connection with customs data
   ↓
EU Customs Data Hub
```

This connection is consistent with the elements examined in Chapter 3 relating to traceability infrastructures, the DPP and customs systems.

It does not, however, demonstrate that all these data are already brought together within the same system.

---

### Several previously hypothetical connections become institutionally documented

After Sections 5.2 and 5.3, the mapping can now be expanded:

```
EUDI / digital identity
   ↓
European Business Wallet
```

```
European Business Wallet
   ↓
ViDA / VAT / transaction data / invoicing
```

```
European Business Wallet
   ↓
Digital Product Passport / product / compliance / sustainability data
```

```
eInvoicing
   ↓
planned reuse for sustainability reporting
```

```
eInvoicing
   ↓
planned connection with customs data
```

```
DPP + eInvoicing + Business Wallet + other infrastructures
   ↓
coherent digital ecosystem and creation of synergies
```

**ESTABLISHED:**

> The Commission's documents therefore now establish explicit institutional links between several infrastructures examined separately in the previous chapters [S30][S31].

---

### What this changes in the investigation

At the end of Chapter 3, the connection between transaction data and environmental data was primarily based on a technical possibility:

```
identify the product in a transaction
   ↓
retrieve its DPP
   ↓
access the corresponding environmental data
```

The elements examined in this section now add three distinct facts:

**ESTABLISHED:**

> The Commission provides for a connection between the Business Wallet and the DPP for identity, access rights and the secure exchange of product data, notably compliance and sustainability data [S30].

**ESTABLISHED:**

> The same Business Wallet infrastructure is connected with ViDA, VAT attestations and transaction data [S30].

**ESTABLISHED / PLANNED PROJECT:**

> The Commission plans to directly test the reuse of eInvoicing data for sustainability reporting [S31].

The proximity between transaction data and sustainability data is therefore no longer merely the result of a theoretical combination made in this investigation.

**ESTABLISHED:**

> The European Commission is explicitly working on the reuse and interoperability of these categories of data within a common digital ecosystem [S30][S31].

---

### What this still does not demonstrate

These elements do not make it possible to claim that:

- each invoice line will automatically be matched with a DPP;  
- each purchased product will be associated with its carbon footprint in a central database;  
- an administration will calculate an individual environmental footprint from invoices;  
- sustainability data will be transmitted to banks or the Eurosystem;  
- environmental data from a DPP will be used as a condition for a payment;  
- the envisaged sustainability reporting concerns an individual environmental profile of consumers.

**NOT ESTABLISHED:**

> The specific connection between environmental data relating to a product and the conditionality layer of a payment remains to be demonstrated.

---

### An institutional chain nevertheless emerges

Without turning the preceding elements into evidence of a use that is not documented, a more precise institutional chain can now be represented:

```
eInvoicing / transaction data
   ↓
planned data reuse
   ↘ sustainability reporting
     ↘ **customs data / EU Customs Data Hub
```

in parallel:

```
     European Business Wallet
   ↙                         ↘
ViDA / transaction     DPP / product / sustainability
```

all of which is placed by the Commission within:

**a coherent ecosystem of digital solutions intended to create synergies**

**ESTABLISHED:**

> The existence of a strategy for connecting and reusing data between several of these infrastructures is now explicitly documented [S30][S31].

**TECHNICALLY DEDUCIBLE:**

> An infrastructure capable of identifying the operator, verifying its access rights and exchanging product data can serve as an interoperability layer between transaction systems and systems containing sustainability information, when the applicable rules authorize such an exchange.

---

### Interim conclusion

**ESTABLISHED:**

> European Business Wallets are explicitly connected with the Digital Product Passport and can contribute to the identification of operators, the verification of access rights and the secure and verifiable exchange of product-related data, notably compliance and sustainability data [S30].

**ESTABLISHED:**

> European Business Wallets are also connected with ViDA, VAT attestations and transaction data [S30].

**ESTABLISHED:**

> The Commission places the DPP, eInvoicing, the Business Wallet and several other infrastructures within the same coherent ecosystem of digital solutions intended to create synergies [S31].

**ESTABLISHED / PLANNED PROJECT:**

> The Commission plans to test the reuse of eInvoicing data for sustainability reporting [S31].

**ESTABLISHED / PLANNED PROJECT:**

> The Commission also plans to connect eInvoicing data with customs data in relation to the EU Customs Data Hub [S31].

**TECHNICALLY DEDUCIBLE:**

> These mechanisms reduce the technical and institutional distance between data describing a transaction, data describing a product and data relating to its sustainability.

**NOT ESTABLISHED:**

> None of the elements examined yet demonstrate that environmental data originating from a DPP are transmitted to a payment infrastructure in order to authorize or refuse a transaction.

The question is therefore no longer merely whether these infrastructures can communicate.

The Commission itself documents their interoperability, their reuse and the synergies being pursued.

It remains to determine **through which identifiers, standards and APIs these connections can concretely be implemented**.

---

## 5.4 Common identifiers, standards and APIs

**Status: ESTABLISHED / TECHNICALLY DEDUCIBLE / TO BE ESTABLISHED**

The previous sections established that the European Commission is explicitly seeking synergies between several digital infrastructures relating to invoicing, businesses, products and their sustainability.

The existence of an intention to achieve interoperability is not, however, sufficient to demonstrate that data can actually be matched.

For an interconnection to work, several technical conditions generally need to be met: systems must be able to identify the objects or actors concerned, understand the data exchanged, verify access rights and have interfaces enabling automated exchanges.

The infrastructures examined already have several of these components.

---

### eInvoicing → common semantic model

**ESTABLISHED:**

> The European EN 16931 standard defines a common semantic model enabling issuing and receiving systems to automatically understand and process the information contained in an electronic invoice [S32].

The purpose of the standard is precisely to reduce differences between national formats and systems in order to enable interoperability.

The general technical chain is therefore:

```
invoicing system A
   ↓
data structured according to a common semantic model
   ↓
invoicing system B
```

The data are no longer intended solely to be read by a person.

They are structured so that they can be automatically interpreted by different systems.

---

### EN 16931 is evolving toward other data uses

European standardization work no longer concerns only the traditional exchange of an invoice between supplier and customer.

The 2026 European standardization plan provides for keeping EN 16931 aligned with ViDA and integrating requirements arising from various European policies.

The areas explicitly mentioned include:

- tax reporting;  
- sustainability reporting;  
- customs;  
- other automated processes.

**ESTABLISHED:**

> The evolution of the European invoicing standard explicitly takes into account requirements arising from tax reporting, sustainability reporting and customs procedures [S32].

This evolution is consistent with the eInvoicing data reuse projects identified in the previous section.

It does not mean that all the data required for these uses are already present in every invoice.

---

### DPP → unique and persistent product identifier

The European Ecodesign Regulation requires a Digital Product Passport to be linked to a **unique and persistent product identifier** [S15][S32].

This identifier is associated with a data carrier providing access to the passport.

**ESTABLISHED:**

> The DPP therefore relies on a mechanism enabling different systems to persistently identify the same product, model or batch according to the applicable rules [S15][S32].

The chain is:

```
product
   ↓
unique and persistent identifier
   ↓
Digital Product Passport
```

This mechanism constitutes an essential condition for any automated matching between a physical product and its digital information.

---

### DPP → open standards and interoperable data

The regulation also requires Digital Product Passport data to rely on open standards and, depending on the case, to be:

- machine-readable;  
- structured;  
- searchable;  
- transferable;  
- accessible through an open and interoperable data exchange network [S15][S32].

**ESTABLISHED:**

> DPP interoperability is therefore a regulatory requirement of its architecture and not merely an optional feature [S15][S32].

The system is designed to enable the automated use of data by different authorized actors.

---

### The DPP registry has an API

Implementing Regulation (EU) 2026/1778 specifies the architecture of the European Digital Product Passport registry [S20][S32].

The registry notably includes:

- a secure user interface;  
- an API enabling the registration of Digital Product Passports and the receipt of information from the registry;  
- a verification platform;  
- a user identification and authorization mechanism;  
- a system generating unique registration identifiers;  
- a semantic repository;  
- a logging system [S20][S32].

**ESTABLISHED:**

> The DPP registry therefore has a machine-to-machine interface explicitly designed to enable automated interactions with other systems [S20][S32].

The following chain is directly provided for:

```
authorized external system
   ↓
API
   ↓
DPP registry
   ↓
registration / verification / information
```

---

### The semantic repository facilitates understanding between systems

The DPP registry also includes a semantic repository intended to authoritatively define the meaning, structure, versions and interoperability requirements of passport data [S20][S32].

**ESTABLISHED:**

> The system therefore does not merely provide a technical interface for transmitting data; it also provides a semantic layer enabling systems to consistently understand the information exchanged [S20][S32].

Two conditions necessary for automated interconnection are thus met:

```
common technical interface
   +
common semantic understanding
```

---

### The registry associates a product with a verified economic operator

The implementing regulation also requires the verification of economic operators and other value-chain actors interacting with the registry [S20][S32].

When a DPP is registered, the registry can notably associate:

- the unique product identifier;  
- the identity of the verified economic operator responsible;  
- certain information necessary for registration;  
- a unique registration identifier [S20][S32].

Electronic proof of registration can also be generated.

**ESTABLISHED:**

> The DPP registry therefore establishes a verifiable relationship between an identifiable product and an identifiable economic operator [S20][S32].

The chain becomes:

```
verified economic operator
   ↓
identifiable product
   ↓
DPP
   ↓
registration identifier / verifiable proof
```

---

### Digital identity mechanisms can contribute to operator verification

The implementing regulation provides for several mechanisms enabling the identity of economic operators to be verified.

These notably include, depending on the circumstances, electronic identification means compliant with the eIDAS framework as well as electronic attestations of attributes [S20][S32].

**ESTABLISHED:**

> The DPP infrastructure and the European digital identity infrastructure therefore share mechanisms enabling the identification or verification of economic operators [S20][S32].

This does not yet necessarily constitute a direct connection with the EUDI Wallet in every situation.

But the use of the same European identity and attestation framework facilitates interoperability between these environments.

---

### Business Wallet → verifiable attestations

European Business Wallets also rely on verifiable electronic data and attestations [S30][S32].

These attestations can represent various attributes relating to the business, its representatives, its roles or its authorizations.

The architecture notably provides for:

- structured attribute formats;  
- verification mechanisms;  
- management of mandates and delegations;  
- access controls;  
- traceability of authorizations;  
- cryptographically verifiable proofs [S30][S32].

**ESTABLISHED:**

> Exchanges between infrastructures therefore do not rely solely on the transmission of raw data but can also rely on the presentation and verification of digital attestations [S30][S32].

---

### Business Wallet → interoperable access control

The proposal provides for mechanisms enabling real-time determination of whether an actor has the necessary rights to access data or perform a procedure [S30][S32].

Authorizations must notably be:

- verifiable;  
- auditable;  
- revocable;  
- traceable to their issuer;  
- usable interoperably across Member States.

**ESTABLISHED:**

> The interoperability being pursued therefore also concerns the rights enabling access to data and services, and not only data formats [S30][S32].

This point is essential for the analysis of interconnections.

A system may technically have an API providing access to data while preventing that access when the actor does not have the corresponding authorization.

---

### Business Wallet → European Digital Directory → API

The European Business Wallets proposal also provides for the creation of a **European Digital Directory** [S30][S32].

This directory is intended to include two interfaces:

- a portal intended for users;  
- a machine-readable interface exposed through an API for automated communications between systems.

**ESTABLISHED:**

> The Business Wallet ecosystem therefore also provides for a machine-to-machine interface enabling automated discovery and interaction between actors and systems [S30][S32].

The general structure becomes:

```
actor / system
   ↓
European Digital Directory
   ↓
API
   ↓
identification / discovery / interaction with the relevant actor
```

---

### The same technical principles appear across several infrastructures

The systems examined do not necessarily rely on the same databases or on a single universal identifier.

They nevertheless use converging technical principles:

| Infrastructure  | Identification                      | Structured data                   | Semantics                   | API / automated exchange | Authorization        |
| ----------------| ------------------------------------|-----------------------------------| ----------------------------| -------------------------|----------------------|
| eInvoicing      | businesses / transaction references | yes                               | EN 16931                    | electronic exchanges     | depending on systems |
| DPP             | product / operator                  | yes                               | semantic repository         | registry API             | yes                  |
| Business Wallet | business / roles / mandates         | yes                               | attestations / vocabularies | API / interfaces         | yes                  |
| EUDI            | person / attributes                 | yes                               | verifiable attestations     | exchange protocols       | yes                  |
| digital euro    | users / PSPs / transactions         | yes                               | data model                  | payment interfaces       | yes                  |

**ESTABLISHED:**

> Several European infrastructures therefore simultaneously use structured identifiers, automatically interpretable data models, authorization mechanisms and interfaces intended for machine-to-machine exchanges [S20][S25][S29][S30][S32].

---

### The European Union explicitly seeks interoperability between these systems

This technical convergence is not merely accidental.

More broadly, the Commission indicates that it seeks to ensure cross-border interoperability between public digital solutions such as:

- eInvoicing;  
- electronic signatures;  
- electronic submissions;  
- the Digital Product Passport.

At the same time, it presents the European Business Wallet as a central element enabling businesses to interact digitally with public administrations.

**ESTABLISHED:**

> The European strategy explicitly seeks interoperability between several categories of systems examined in this investigation [S30][S31][S32].

---

### Semantic convergence is also underway for Business Wallets

Technical work relating to European Business Wallets now includes the development of a semantic vocabulary for electronic attestations used across the different use cases.

This work notably relies on verifiable credential standards and formats intended to enable attribute interoperability.

**ESTABLISHED / ONGOING WORK:**

> The development of the Business Wallet ecosystem therefore also includes a layer intended to harmonize the meaning of data and attributes exchanged between systems.

This development brings its operation closer to the principle already observed in EN 16931 and in the DPP semantic repository.

---

### Is there a universal identifier automatically connecting all infrastructures?

At this stage, the sources examined do not establish the existence of a single universal identifier that would simultaneously be present in:

```
invoice
   +
DPP
   +
Business Wallet
   +
identity
   +
payment
```

**NOT ESTABLISHED:**

> No universal identifier enabling all the infrastructures examined to be automatically joined has been identified.

This absence is important.

It prevents any claim that complete matching would be automatic or systematic.

---

### A universal identifier is not, however, technically essential

An interconnection between systems does not necessarily require all of them to use exactly the same identifier.

Matching mechanisms can link multiple identifiers.

For example:

```
business identifier in system A
   ↓
identity or verifiable attestation
   ↓
matching with the business in system B
```

or:

```
product reference in a transaction
   ↓
matching mechanism
   ↓
unique DPP identifier
   ↓
product-related information
```

**TECHNICALLY DEDUCIBLE:**

> Attestations, registries or intermediary services can make it possible to resolve matches between multiple systems without requiring a universal identifier common to the entire architecture.

This is precisely one of the functions that identity infrastructures, registries or interoperability services can perform.

---

### A single common API is no more necessary

The same distinction applies to interfaces.

It is not necessary for a single API to directly connect:

> invoicing → DPP → Business Wallet → payment

A distributed architecture can operate as follows:

```
system A
   ↓ API
intermediary service
   ↓ API
system B
   ↓ verifiable result
system C
```

This logic is already observed in the architectures examined previously.

**TECHNICALLY DEDUCIBLE:**

> The absence of a single API directly connecting all the infrastructures does not, by itself, make it possible to conclude that there is no interconnection.

---

### The question of access rights remains decisive

The technical possibility of matching multiple data points does not mean that such matching is legally or operationally authorized.

The DPP, EUDI and Business Wallet architectures specifically include mechanisms intended to control access rights and the information that may be communicated.

**ESTABLISHED:**

> Technical interoperability and authorization to access data are two distinct questions [S20][S29][S30][S32].

A chain may therefore be technically feasible while remaining legally prohibited or inaccessible to certain actors.

---

### What this section now makes it possible to establish

After the previous sections, it was established that the Commission was seeking synergies between several infrastructures.

This section shows that the main technical components enabling such synergies to be implemented also exist:

```
**identifiers**
   ↓
identify actors, products and transactions
**semantic models**
   ↓
automatically understand the data
**verifiable attestations**
   ↓
prove information without necessarily transferring all the source data
**authorization mechanisms**
   ↓
determine who can access what
**APIs and machine-to-machine interfaces**
   ↓
enable automated exchanges
**registries and directories**
   ↓
find and verify actors, products or services
```

**ESTABLISHED:**

> These components exist in several of the infrastructures examined and are explicitly being developed with interoperability in mind [S20][S30][S32].

---

### Interim conclusion

**ESTABLISHED:**

> eInvoicing relies on a common European semantic model intended to enable the automated and interoperable processing of invoices [S32].

**ESTABLISHED:**

> The DPP relies on unique persistent identifiers, structured and interoperable data, an API, a semantic repository, and identification and authorization mechanisms [S15][S20][S32].

**ESTABLISHED:**

> European Business Wallets rely on verifiable attestations, interoperable authorization mechanisms and interfaces intended for automated communications between systems [S30][S32].

**ESTABLISHED:**

> European standardization policies explicitly seek to align eInvoicing with requirements relating notably to tax reporting, sustainability reporting and customs [S32].

**TECHNICALLY DEDUCIBLE:**

> The components necessary to build automated bridges between several infrastructures therefore exist: identification, matching resolution, common semantics, access control, verifiable attestations and APIs.

**NOT ESTABLISHED:**

> No universal identifier or single API automatically connecting invoicing, the DPP, identity and payment is established by the sources examined.

The search for an interconnection therefore cannot be limited to looking for a single database, identifier or API.

A distributed architecture can connect multiple systems through intermediary services, attestations, identifier matching and successive interfaces.

The next step is therefore to determine whether **the same actors, consortia and pilot projects are actually involved in several of these infrastructures**.

---

## 5.5 Common actors, consortia and experiments

**Status: ESTABLISHED / INDICATION OF INTERCONNECTION / TO BE ESTABLISHED**

The presence of common actors across several infrastructures does not, by itself, demonstrate that data circulate between those infrastructures.

It is nevertheless a relevant element when these actors are concretely involved in the design, integration or experimentation of several systems examined in this investigation.

The analysis of European projects relating to the digital euro, digital identity and Business Wallets shows that this work is not conducted solely by public institutions independently of one another.

It also involves banks, payment service providers, technology companies, economic operators, wallet providers and integrators operating across several ecosystems [S33].

---

### Digital Euro Innovation Platform → private actors

In 2025, the European Central Bank created an innovation platform bringing together around 70 market participants to experiment with features and use cases relating to the digital euro [S28][S33].

The participants notably include:

- banks;  
- payment service providers;  
- fintechs;  
- technology companies;  
- commerce actors;  
- providers of digital infrastructures and services.

**ESTABLISHED:**

> The design and experimentation of services that could be developed around the digital euro therefore directly involve private actors from several economic sectors [S28][S33].

These actors are therefore not limited to observing the project.

As part of the "pioneers" workstream, they were able to connect their own platforms to the simulated environment provided by the ECB in order to experiment with various functionalities [S28].

---

### Several major financial and technology actors are participating in digital euro experimentation

The list published by the ECB notably includes:

- Accenture;  
- CaixaBank;  
- equensWorldline;  
- KPMG;  
- SAP Fioneer;  
- Tata Consultancy Services;  
- Infineon;  
- several European banks and payment service providers [S33].

A consortium called **Digi-Trade** is also participating in both workstreams of the Innovation Platform.

It brings together:

- Amazon;  
- CargoX;  
- Deutsche Bank;  
- Stripe;  
- Swift [S33].

**ESTABLISHED:**

> Major actors in e-commerce, banking, payments, financial messaging and technology infrastructures are therefore jointly participating in the experimentation of services relying on the digital euro environment [S33].

This participation does not demonstrate that their existing commercial infrastructures will automatically be connected to the digital euro.

It does, however, establish that they have direct access to the experimental work enabling the assessment and development of future services around this infrastructure.

---

### WE BUILD → a cross-sector consortium

The **WE BUILD** Large Scale Pilot constitutes another important element [S33].

This European project brings together more than 200 organizations from several dozen countries.

It notably includes:

- public authorities;  
- business registries;  
- tax administrations;  
- banks and financial institutions;  
- wallet and trust service providers;  
- technology companies;  
- SMEs;  
- research organizations [S33].

**ESTABLISHED:**

> The same European consortium therefore brings together public, tax, financial, technological and economic actors to develop and test interoperable infrastructures relying on the EUDI Wallet and European Business Wallets [S33].

---

### WE BUILD does not deal solely with identity

Official documentation relating to the Large Scale Pilots presents WE BUILD as a project dedicated to use cases relating to businesses **and payments** [S33].

Its architecture divides the work into several domains.

These notably include:

**Business**  
business identity / representation / data sharing

**Supply Chain**  
processes relating to supply chains and electronic invoicing

**Payments & Banking**  
secure payments / banking services / financial onboarding [S33]

**ESTABLISHED:**

> Use cases relating to electronic invoicing and use cases relating to payments and banking services are therefore being developed within the same European Large Scale Pilot and the same general interoperability architecture [S33].

This finding does not demonstrate that an invoice is used as a condition for a payment.

It does, however, establish that both domains are being experimented with within the same technical program.

---

### Business Wallet → supply chain → eInvoicing

The WE BUILD architecture blueprint explicitly mentions electronic invoicing among the processes covered in the Supply Chain domain [S33].

The same project is also developing mechanisms relating to:

- business identity;  
- mandates and representation;  
- data sharing;  
- relationships between buyers and suppliers;  
- payments and banking services.

**ESTABLISHED:**

> Electronic invoicing, business identity, data sharing and payments are therefore no longer examined solely in separate European programs: they also appear as different use cases within the same experimental environment [S33].

---

### WE BUILD → tax administrations

The consortium also includes tax administrations [S33].

The Finnish Tax Administration, for example, states that it is directly participating in WE BUILD to experiment with:

- the transmission of tax information through wallets;  
- cross-border VAT declarations;  
- the issuance and receipt of digital tax documents;  
- various processes requiring tax attestations.

**ESTABLISHED:**

> Tax administrations are therefore directly participating in the experimentation of Business Wallets and the use of tax data and digital attestations within this environment [S33].

The experimental chain thus includes:

```
business
   ↓
Business Wallet
   ↓
tax data / attestation
   ↓
tax administration
```

---

### WE BUILD → payments

WE BUILD also includes work specifically dedicated to payments.

In 2026, the consortium created a dedicated payments community to present and discuss the technical solutions being experimented with around EUDI Wallets and Business Wallets for payments and banking services [S33].

**ESTABLISHED:**

> EUDI Wallets and Business Wallets are therefore actually being experimented with in use cases relating to payments and banking services within the consortium [S33].

The work notably covers regulatory requirements, standards, technical architectures and interactions with financial institutions and payment service providers.

---

### Some actors appear in several environments

Analysis of the participants makes it possible to identify several overlaps between the ecosystems.

**CaixaBank** participates in the ECB's Digital Euro Innovation Platform [S33].

The bank also appears in WE BUILD consortium work and events dedicated to wallets and payments.

**Worldline**, through equensWorldline, participates in the Digital Euro Innovation Platform [S33].

The group also participates in Large Scale Pilots relating to the EUDI Wallet, notably WE BUILD, in work related to payments.

These overlaps can be represented as follows:

```
Digital Euro Innovation Platform
   ↕
banking actors / PSPs / integrators
   ↕
EUDI / WE BUILD
   ↕
Business Wallet / payments / banking services
```

**ESTABLISHED:**

> Certain financial and technology actors are therefore actually involved in several European initiatives relating to digital identity, wallets and payments [S33].

---

### The same actor in two projects does not prove a data exchange

This distinction is essential.

A company may simultaneously participate in several European projects for different reasons:

- technical expertise;  
- regulatory preparation;  
- business development;  
- research;  
- standardization;  
- experimentation.

**NOT ESTABLISHED:**

> The presence of an actor in several projects does not make it possible to claim that this actor transfers data from one infrastructure to another.

For example:

```
actor A participates in project X
   +
actor A participates in project Y
```

does not automatically mean:

data from project X → actor A → project Y

To establish such a connection, it is necessary to identify a use case, an interface, a flow, an architecture or documentation actually describing this exchange.

---

### The WE BUILD case is stronger than a simple overlap of actors

WE BUILD nevertheless presents an important difference.

It is not merely a matter of observing that the same companies participate separately in several projects.

The domains examined are brought together **within the same consortium and the same integration architecture**.

The project's blueprint explicitly distinguishes:

```
Business
   +
Supply Chain
   +
Payments & Banking [S33]
```

and provides for a common architecture intended to ensure interoperability between the different use cases.

**ESTABLISHED:**

> Business identity, data sharing, supply chains, electronic invoicing and payments are therefore being tested as different components of the same ecosystem of interoperable wallets [S33].

This finding constitutes stronger evidence of interconnection than the mere presence of a common actor across several programs.

---

### A European project now explicitly connects Business Wallet and payments

The European Business Wallets examined in Section 5.2 had primarily emerged as an infrastructure for identity, attestations and data exchange for businesses.

WE BUILD shows that this infrastructure is also being experimented with in banking and payment use cases [S33].

The chain therefore becomes:

```
business identity
   ↓
European Business Wallet
   ↓
attestations / business data
   ↓
banking services / payments
```

**ESTABLISHED:**

> The functional connection between the Business Wallet and the banking or payment environment is therefore already being experimented with in a Large Scale Pilot funded by the European Union [S33].

---

### Invoicing and payment are now found within the same experimental environment

Combining only the elements explicitly documented in WE BUILD:

```
European Business Wallet
   ↓
identity / representation / data sharing
```

in parallel:

```
Supply Chain
   ↓
electronic invoicing
```

in parallel:

```
Payments & Banking
   ↓
payments / financial services
```

**ESTABLISHED:**

> Electronic invoicing and payments therefore now appear within the same European wallet experimentation program [S33].

**NOT ESTABLISHED:**

> None of the elements examined yet make it possible to claim that data originating directly from an electronic invoice are used as a criterion for authorizing or refusing a payment in WE BUILD.

---

### Work brings digital identity and payment even closer together

Experiments relating to the EUDI Wallet are not merely conceptual.

Work conducted within the Large Scale Pilots has already addressed payment authentication using the wallet.

WE BUILD is now continuing this trajectory with use cases dedicated to payments and banking services.

**ESTABLISHED:**

> Digital identity and payment infrastructures are therefore being jointly experimented with, involving banks, payment service providers, wallet providers and technology companies [S29][S33].

---

### The mapping of actors becomes cross-sectoral

The projects examined reveal several categories of actors present at different levels of the ecosystem:

```
**European institutions**
European Commission / ECB
   ↓
**national administrations**
registries / tax administrations / public authorities
   ↓
**banks and PSPs**
   ↓
**wallet and trust service providers**
   ↓
**integrators and technology companies**
   ↓
**businesses and merchants**
```

**ESTABLISHED:**

> The infrastructures examined are therefore being developed within a common institutional and industrial environment simultaneously involving public actors, tax administrations, banks, payment service providers and technology companies [S33].

This still does not demonstrate any centralization of data between all these actors.

It does, however, establish the existence of a common space for design, standardization and experimentation.

---

### What this changes in the investigation

At the beginning of Chapter 5, several infrastructures were still connected primarily through their technical characteristics.

The previous sections have progressively established:

```
DPP + eInvoicing + Business Wallet
→ same European interoperability strategy

eInvoicing
→ planned reuse for sustainability reporting

Business Wallet
→ DPP / product / sustainability data

Business Wallet
→ ViDA / transaction data

EUDI Wallet
→ payment

external system
→ conditional payment

WE BUILD
→ Business + Supply Chain + eInvoicing + Payments & Banking
```

**ESTABLISHED:**

> Several domains previously examined separately are now found within common strategies, architectures and experimental programs [S30][S31][S32][S33].

---

### What this still does not make it possible to claim

Even with these new elements, it is not established that:

- French electronic invoicing data are transmitted to payment infrastructures;  
- DPP data are transmitted to a bank;  
- a carbon footprint is used in a payment decision;  
- a tax administration can automatically order the refusal of a purchase based on environmental data;  
- participants common to the different projects organize a data exchange between these infrastructures.

**NOT ESTABLISHED:**

> The specific operational connection from environmental data to a payment condition remains to be demonstrated.

---

### Interim conclusion

**ESTABLISHED:**

> The Digital Euro Innovation Platform brings together banks, PSPs, technology companies, fintechs and commercial actors to experiment with services that could be developed around the digital euro [S28][S33].

**ESTABLISHED:**

> Certain financial and technology actors participate in several initiatives relating to digital identity, wallets and payments [S33].

**ESTABLISHED:**

> WE BUILD brings together more than 200 public and private organizations and develops use cases relating to businesses, supply chains and payments within the same program [S33].

**ESTABLISHED:**

> Electronic invoicing appears among the Supply Chain use cases, while payments and banking services have their own domain within the same project [S33].

**ESTABLISHED:**

> Tax administrations, banks, financial institutions, wallet providers and technology companies participate in the same experimental environment [S33].

**ESTABLISHED:**

> The functional connection between the Business Wallet, business identity and banking or payment services is being experimented with [S33].

**INDICATION OF INTERCONNECTION:**

> The presence of several infrastructures and categories of actors within the same program further reduces the institutional and technical separation between the domains examined, without by itself demonstrating that data actually circulate from one to another.

**NOT ESTABLISHED:**

> No operational flow directly connecting environmental data originating from a product to a condition determining the execution of a payment has yet been established.

The common actors exist.

The common programs exist.

The integration architectures exist.

Use cases relating to invoicing and payments are now found within the same experimental environment.

The next step is therefore to stop examining the components separately and reconstruct the **end-to-end interconnection chains that are actually documented**.

---

## 5.6 Documented interconnection chains

**Status: ESTABLISHED / EXPERIMENTED / TECHNICALLY DEDUCIBLE / TO BE ESTABLISHED**

The previous sections separately identified interoperable infrastructures, identifiers, APIs, wallets, common actors and experimental programs bringing together invoicing, identity and payment.

It is now possible to look not only for compatible components, but for chains in which several of these components actually intervene during the same transaction or process.

The work conducted within WE BUILD makes it possible to document several such chains.

---

### Business identity → bank account → payment → proof of transaction

In September 2026, the WE BUILD consortium presents a B2B chain using the European Business Wallet as a common trust infrastructure [S34].

The described journey follows a business from its identification through to proof of the transaction.

It notably includes:

```
business
   ↓
identity / cross-border KYC / KYB
   ↓
European Business Wallet
   ↓
bank account opening or identification
   ↓
verifiable IBAN attestation
   ↓
payment using the verified IBAN
   ↓
eReceipt
   ↓
proof of the transaction
```

**ESTABLISHED / EXPERIMENTED:**

> WE BUILD therefore documents a chain in which digital business identity, verified banking data, payment and electronic proof of transaction are involved in the same B2B journey [S34].

This connection goes beyond the mere presence of distinct use cases within the same consortium.

Here, the components are used successively within the same transactional process.

---

### EUDI Wallet → payment authentication

The PA4 use case documented by a participant in the consortium provides an additional level of detail [S34].

An employee acts on behalf of a business.

Their EUDI Wallet makes it possible to present the elements required for authentication and authorization.

The payment can be made from an account or card associated with the journey.

The transaction notably contains:

- the amount;  
- the currency;  
- the beneficiary;  
- the selected payment method.

The user confirms the transaction data and the bank processes the payment.

The experimented chain becomes:

```
authorized person
   ↓
EUDI Wallet
   ↓
strong authentication
   ↓
transaction data
   ↓
bank
   ↓
payment settlement
```

**EXPERIMENTED:**

> The connection between digital identity, authorization of the person acting on behalf of the business and payment is therefore materialized in a technical demonstration journey [S34].

---

### Payment → automatic issuance of verifiable proof

Once the payment is confirmed, the seller issues an eReceipt in the form of a verifiable credential [S34].

This proof is sent directly to the European Business Wallet of the purchasing business.

The chain becomes:

```
confirmed payment
   ↓
seller / Business Wallet
   ↓
eReceipt generation
   ↓
verifiable credential
   ↓
purchaser's European Business Wallet
```

**EXPERIMENTED:**

> An event originating directly from the payment process can therefore trigger the issuance and automated transfer of a structured transactional document to the business's wallet [S34].

The payment → structured transaction data connection is therefore no longer merely theoretical in this use case.

---

### The proof contains the economic details of the transaction

The eReceipt used in the demonstration is not merely proof indicating that an overall amount has been paid.

According to the technical documentation published by the project participant, it notably contains:

- the identity of the seller;  
- its VAT number;  
- the purchase lines;  
- the amounts excluding VAT and including VAT;  
- VAT subtotals by rate;  
- the payment reference [S34].

**EXPERIMENTED:**

> The same digital object can therefore establish a verifiable link between the payment and the detailed economic content of the transaction [S34].

The chain becomes:

```
payment
   ↓
payment reference
   ↓
verifiable eReceipt
   ↓
purchase lines + amounts + VAT + seller
```

This point is important for the investigation.

In this experimental case, the transactional layer and the details of the goods or services purchased are no longer necessarily two sets without a technical relationship.

Verifiable proof can serve as a bridge between them.

---

### Proof → accounting

The Business Wallet can also be connected to the systems used by the business.

In the PA4 demonstration, a connector transmits the eReceipts to the accounting system in order to automatically record expenses [S34].

The chain becomes:

```
payment
   ↓
verifiable eReceipt
   ↓
Business Wallet
   ↓
connector
   ↓
accounting
```

**EXPERIMENTED:**

> Data originating from the transaction can therefore be automatically reused by a system external to the wallet without manual re-entry [S34].

This mechanism confirms the role of interoperability layer attributed to wallets in the previous sections.

---

### Proof → tax administration

The experimental use case described by the participant goes even further.

The verified proofs can be communicated to a demonstration tax service.

It notably verifies:

- the signature of the proof;  
- the trust placed in its issuer;  
- its revocation status.

The system can then use the VAT information contained in the proofs to perform VAT reconciliation [S34].

The complete experimental chain becomes:

```
B2B purchase
   ↓
payment
   ↓
verifiable eReceipt
   ↓
European Business Wallet
   ↓
detailed transaction data
   ↓
accounting system
```

and:

```
verifiable eReceipt
   ↓
demonstration tax service
   ↓
verification
   ↓
VAT reconciliation
```

**EXPERIMENTED — PARTICIPANT SOURCE:**

> A WE BUILD participant therefore documents a technical demonstration connecting payment, structured proof, business wallet, accounting and tax processing from end to end [S34].

**LIMIT:**

> This demonstration does not constitute evidence that a national tax administration currently uses this chain in production.

---

### Payment and taxation can therefore belong to the same technical chain

This distinction is important compared with the previous chapters.

Until now, the investigation had separately established:

```
payment
→ payment data

invoicing / transaction
→ tax data

Business Wallet
→ attestations and business data
```

The pilot now makes it possible to represent a single experimental chain:

```
business identity
   ↓
identity / delegation of the person
   ↓
EUDI Wallet
   ↓
account or card
   ↓
payment
   ↓
verifiable eReceipt
   ↓
European Business Wallet
   ↓
transaction details / VAT
   ↓
accounting
   ↓
experimental tax processing
```

**EXPERIMENTED:**

> The technical connection payment → structured proof → tax data → tax processing has therefore been demonstrated end to end within the WE BUILD ecosystem [S34].

---

### This connection does not depend on a single central database

The journey also confirms a principle identified previously.

The information does not need to be brought together in a single central database.

The different components can successively exchange verifiable proofs or credentials.

For example:

```
bank
→ payment confirmation

seller
→ issuance of the proof

wallet
→ storage / presentation of the credential

accounting
→ use of the proof

tax service
→ verification of the proof
```

**ESTABLISHED / EXPERIMENTED:**

> An interconnection chain can therefore operate end to end through several distributed systems without requiring a central actor to hold all the data from every stage [S34].

This distributed architecture makes the analysis of interfaces and access rights particularly important, rather than focusing solely on the search for a central database.

---

### Electronic invoicing and payment: another chain examined within the same program

WE BUILD does not limit its work to eReceipts.

The program documentation also lists among its use cases:

- Business Payments;  
- eInvoicing;  
- Foreign Tax Declaration [S33][S34].

Interoperability workshops have also addressed business payments, invoicing and digital proofs within the EUDI Wallet and Business Wallet environments.

**ESTABLISHED:**

> Business payment, electronic invoicing and tax processing are therefore among the domains actually being experimented with within the same European program [S33][S34].

**NOT ESTABLISHED:**

> The elements examined do not yet make it possible to claim that the PA4 chain relating to eReceipts directly constitutes the future ViDA electronic invoicing mechanism or the French electronic invoicing mechanism.

---

### An important bridge is now closed

At the beginning of Chapter 5, several connections remained separate:

- identity        → payment  
- transaction     → taxation  
- Business Wallet → business data

The WE BUILD use case now makes it possible to bring them together experimentally:

```
identity
   ↓
payment
   ↓
structured proof of transaction
   ↓
Business Wallet
   ↓
tax data
   ↓
tax processing
```

**EXPERIMENTED:**

> There is therefore at least one European use case in which these domains are technically connected from end to end.

This does not demonstrate any purpose of controlling purchases.

It does, however, demonstrate that their technical interconnection is no longer merely an abstract possibility.

---

### The environmental connection remains

Chapter 3 separately established:

```
identifiable product
   ↓
DPP
   ↓
product data
   ↓
sustainability / environmental data
```

Sections 5.2 and 5.3 then established:

```
Business Wallet
   ↔
DPP / product / sustainability data
```

and:

```
Business Wallet
   ↔
transaction / VAT / invoicing
```

The present section now experimentally establishes:

```
payment
   ↓
proof containing purchase lines
   ↓
Business Wallet
   ↓
accounting / tax processing
```

It therefore becomes possible to place the two documented chains side by side:

```
DPP / sustainability data
   ↕
European Business Wallet
```

and:

```
payment
   ↓
eReceipt / purchase lines
   ↓
European Business Wallet
```

**TECHNICALLY DEDUCIBLE:**

> When a purchase line makes it possible to identify the corresponding product and the necessary access rights exist, the Business Wallet or an interconnected service technically has the components required to match the proof of transaction with the corresponding information contained in the DPP ecosystem.

This matching is no longer deduced solely from the theoretical compatibility of two formats.

It is now based on the documented existence of a wallet environment connected, on the one hand, to product and sustainability data and, on the other, to detailed proofs originating from a payment.

---

### The final connection to conditional payment remains distinct

Chapter 4 established another chain:

```
external system
   ↓
verification of a condition
   ↓
conditionality layer
   ↓
payment
```

The ECB's work also experimentally demonstrated that platforms operated by market actors could communicate via API with an environment simulating the digital euro [S27][S28].

We therefore now have two sets:

**Set A**

```
product / DPP / sustainability
   ↕
Business Wallet
   ↕
detailed transaction / eReceipt
   ↕
payment
```

**Set B**

```
external system
   ↓
external condition
   ↓
conditionality layer
   ↓
payment
```

**TECHNICALLY DEDUCIBLE:**

> The documented architectures therefore contain the components necessary for information originating from an external system to be verified and used in a process surrounding the execution of a payment.

**NOT ESTABLISHED:**

> None of the elements examined demonstrate, however, that environmental data from the DPP are currently used as a condition in a digital euro payment or in another payment system.

---

### The difference between "possible", "experimented" and "planned"

At this stage of the investigation, three levels must be strictly distinguished.

**EXPERIMENTED:**

> identity → payment → structured proof → Business Wallet → accounting / tax processing.

**ESTABLISHED / PLANNED:**

> Business Wallet ↔ DPP / product and sustainability data.

**ESTABLISHED / EXPERIMENTED:**

> external system → verification of a condition → conditional payment.

But:

**NOT ESTABLISHED:**

> environmental data → condition determining the execution of a payment.

This final arrow must not be artificially added to the chain as long as no source documents it.

---

### What this section changes in the demonstration

At the beginning of the investigation, it would have been possible to argue that the different systems examined had no connection with one another:

"the invoice is tax-related";

"the DPP is environmental";

"the wallet is used for identity";

"payment belongs to banks";

"the digital euro is a separate monetary infrastructure".

The sources examined now make it possible to rule out such an absolute version of this separation.

**ESTABLISHED:**

> The Commission explicitly seeks synergies between several of these infrastructures [S30][S31].

**ESTABLISHED:**

> Standards, APIs, attestations and interoperability mechanisms enable interactions between them [S20][S30][S32].

**ESTABLISHED:**

> European programs bring together identity, invoicing, taxation and payment within the same experimental environments [S33][S34].

**EXPERIMENTED:**

> An end-to-end chain connecting identity, payment, detailed proof, Business Wallet, accounting and tax processing has been demonstrated by WE BUILD participants [S34].

**NOT ESTABLISHED:**

> The use of environmental data as a payment criterion remains unproven.

---

### Interim conclusion

**ESTABLISHED / EXPERIMENTED:**

> A wallet infrastructure can participate in a chain connecting the identity of a business and its representative, an account or card, a payment and structured proof of the transaction [S34].

**EXPERIMENTED:**

> This proof can contain the purchase lines, amounts, VAT information and a payment reference, then be automatically transmitted to the European Business Wallet of the business [S34].

**EXPERIMENTED:**

> Connectors then enable the proof to be reused by an accounting system and, in the demonstration case examined, by a tax service performing VAT reconciliation [S34].

**ESTABLISHED:**

> The same Business Wallet ecosystem is also connected with the Digital Product Passport and its data relating to products and their sustainability [S30].

**ESTABLISHED / EXPERIMENTED:**

> A separate conditional payment architecture also enables a condition verified by an external system to intervene in the execution of a transaction [S27][S28].

**TECHNICALLY DEDUCIBLE:**

> The infrastructures examined therefore make it possible to construct a technical chain in which a detailed transaction can be linked to an identifiable product, the product to external data, and the result of an external verification to conditional logic surrounding a payment.

**NOT ESTABLISHED:**

> None of the documents examined demonstrate, however, that this chain is currently assembled in order to use environmental data to authorize, refuse or limit a payment.

The number of missing connections has therefore been considerably reduced.

It now remains to examine precisely **the final connection in the chain: environmental data → payment**, looking not only at whether it is technically possible, but whether a project, pilot, standard or documentation exists that experiments with it or explicitly provides for it.

---

## [S35] CEN/TS 16931-8:2024 — eReceipts, DPP identifier and environmental product information

**Organization:** European Committee for Standardization (CEN)

**Document:** CEN/TS 16931-8:2024 — Electronic invoicing — Part 8: Semantic data model of the elements of an e-receipt

**Date:** 2024

**Used in:** Chapter 5

**Established elements:** European semantic model relating to electronic receipts; description of a process in which the buyer selects a payment method, makes or initiates the payment and then receives an eReceipt generated by the seller; possibility of including, in certain environments, specific information relating to the product; explicit mention of the Digital Product Passport for the product categories concerned; use of a DPP identifier enabling the receipt to be linked to verified information relating to the product; mention among this information of the sustainability of materials as well as the social and environmental impacts associated with the materials, production, use and end of life of the product.

**Methodological precaution:** the existence of a field or mechanism enabling an eReceipt to be linked to the DPP demonstrates the standardized possibility of establishing this connection. It does not demonstrate that every eReceipt will contain a DPP identifier, that the corresponding environmental data will be systematically retrieved, or that they will be used by a payment system.

**Reference:** CEN/TS 16931-8:2024

---

## 5.7 The environmental data → payment connection

**Status: ESTABLISHED / EXPERIMENTED / TECHNICALLY DEDUCIBLE / NOT ESTABLISHED**

The previous sections have progressively reduced the number of missing connections between the infrastructures examined.

At the end of Section 5.6, two distinct chains had been established.

The first now experimentally connects payment to the economic details of the transaction:

```
payment
   ↓
eReceipt
   ↓
purchase lines
   ↓
European Business Wallet
```

The second connects information originating from an external system to the execution of a conditional payment:

```
external system
   ↓
verification of a condition
   ↓
conditionality layer
   ↓
payment
```

The question addressed in this section is therefore deliberately limited to a single arrow:

> **Is there a documented mechanism enabling environmental information relating to a product to be linked to the transaction or to the condition determining the execution of the payment?**

---

### eReceipt → Digital Product Passport

An additional element appears in European standardization work relating to electronic receipts [S35].

The CEN/TS 16931-8:2024 model describes the economic process in which the buyer selects a payment method, makes or initiates the payment, and then receives an eReceipt generated by the seller.

The same document provides that, in certain environments, specific information relating to the product may be associated with the receipt.

For product categories subject to the Digital Product Passport, the standard explicitly mentions the use of a **DPP identifier enabling the receipt to be linked to verified information relating to the product** [S35].

**ESTABLISHED:**

> A European standard relating to eReceipts therefore explicitly provides for a connection between the receipt for a transaction and the Digital Product Passport of the corresponding product [S35].

The chain becomes:

```
purchase
   ↓
payment
   ↓
eReceipt
   ↓
DPP identifier
   ↓
Digital Product Passport
```

This connection is more precise than the mere possibility of subsequently matching a commercial reference with a product identifier.

The mechanism for linking to the DPP is directly envisaged in the receipt model.

---

### The connection provides access to environmental information

The same standard explains the purpose of this relationship with the DPP.

The identifier makes it possible to link the product to verified information concerning its life cycle.

The information explicitly mentioned notably includes:

- the sustainability of material sourcing;  
- the social impacts of the materials used;  
- the environmental impacts of the materials used;  
- production;  
- use;  
- the end of life of the product [S35].

**ESTABLISHED:**

> The eReceipt → DPP identifier connection therefore does not lead solely to an administrative reference for the product: it can lead to verified information including characteristics relating to its sustainability and environmental impacts [S35].

The following chain is thus explicitly documented at the semantic model level:

```
transaction
   ↓
eReceipt
   ↓
DPP identifier
   ↓
product
   ↓
verified information
   ↓
sustainability / environmental impacts
```

---

### Payment → eReceipt → DPP → environment

This new element can be considered alongside the chain experimented with in WE BUILD.

Section 5.6 established:

```
payment
   ↓
verifiable eReceipt
   ↓
purchase lines / transaction information
```

The CEN/TS 16931-8 standard adds:

```
eReceipt
   ↓
DPP identifier
   ↓
verified product information
   ↓
environmental information
```

**ESTABLISHED / EXPERIMENTED DEPENDING ON THE LINK:**

> The documented components therefore now make it possible to construct a chain in which a payment is linked to an electronic receipt and in which an electronic receipt can itself be linked, by means of a DPP identifier, to verified environmental information relating to the product [S34][S35].

The complete chain can be represented as follows:

```
payment
   ↓
eReceipt
   ↓
identifiable product
   ↓
DPP identifier
   ↓
Digital Product Passport
   ↓
sustainability / environmental data
```

**LIMIT:**

> This representation combines two connections documented in different contexts. It does not demonstrate that the entire chain is currently used end to end within the same operational system.

---

### The transaction → environment connection is therefore no longer merely hypothetical

At the beginning of the investigation, the link between a purchase and the environmental characteristics of the product was based on a deduction:

```
transaction
   ↓
identify the product
   ↓
look up its DPP
   ↓
retrieve the environmental data
```

The standard relating to eReceipts provides an additional element.

**ESTABLISHED:**

> The European model directly provides that a DPP identifier may be associated with the receipt in order to link the purchase to verified information relating to the product [S35].

It is therefore no longer necessary to assume that matching would necessarily have to be performed after the transaction using independent databases.

The receipt itself can carry the mechanism enabling access to the product passport.

---

### Another convergence exists with electronic invoicing

This relationship must also be considered alongside the elements established in Sections 5.3 and 5.4.

The Commission provides for:

```
eInvoicing
   ↓
data reuse
   ↓
sustainability reporting
```

and standardization work relating to EN 16931 explicitly takes into account requirements arising from sustainability reporting [S31][S32].

The standard relating to eReceipts now adds:

```
eReceipt
   ↓
DPP identifier
   ↓
environmental product information
```

**ESTABLISHED:**

> Several distinct European initiatives therefore organize the connection between data describing a transaction and information relating to sustainability or the environment [S31][S32][S35].

This still does not demonstrate the establishment of an individual environmental profile.

---

### Conditional payment accepts a condition originating from an external source

At the other end of the chain, the ECB's work establishes that conditional logic does not need to be integrated into the money itself.

The system examined separates:

```
settlement infrastructure
   +
market-developed conditionality layer
```

This layer can use external monitoring to verify that a condition is satisfied [S27][S28].

Once this condition has been verified:

```
condition satisfied
   ↓
release of funds
```

or, if it is not:

```
condition not satisfied
   ↓
cancellation / expiration of the reservation
```

**ESTABLISHED / EXPERIMENTED:**

> The current design therefore enables information verified outside the settlement infrastructure to intervene in the decision to execute a conditional payment [S27][S28].

---

### The nature of the condition is not technically limited to delivery

The examples most frequently presented by the ECB concern the delivery of a product, the arrival of a train, the use of a service or the completion of a step.

These examples describe use cases.

They do not constitute a technically exhaustive list of the only information that can be verified by a conditionality layer.

Experimental work shows that service providers can develop the conditional logic and that external platforms can intervene in its verification [S27][S28].

**TECHNICALLY DEDUCIBLE:**

> A condition originating from an environmental infrastructure could technically be processed according to the same principle if a service provider developed such a service, if the corresponding data were accessible and if such use were legally authorized.

For example:

```
DPP identifier
   ↓
external service
   ↓
reading of an environmental characteristic
   ↓
evaluation of a rule
   ↓
verification result
```

The payment system would not necessarily need to receive the entire DPP.

It could technically receive only a result:

```
condition satisfied
   or
condition not satisfied
```

---

### The final technical connection can therefore be represented

By combining only the documented capabilities:

```
purchased product
   ↓
eReceipt
   ↓
DPP identifier
   ↓
Digital Product Passport
   ↓
environmental data
   ↓
external verification service
   ↓
result of a condition
   ↓
conditionality layer
   ↓
payment
```

**TECHNICALLY DEDUCIBLE:**

> No architectural obstacle identified in the sources examined requires the data verified by the external system to be delivery data rather than other data accessible to that system.

But this deduction must immediately be distinguished from evidence of actual use.

---

### The search for an environmental use case in the ECB's work

The Digital Euro Innovation Platform documents make it possible to determine whether this possibility has already been turned into an environmental use case.

The documented scenarios notably concern:

- delivery;  
- pay-per-use payments;  
- milestone payments;  
- mobility and transport;  
- e-commerce;  
- financial services;  
- certain industrial applications;  
- machine-to-machine interactions [S28].

Work relating to eReceipts also mentions an environmental benefit resulting from reduced paper use.

**NOT ESTABLISHED:**

> The Digital Euro Innovation Platform documents examined do not, however, describe a scenario in which the carbon footprint, environmental performance, DPP or other sustainability data relating to a product constitute the condition triggering or preventing a payment [S28].

This negative finding is important.

It prevents the technical possibility from being turned into a claim about a currently documented project.

---

### The digital euro cannot be used as programmable money

Another limitation must remain explicitly stated.

The proposed regulation on the digital euro excludes **programmable money** [S22].

This means that units of digital euro must not intrinsically contain restrictions determining:

- the categories of goods that can be purchased;  
- the merchants with whom they can be used;  
- the period during which they can be spent;  
- or other limitations undermining their full fungibility.

**ESTABLISHED:**

> The Eurosystem therefore does not plan to encode within the monetary units themselves a rule such as "this euro cannot purchase a product whose carbon footprint exceeds X" [S22][S27].

---

### Conditional payment and programmable money nevertheless remain two different mechanisms

The exclusion of programmable money does not eliminate conditional payments.

The European proposal separately defines a conditional payment transaction as a transaction executed automatically when predetermined conditions agreed between the payer and the payee are fulfilled [S22].

The ECB also provides for payment service providers to develop the conditionality layer [S27][S28].

The distinction is therefore:

```
**PROGRAMMABLE MONEY**
rule embedded in the monetary unit
→ excluded

versus:

**CONDITIONAL PAYMENT**
rule applied to the transaction process
→ provided for / experimented
```

**ESTABLISHED:**

> The prohibition of programmable money therefore does not constitute a general prohibition of all automated logic surrounding the execution of a payment [S22][S27][S28].

---

### The conditions are presented as agreed between the parties

This limitation is also essential.

In the legislative proposal, the conditions of a conditional payment are defined as predetermined conditions **agreed between the payer and the payee** [S22].

The additional services examined by the ECB are also presented as services developed by market actors and used voluntarily by users.

**ESTABLISHED:**

> The documents examined therefore do not grant the ECB or the Eurosystem a general power to unilaterally impose an environmental condition on users' purchases.

**NOT ESTABLISHED:**

> No mechanism has been identified that would enable an administration to directly transform individual environmental data into a payment prohibition imposed on the payer.

---

### The technical chain and the legal chain must be kept separate

The result of the analysis can therefore be represented in two different ways.

**TECHNICAL CAPABILITY:**

```
transaction
   ↓
eReceipt
   ↓
DPP identifier
   ↓
environmental data
   ↓
external service
   ↓
condition
   ↓
conditional payment
```

**TECHNICALLY DEDUCIBLE:**

> The components required to construct this chain exist separately, and the interfaces necessary for several of its connections are documented.

But:

**ESTABLISHED USE:**

```
environmental data
   ↓
imposed environmental condition
   ↓
authorization / refusal of payment
```

**NOT ESTABLISHED:**

> No institutional project, regulation, pilot or technical documentation examined currently demonstrates the use of environmental data relating to a product in order to authorize, refuse or limit a payment.

---

### An important difference nevertheless emerges compared with the beginning of the investigation

At the beginning of the analysis, almost the entire chain had to be reconstructed by hypothesis:

```
invoice
   ?
product
   ?
environment
   ?
identity
   ?
payment
```

At this stage, the documented connections are much more numerous:

```
invoicing / transaction
   ↓
structured data

product
   ↓
DPP
   ↓
environmental data

eReceipt
   ↓
DPP identifier

Business Wallet
   ↔
DPP / sustainability

Business Wallet
   ↔
transaction / taxation

identity
   ↓
wallet
   ↓
payment

payment
   ↓
detailed eReceipt

external system
   ↓
condition
   ↓
conditional payment
```

The point that remains unproven is therefore no longer the existence of the necessary infrastructures.

It is now much more precise:

> **the existence of a rule or use case actually using environmental data as a condition determining the execution of a payment.**

---

### The current documentary boundary

The boundary between what is established and what is not can now be precisely defined.

**ESTABLISHED:**

> A product can be linked to environmental data through the Digital Product Passport [S15][S19].

**ESTABLISHED:**

> An eReceipt can contain an identifier enabling the purchase to be linked to the DPP and its verified information relating to the product [S35].

**EXPERIMENTED:**

> A payment can be linked to an eReceipt containing the economic details of the transaction [S34].

**ESTABLISHED / EXPERIMENTED:**

> An external system can verify a condition used by a conditionality layer surrounding a payment [S27][S28].

**TECHNICALLY DEDUCIBLE:**

> Environmental data accessible through the DPP could be verified by an external service and its result used as a technical condition according to the same architecture.

**NOT ESTABLISHED:**

> The sources examined do not demonstrate that such an environmental service is currently planned or being experimented with to determine the execution of a payment.

---

### Interim conclusion

**ESTABLISHED:**

> The European standard relating to eReceipts explicitly provides that a DPP identifier can link a transaction receipt to verified product information, including information relating to its sustainability and environmental impacts [S35].

**EXPERIMENTED:**

> European work has also demonstrated a chain connecting payment, detailed eReceipt and Business Wallet [S34].

**ESTABLISHED / EXPERIMENTED:**

> The conditional payment architecture enables an external system to verify a condition whose result intervenes in the execution of the payment [S27][S28].

**TECHNICALLY DEDUCIBLE:**

> The documented components therefore technically make it possible to construct a chain payment ↔ identifiable transaction ↔ product ↔ DPP ↔ environmental data, as well as a chain external data → condition → payment.

**NOT ESTABLISHED:**

> No element identified demonstrates, however, that these two chains are currently connected so that environmental data determine the authorization, refusal or limitation of a payment.

**ESTABLISHED:**

> Under the proposed legal framework for the digital euro, the conditions of a conditional payment are presented as predetermined and agreed between the payer and the payee, while programmable money intrinsically limiting the goods or services that can be purchased is explicitly excluded [S22].

The search for the environmental data → payment connection therefore leads to a nuanced but precise result:

> **the technical chain can be reconstructed using components and connections that are now largely documented; its environmental use as a payment decision mechanism remains unestablished.**

This boundary must be preserved in the conclusion of the investigation.

The following section must now examine the **limitations of the demonstration**, in order to definitively distinguish what the architecture enables, what has been experimented with and what no source yet makes it possible to claim.

---

## 5.8 Limitations of the demonstration

**Status: ESTABLISHED LIMITATIONS / NOT ESTABLISHED**

The previous sections have made it possible to identify numerous connections between the infrastructures examined.

These connections must not, however, be interpreted beyond what the sources actually demonstrate.

This section therefore establishes the limitations of the demonstration before presenting its synthesis.

---

### Interoperability does not mean systematic data exchange

The infrastructures examined use identifiers, standards, APIs, verifiable attestations and authorization mechanisms enabling their interoperability [S20][S30][S32].

**ESTABLISHED:**

> Several of these systems are technically designed to be able to exchange or verify information originating from other systems.

But:

**NOT ESTABLISHED:**

> This interoperability does not mean that all their data are automatically pooled, transmitted or centralized.

A possibility of interconnection must therefore be distinguished from an actually activated flow.

---

### A connection between two systems does not demonstrate a complete chain

Several connections have been documented separately:

- transaction     → eReceipt  
- eReceipt        → DPP  
- DPP             → environmental data  
- identity        → payment  
- external system → condition → payment

The existence of each of these connections is not sufficient to demonstrate that they are all used simultaneously within the same process.

**NOT ESTABLISHED:**

> No operational system identified in the sources examined currently connects environmental data originating from the DPP end to end with a decision authorizing or refusing a payment.

---

### A planned standard does not mean systematic use

The standard relating to eReceipts provides for the possibility of linking a receipt to the Digital Product Passport by means of a DPP identifier [S35].

This demonstrates the existence of a standardized mechanism enabling this connection.

But:

**NOT ESTABLISHED:**

> Not all eReceipts will necessarily contain a DPP identifier, and not all products will necessarily be subject to the same digital passport requirements.

The standardized possibility of including data therefore does not demonstrate its systematic use.

---

### A pilot project does not mean a deployed system

The WE BUILD experiments and those of the Digital Euro Innovation Platform make it possible to demonstrate the feasibility of several technical chains [S28][S33][S34].

They constitute evidence of experimentation.

They do not necessarily constitute evidence of operational deployment.

**NOT ESTABLISHED:**

> The processes experimented with in these pilots must not be presented as mechanisms already generalized to all European businesses, administrations, banks or users.

This distinction is particularly important for demonstrations using simulated tax services or experimental payment environments.

---

### A legislative proposal does not mean definitively adopted law

The European Business Wallets examined in this chapter are notably based on a proposed regulation presented by the European Commission [S30].

At the date of the analysis, this proposal is still going through the European legislative procedure.

**ESTABLISHED:**

> The proposal makes it possible to establish the proposed direction, the envisaged functionalities and the intended architecture.

But:

**NOT ESTABLISHED:**

> Not all the provisions examined can be presented as already constituting the definitive applicable law in their current wording.

The final text may still evolve during the legislative procedure.

---

### Technical possibility does not mean legal authorization

An infrastructure may technically enable two systems to communicate without all actors being legally authorized to access the corresponding data.

The DPP notably provides for differentiated access rights depending on the data and product categories [S15][S20].

The EUDI and Business Wallet architectures also rely on authorization mechanisms and selective presentation of information [S29][S30].

**ESTABLISHED:**

> Technical access to an infrastructure and the right to access particular data are two different questions.

Consequently:

**TECHNICALLY DEDUCIBLE:**

> A chain may be architecturally feasible.

without this making it possible to claim:

> that a specific actor legally has the right to use it for a specific purpose.

---

### The DPP is not an individual consumption profile

The Digital Product Passport describes the product, its model, batch or item according to the applicable rules [S15].

The regulation also provides that personal data relating to customers must not be stored in the DPP without their explicit consent [S15].

**ESTABLISHED:**

> The DPP is an infrastructure relating to the product and is not, by its nature, a database intended to establish the individual profile of its purchaser.

**NOT ESTABLISHED:**

> The existence of the DPP therefore does not demonstrate the existence of a centralized European registry associating each individual with all the products they purchase.

Matching with a transaction or identity would require additional mechanisms as well as an appropriate legal basis or consent, depending on the case.

---

### Business Wallet does not mean an individual consumer wallet

European Business Wallets are intended for economic operators and professional or administrative interactions [S30].

They must be distinguished from the EUDI Wallet intended for natural persons.

**ESTABLISHED:**

> The B2B chains documented in WE BUILD do not demonstrate that an identical mechanism is automatically applied to the personal purchases of every consumer.

This distinction prevents a B2B pilot from being directly transposed to a scenario of individual consumption control.

---

### Tax data does not mean exhaustive knowledge of individual purchases

Chapter 1 showed that the data transmitted under the French electronic invoicing and e-reporting framework differ depending on the transactions.

B2C transactions do not necessarily result in the transmission to the tax administration of individualized details of every product purchased by every consumer [S1][S2][S3][S4].

**NOT ESTABLISHED:**

> The French electronic invoicing reform therefore cannot, on the basis of the sources examined, be presented as creating by itself an exhaustive nominative registry of every individual's purchases.

This limitation remains even if other infrastructures separately hold more detailed information about certain products or transactions.

---

### Available environmental data does not mean an individual carbon profile

The DPP and other European regulations enable or require, depending on the products concerned, the availability of data relating to sustainability or certain environmental impacts [S15][S18][S19].

Technical matching between a transaction and this information can also be envisaged or standardized [S31][S35].

But:

**NOT ESTABLISHED:**

> No general mechanism automatically establishing an individual carbon footprint based on all of a person's purchases has been identified in the sources examined.

Such a purpose would notably require the identification of the relevant transactions, their attribution to a person, the retrieval of the corresponding environmental data and a method enabling their aggregation.

---

### Conditional payment does not mean programmable money

Chapter 4 established a fundamental distinction [S22][S27][S28].

The digital euro must not be designed as programmable money whose units would be restricted to certain goods, merchants, locations or periods.

However, conditional payment services are provided for and being experimented with.

The distinction is:

**programmable money**  
rule embedded in the monetary unit  
→ excluded

and:

**conditional payment**  
rule applied to the process surrounding the transaction  
→ provided for / experimented

**ESTABLISHED:**

> The existence of conditional payments therefore does not make it possible to claim that the digital euro itself can be programmed to prohibit certain categories of purchases [S22][S27][S28].

---

### A technically possible condition does not mean an imposed condition

Conditional payments are presented as relying on predetermined conditions involved in the transaction process [S22][S27][S28].

Market actors can develop services using this conditionality layer.

**TECHNICALLY DEDUCIBLE:**

> Data accessible to an external system could technically be used to verify a condition if a corresponding service were developed.

But:

**NOT ESTABLISHED:**

> No general power enabling an administration to impose an environmental condition on all users' payments has been identified in the sources examined.

---

### The ECB has not documented an environmental payment condition

The Digital Euro Innovation Platform experiments include various conditional payment scenarios [S28].

The use cases examined notably concern delivery, the use of a service, contractual milestones, transport or machine-to-machine processes.

**NOT ESTABLISHED:**

> The documents examined do not present the carbon footprint, the DPP or another environmental characteristic of the product as a condition determining the execution of a payment.

This absence currently constitutes the main documentary limitation of the chain examined.

---

### A common actor does not mean data exchange

Several banks, payment service providers, technology companies and integrators participate in different European projects [S33].

These overlaps make it possible to identify a common industrial environment.

But:

**NOT ESTABLISHED:**

> The participation of the same organization in several projects does not demonstrate that it transfers data between these projects or their infrastructures.

An interconnection must be established on the basis of a flow, an interface, a use case or documentation actually describing the connection.

---

### Distributed infrastructure does not mean a central surveillance database

The chains examined can operate by means of:

- APIs;  
- verifiable attestations;  
- wallets;  
- registries;  
- intermediary services;  
- external verification mechanisms.

Information can therefore be verified without necessarily being copied in full into every system involved in the process.

**NOT ESTABLISHED:**

> The sources examined do not demonstrate the existence of a central European database simultaneously bringing together individual identity, complete purchase history, environmental data, tax data and payment data.

The possibility of distributed interconnection must therefore be distinguished from the hypothesis of complete data centralization.

---

### Stated purpose and technical capability are two different levels

The investigation documents two categories of elements that should not be confused.

On the one hand:

> **explicitly stated purposes**

For example:

- combating fraud;  
- administrative simplification;  
- tax reporting;  
- product information;  
- sustainability;  
- digital identity;  
- interoperability;  
- innovation in payments.

On the other hand:

> **technical capabilities resulting from the architecture**

For example:

- matching multiple identifiers;  
- querying a registry;  
- verifying an attestation;  
- linking a receipt to a product;  
- retrieving environmental information;  
- verifying an external condition;  
- automating certain stages of a transaction.

**TECHNICALLY DEDUCIBLE:**

> A capability may exist before a particular purpose is assigned to it.

But:

**NOT ESTABLISHED:**

> The existence of this capability does not constitute evidence that European or national institutions intend to use it for an undocumented purpose.

This distinction constitutes one of the central methodological limitations of the investigation.

---

### The boundary of the demonstration

After all the research conducted in Chapter 5, the boundary can be precisely defined.

**ESTABLISHED OR EXPERIMENTED:**

> invoicing / transaction → structured data

> product → DPP → environmental data

> eReceipt → DPP identifier → product information

> identity → wallet → payment

> payment → detailed eReceipt

> Business Wallet ↔ transaction / tax data

> Business Wallet ↔ product / sustainability ecosystem

> external system → verification of a condition → conditional payment

But:

**NOT ESTABLISHED:**

> environmental data → imposed rule → authorization / refusal of a payment

and:

**NOT ESTABLISHED:**

> all of these infrastructures → centralized system for individual consumption control

---

### Interim conclusion

The research conducted in this chapter therefore makes it possible to go much further than simply observing the parallel existence of several digital infrastructures.

Institutional, standardization and technical connections genuinely exist.

Some are already provided for by legal texts.

Others are standardized.

Still others have been experimented with in European pilots.

But several limitations remain essential:

> **interoperable** does not mean **permanently interconnected**;

> **interconnected** does not mean **centralized**;

> **technically possible** does not mean **legally authorized**;

> **experimented** does not mean **deployed**;

> **environmental data accessible** does not mean **individual carbon profile**;

> **conditional payment** does not mean **programmable money**;

> **technical capability** does not mean **political intention**.

Finally, the main documentary boundary remains unchanged:

> **the infrastructures enabling transaction, product, environmental data and a conditionality mechanism to be linked exist or can be technically connected, but none of the sources examined currently demonstrate that environmental data are used to authorize, refuse or limit a user's payment.**

---

## 5.9 What this chapter establishes

Chapter 5 aimed to determine whether the infrastructures examined previously should be considered independent systems or whether concrete interconnections between them could be documented.

The research now makes it possible to provide a more precise answer.

The systems do not form a single centralized infrastructure.

However, they are not entirely independent of one another either.

Institutional, standardization and technical connections exist between several of them. Some are provided for by legal texts, some are standardized and others have already been experimented with.

---

### A common European ecosystem is explicitly being pursued

The European Commission no longer presents some of these infrastructures solely as isolated projects.

Its Single Market Strategy notably brings together:

- the Digital Product Passport;  
- eInvoicing;  
- European Business Wallets;  
- the Single Digital Gateway;  
- the Once Only Technical System;  
- European identification and data exchange systems.

The Commission indicates that these tools should collectively form a **coherent ecosystem of digital solutions** intended to create synergies between the different systems [S30][S31].

**ESTABLISHED:**

> The existence of a European strategy aimed at interoperability and the creation of synergies between several infrastructures examined in this investigation is explicitly documented.

This institutional convergence does not, however, demonstrate that all the data from these systems are exchanged between them.

---

### Electronic invoicing → other uses of data

Electronic invoicing is not merely a mechanism for transmitting a document between seller and buyer.

In France, structured data notably feed the tax administration [S1][S2][S3][S4].

At the European level, the Commission also plans to develop the reuse of eInvoicing data for other functions [S31].

The explicitly documented directions include:

```
eInvoicing
   ↓
VAT reporting
```

but also:

```
eInvoicing
   ↓
sustainability reporting
```

and:

```
eInvoicing
   ↓
customs data / EU Customs Data Hub
```

**ESTABLISHED:**

> The reuse of electronic invoicing data beyond the sole production of the invoice is part of the documented European directions [S31].

---

### Transaction → product → environment

Chapter 3 established the existence of an infrastructure enabling a product to be associated with a Digital Product Passport containing, depending on the categories concerned, information relating to its sustainability or environmental characteristics [S15][S18][S19][S20].

Chapter 5 identified an additional connection.

The European model relating to eReceipts provides that a receipt may contain an identifier enabling the purchased product to be linked to its Digital Product Passport [S35].

The chain becomes:

```
transaction
   ↓
eReceipt
   ↓
DPP identifier
   ↓
product
   ↓
sustainability / environmental data
```

**ESTABLISHED:**

> A standardized mechanism enabling a transaction receipt to be linked to the Digital Product Passport and to verified product information is documented [S35].

**LIMIT:**

> This does not mean that all products or all receipts will systematically use this mechanism.

---

### Business Wallet → identity, transaction and product data

European Business Wallets constitute another important connection point.

The documents examined provide for their use to:

- identify and authenticate economic operators;  
- manage verifiable attestations;  
- exchange information relating to VAT and transactions;  
- support invoicing-related processes;  
- interact with the Digital Product Passport and certain data relating to products and their sustainability [S30].

The institutional chain can therefore be represented as follows:

```
business identity
   ↕
Business Wallet
   ↔ tax / transaction data
   ↔ invoicing
   ↔ DPP / product data
```

**ESTABLISHED:**

> The Business Wallet is designed as a cross-cutting infrastructure enabling several categories of business data to be presented, verified or exchanged within an interoperable environment [S30][S32].

**LIMIT:**

> The legislative proposal relating to European Business Wallets has not yet been definitively adopted in its current wording.

---

### Identity → payment

The connection between digital identity and payment is also explicitly documented.

The EUDI Wallet can be used for payment authentication and the selective presentation of certain attestations [S29].

Work relating to the digital euro also provides for its use as a possible authentication mechanism for certain transactions [S22][S29].

The chain:

```
digital identity
   ↓
EUDI Wallet
   ↓
authentication
   ↓
payment
```

is therefore:

**ESTABLISHED / EXPERIMENTED:**

> European digital identity and payment infrastructures are already the subject of common connections and experiments [S29].

---

### Payment → detailed transaction → Business Wallet

The experiments examined in WE BUILD provide an additional connection.

A B2B journey connects:

```
business identity
   ↓
authorized person
   ↓
wallet
   ↓
account or card
   ↓
payment
   ↓
verifiable eReceipt
   ↓
purchase lines / VAT / payment reference
   ↓
European Business Wallet
```

The receipt can then be reused by accounting systems and, in the demonstration examined, by a tax service for VAT reconciliation [S34].

**EXPERIMENTED:**

> A chain connecting identity, payment, detailed transaction receipt, Business Wallet and accounting or tax processing has therefore been the subject of a technical demonstration [S34].

This chain must not, however, be presented as a system already generalized or deployed by European tax administrations.

---

### External system → condition → payment

Work relating to the digital euro also establishes that a conditional payment can depend on a condition verified outside the settlement infrastructure [S22][S27][S28].

The architecture can be represented as follows:

```
external event or information
   ↓
verification service
   ↓
condition satisfied / not satisfied
   ↓
conditionality layer
   ↓
execution of the payment
```

**ESTABLISHED / EXPERIMENTED:**

> External systems can intervene in the verification of a condition used by a conditional payment service [S27][S28].

The conditional logic can be developed by market actors without being integrated into the monetary unit itself.

---

### The main documented chains

At the end of Chapter 5, the connections can be summarized as follows:

```
**INVOICING / TRANSACTION**
structured data
   ↓
taxation
   ↓
planned reuse for other reporting purposes
```

---

```
**TRANSACTION / PRODUCT**
eReceipt
   ↓
DPP identifier
   ↓
Digital Product Passport
   ↓
product / sustainability / environmental information
```

---

```
**BUSINESS**
identity
   ↓
European Business Wallet
   ↔ attestations
   ↔ transaction / VAT / invoicing
   ↔ product environment / DPP
```

---

```
**IDENTITY / PAYMENT**
EUDI Wallet
   ↓
authentication
   ↓
payment
```

---

```
**PAYMENT / RECEIPT**
payment
   ↓
verifiable eReceipt
   ↓
transaction details
   ↓
Business Wallet
   ↓
accounting / experimental tax processing
```

---

```
**CONDITIONAL PAYMENT**
external system
   ↓
verification of a condition
   ↓
conditionality layer
   ↓
payment
```

---

### The technically reconstructible chain

These connections now make it possible to reconstruct a much more complete chain than the one available at the beginning of the investigation:

```
identity
   ↓
wallet
   ↓
transaction / payment
   ↓
structured receipt
   ↓
identifiable product
   ↓
Digital Product Passport
   ↓
environmental data
```

In parallel:

```
external data
   ↓
verification service
   ↓
result of a condition
   ↓
conditional payment
```

**TECHNICALLY DEDUCIBLE:**

> The documented architectures technically enable information relating to a product to be retrieved from an external infrastructure, evaluated by a service and transformed into a result that can be used by automated logic surrounding a transaction.

This conclusion does not require the existence of a central database bringing together all the information.

The different systems can operate by means of identifiers, APIs, wallets, verifiable attestations and intermediary services [S20][S30][S32].

---

### The connection that was not found

Despite the research conducted across the different infrastructures, none of the documents examined makes it possible to add the following arrow as an established element:

```
environmental data
   ↓
environmental condition
   ↓
authorization / refusal / limitation of payment
```

**NOT ESTABLISHED:**

> No regulation, institutional project, standard or pilot identified in this investigation currently demonstrates that environmental data originating from the DPP or an equivalent infrastructure are used to determine the execution of a payment.

The conditional payment examples examined concern other events or conditions [S27][S28].

The presence of the necessary components therefore does not constitute evidence that they are assembled for this purpose.

---

### What nevertheless changes compared with the initial hypothesis

At the beginning of the investigation, a possible representation would have been:

```
invoicing
   ?
product
   ?
environment
   ?
identity
   ?
payment
```

After analysis of the official sources, the situation is different.

Several question marks can be replaced by documented connections:

```
transaction
   → eReceipt
   → DPP
   → environmental data
```

and:

```
identity
   → wallet
   → payment
```

as well as:

```
payment
   → detailed eReceipt
   → Business Wallet
```

and:

```
external system
   → condition
   → conditional payment
```

Finally, the Commission itself documents a strategy aimed at creating synergies between several digital infrastructures examined in this investigation [S30][S31].

**ESTABLISHED:**

> The hypothesis that all these infrastructures are necessarily designed and operated as completely independent systems is therefore not consistent with the documents examined as a whole.

But the opposite claim would also be excessive.

**NOT ESTABLISHED:**

> The sources do not demonstrate the existence of a single infrastructure bringing together all these data, nor of a European system for individual environmental control of payments.

---

### Summary table

| Connection examined                                                                                 | Status                                                  |
|-----------------------------------------------------------------------------------------------------|---------------------------------------------------------|
| Electronic invoicing → tax administration                                                           | **ESTABLISHED**                                         |
| Tax data → economic analysis / public policy                                                        | **ESTABLISHED**                                         |
| Product → Digital Product Passport                                                                  | **ESTABLISHED**                                         |
| DPP → sustainability / environmental data                                                           | **ESTABLISHED**                                         |
| DPP → registry / API / external systems                                                             | **ESTABLISHED**                                         |
| eReceipt → DPP identifier                                                                           | **ESTABLISHED**                                         |
| eReceipt → environmental information via DPP                                                        | **ESTABLISHED**                                         |
| eInvoicing → reuse for sustainability reporting                                                     | **PLANNED / ESTABLISHED**                               |
| eInvoicing → matching with customs data                                                             | **PLANNED / ESTABLISHED**                               |
| Business Wallet → business identity                                                                 | **ESTABLISHED IN THE PROJECT**                          |
| Business Wallet → VAT / transaction / invoicing data                                                | **ESTABLISHED IN THE PROJECT**                          |
| Business Wallet → DPP / product data                                                                | **ESTABLISHED IN THE PROJECT**                          |
| EUDI Wallet → payment authentication                                                                | **ESTABLISHED / EXPERIMENTED**                          |
| EUDI Wallet → digital euro                                                                          | **PLANNED / EXPERIMENTED**                              |
| Payment → detailed eReceipt → Business Wallet                                                       | **EXPERIMENTED**                                        |
| eReceipt → accounting / tax processing                                                              | **EXPERIMENTED**                                        |
| External system → condition → payment                                                               | **ESTABLISHED / EXPERIMENTED**                          |
| Transaction → product → environmental data                                                          | **ESTABLISHED / DEDUCIBLE DEPENDING ON ACTUAL LINKAGE** |
| Environmental data → external verification service                                                  | **TECHNICALLY DEDUCIBLE**                               |
| Environmental data → payment condition                                                              | **TECHNICALLY DEDUCIBLE**                               |
| Environmental data → actual refusal or limitation of payment                                        | **NOT ESTABLISHED**                                     |
| Generalized individual carbon profile based on purchases                                            | **NOT ESTABLISHED**                                     |
| Central database combining identity + purchases + taxation + environment + payment                  | **NOT ESTABLISHED**                                     |
| Institutional control of purchases according to their environmental impact                          | **NOT ESTABLISHED**                                     |

---

### Conclusion of Chapter 5

Chapter 5 makes it possible to rule out two opposing conclusions.

The first would be to claim:

> **"These infrastructures have no connection with one another."**

This claim is contradicted by the sources.

Connections exist between invoicing, transaction data, digital identity, Business Wallets, the Digital Product Passport, sustainability data, taxation and payment.

Some connections are provided for in legal texts or standards.

Others form part of European strategies explicitly dedicated to interoperability.

Others have already been implemented in experiments.

The second excessive conclusion would be to claim:

> **"A European system already uses all these infrastructures to monitor individual environmental footprints and authorize or block purchases."**

The sources examined do not support this claim.

The documentary findings lie between these two positions.

**ESTABLISHED:**

> The European Union is developing several interoperable digital infrastructures capable of linking identity, businesses, transactions, products, tax data and, depending on the systems concerned, environmental information.

**ESTABLISHED:**

> The European Commission explicitly seeks synergies and data reuse between several of these infrastructures.

**ESTABLISHED / EXPERIMENTED:**

> Chains connecting identity, payment, detailed receipts, Business Wallets and tax processing have already been experimented with.

**ESTABLISHED:**

> A European standard provides that an electronic receipt can be linked to the Digital Product Passport and to verified environmental information relating to the product.

**ESTABLISHED / EXPERIMENTED:**

> Conditional payment architectures enable an event or information verified by an external system to intervene in the execution of a transaction.

**TECHNICALLY DEDUCIBLE:**

> These components make it possible to construct an architecture in which environmental data relating to a product could be queried by an external service and the result used in conditional logic surrounding a payment.

**NOT ESTABLISHED:**

> None of the elements examined demonstrate that this environmental use of conditional payment is currently planned, experimented with or deployed.

**NOT ESTABLISHED:**

> None of the elements examined demonstrate the existence of a centralized system assigning each individual a comprehensive environmental consumption profile used to control their payments.

The conclusion of the chapter is therefore not that the scenario examined exists.

It is more precise:

> **a significant part of the architecture that would make it technically possible to interconnect transaction, product, environmental, identity and payment data is now documented; several connections are explicitly provided for or experimented with; but the decisive connection transforming environmental data into an imposed rule authorizing or refusing a payment has not been established.**