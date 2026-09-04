# Chapter 7 — General Summary

> **Navigation:** [← Back to table of contents](#documentation)

This chapter brings together the main elements established over the course of the investigation and puts the results of the various chapters into perspective.

The aim is to clearly distinguish:

- what is **ESTABLISHED** by the sources examined;  
- what has been **TESTED/PILOTED** in documented projects or pilots;  
- what is **TECHNICALLY DEDUCIBLE** from the identified architectures and connections;  
- what remains **NOT ESTABLISHED** or **TO BE ESTABLISHED**.

The summary does not seek to turn a technical possibility into an established fact. On the contrary, it aims to determine how far the sources allow the chain under study to be traced back, and to precisely identify the points at which the demonstration stops.

---

## Table of contents

- [Chapter 1 — Invoicing data transmitted to the administration](#chapter-1--invoicing-data-transmitted-to-the-administration)  
- [Chapter 2 — Data retention, access, and purposes](#chapter-2--data-retention-access-and-purposes)  
- [Chapter 3 — Environmental data](#chapter-3--environmental-data)  
- [Chapter 4 — Digital euro and payment infrastructures](#chapter-4--digital-euro-and-payment-infrastructures)  
- [Chapter 5 — Interconnections](#chapter-5--interconnections)  
- [Chapter 6 — Legal safeguards](#chapter-6--legal-safeguards)  
- [General conclusion](#general-conclusion)

---

## Chapter 1 — Invoicing data transmitted to the administration

**Status: ESTABLISHED**

The French electronic invoicing reform puts in place an infrastructure enabling the automated transmission of structured economic data to the tax administration.

This data notably includes the identification of the businesses party to a transaction, invoice dates and numbers, amounts excluding tax, VAT rates and amounts, as well as certain information relating to deliveries and payments.

From 1 September 2027, for the B2B transactions concerned, the data transmitted will also include information at the invoice-line level:

- the precise description of the good or service;  
- the quantity;  
- the unit price excluding tax.

In these situations, the system therefore makes it possible to transmit to the administration structured data precisely describing the economic content of a B2B transaction.

For B2C transactions falling under e-reporting, by contrast, the data currently planned is aggregated on a daily basis. The documented elements therefore do not make it possible to assert that the details of each individual purchase made by a private individual are transmitted to the administration.

→ [See the evidence and sources for Chapter 1](01-invoicing-data.md)

---

## Chapter 2 — Data retention, access, and purposes

**Status: ESTABLISHED / TO BE ESTABLISHED**

The texts examined establish that the reform is not limited to the technical transmission of invoices. Structured data from invoices, transactions, and, in the situations provided for, payments, is transmitted to the administration within an organized framework involving accredited platforms.

Businesses remain subject to their own obligations to retain tax documents. These obligations do not, however, make it possible to infer that the administration retains the data it receives for an identical period.

Combating VAT fraud, pre-filling VAT returns, real-time knowledge of business activity, and steering public policy are among the officially stated objectives of the reform.

DGFiP documentation also indicates that the availability and use of data obtained automatically and continuously is intended to facilitate understanding of economic conditions, notably by sector of activity, as well as the steering of the economy by public authorities.

The reform's preparatory work also mentions the possibility of enriching analytical models with the data collected, in particular to facilitate the detection of, and support for, businesses in difficulty.

It is therefore established that the data collected does not serve solely a function of invoice transmission or VAT determination: its exploitation must also contribute to monitoring economic activity and steering public policy.

Several elements nevertheless remain to be established, notably the precise retention period for the various categories of data by the administration, access and authorization rules, the automated processing actually applied, any cross-referencing with other databases, and the legal conditions allowing their reuse for other public policies.

The sources examined do not make it possible to establish the existence of an interconnection with environmental data, a digital monetary infrastructure, or mechanisms allowing certain transactions to be made conditional. These possibilities must be examined separately in the following chapters.

→ [See the evidence and sources for Chapter 2](02-data-retention-access-and-purposes.md)

---

## Chapter 3 — Environmental data

**Status: ESTABLISHED / TECHNICALLY DEDUCIBLE / TO BE ESTABLISHED**

The European Union has established a legal and technical framework for the Digital Product Passport (DPP), allowing structured, machine-readable, interoperable digital data to be associated with identifiable products.

Depending on the requirements applicable to different product categories, the passport can be defined at the model, batch, or individual item level.

The information that may be associated with certain products notably includes data relating to their composition, durability, repairability, recyclability, and their carbon or environmental footprint.

The European Union also has methods enabling it to quantify certain environmental impacts of products over their life cycle. The battery regulation already provides a concrete example in which a quantitative carbon footprint is officially associated with certain categories of products.

The DPP is based on structured identifiers and may notably include a GTIN or an equivalent identifier. The standards used in electronic commercial exchanges also make it possible to carry standardized identifiers at item level.

It is therefore technically possible, where a common identifier or a matching mechanism exists and the necessary access rights are in place, to cross-reference a commercial transaction with the environmental information associated with the corresponding product.

Environmental data does not need to be directly recorded on the invoice for such cross-referencing to be technically achievable: the product identifier can be used to retrieve this information from a separate system.

Likewise, the buyer's identity does not need to be stored in the DPP for cross-referencing to be technically possible, if another system separately holds the information needed to identify the party to the transaction and the product concerned.

Where several transactions involve identifiable products to which quantitative environmental values are attached, these values can also, from a technical standpoint, be cross-referenced and aggregated by a system with the necessary data and access rights.

The DPP's regulatory architecture also provides for interoperability mechanisms, automated exchanges, an API, a European registry, and an interconnection with customs systems. Several European projects also combine digital traceability, proof of commercial transactions, and administrative actors responsible in particular for VAT and customs.

These elements do not, however, make it possible to establish that an individual environmental footprint of purchases is currently calculated by the administration, that products' environmental data is automatically cross-referenced with French invoicing or e-reporting data, or that it is used to authorize, refuse, or make a payment conditional.

→ [See the evidence and sources for Chapter 3](03-environmental-data.md)

---

## Chapter 4 — Digital euro and payment infrastructures

**Status: ESTABLISHED / TECHNICALLY DEDUCIBLE / TO BE ESTABLISHED**

The digital euro project rests on a centralized settlement infrastructure operated by the Eurosystem and distributed to users via payment service providers.

This infrastructure does not rest on a blockchain as the foundation of the system. Users would mainly retain a relationship with their bank or payment service provider, while the Eurosystem would perform the central functions needed for settlement and for the infrastructure's operation.

For online payments, the published technical model provides for the processing of structured data relating to users, accounts, devices, providers, payers, payees, and transactions.

Transactions notably have identifiers, an amount, a date and time, a type, an environment, and a status. The model also includes various pieces of information enabling the identification or categorization of the actors involved in a transaction.

Certain information relating to the merchant may also come into play in the process. The Merchant Category Code, or MCC, notably makes it possible to categorize the type of commercial activity of the payee and is among the information transmitted at certain stages of the documented payment process.

The architecture, however, distinguishes between the data present in the model, the data actually transmitted during a transaction, and the data each actor can actually access. The existence of a data field in the technical model therefore does not mean that all participants in the system can view it.

The project also provides for offline functionality allowing certain payments to be made directly between devices without an internet connection. In this mode, the personal details of the transaction are not transmitted to payment service providers or to the Eurosystem, either during or after the payment. This architecture constitutes an important limitation on the possibilities for systematically centralizing transaction-related information.

The digital euro proposal explicitly excludes the creation of a programmable currency, understood as monetary units to which restrictions determining the goods, services, places, persons, or periods for which they could be used would be intrinsically attached.

This prohibition does not, however, mean the absence of automated mechanisms around payments.

European Central Bank documentation explicitly provides for conditional payments, in which the execution of a transaction may depend on the prior verification of a condition.

The Eurosystem can provide the fundamental monetary functions necessary for these mechanisms, notably the reservation of funds, while the logic used to determine whether a condition is satisfied can be managed by payment service providers or other market actors.

The ECB's technical work also indicates that external monitoring can play a part in triggering these conditions.

This general mechanism is no longer merely a theoretical possibility. Market actors have connected their own platforms, via APIs, to an environment simulating the digital euro's back end in order to experiment with various conditional payment scenarios.

The scenarios studied notably include payment on delivery, pay-per-use, staged payments, certain automated refunds, and machine-to-machine payments.

It is therefore established, in principle, that information or an event originating from a system external to the monetary layer can be verified by a service in order to play a part in the decision to execute, release, hold, or return funds associated with a given transaction.

The external information used to verify a condition does not necessarily need to be stored in full within the monetary infrastructure: an external system can perform the verification and transmit only the result needed for the conditional process.

European digital identity, moreover, has an explicitly documented link with payment infrastructures.

The European Digital Identity Wallet, or EUDI Wallet, can be used in payment authentication processes. The ECB also plans to use it as a strong authentication method by providers participating in the digital euro pilot for certain online transactions.

The EUDI Wallet notably relies on mechanisms for verifiable attestations, data minimization, and selective disclosure. The existence of this link therefore does not mean that all the information held in the wallet is communicated to the merchant, the payment provider, or the Eurosystem.

The elements examined thus make it possible to separately establish the existence of structured and identifiable transactions, conditional payments, a conditionality layer capable of using information from external systems, interfaces allowing market-actor platforms to interact with the payment environment, and an explicit link between digital identity and payment.

These elements make it technically possible to build services in which information from an external infrastructure plays a part in an automated decision concerning a given transaction, without the currency itself becoming programmable.

They do not, however, make it possible to establish that a digital product passport, a GTIN, a carbon footprint, data from electronic invoicing, or an individual environmental profile is currently used to trigger, prevent, or modify a payment in digital euros.

The generic link between an external system and a conditional payment is therefore documented. The specific link between environmental or tax data and the execution of a payment remains to be established.

→ [See the evidence and sources for Chapter 4](04-digital-euro-and-payments.md)

---

## Chapter 5 — Interconnections

**Status: ESTABLISHED / TESTED/PILOTED / TECHNICALLY DEDUCIBLE / NOT ESTABLISHED**

Chapter 5 examined the links — existing, planned, tested, or technically possible — between the infrastructures studied separately in the preceding chapters.

The research shows that these infrastructures do not constitute a single, centralized system, but that they are not entirely independent of one another either.

The European Commission explicitly places several of these mechanisms within a shared objective of interoperability and the creation of synergies. The Digital Product Passport, eInvoicing, the European Business Wallets, and other European infrastructures are notably presented as forming part of a coherent ecosystem of digital solutions.

The reuse of electronic invoicing data, moreover, goes beyond the mere processing of the invoice itself. European work notably provides for its reuse for sustainability reporting and its cross-referencing with certain customs data.

The European Business Wallets constitute another documented point of convergence. The project provides for their use in identifying economic operators, verifiable attestations, certain tax and transactional information, and interactions with the Digital Product Passport and product-related data.

Standardization work also provides a direct link between transaction and product. The European model for eReceipts provides that a receipt may contain an identifier linking the purchased product to its Digital Product Passport and the corresponding verified information, notably including certain information on its durability and environmental impacts.

The following chain therefore now has documented links:

```
transaction
   ↓
eReceipt
   ↓
DPP identifier
   ↓
Digital Product Passport
   ↓
product / durability / environmental information
```

At the same time, the European pilots examined have documented a chain linking business identity, payment, a detailed electronic receipt, the Business Wallet, and experimental accounting or tax processing.

```
identity / authorization
   ↓
wallet
   ↓
payment
   ↓
detailed eReceipt
   ↓
Business Wallet
   ↓
accounting / experimental tax processing
```

The link between digital identity and payment is also documented: the EUDI Wallet can be involved in payment authentication, and its use is planned in the work relating to the digital euro pilot.

Finally, the ECB's work establishes that an external system can play a part in verifying a condition used by a conditional payment service.

```
external system
   ↓
verification of a condition
  ↓
conditionality layer
   ↓
payment
```

These various elements make it technically possible to reconstruct an architecture in which data relating to a product could be retrieved from an external infrastructure, evaluated by a service, and turned into a result usable by automated logic surrounding a transaction.

It nevertheless remains **NOT ESTABLISHED** that environmental data originating from the Digital Product Passport or an equivalent infrastructure is currently used as a condition to authorize, refuse, or limit a payment.

It also remains **NOT ESTABLISHED** that a centralized system brings together individual identity, a comprehensive purchase history, tax data, environmental data, and payment data, or that a generalized individual carbon profile is calculated from these infrastructures.

The work relating to the digital euro also maintains an essential distinction: programmable currency, whose units would intrinsically carry restrictions on the goods or services that could be purchased, is explicitly excluded, whereas conditional payment services distinct from the currency itself are planned and being tested.

The result of Chapter 5 is therefore precise: **a significant portion of the infrastructures and links technically enabling transaction, product, environment, identity, and payment to be associated with one another is now documented; some of these links are explicitly planned, standardized, or tested; but the link that would actually turn environmental data into an imposed rule authorizing or refusing a payment has not been established.**

→ [See the evidence and sources for Chapter 5](05-interconnections.md)

---

## Chapter 6 — Legal safeguards

**Status: ESTABLISHED / LEGAL SAFEGUARDS / LEGAL VULNERABILITIES / DOCUMENTARY BLIND SPOTS**

Chapter 6 examined whether the technical capabilities and interconnections identified in the preceding chapters could be freely exploited and combined.

The answer is no.

The existence of a piece of data, an identifier, an interface, or a technical possibility for cross-referencing does not in itself constitute legal authorization to use it for a new purpose.

The GDPR, EU law, national law, and the safeguards specific to the various infrastructures notably impose requirements relating to:

- the legal basis of processing operations;  
- the determination and compatibility of purposes;  
- necessity and proportionality;  
- data minimization;  
- security and access control;  
- the rights of individuals;  
- profiling and automated decisions;  
- oversight by independent authorities and the courts.

The investigation nevertheless established that these protections do not all constitute technical impossibilities or guarantees of permanence.

The example of CFVR is particularly important.

This processing operation has had its scope legally modified on several occasions since its creation. In 2026, data from electronic invoicing was integrated among its new sources, within an architecture allowing its large-scale algorithmic exploitation and its cross-referencing with other information used for anomaly detection and the targeting of tax audits.

This development concretely demonstrates that a data infrastructure created for one specific function can subsequently become a legally authorized source for another processing operation.

It does not demonstrate that every future interconnection will be authorized.

It demonstrates that the current legal scope of processing operations must not be confused with a permanent impossibility of their uses evolving.

Chapter 6 also identified an essential distinction between physical centralization and functional centralization.

An architecture does not need to bring all information together in a single database in order to enable it to be cross-referenced.

Distinct systems can exchange:

```
identifier
   +
attribute
   +
proof
   +
result
   +
verified condition
```

without necessarily transferring the entirety of their raw data.

This property is particularly important for the analysis of the infrastructures studied in this report, which rely heavily on structured identifiers, registries, interfaces, verifiable attestations, and interoperability mechanisms.

Chapter 6 also established that certain important safeguards are explicitly written into the frameworks studied.

The DPP notably provides for restrictions concerning customers' personal data.

The European Digital Identity Wallet provides for mechanisms of minimization, user control, and selective disclosure.

The framework currently proposed for the digital euro excludes programmable currency, that is, a currency whose units would intrinsically carry restrictions determining the goods, services, persons, places, or periods for which they can be used.

This prohibition, however, coexists with the possibility of developing conditional payment services based on externally verified conditions.

The distinction is fundamental:

```
programmable currency
   ≠
conditional payment
```

The first mechanism is excluded within the framework studied.

The second is planned for and has been the subject of experiments.

Chapter 6 identified no basis for asserting that environmental data relating to a product is currently being turned into an individual payment restriction.

But it confirms the legal importance of the boundary located between:

```
information
   ↓
verification
   ↓
profiling
   ↓
condition
   ↓
individual consequence
```

The more determinative a piece of data or a result becomes for access to a payment, a service, a right, or another significant possibility, the more central the requirements relating to legal basis, necessity, proportionality, accuracy, transparency, the ability to challenge, and fundamental rights become.

**ESTABLISHED:**

> The technical capabilities documented in the preceding chapters are legally regulated and cannot be freely combined for any purpose whatsoever.

**ESTABLISHED:**

> Data from electronic invoicing joined a pre-existing tax processing operation, CFVR, in 2026; CFVR's scope had already undergone several successive changes.

**LEGAL SAFEGUARD:**

> A new technical capability or a new interconnection does not, on its own, constitute legal authorization to produce an individual consequence.

**LEGAL VULNERABILITY:**

> The legally authorized scope of an infrastructure can evolve, subject to compliance with the applicable higher-order norms.

**LEGAL VULNERABILITY:**

> An increase in the possibilities for cross-referencing does not necessarily require the creation of a centralized database physically bringing all the data together.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined make it easier to assess each infrastructure and each extension separately than to assess the cumulative effect of the full set of their developments and interconnections.

**NOT ESTABLISHED:**

> No element examined currently demonstrates the existence of a mechanism using an individual environmental profile to authorize, refuse, or limit a person's payments, purchases, services, or rights.

**NOT ESTABLISHED:**

> No element examined demonstrates the existence of a single infrastructure automatically bringing together electronic invoicing, digital identity, environmental data, the Digital Product Passport, and the digital euro in order to control individual transactions.

→ [See the evidence and sources for Chapter 6](06-legal-safeguards.md)

---

## General conclusion

The six chapters now make it possible to trace a chain that, at the start of the investigation, was only a hypothesis to be verified.

The French electronic invoicing reform is transforming a significant portion of economic activity into structured, standardized, transmissible data that can be exploited automatically.

This data does not serve merely to carry an invoice.

The sources examined establish its use, or intended use, for various tax and economic purposes, notably combating fraud, pre-filling VAT returns, monitoring economic activity, and steering public policy.

Since 2026, certain data from electronic invoicing has also become a source for the CFVR processing operation and its large-scale processing infrastructure.

At the same time, the European Union is developing several other digital infrastructures.

The Digital Product Passport makes it possible to associate structured data with identifiable products, which may include information relating to their durability and environmental impacts.

European standards for electronic receipts make it possible to link a transaction and a product to its Digital Product Passport.

Digital identity infrastructures enable the presentation and verification of attributes.

The link between digital identity and payment is documented.

Pilots have connected identity, payment, a transactional receipt, and the Business Wallet.

Finally, work relating to the digital euro has established that an external system can play a part in verifying a condition used by a conditional payment service.

---

### The bridge sought at the start of the investigation has therefore indeed been partially built

The investigation does not end at the same point where it began.

At the outset, the question was whether infrastructures concerning:

```
invoicing
   +
transaction
   +
product
   +
environment
   +
identity
   +
payment
```

could actually have points of connection.

Several of these links are now **ESTABLISHED**, **STANDARDIZED**, or **TESTED/PILOTED**.

The resulting documentary chain can be represented as follows:

```
INVOICING / TRANSACTION
   ↓
STRUCTURED DATA
   ↓
PROCESSING AND CROSS-REFERENCING

TRANSACTION
   ↓
eRECEIPT
   ↓
IDENTIFIABLE PRODUCT
   ↓
DIGITAL PRODUCT PASSPORT
   ↓
PRODUCT INFORMATION
   ↓
DURABILITY / ENVIRONMENT
```

At the same time:

```
IDENTITY / ATTRIBUTES
   ↓
WALLET
   ↓
AUTHENTICATION
   ↓
PAYMENT
```

and:

```
EXTERNAL SYSTEM
   ↓
VERIFICATION
OF A CONDITION
  ↓
CONDITIONAL
PAYMENT SERVICE
   ↓
PAYMENT
```

Another chain has also been tested:

```
IDENTITY / AUTHORIZATION
   ↓
WALLET
   ↓
PAYMENT
   ↓
DETAILED eRECEIPT
   ↓
BUSINESS WALLET
   ↓
ACCOUNTING /
TAX PROCESSING
```

The result is therefore different from a simple juxtaposition of independent infrastructures.

> **Bridges exist.**

But not all segments carry the same status or the same level of evidence.

---

### The final decisive connection has not been established

The investigation makes it technically possible to reconstruct:

```
transaction
   ↓
identifiable product
   ↓
DPP
   ↓
environmental information
```

It also makes it possible to reconstruct separately:

```
external system
   ↓
verified condition
   ↓
conditional payment
```

It further documents:

```
digital identity
   ↓
payment
```

But it has not established the final connection:

```
IDENTITY
   +
TRANSACTION HISTORY
   +
PRODUCTS
   +
ENVIRONMENTAL DATA
   ↓
INDIVIDUAL
ENVIRONMENTAL PROFILE
   ↓
IMPOSED CONDITION
   ↓
AUTHORIZATION / REFUSAL /
LIMITATION OF A PAYMENT
```

**NOT ESTABLISHED:**

> No element examined currently demonstrates that this complete chain is deployed or legally organized in order to control an individual's payment possibilities.

This limitation is fundamental.

It prevents presenting as a fact what remains a possibility constructed from separately documented capabilities.

---

### But it would also be incorrect to conclude that the bridge does not exist

The absence of the final connection does not reset the findings of the investigation.

The sources made it possible to move from:

```
HYPOTHESIS
“these systems might perhaps
one day be connected”
```

to:

```
FINDING
several connections already exist,
are standardized,
provided for
or have been experimented with
```

The documentary boundary is now located much further along the chain.

What remains **NOT ESTABLISHED** is no longer the general possibility of linking transactions, products, environmental data, identity and payments.

What remains **NOT ESTABLISHED** is their combined use for a single purpose producing an individual restriction.

This distinction constitutes one of the main findings of the investigation.

---

### Chapter 6 nevertheless introduces a second boundary: technical possibility is not legal authorization

Even when a connection is technically possible, it cannot be freely exploited.

Processing remains subject in particular to:

```
legal basis
   +
purpose
   +
necessity
   +
proportionality
   +
data minimization
   +
data subject rights
   +
oversight
   +
fundamental rights
```

An infrastructure capable of linking two pieces of information is therefore not automatically authorized to do so.

And an infrastructure capable of producing a condition is not automatically authorized to use that condition to restrict a payment, a service or a right.

This distinction constitutes a genuine safeguard.

---

### But the legal framework is not immutable

The investigation has also established that the purposes, sources, categories of data and recipients of a processing operation can evolve legally.

CFVR provides a concrete example.

Since its creation, its scope has been amended several times.

In 2026, data from electronic invoicing became a new source for this pre-existing processing system.

The boundary between:

```
"technically possible
but not used"
```

and:

```
"legally authorised
and effectively used"
```

can therefore evolve.

This finding does not demonstrate any particular future development.

It demonstrates that the legal framework observed today should not be presented as a guarantee of immutability.

---

### The electronic invoicing reform must therefore be placed within a broader shift in scale

The investigation does not establish that electronic invoicing constitutes a central database bringing together all the information examined.

Such a claim would be excessive.

It does establish, however, that this reform transforms a significant share of economic activity into structured data that can be transmitted and processed automatically.

In the tax domain, its integration into CFVR now provides a concrete example of reuse within a broader algorithmic infrastructure.

The reform therefore constitutes a **\*\*structuring infrastructure for economic data\*\***.

Its significance does not come from the fact that it already centralises "everything".

It comes from the fact that it makes a growing share of economic activity:

```
STRUCTURED
↓
STANDARDISED
↓
MACHINE-READABLE
↓
TRANSMISSIBLE
↓
CROSS-REFERENCABLE
↓
ANALYSABLE
```

The question of its future interconnections therefore becomes just as important as that of its present purposes.

---

### The final result must therefore be formulated with two simultaneous truths

First truth:

> **the investigation has not demonstrated the current existence of a generalised system using identity, purchases, environmental data and digital currency to control individuals' economic possibilities.**

Second truth:

> **the investigation has demonstrated that a significant part of the technical building blocks and connections enabling transactions, products, environmental information, identity and payment to be linked already exists, is provided for by standards, integrated into European architectures or has been the subject of experiments.**

These two statements are not contradictory.

They precisely define the level of evidence reached.

---

### What has been established

**ESTABLISHED:**

> Electronic invoicing creates a massive infrastructure of structured economic data that can be processed automatically.

**ESTABLISHED:**

> Certain data from this infrastructure now feeds into CFVR, where it can be cross-referenced with other information as part of algorithmic processing intended in particular for anomaly detection and tax targeting.

**ESTABLISHED:**

> Standards make it possible to link a transaction, an identifiable product, a Digital Product Passport and verified information relating to the product, including certain environmental information.

**ESTABLISHED / EXPERIMENTED:**

> Digital identity can be involved in payment processes, and experiments have linked identity, payment, detailed electronic receipts and the Business Wallet.

**ESTABLISHED / EXPERIMENTED:**

> An external system can verify a condition whose result is used within a conditional payment service.

**TECHNICALLY DEDUCIBLE:**

> The documented connections make it technically possible to build a chain linking an identifiable transaction to information relating to the product and its environmental impact, and then to use the result of an external verification within conditional logic surrounding a payment.

---

**### What has not been established**

**NOT ESTABLISHED:**

> It has not been demonstrated that a generalised individual environmental profile is currently calculated from citizens' purchases.

**NOT ESTABLISHED:**

> It has not been demonstrated that environmental information from the DPP is currently used as a condition for authorising, refusing or limiting a person's payments.

**NOT ESTABLISHED:**

> It has not been demonstrated that electronic invoicing, the DPP, digital identity and the digital euro are brought together within a single infrastructure intended to control individual behaviour.

**NOT ESTABLISHED:**

> It has not been demonstrated that the digital euro will make it possible to intrinsically programme the currency in order to prohibit the purchase of certain categories of goods; on the contrary, the framework examined explicitly excludes programmable money.

---

### The conclusion of the investigation is therefore neither a validation nor an accusation

It is a mapping.

It shows:

```
what exists
   +
what communicates
   +
what has been experimented with
   +
what is technically possible
   +
what the law allows
   +
what it prohibits or regulates
   +
what remains to be demonstrated
```

The essential finding is that **the bridge has indeed been built over a substantial part of its path**.

It no longer rests solely on a succession of hypotheses.

Several of its pillars are documented by regulations, standards, technical architectures, European projects and experiments.

But the final passage:

```
ENVIRONMENTAL DATA
   ↓
INDIVIDUAL PROFILE
   ↓
IMPOSED RULE
   ↓
ECONOMIC
OR MONETARY RESTRICTION
```

remains **NOT ESTABLISHED**.

This is exactly where the available evidence ends today.

---

### Final conclusion

> **This investigation does not establish the current existence of a system for environmental control of payments or individual economic behaviour.**

> **It does establish, however, that a substantial part of the technical architecture that would make certain connections possible already exists: structured economic data, identification of transactions and products, Digital Product Passport, environmental data associated with products, digital identity, payment infrastructures, verification of external conditions and conditional payments.**

> **Several connections between these building blocks are established, standardised or have been experimented with. The technical bridge is therefore no longer an abstract hypothesis.**

> **What has not been established is its full activation for a single purpose enabling an individual environmental profile to be established and an imposed consequence to be derived from it regarding a payment, purchase, service or right.**

> **Current law also provides several safeguards against such a development. However, the study of CFVR demonstrates that the legal scope of processing operations can evolve over time.**

> **The boundary to monitor is therefore no longer limited to the emergence of new databases. It lies in new connections, new purposes, new attributes, new conditions and, above all, the new consequences that the law could progressively authorise on the basis of already existing infrastructures.**

> **The investigation therefore stops exactly at the limit of the available evidence: far enough to establish that the building blocks and several bridges exist; not far enough to assert that they currently constitute the integrated control system that their combination would make technically possible.**