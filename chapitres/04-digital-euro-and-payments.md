# Chapter 4 — Digital Euro and Payment Infrastructures

> **Navigation:** [← Back to the table of contents](#documentation)

This chapter examines the proposed architecture for the digital euro, the actors involved in its operation, the data necessary for the execution of payments, as well as the technical mechanisms enabling certain operations to be automated.

The objective is notably to determine what the digital euro infrastructure would technically enable, what data could be processed by the different actors, and what safeguards are provided concerning the programmability of money, data protection and the possibilities for conditioning payments.

An essential distinction must be made between:

- the programmability of the money itself;  
- conditional payments;  
- the automation of payment execution;  
- the data used to verify a condition;  
- the identification of the payer or beneficiary;  
- the potential use of information originating from other digital systems.

The existence of a mechanism enabling a payment to be automatically triggered when a condition is met does not mean that the money itself is programmable.

---

## Table of contents

- [4.1 — General architecture of the digital euro](#41-general-architecture-of-the-digital-euro)  
- [4.2 — Actors and payment infrastructures](#42-actors-and-payment-infrastructures)  
- [4.3 — Data processed during payments](#43-data-processed-during-payments)  
- [4.4 — Online and offline payments](#44-online-and-offline-payments)  
- [4.5 — Programmable money and conditional payments](#45-programmable-money-and-conditional-payments)  
- [4.6 — External conditions and payment automation](#46-external-conditions-and-payment-automation)  
- [4.7 — Digital identity and payment infrastructures](#47-digital-identity-and-payment-infrastructures)  
- [4.8 — Limitations and safeguards provided](#48-limitations-and-safeguards-provided)  
- [4.9 — What this chapter establishes](#49-what-this-chapter-establishes)

---

## 4.1 General architecture of the digital euro

**Status: ESTABLISHED / ONGOING PROJECT**

The digital euro is a central bank digital currency project intended to complement cash and other existing means of payment in the euro area [S22][S23].

It is not a crypto-asset or a currency issued by a private institution. Digital euro units would constitute a direct claim on the Eurosystem [S23].

As of the date of the sources examined, the digital euro has not yet been issued. The project continues its technical development and remains dependent on the adoption of the corresponding European legislative framework [S23].

---

### A central settlement infrastructure

The technical architecture currently envisaged is based on a centralized settlement platform operated by the Eurosystem [S23].

The Eurosystem would process and verify settlements as well as digital euro holdings recorded within the infrastructure [S23].

The ECB specifies that this architecture does not rely on blockchain or distributed ledger technology as the system's fundamental infrastructure [S23].

It nevertheless incorporates certain technical principles used in distributed systems, notably to improve resilience and performance.

**ESTABLISHED:**

> The architecture currently envisaged for the digital euro is based on a central settlement infrastructure controlled by the Eurosystem [S23].

---

### Distribution through intermediaries

The existence of a central infrastructure does not mean that users would directly hold an account with the ECB for their day-to-day transactions.

The proposed regulation provides that digital euro payment services would be distributed through payment service providers [S22].

These intermediaries would notably enable:

- access to and use of the digital euro;  
- initiation and receipt of payments;  
- provision of the instruments enabling these payments to be made;  
- management of digital euro payment accounts;  
- operations enabling the corresponding holdings to be funded or defunded [S22].

The ECB also indicates that a user could access the digital euro through an account set up with their bank or a public intermediary [S23].

The architecture therefore distinguishes at least two levels:

```
User
   ↓
Payment service provider
   ↓
Eurosystem infrastructure
   ↓
Settlement in digital euros
```

This separation between the relationship with the user and central settlement will become important in determining which data are accessible to the different actors.

---

### Money recorded on the Eurosystem's balance sheet

Digital euros held by users would constitute direct liabilities of the Eurosystem [S23].

This characteristic distinguishes the digital euro from commercial bank money usually held in a bank account.

The payment service provider would therefore manage the relationship with the user and provide the service, while the corresponding monetary value would remain a claim on the central bank.

**ESTABLISHED:**

> Intermediation by a bank or payment service provider does not transform the digital euro into private bank money: the corresponding holdings would remain a direct claim on the Eurosystem [S23].

---

### An infrastructure designed to operate at scale

The ECB envisages an architecture distributed across several geographical regions, each with multiple servers, in order to ensure service continuity and infrastructure resilience [S23].

The objective is notably to enable the system to continue operating in the event of a failure affecting part of the infrastructure.

The digital euro is therefore envisaged as a European retail payment infrastructure intended to operate at scale, rather than as an experiment limited to a small number of actors.

---

### Online and offline payments

The architecture provides for two main modes of use:

- online payments;  
- offline payments [S23].

The possibility of making offline payments is an important feature of the project.

In this situation, the ECB indicates that the transaction details would be known only to the payer and the beneficiary, in order to provide a level of privacy close to that of cash.

Online payments, by contrast, use the payment infrastructure and involve the intermediaries necessary for their execution.

The distinction between these two modes must therefore be preserved when examining the data accessible to the different actors.

---

### A centralized architecture does not mean that the ECB directly knows users' identities

Centralized settlement does not mean that the ECB would automatically have access to the civil identity of the users corresponding to each transaction.

The ECB indicates that the information made available to the Eurosystem would be pseudonymized and that it should not be able to directly identify the user from the payment data it receives [S23].

The intermediaries managing the relationship with the user would, however, have access to the information necessary to comply with their legal obligations.

This distinction will be examined more specifically in the section devoted to payment data.

---

### An architecture still under development

The digital euro is not currently a currency in circulation [S23].

The ECB is continuing the technical development of the system and indicates that it aims to be prepared for a potential first issuance in 2029, subject notably to the adoption of the European legislative framework [S23].

The technical specifications therefore continue to evolve.

The elements examined in this chapter should be understood as describing the architecture currently proposed or being prepared, rather than the definitive operation of a system already deployed.

---

### Interim conclusion

**ESTABLISHED:**

> The digital euro is designed as central bank money whose holdings would constitute a direct claim on the Eurosystem [S22][S23].

**ESTABLISHED:**

> The architecture currently envisaged is based on a centralized settlement platform controlled by the Eurosystem, while distribution and the relationship with users are handled through payment service providers [S22][S23].

**ESTABLISHED:**

> The infrastructure provides for online and offline payments, as well as specific technical mechanisms intended to ensure its resilience [S23].

**ESTABLISHED:**

> The ECB indicates that the Eurosystem should not be able to directly identify users from the payment data to which it would have access, while intermediaries would retain the information necessary to comply with their legal obligations [S23].

**TO BE ESTABLISHED:**

> What exact data circulate between the user, their payment service provider and the central infrastructure during the different types of transactions?

**TO BE ESTABLISHED:**

> Which technical components have access to the information required to initiate, verify, authorize, settle or potentially condition the execution of a payment?

---

## 4.2 Actors and payment infrastructures

**Status: ESTABLISHED / ONGOING PROJECT**

The architecture envisaged for the digital euro is not based on a single direct relationship between the user and the European Central Bank.

It involves several categories of actors performing distinct functions in access to the service, payment initiation, acceptance, control and settlement [S22][S24].

This distribution of functions is important in determining what information is accessible to each actor and at what point in a transaction.

---

### The Eurosystem

The Eurosystem constitutes the central level of the infrastructure.

As established in the previous section, the architecture currently envisaged provides for a central platform enabling, notably, the processing and settlement of digital euro transactions [S23].

The Eurosystem also defines the common rules and specifications necessary for the operation of the system.

The digital euro rulebook notably describes:

- the actors participating in the system;  
- the different use cases;  
- end-to-end payment flows;  
- the interfaces between the different components;  
- the technical requirements applicable to payment service providers;  
- data management mechanisms;  
- data exchanges;  
- risk and fraud management mechanisms;  
- transaction settlement [S24].

**ESTABLISHED:**

> The Eurosystem is therefore not only the issuer of the currency: it also provides the central infrastructure and defines the common technical rules enabling the different actors in the system to interact [S23][S24].

---

### Payment service providers

The proposed regulation provides that the distribution of the digital euro is based on payment service providers [S22].

Users establish a contractual relationship with these providers rather than directly with the European Central Bank [S22].

Payment service providers may notably enable users:

- to access the digital euro;  
- to initiate and receive payments;  
- to use digital euro payment instruments;  
- to manage their digital euro payment account;  
- to perform the funding and defunding operations provided for by the system [S22].

Payment service providers therefore constitute an intermediary layer between the user and the central infrastructure.

---

### The payer's payment service provider

In a transaction, the provider managing the relationship with the payer is involved in the initiation and processing of the payment [S24].

It notably constitutes the point of contact between the user, their payment instrument and the services necessary for the execution of the transaction.

The system's technical documentation explicitly distinguishes the functions and requirements applicable to providers distributing the digital euro [S24].

These providers must notably interact with the central services necessary for access to the system, liquidity management and transaction processing.

They also remain subject to the legal obligations applicable to payment service providers.

This position is important for the analysis of data: unlike the Eurosystem, which is intended to receive pseudonymized information in certain situations, the provider managing the relationship with the user has access to the information necessary to provide the service and comply with its regulatory obligations.

---

### The beneficiary's payment service provider

A commercial transaction may also involve a provider on the beneficiary's side of the payment.

The rulebook thus distinguishes providers distributing the digital euro from providers performing the acquiring functions necessary for payment acceptance [S24].

In a commercial transaction, the acquiring provider notably enables interaction between the merchant's acceptance device and the infrastructure necessary for processing the payment.

The architecture can therefore be represented in simplified form as follows:

```
Payer
   ↓
Payer's PSP
   ↓
Digital euro infrastructure
   ↓
Beneficiary's PSP / acquirer
   ↓
Merchant or beneficiary
```

This diagram is intentionally simplified: the technical flows may involve several additional common services.

---

### Acceptance devices

The infrastructure is not limited to banks and the Eurosystem.

The rulebook also provides specifications relating to devices enabling digital euro payments to be accepted [S24].

These devices may notably be involved in payments made to a merchant.

They constitute the technical point at which the information necessary for the transaction is presented, exchanged or captured before being transmitted to the other components of the system.

The acceptance device must therefore be distinguished from the central settlement system: it operates close to the commercial transaction, while monetary settlement is carried out in another layer of the infrastructure.

---

### Common services between the different actors

The rulebook also provides for a category of common services that can be used by different participants in the system [S24].

The technical specifications published by the ECB notably cover:

- access management;  
- alias lookup and resolution;  
- liquidity management;  
- payment processing;  
- risk and fraud management;  
- data exchanges;  
- transaction settlement [S24].

The existence of these services shows that the execution of a payment does not simply correspond to a direct transfer between two wallets.

It involves several technical functions that may operate successively or simultaneously in the processing of a transaction.

---

### Risk control, fraud prevention and compliance with legal obligations

Payment service providers remain responsible for the controls imposed on them by the applicable regulations.

The project's technical documentation notably provides for mechanisms relating to risk and fraud management [S24].

The versions of the rulebook preparing the architecture also indicate that the payer's payment service provider must carry out, before the final execution of a transaction, the legally required controls relating to fraud, anti-money laundering and counter-terrorist financing, as well as, where applicable, controls relating to sanctions and embargoes.

The provider remains responsible for the execution or non-execution of the transaction in accordance with the applicable legal framework.

**ESTABLISHED:**

> The execution of a digital euro payment is therefore not designed as a technically blind operation: regulatory controls and risk and fraud management mechanisms are involved in the processing of transactions [S24].

These controls correspond to existing legal obligations and do not, in themselves, constitute a general ability to condition payments according to any criterion.

---

### Several actors may therefore be involved in the same transaction

The architecture makes it possible to distinguish several functions:

```
User
   ↓
Payment instrument or interface
   ↓
Distributing PSP / payer's PSP
   ↓
Common services
   ↓
Central infrastructure
   ↓
Acquiring PSP / beneficiary's PSP
   ↓
Acceptance device
   ↓
Beneficiary
```

Not all of these actors or components necessarily have access to the same information.

Knowledge of the payer's identity, the beneficiary's identity, the amount, the instrument used, the commercial context or the technical information necessary for settlement may be distributed across several components.

It is therefore necessary to distinguish the overall existence of information within the payment chain from its actual accessibility by a specific actor.

---

### An essential distinction between knowledge and capacity to act

The presence of an actor in the processing of a transaction does not automatically mean that it has access to all the data relating to that transaction.

Conversely, an actor does not necessarily need to know the entire commercial context in order to perform a technical operation such as authentication, control, authorization or settlement.

This distinction will be particularly important when examining conditional payments.

A system may receive the result of an external verification without necessarily receiving all the data used to produce that result.

An architecture of this type can be represented as follows:

```
External system
   ↓
Result of a condition
   ↓
Payment component
   ↓
Execution or non-execution
```

**This representation describes only a principle of computer architecture. It does not mean that an external system using environmental, tax or individual data is currently connected to the digital euro.**

---

### Interim conclusion

**ESTABLISHED:**

> The architecture envisaged for the digital euro distributes functions among several categories of actors and components, notably the Eurosystem, payment service providers, providers operating on the payer's or beneficiary's side, acceptance devices and various common services [S22][S24].

**ESTABLISHED:**

> The rulebook provides distinct technical specifications concerning, notably, end-to-end flows, distributing and acquiring providers, acceptance devices, data management, data exchanges, risk and fraud, as well as settlement [S24].

**ESTABLISHED:**

> Regulatory controls and risk and fraud management mechanisms may intervene before the final execution of a transaction, in accordance with the obligations applicable to payment service providers [S24].

**TECHNICALLY DEDUCIBLE:**

> The distribution of functions among several components makes it possible for a decision or verification necessary for processing a payment to be produced in a separate system and then communicated to the component responsible for continuing or not continuing the operation, without that component necessarily having access to all the data used to produce that decision.

**TO BE ESTABLISHED:**

> What exact data are accessible to each of the actors involved in a digital euro transaction, and which data are exchanged between their different systems?

**TO BE ESTABLISHED:**

> Which services technically have the ability to block, suspend, defer or trigger a transaction, in what situations and according to what rules?

**TO BE ESTABLISHED:**

> Can information originating from systems external to the payment system be used by certain components of this architecture to determine whether an operation is executed, and if so, in which cases?

---

## 4.3 Data processed during payments

**Status: ESTABLISHED / ONGOING PROJECT**

The technical documentation published for the digital euro project makes it possible to go beyond a general description of the architecture and examine the categories of data provided for its operation [S24][S25].

Rulebook v0.91 notably includes a data model, a data dictionary and specifications dedicated to data exchanges between the different components of the system [S25].

These documents remain provisional and non-binding specifications. They nevertheless describe in detail the information currently provided for in the design of the system.

---

### A structured model of users, accounts, devices and transactions

The data model distinguishes several categories of entities necessary for the operation of the digital euro [S25].

It notably includes:

- users;  
- business users;  
- digital euro payment accounts;  
- certain non-digital-euro payment accounts linked to the system;  
- payment service providers;  
- devices used;  
- aliases;  
- merchant interaction points;  
- transactions;  
- payers;  
- beneficiaries;  
- dispute-related data;  
- risk and fraud data [S25].

The document specifies that this model represents the entities, their essential attributes and the relationships between them.

It should not, however, be interpreted as a complete representation of all the databases in the system or as indicating that each actor retains all of this information.

**ESTABLISHED:**

> The current design of the digital euro is based on a structured data model linking, notably, users, accounts, devices, payment service providers and transactions [S25].

---

### Identifiers specific to users and accounts

The model provides for a unique digital euro user identifier as well as an identifier for the digital euro payment account, notably referred to as DEAN in the specifications [S25].

It also provides for pseudonymous aliases.

The rulebook defines an alias as a pseudonymous identifier intended to protect the user's identity during payment processing. According to the specification, this alias can only be linked to an identifiable natural or legal person by the payment service provider distributing the digital euro or by the user concerned [S25].

The alias is intended to serve as a primary identifier that can be shared in certain transactions.

**ESTABLISHED:**

> The architecture therefore distinguishes between the identity known to the payment service provider and the pseudonymous identifier that may circulate in certain transaction processing operations [S25].

This separation constitutes an important identity protection measure but does not mean that the user is anonymous to their payment service provider.

---

### Detailed data describing the transaction

The model defines a transaction as the representation of a financial exchange between actors.

The examples mentioned notably include funding and defunding operations, recurring payments, reservations, payments, purchases, withdrawals and other operations [S25].

The information provided for notably includes:

- a transaction identifier;  
- an end-to-end transaction identifier known to the relevant providers;  
- the transaction amount;  
- the date and time of creation;  
- the transaction direction;  
- the currency;  
- additional information that may be provided by the user during initiation;  
- the transaction type;  
- the initiation method;  
- the transaction status;  
- the environment in which it takes place [S25].

The types and environments provided for notably make it possible to distinguish purchases, refunds, reservations, account-to-account payments, P2P transactions, e-commerce, mobile commerce, recurring payments or standing orders [S25].

**ESTABLISHED:**

> A digital euro transaction is therefore not represented solely by a transferred amount: the technical model provides for several attributes enabling it to be identified, dated, categorized and tracked throughout its processing cycle [S25].

---

### Identification of the payer and beneficiary

The model provides for separate entities for the payer and the beneficiary [S25].

The payer may be a natural person, a business, an administration or another public authority.

The beneficiary may also belong to these different categories.

The specifications provide for unique identifiers for the payer and the beneficiary within the data model [S25].

This does not mean that their full civil identity is communicated to all components of the system.

As indicated previously, the architecture notably provides for the use of pseudonymous aliases and a distribution of information between providers and the central infrastructure.

**ESTABLISHED:**

> The data model technically makes it possible to distinguish and identify the parties participating in a transaction, while providing mechanisms intended to limit the circulation of their directly identifiable identity [S25].

---

### The devices used can also be represented

The model provides for information relating to the devices used to interact with the system [S25].

A device may notably correspond to an application, a card or browser access.

The attributes provided for notably include:

- a device identifier;  
- its type;  
- its IP address where applicable [S25].

This information may notably be involved in technical, security or risk management processes.

Its presence in the model does not necessarily mean that it is transmitted to all actors participating in the settlement of a transaction.

---

### The commercial context can be categorized

The documentation also provides for data relating to the merchant and its activity [S25].

It notably uses the **Merchant Category Code**, or MCC, based on the ISO 18245 classification.

This code makes it possible to classify a merchant according to the type of goods or services corresponding to its activity, for example transportation, retail or vehicle rental [S25].

The model also provides for a merchant identifier as well as the identifier of its digital euro payment account.

**ESTABLISHED:**

> The currently documented architecture therefore makes it possible, in certain flows, to know not only the amount and the parties to a transaction but also a category corresponding to the beneficiary's commercial activity [S25].

This data does not, however, describe the individual product purchased.

A Merchant Category Code classifies the merchant's activity; it does not constitute a GTIN, a DPP identifier or an item identifier.

This distinction is essential to avoid confusing **merchant category** with **detailed basket contents**.

---

### The Merchant Category Code circulates in the payment request

The documentation goes further regarding the MCC.

It indicates that, among the information relating to the merchant's type of activity, **only the Merchant Category Code is transmitted in the payment request to the Digital Euro Service Platform (DESP) and to the distributing payment service provider**, and that it is transmitted in encrypted form [S25].

**ESTABLISHED:**

> In the currently documented architecture, information categorizing the merchant's activity is therefore among the data that may circulate within the technical chain of a payment request [S25].

The encryption of this information must be taken into account: its presence in a message does not mean that every intermediary component can necessarily read or use it.

It will therefore be necessary, for each processing operation, to distinguish the technical circulation of data from the actual ability of a specific actor to decrypt and use it.

---

### Information relating to the point of interaction and its location

The model also describes the point of interaction, or POI, where a transaction may be carried out [S25].

This may correspond to a physical location, such as a payment terminal in a store, or to a virtual location, such as an online payment page or mobile application.

The information envisaged notably includes:

- a point of interaction identifier;  
- its type;  
- a legal entity identifier;  
- a local business identifier, for example a SIRET in France;  
- an online identifier such as a domain name or IP address;  
- a physical address;  
- a city;  
- a postal code;  
- a country [S25].

The documentation specifies, however, that several of these pieces of information must be managed **internally by the acquiring PSP**, notably for traceability, auditing, management of acceptance capabilities and, for certain data, management of pre-disputes or disputes [S25].

**ESTABLISHED:**

> Information making it possible to characterize or locate a commercial point of interaction exists in the model, but the documentation provides that several of these pieces of information remain managed at the acquiring PSP level rather than necessarily being transmitted throughout the entire infrastructure [S25].

---

### Link with a non-digital-euro bank account

The model also provides for the possibility of linking a digital euro payment account to a non-digital-euro payment account [S25].

For the latter, the documentation notably mentions:

- the IBAN;  
- opening and closing dates;  
- the balance;  
- the date corresponding to the balance [S25].

This relationship is notably involved in the mechanisms enabling digital euro holdings to be funded or defunded.

**ESTABLISHED:**

> The architecture therefore provides for a possible technical link between a user's digital euro account and a conventional bank payment account used notably for funding or defunding operations [S25].

This link does not mean that the Eurosystem has unrestricted access to all the data from the traditional bank account: the distribution of data between the PSP and the DESP remains decisive.

---

### Risk and fraud data

The payment model also includes data relating to risk and fraud assessment [S25].

It notably provides for an entity corresponding to a **fraud and risk score**, as well as a type used to classify this score.

This information must be considered within the fraud prevention and detection function provided for by the payment architecture.

**ESTABLISHED:**

> The architecture therefore provides for the use of structured scores or indicators intended for risk and fraud assessment in payment processing [S25].

The presence of a risk or fraud score does not demonstrate the existence of a general social, environmental or behavioral score.

None of the sources examined at this stage establish that environmental data or an environmental profile are included in the calculation of these scores.

---

### Data that may be used for reports, queries and analyses

The data exchange service specifications provide for the DESP to make various reports and query mechanisms available to participants [S25].

The documentation explicitly indicates that these functions are intended to meet the **operational, analytical and statistical** needs of participants.

The reports and queries provided for notably concern:

- transactions;  
- accounts;  
- certain reference data;  
- disputes;  
- the calculation of certain fees;  
- risk and fraud management [S25].

Some reports may be detailed, others aggregated, and access to them depends on the role of the provider concerned.

The documentation provides, for example, detailed transaction reports for eligible PSPs as well as a periodic aggregated report relating to the fraud risk situation [S25].

**ESTABLISHED:**

> The infrastructure therefore provides not only for the immediate transactional processing of data but also for structured mechanisms enabling certain authorized participants to obtain reports and perform queries for operational, analytical or statistical purposes [S25].

This capability remains governed by the roles and access rights defined within the system.

---

### The model distinguishes the existence of data from its actual accessibility

One methodological point is essential.

The data model describes the information necessary for the different processes but specifies that it does not represent the entirety of an information system and does not automatically determine the information already managed in existing systems [S25].

Similarly, the data exchange service provides that the reports and queries accessible to a PSP depend on its role and the data for which it is eligible.

Three levels must therefore be distinguished:

```
Data provided for in the model
   ↓
Data actually transmitted in a specific flow
   ↓
Data actually accessible and usable by a specific actor
```

These three levels must not be confused.

---

### What the payment data do not yet establish

The elements examined make it possible to document a significant level of granularity in the information necessary for the operation of the system.

They do not, however, establish that the payment system systematically knows the individual product purchased.

At this stage, the data identified notably include the amount, date and time, parties, necessary accounts or aliases, transaction type and environment, certain technical elements, as well as the merchant's activity category.

None of the sources examined in this section establish that the payment request systematically contains:

- the GTIN of the product purchased;  
- the identifier of its Digital Product Passport;  
- its detailed description;  
- its carbon footprint;  
- the different line items making up the basket;  
- the detailed tax data from an electronic invoice.

**TO BE ESTABLISHED:**

> Can data originating from the commercial system, an electronic invoice, a DPP or another external system be associated with the transaction identifier or used by another layer of the infrastructure without being directly contained in the payment message?

---

### Interim conclusion

**ESTABLISHED:**

> The technical model currently published for the digital euro provides for structured data relating to users, accounts, devices, providers, payers, beneficiaries and transactions [S25].

**ESTABLISHED:**

> Transactions have identifiers, including an end-to-end identifier, and notably include information relating to the amount, date and time, type, environment and status of the operation [S25].

**ESTABLISHED:**

> The architecture provides for pseudonymous identifiers that limit the circulation of the user's directly identifiable identity, while their payment service provider retains the ability to link certain information to its customer [S25].

**ESTABLISHED:**

> The Merchant Category Code makes it possible to categorize the beneficiary's commercial activity, and the documentation provides for its encrypted transmission in the payment request to the DESP and the distributing PSP [S25].

**ESTABLISHED:**

> The model also includes information relating to points of interaction, certain location elements, devices and risk and fraud scores, with their management distributed among the different actors [S25].

**ESTABLISHED:**

> The DESP provides for reports and query mechanisms intended for certain PSPs according to their rights and roles, notably for operational, analytical and statistical purposes [S25].

**NOT ESTABLISHED:**

> The sources examined do not establish that the payment infrastructure systematically receives the precise identifier of the product purchased, its DPP, its GTIN, its environmental footprint or the complete details of the basket.

**TO BE ESTABLISHED:**

> What additional information can be associated with a transaction by PSPs, merchants or external systems through the transaction identifiers provided for in the architecture?

**TO BE ESTABLISHED:**

> What data are actually accessible to the DESP, distributing PSPs, acquiring PSPs and other technical services, in what form and for how long?

**TO BE ESTABLISHED:**

> In what situations can information describing the context of a transaction contribute to an automated decision concerning its processing?

---

## 4.4 Online and offline payments

**Status: ESTABLISHED / ONGOING PROJECT**

The architecture envisaged for the digital euro distinguishes two operating modes with different technical characteristics and levels of access to data:

- online payment;  
- offline payment [S23][S26].

This distinction is essential for the analysis of data processing possibilities.

An online payment uses the infrastructures and intermediaries necessary for its processing and settlement.

An offline payment, by contrast, is designed to enable the transfer of value without an Internet connection and without real-time intervention by the central infrastructure [S26].

---

### Online payment

In online operation, the different components examined in the previous sections are involved in processing the transaction.

Depending on the type of operation, this may notably involve:

- the payer's payment service provider;  
- the beneficiary's payment service provider;  
- the system's common services;  
- the Digital Euro Service Platform;  
- the Eurosystem's settlement infrastructure [S24][S25].

The data necessary for processing the transaction may then circulate between different components according to the rules, roles and access rights provided for by the architecture.

As established in section 4.3, these data may notably include transaction identifiers, the amount, date and time, the type and environment of the operation, the pseudonymous identifiers necessary for processing, as well as certain information relating to the commercial context [S25].

The ECB indicates, however, that the Eurosystem should not be able to directly identify the payer or beneficiary from the information received for online payments [S23].

The link between the pseudonymized identifiers used within the infrastructure and the identity of users would remain known to their payment service providers in accordance with the applicable obligations [S23].

**ESTABLISHED:**

> Online operation therefore involves a structured circulation of data necessary for payment, but the architecture provides for a separation between directly identifying information held by PSPs and pseudonymized information accessible to the Eurosystem [S23][S25].

---

### Offline payment

Offline operation is based on a different architecture.

The ECB provides that a payment can be made directly between the payer's and beneficiary's devices without an Internet connection at the time of the transaction [S26].

In the technical work currently being conducted for the pilot, offline payments between individuals notably rely on proximity communication using NFC.

The value necessary for the payment is stored locally in a secure hardware environment on the device.

The ECB is notably examining the use of:

- embedded Secure Elements;  
- eSIMs;  
- other hardware components capable of protecting the values and cryptographic operations necessary for offline operation [S26].

These components are intended notably to prevent the extraction of cryptographic keys, fraudulent modification of the balance or alteration of operations performed within the secure environment.

---

### A direct transfer between devices

In offline mode, the transfer does not require the intervention of an online system at the time of payment [S26].

The ECB describes the mechanism as a direct transfer of cryptographically secured values between two devices.

The operation can be represented simply as follows:

```
Payer's device
   ↓
Secure local communication
   ↓
Beneficiary's device
```

The central infrastructure therefore does not intervene in real time in the individual processing of this transaction.

**ESTABLISHED:**

> An offline digital euro payment is designed to be executed directly between the payer's and beneficiary's devices without transmitting the transaction to an online system at the time of payment [S26].

---

### Transaction details remain on the devices

The difference from online payment is particularly significant with regard to data.

The ECB indicates that, for offline payments, sensitive information relating to the transaction remains within the secure environment of the devices and is accessible neither to the Eurosystem nor to payment service providers [S26].

The documentation notably specifies that information relating to:

- the goods purchased or the purpose of the payment;  
- the location where the goods were purchased;  
- the merchant from whom the purchase was made or the person who received the payment,

is not accessible to the ECB, banks or PSPs in the context of offline payment [S26].

**ESTABLISHED:**

> Under the architecture currently announced, the personal details of an offline payment are designed to be known only to the payer and the beneficiary [S23][S26].

This characteristic constitutes a major difference from the online operation examined previously.

---

### A level of privacy comparable to cash

The ECB explicitly presents offline payment as being intended to offer a level of privacy comparable to that of cash [S23][S26].

Offline operation prevents the Eurosystem from directly linking the transaction to a person.

But it goes further: unlike online payment, PSPs also do not receive the personal details of the transaction itself during or after its execution [S26].

The difference can be summarized as follows:

**Online payment**

Transaction processed by the digital infrastructure:

- necessary data distributed among several components  
- PSP able to identify its customer  
- Eurosystem receiving information designed not to enable it to directly identify the user

**Offline payment**

Transaction executed locally between devices:

- personal details retained on the devices  
- PSP not receiving the personal details of the transaction  
- Eurosystem not receiving the personal details of the transaction

This distinction constitutes an important architectural safeguard in the analysis of payment tracking possibilities.

---

### Funding and defunding operations remain distinct

The private nature of offline payment does not, however, mean that the user can obtain or convert digital euros offline without any interaction with their provider.

Operations enabling funds to be loaded into the offline functionality or converted back into other forms of money require the involvement of the payment service provider [S26].

The ECB indicates that anti-money laundering controls are carried out by the PSP at the time of these funding and defunding operations, according to an approach comparable to the controls applicable to cash withdrawals and deposits [S23][S26].

It is therefore necessary to distinguish:

**Funding of funds**   → interaction with the PSP  
**Offline payment**    → local transfer between devices  
**Defunding of funds** → interaction with the PSP

**ESTABLISHED:**

> The privacy of offline payment concerns the transaction carried out between users; it does not eliminate the regulated interactions with the PSP necessary for funds to enter and leave the offline functionality [S23][S26].

---

### Locally stored value requires specific technical protections

The ability to perform a transaction without a connection requires the device to be able to securely store and transfer the corresponding value.

The ECB's current work notably relies on the use of a secure hardware element [S26].

This component notably protects:

- cryptographic keys;  
- the available value;  
- debit and credit operations;  
- critical information necessary for the operation of the offline mechanism [S26].

The objective is notably to prevent a user from artificially modifying their balance or duplicating the same value to make multiple payments.

Offline mode is therefore not simply an online mode that is temporarily disconnected: it requires a technical architecture specifically designed to enable a secure local transfer of value.

---

### A protection that also limits certain interconnection possibilities

The safeguards of offline mode have an important consequence for the subject of this investigation.

If the details of a transaction remain exclusively on the payer's and beneficiary's devices and are transmitted neither to the PSP nor to the Eurosystem, external infrastructures do not automatically have the information necessary to link this individual payment to other databases.

**TECHNICALLY DEDUCIBLE:**

> The offline architecture currently described therefore constitutes a technical obstacle to systematic centralized cross-referencing between each individual payment and information originating from other infrastructures, since the personal details of the transaction are not transmitted to the central infrastructure.

This conclusion must, however, remain limited to offline operation as it is currently designed.

It does not establish that all interactions surrounding the payment are anonymous, since funding and defunding operations involve the PSP.

Nor does it establish that no usage limit, security rule or anti-fraud mechanism can be applied to the offline functionality.

These elements must be examined separately.

---

### An architecture currently being tested

Offline operation is no longer merely a conceptual hypothesis.

The ECB is preparing a digital euro pilot scheduled to begin in the second half of 2027 and is currently continuing the work necessary to implement the offline functionality [S26].

In August 2026, the ECB notably launched a technical consultation concerning the standards required to deploy offline mode in the secure hardware components of smartphones.

The work notably concerns embedded Secure Elements and eSIMs.

**ESTABLISHED:**

> The offline architecture is therefore currently the subject of concrete technical work concerning hardware components, security standards and preparation for the pilot [S26].

It nevertheless remains a feature of a project that has not yet been deployed as a means of payment in general circulation.

---

### What offline mode does not establish

The existence of an offline functionality does not mean that all digital euro payments will have the same level of privacy.

Online payments follow a different architecture.

Nor does it mean that offline mode will necessarily be usable without any limits on amount, holdings, frequency or security.

Finally, the fact that the personal details of an offline transaction are not transmitted does not establish that the merchant or beneficiary does not itself hold any information relating to the purchase in its own commercial systems.

A merchant may separately hold:

- a receipt;  
- an order;  
- a customer account;  
- an invoice;  
- a product identifier;  
- or other commercial data.

**NOT ESTABLISHED:**

> The sources examined therefore do not establish that offline mode makes it impossible for cross-referencing to be performed independently by the merchant or by another system that separately holds the necessary commercial data.

This distinction is essential: the privacy of the **payment rail** does not necessarily mean the absence of data in the **commercial system** surrounding that payment.

---

### Interim conclusion

**ESTABLISHED:**

> The digital euro is designed to enable online and offline payments based on different architectures [S23][S26].

**ESTABLISHED:**

> An offline payment is intended to be executed directly between the payer's and beneficiary's devices without an Internet connection and without the intervention of an online system at the time of the transaction [S26].

**ESTABLISHED:**

> The value and sensitive information necessary for offline payment must be protected within a secure hardware environment on the device [S26].

**ESTABLISHED:**

> According to the architecture announced by the ECB, the personal details of offline transactions are accessible neither to the Eurosystem nor to PSPs and remain known to the payer and the beneficiary [S23][S26].

**ESTABLISHED:**

> Operations enabling funds to be funded or defunded remain, however, linked to the PSP, which performs the corresponding regulatory controls [S23][S26].

**TECHNICALLY DEDUCIBLE:**

> The absence of central transmission of the details of an offline payment significantly limits the possibility, at the payment infrastructure level, of systematically cross-referencing that transaction centrally with external tax, commercial or environmental data.

**NOT ESTABLISHED:**

> This protection does not establish that no cross-referencing can be performed independently within the beneficiary's commercial system when it holds data enabling the transaction, product or customer to be identified.

**TO BE ESTABLISHED:**

> What limits on amount, holdings, frequency or operation will ultimately be applied to offline payments?

**TO BE ESTABLISHED:**

> What information relating to funding and defunding operations will be retained by PSPs and for how long?

**TO BE ESTABLISHED:**

> Under what conditions can security, fraud prevention or limit management mechanisms prevent or defer an offline operation?

**TO BE ESTABLISHED:**

> Can an offline payment participate in a conditional payment mechanism, or do conditional mechanisms necessarily require an online component?

---

## 4.5 Programmable money and conditional payments

**Status: ESTABLISHED / TECHNICALLY DEDUCIBLE / ONGOING PROJECT**

The distinction between programmable money and conditional payments constitutes a central element of the architecture envisaged for the digital euro.

The European Central Bank explicitly excludes the digital euro becoming programmable money [S22][S27].

At the same time, the architecture is designed to enable conditional payments, meaning payments whose execution can be automatically triggered when certain predetermined conditions are met [S27].

These two mechanisms must not be confused.

---

### Programmable money is explicitly excluded

The ECB defines programmable money as money whose use would be intrinsically limited according to certain rules.

Such money could, for example, be designed to:

- allow the purchase only of certain goods or services;  
- be usable only during a specified period;  
- be spendable only within a particular geographical area;  
- or directly impose other restrictions on use attached to the monetary units [S27].

The ECB explicitly indicates that such operation is incompatible with the principles adopted for the digital euro.

Digital euro units must remain fungible and retain the same value as other forms of the euro.

**ESTABLISHED:**

> The Eurosystem explicitly excludes digital euro units themselves containing rules limiting the goods, services, periods, locations or beneficiaries for which they can be used [S22][S27].

The ECB presents this safeguard as a fundamental difference between money and a voucher restricted to a specific use.

---

### A payment can nevertheless be conditional

The exclusion of programmable money does not mean that all payments must be executed immediately and without conditions.

The ECB defines conditional payments as payments executed automatically when predetermined conditions are met [S27].

The condition does not alter the properties of the monetary units themselves.

It operates within the process determining **when a specific payment is to be executed**.

The distinction can be summarized as follows:

**Programmable money**

The rule is attached to the money itself.  
Example: this monetary unit can only be used to purchase a specified category of goods.

**Conditional payment**

The money remains freely usable, but a specific transaction is executed only when the condition agreed for that transaction is met.  
Example: payment for a product is released when its delivery is confirmed.

**ESTABLISHED:**

> The ECB therefore explicitly distinguishes a restriction attached to the money, which it excludes, from the conditional automation of a transaction, which is provided for in the digital euro architecture [S27].

---

### Funds reservation constitutes the basic mechanism

The envisaged architecture provides for a funds reservation functionality to support conditional payments [S27].

When a conditional payment is initiated, the corresponding amount can be temporarily reserved in the payer's account.

The reserved amount then reduces the balance available for other spending, but it is not immediately transferred to the beneficiary.

The funds remain available to execute the payment when the specified condition is met.

The mechanism can be represented as follows:

```
Payment initiated
   ↓
Amount reserved
   ↓
Verification of the condition
   ↓
Condition met     → funds transferred to the beneficiary
Condition not met → reservation cancelled or expired
```

**ESTABLISHED:**

> The envisaged central infrastructure therefore provides a technical funds reservation capability enabling their transfer to be deferred until a condition has been verified [S27].

---

### A settlement layer separate from a conditionality layer

The preparation phase closure report explicitly describes a separation between two layers [S27].

The first is the **settlement layer**, located in the back-end infrastructure and provided by the Eurosystem.

The second is a **conditionality layer**, developed by market actors.

The settlement layer handles monetary processing.

The conditionality layer determines whether the conditions specified for releasing the funds have been met.

The operation can be represented as follows:

**Conditionality layer — market actors**

```
Verification of an event or condition
   ↓
Result of the verification
   ↓
Funds reservation function / payment infrastructure
   ↓
Settlement layer — Eurosystem
   ↓
Transfer or release of funds
```

**ESTABLISHED:**

> The architecture currently described therefore technically separates the monetary settlement function from the logic used to determine whether a condition associated with a transaction has been met [S27].

This separation is essential.

It means that the Eurosystem does not necessarily need to know or evaluate itself the data used to verify the condition.

---

### External monitoring can trigger the condition

The ECB's preparation phase closure report specifies that this architecture must provide flexibility for **external monitoring capable of triggering the conditions** [S27].

In the example provided by the ECB, a system can determine that a train has actually arrived.

When this information confirms that the specified condition has been met, the reserved funds are transferred to the beneficiary.

If the train does not arrive or if the specified condition is not met, the reservation can be cancelled or expire and the funds become available to the payer again [S27].

**ESTABLISHED:**

> Information produced or verified outside the settlement layer can therefore technically contribute to triggering or not triggering a conditional payment [S27].

This constitutes a first explicitly documented link between **data or an event external to monetary settlement** and **the execution of a transaction**.

---

### Examples already identified and experimented

The work of the ECB and market actors has examined several categories of conditional payments [S27].

The documented examples notably include:

- payment on delivery;  
- pay-per-use;  
- payments triggered by stages or milestones;  
- automatic refunds;  
- subscriptions;  
- split payments;  
- machine-to-machine payments;  
- certain payments linked to energy consumption [S27].

In the case of payment on delivery, the transaction can be finalized when delivery of the product is confirmed.

In a machine-to-machine payment, a machine can automatically contribute to triggering a payment when a specified event occurs.

The ECB and market actors have already tested the feasibility of several of these mechanisms in an environment simulating the digital euro back-end [S27].

**ESTABLISHED:**

> Conditional payments are therefore no longer merely an abstract possibility described in a regulatory proposal: their technical feasibility has been experimented with market actors in the ECB's innovation environment [S27].

These experiments did not, however, use actual digital euros and do not constitute the deployment of a production system.

---

### The condition can be verified by a third party

Earlier ECB work also provides an example in which the triggering of a payment on delivery can depend on a third party other than the payer or beneficiary, such as the postal service responsible for confirming delivery of a product [S27].

This architecture therefore potentially introduces a third actor into the technical decision enabling the payment to proceed.

```
Payer + beneficiary define or accept the condition
   ↓
Third party or external system verifies the event
   ↓
Confirmation of the condition
   ↓
Payment executed automatically
```

**ESTABLISHED:**

> Verification of a condition can therefore be carried out on the basis of information originating from an actor or system distinct from the payer, the beneficiary and the central settlement layer [S27].

---

### Market actors develop the conditional logic

The ECB considers supervised intermediaries and other market actors to be best placed to develop conditional payment services [S27].

The digital euro infrastructure notably provides the fundamental funds reservation functionality.

Market actors can build value-added services on top of this infrastructure using their own logic and the information necessary for the relevant use cases.

In July 2026, the ECB also indicated that banks could use the digital euro infrastructure to automatically trigger payments when an agreed condition is met and develop new services by relying on the data available to them [S27].

**ESTABLISHED:**

> Conditional logic is therefore not designed as a function exclusively defined and operated by the European Central Bank: banks, PSPs and other market actors can develop conditional services on top of the common infrastructure [S27].

---

### The first technical bridge with external data

The previous sections established that the payment architecture can process different information relating to transactions and that market actors have their own systems and data.

This section adds a further element: the conditionality layer can use the verification of an external event to determine whether the reserved funds should be transferred [S27].

The general mechanism therefore becomes:

```
External data or event
   ↓
Verification of the condition
   ↓
Conditionality layer
   ↓
Instruction relating to the reserved funds
   ↓
Execution or non-execution of the payment
```

**ESTABLISHED:**

> The principle whereby information external to monetary settlement can trigger the execution of a conditional payment is explicitly provided for in the architecture examined [S27].

This finding constitutes a **technical bridge between external information and the execution of a payment**.

It does not, however, establish that any information can be used as a condition.

---

### This bridge does not demonstrate the use of environmental data

None of the sources examined in this section provide for a payment being conditioned by:

- the carbon footprint of a product;  
- a Digital Product Passport;  
- a GTIN;  
- a cumulative environmental footprint;  
- an individual environmental quota;  
- tax data originating from electronic invoicing;  
- or a user's behavioral profile.

The examples currently documented mainly concern events directly related to the performance of a contract or service: delivery, completion of a service, use of a service, timing, consumption or a verifiable event [S27].

**NOT ESTABLISHED:**

> The existence of a conditionality layer capable of using external information does not demonstrate that it is currently designed to receive or use environmental data, tax data or individual profiles.

This distinction is fundamental to the analysis.

---

### But the technical nature of the condition is not intrinsically monetary

The condition enabling the payment to be triggered may correspond to an event verified by a separate system.

The settlement system does not necessarily need to know all the information used to establish that this condition has been met.

**TECHNICALLY DEDUCIBLE:**

> A conditional payment architecture can technically use the result of a verification performed by an external system without the data used for that verification being directly integrated into the monetary infrastructure.

For example, the payment system could receive only a logical result:

```
Condition verified: YES
or
Condition verified: NO
```

without necessarily receiving all the data that led to that result.

This technical property means that an interconnection does not necessarily require the complete merging of the databases concerned.

---

### Who decides the condition is a separate legal question

The technical ability to construct a condition does not mean that any actor can arbitrarily impose that condition on a user.

The ECB indicates that conditional payments are based on predetermined and agreed conditions and states that users remain free to choose whether to use these services [S27].

In a January 2026 communication, the ECB also specified that the conditions of a payment could only be set by the payer and the beneficiary.

**ESTABLISHED:**

> Under the framework currently presented by the ECB, conditional payments are voluntary services based on conditions agreed between the parties and do not give the Eurosystem a general power to determine what a user may purchase [S27].

This safeguard must be distinguished from the system's technical ability to automatically execute a transaction when the agreed condition has been met.

---

### The exact boundary with an external restriction must remain under scrutiny

The conceptual distinction between programmable money and conditional payment is clear:

- programmable money imposes a restriction on the monetary unit itself;  
- conditional payment applies logic to a specific transaction.

From the user's perspective, however, a condition may nevertheless have the practical effect that a specific payment is not executed until the specified criterion is met.

This observation does not establish that the system constitutes programmable money.

It merely shows that **the absence of programmability of the money does not imply the absence of programmable logic surrounding the execution of payments**.

**TECHNICALLY DEDUCIBLE:**

> An infrastructure can therefore simultaneously use fully fungible and non-programmable money while enabling external services to apply automated rules to the execution of specific transactions.

The determining question then becomes the governance of these rules: who can define a condition, with what consent, based on what data and within what legal framework?

---

### Interim conclusion

**ESTABLISHED:**

> The ECB explicitly excludes the digital euro being programmable money that intrinsically limits the goods, services, periods, locations or beneficiaries for which the monetary units can be used [S22][S27].

**ESTABLISHED:**

> The architecture nevertheless provides for conditional payments executed automatically when predetermined conditions are met [S27].

**ESTABLISHED:**

> A funds reservation functionality is provided to temporarily retain the necessary amount until the condition has been verified [S27].

**ESTABLISHED:**

> The ECB describes an architecture separating a settlement layer provided by the Eurosystem from a conditionality layer developed by market actors, with the possibility for an external verification to trigger the condition [S27].

**ESTABLISHED:**

> Conditional payments have already been experimented in a simulated environment with market actors, notably for payment-on-delivery, pay-per-use, milestone payment and other automated service scenarios [S27].

**ESTABLISHED:**

> The ECB indicates that banks and other providers will be able to develop conditional services on top of the common infrastructure and rely on the data available to them to offer innovative services [S27].

**TECHNICALLY DEDUCIBLE:**

> Information originating from an external system can technically contribute to the execution or non-execution of a transaction without that information necessarily being stored in the money itself or fully transmitted to the settlement layer.

**NOT ESTABLISHED:**

> The sources examined do not establish that environmental data, DPPs, tax data or an individual profile are used as payment conditions in the architecture currently envisaged.

**ESTABLISHED:**

> Under the framework currently presented by the ECB, conditions are designed to be agreed between the parties, and the Eurosystem states that it does not have the power to block categories of purchases [S27].

**TO BE ESTABLISHED:**

> What categories of external data can technically be used by services developing the conditionality layer?

**TO BE ESTABLISHED:**

> Which actors can provide the proof or result enabling a condition to be considered satisfied?

**TO BE ESTABLISHED:**

> What legal safeguards prevent a condition initially designed as voluntary or contractual from being imposed by an intermediary, regulation or another actor?

**TO BE ESTABLISHED:**

> Are there projects or experiments linking conditional payments to invoicing, product traceability or environmental data infrastructures?

---

## 4.6 External conditions and payment automation

**Status: ESTABLISHED / TECHNICALLY DEDUCIBLE / TO BE ESTABLISHED**

The previous section established that the architecture envisaged for the digital euro distinguishes between a settlement layer provided by the Eurosystem and a conditionality layer developed by market actors [S27].

The work carried out within the innovation platform makes it possible to go further: market actors have actually connected their own platforms to an environment simulating the digital euro interfaces in order to experiment with conditional payments [S28].

It therefore becomes possible to distinguish three components:

```
External system or platform
   ↓
Logic used to verify a condition
   ↓
Infrastructure enabling funds to be reserved and then transferred
```

This architecture has been the subject of technical experiments, even though the digital euro itself is not yet in circulation [S28].

---

### Participant platforms were connected to the simulated interfaces

As part of the "pioneers" workstream, the ECB provided participants with an environment simulating the digital euro back-end, as well as technical specifications and programming interfaces [S28].

Participants were able to connect their own platforms to this environment through APIs.

In the experiment, they acted as providers developing their own services on top of the core functionalities provided by the Eurosystem.

**ESTABLISHED:**

> Platforms developed or operated by market actors were therefore effectively connected, on an experimental basis, to interfaces simulating the digital euro infrastructure [S28].

This is not yet a connection to the future production system.

Nevertheless, this experiment demonstrates that the architecture is designed to enable external systems developed by market actors to use the functionalities provided by the common infrastructure.

---

### The Eurosystem provides the monetary function, the market develops the condition

The distribution of responsibilities experimented follows the separation described previously [S27][S28].

The Eurosystem provides the fundamental functions necessary for monetary processing, notably the reservation of funds.

PSPs and other market actors develop the layer determining the conditions necessary for their release.

The mechanism can be represented as follows:

```
**Eurosystem infrastructure**

funds reservation
   ↓
**PSP or market actor platform**

definition and management of the condition
   ↓
**Information enabling the condition to be verified**
   ↓
condition met
   ↓
instruction enabling the release of funds
```

**ESTABLISHED:**

> In the experiments carried out, the logic determining the condition was therefore not necessarily located within the Eurosystem's central infrastructure: it could be developed and managed by the platforms of market actors [S28].

---

### The condition can depend on an event external to the payment

Several scenarios examined show that the condition does not need to be information produced by the monetary system itself [S27][S28].

In a payment on delivery, the determining information is confirmation of the product's delivery.

In a transport-related refund, it may be linked to the performance, delay or cancellation of the service.

In a pay-per-use payment, it may depend on the actual use of a service or equipment.

In a milestone payment, it may depend on the successive completion of predetermined objectives or milestones [S28].

**ESTABLISHED:**

> The conditions examined can therefore depend on facts or events produced outside the monetary infrastructure and verified by the conditional layer developed by market actors [S27][S28].

---

### An external system does not necessarily need to transmit all its data

The separation between the conditional layer and the settlement layer allows an external system to perform certain verifications itself.

The monetary layer does not then necessarily need to receive all the information used to perform that verification.

The mechanism can be summarized as follows:

```
external system holds information
   ↓
external system verifies a rule
   ↓
result: condition met or not met
   ↓
conditional layer processes this result
   ↓
funds released or kept reserved
```

**TECHNICALLY DEDUCIBLE:**

> Data used to determine the execution of a payment therefore do not necessarily need to be stored within the monetary infrastructure or even transmitted to it in full: a verification result may technically be sufficient.

This property is important for the study of interconnections.

The absence of data from the digital euro data dictionary is not, by itself, sufficient to establish that such data could never indirectly contribute to the logic of a payment service developed around the infrastructure.

---

### Machine-to-machine payments extend automation

The experiments also examined scenarios related to Industry 4.0 and machine-to-machine payments [S28].

In these scenarios, equipment or digital systems can automatically participate in the initiation or triggering of financial operations.

One example examined involves a machine detecting by itself the need for a replacement part and participating in the automation of the corresponding commercial process.

These scenarios notably seek to reduce manual intervention and enable real-time settlements or settlements based on the actual use of a service [S28].

**ESTABLISHED:**

> The experimental work is therefore not limited to payments manually triggered by a person: it also examines chains in which systems or machines can automatically participate in the initiation and processing of a transaction [S28].

This automation does not mean that a machine can arbitrarily spend a user's money: it operates within a framework of service, mandate, authorization and predefined conditions.

---

### Milestones can progressively determine the release of funds

The experiments examined payments based on stages or "milestones" [S28].

In this type of scenario, the full amount of funds is not necessarily released at once.

Payment can be made progressively when different predefined objectives are considered to have been achieved.

One example examined concerns online training for which funds could be released progressively as the learner achieves certain objectives.

Another example concerns crowdfunding, in which funds could be released according to the progress of a project [S28].

**ESTABLISHED:**

> An external condition can therefore not only determine whether a payment should be executed, but also contribute to determining the time or stage at which part of the funds should be released [S28].

---

### Pay-per-use payments rely on measurable data

Pay-per-use constitutes another category examined by the platform [S28].

In this type of mechanism, the amount or timing of the payment depends on the actual use of a good or service.

The condition can therefore be supplied by information measuring that use.

This may notably concern mobility services, infrastructures or certain connected equipment.

**TECHNICALLY DEDUCIBLE:**

> When an external system is capable of measuring an event or quantity and communicating the corresponding result to the conditional layer, this information can technically contribute to the automation of the payment.

This is a general operating principle of conditional payments and not evidence that any category of data can be used without restriction.

---

### Automation can also apply to refunds

The ECB's work does not focus solely on triggering a payment to a merchant [S27][S28].

It also examines the automation of refunds when certain conditions are met.

In the transport sector, for example, a cancellation or delay may lead to the automation of a refund.

The same general principle applies:

```
external event
   ↓
verification of the situation
   ↓
automatic triggering
   ↓
payment or refund
```

**ESTABLISHED:**

> The use of an external condition can therefore affect different financial flows, notably the release of a payment or the triggering of a refund [S27][S28].

---

### Payment can be associated with additional commercial information

The innovation platform also examined complementary services such as electronic receipts [S28].

The ECB presents e-receipts as a functionality that could be associated with digital euro payments, notably to enable users to track their spending and manage their warranties.

This functionality is distinct from monetary settlement.

It nevertheless shows that market actors are considering services in which a payment transaction can be associated with additional commercial information.

**ESTABLISHED:**

> The work of the innovation platform therefore also envisages associating a digital euro payment with commercial information external to the strict monetary transfer, notably through electronic receipts [S28].

**TO BE ESTABLISHED:**

> What level of granularity could these electronic receipts contain, and could they notably include product references, purchase line items or standardized identifiers?

---

### The link with the product becomes technically concrete in certain scenarios

The payment-on-delivery scenario already relies on a relationship between:

- an order;  
- a purchased product;  
- a delivery;  
- a transaction;  
- a condition;  
- and the release of funds [S27][S28].

The system must be able to determine that the verified event corresponds to the transaction for which the funds were reserved.

There is therefore necessarily, within the service developed around the payment, a mechanism enabling the verified condition to be matched with the transaction concerned.

**ESTABLISHED:**

> The scenarios experimented demonstrate that an external platform can technically associate a commercial event relating to an order or service with the transaction whose execution depends on that event [S28].

This does not mean that the central infrastructure knows the details of the product.

The matching can be performed within the external platform, which then transmits only the information necessary for the payment to proceed.

---

### The generic bridge between external data and payment is established

At this stage, several elements can be assembled.

Chapter 4 has established:

- that a transaction has structured identifiers [S25];  
- that a funds reservation architecture enables their transfer to be deferred [S27];  
- that a conditionality layer can be developed by market actors [S27][S28];  
- that external monitoring can trigger a condition [S27];  
- that participant platforms have actually been connected to the simulated digital euro interfaces [S28];  
- that commercial events external to settlement have been used in conditional payment scenarios [S28].

The following chain is therefore now documented in principle:

```
event or data originating from an external system
   ↓
platform or service of the market actor
   ↓
verification of a condition
   ↓
association with the corresponding transaction
   ↓
use of the funds reservation functionality
   ↓
execution, release, retention or return of funds depending on the scenario
```

**ESTABLISHED:**

> The architecture and experiments examined therefore establish that a system external to the settlement layer can provide or verify information used by a conditional service to determine the execution of a specific transaction [S27][S28].

This finding now goes beyond the mere abstract possibility of a computer architecture: the general mechanism has been the subject of technical experiments involving market actor platforms connected to an environment simulating the digital euro [S28].

---

### The specific bridge with environmental data is not established

This conclusion must not, however, be extended beyond what the sources demonstrate.

None of the experiments examined establish that a payment condition has been supplied by:

- a Digital Product Passport;  
- a DPP identifier;  
- a GTIN used to query a DPP;  
- the carbon footprint of a product;  
- a cumulative environmental footprint;  
- data originating from the French electronic invoicing system;  
- an individual environmental profile.

**NOT ESTABLISHED:**

> The generic bridge between an external system and a conditional payment is documented, but the specific bridge between environmental or tax data and the execution of a payment is not established at this stage.

This distinction constitutes an essential limitation of the investigation.

---

### The combination with Chapter 3 nevertheless becomes technically analyzable

Chapter 3 separately established that a product can be associated with a digital identifier and structured environmental data and that, when compatible identifiers exist, this information can technically be matched with a commercial transaction.

The present chapter now establishes that information originating from an external system can be verified within a conditionality layer and contribute to the execution of a payment.

These two findings do not demonstrate that they are actually interconnected.

They nevertheless make it possible to identify precisely the technical connection that would be required:

```
transaction or order
   ↓
identifiable product
   ↓
external system holding information relating to the product
   ↓
rule or condition applied within an external service
   ↓
verification result
   ↓
payment conditionality layer
   ↓
execution or non-execution depending on the condition
```

**TECHNICALLY DEDUCIBLE:**

> If an authorized actor had environmental data relating to a product and if that data were used as a criterion for a payment condition, the architecture described for conditional payments would technically enable the result of that verification to contribute to the execution of the transaction without the environmental data being integrated into the money itself.

This proposition describes a technical possibility resulting from the combination of components documented separately.

**It demonstrates neither the existence of such a service, nor its legal authorization, nor its use by an administration, bank or PSP.**

---

### An interconnection does not necessarily require a single database

The findings from Chapters 3 and 4 also show that a potential interconnection would not necessarily need to centralize all information within a single system.

A service could theoretically:

```
receive the identifier necessary for a transaction
   ↓
query an authorized external system
   ↓
verify a condition
   ↓
obtain a result
   ↓
transmit only that result to the system responsible for the payment
```

**TECHNICALLY DEDUCIBLE:**

> The absence of physical merging between environmental, commercial and monetary databases is therefore not sufficient to technically exclude a decision-making mechanism based on their interoperability.

This deduction is consistent with the architectures examined: they rely precisely on identifiers, APIs, access rights and exchanges between specialized components.

---

### Consent and governance remain decisive

The technical ability to use an external condition does not determine who has the right to define that condition.

In the use cases currently presented by the ECB, conditional payments are services intended to meet a need of the payer and the beneficiary [S27].

They do not constitute a general power granted to the Eurosystem to decide which purchases should be authorized.

A distinction must therefore be maintained between:

- a voluntary condition chosen within a service;  
- a contractual condition imposed by the terms of use of a service;  
- a regulatory condition imposed by law;  
- a decision taken by an intermediary in accordance with its legal obligations;  
- a restriction attached to the money itself.

These situations may produce similar technical effects on a transaction but are based on different legal grounds and decision-making actors.

**TO BE ESTABLISHED:**

> What safeguards prevent or regulate the use of the conditional layer for criteria other than those voluntarily accepted by the payer and the beneficiary?

---

### Experiments continue in 2026

The work of the innovation platform did not end with the first experiment [S28].

The ECB announced a new phase of collaboration with market actors in 2026.

This phase is intended notably to further explore conditional payments and other value-added services, such as electronic receipts, bill splitting and budgeting tools.

The ECB also indicates that it intends to continue exploring machine-to-machine payments, artificial intelligence applied to payments, micropayments and various B2B use cases.

**ESTABLISHED:**

> The integration of external services and payment automation therefore remain an active area of development and experimentation for the project in 2026 [S28].

The final characteristics of the resulting services have not, however, yet been established.

---

### Interim conclusion

**ESTABLISHED:**

> Market actors have connected their own platforms, through APIs, to an environment simulating the digital euro interfaces in order to test conditional payments [S28].

**ESTABLISHED:**

> In the architecture experimented, the Eurosystem provides the fundamental monetary functionalities, while PSPs and other market actors can develop and manage the logic determining the conditions for releasing funds [S27][S28].

**ESTABLISHED:**

> The conditions experimented can depend on events external to monetary settlement, notably delivery, use of a service, completion of a milestone or other verifiable events [S28].

**ESTABLISHED:**

> Machine-to-machine scenarios have also been examined, enabling systems or equipment to automatically participate in certain commercial and payment processes [S28].

**ESTABLISHED:**

> The generic mechanism enabling an external system to provide or verify information contributing to the execution of a conditional payment has therefore moved beyond the stage of a mere technical hypothesis and has been the subject of experiments in a simulated environment [S27][S28].

**TECHNICALLY DEDUCIBLE:**

> External data do not necessarily need to be directly transmitted to or stored within the monetary infrastructure: the conditional layer can technically perform or receive a verification and communicate only the result necessary for the execution of the payment.

**TECHNICALLY DEDUCIBLE:**

> The combination with the infrastructures examined in Chapter 3 makes technically possible an architecture in which an environmental characteristic of a product would be verified in an external system and then used as a criterion for a conditional payment service.

**NOT ESTABLISHED:**

> None of the elements examined establish that a DPP, a GTIN, a carbon footprint, data originating from electronic invoicing or an individual environmental profile are currently used to trigger, prevent or modify a digital euro payment.

**TO BE ESTABLISHED:**

> Are there experiments, consortia, public procurement contracts, specifications or partnerships concretely linking product traceability, electronic invoicing or environmental data infrastructures to conditional payment services?

**TO BE ESTABLISHED:**

> Will the electronic receipts envisaged with the digital euro be able to carry product identifiers or other information enabling automated matching with commercial or environmental systems?

**TO BE ESTABLISHED:**

> Which actors are simultaneously involved in DPP, electronic invoicing and digital euro projects, and are they developing interfaces or services enabling these infrastructures to be linked?

---

## 4.7 Digital identity and payment infrastructures

**Status: ESTABLISHED / ONGOING PROJECT**

European digital identity constitutes an infrastructure distinct from the digital euro.

Official sources nevertheless establish an explicit connection between the European Digital Identity Wallet, or EUDI Wallet, and payment infrastructures [S29].

The European Commission documents a use case specifically dedicated to payment authentication using the EUDI Wallet.

In parallel, the European Central Bank provides for providers participating in the digital euro pilot to be able to use this wallet as a strong authentication method for certain online transactions [S29].

The link between digital identity and payment is therefore not merely technically deducible: it is explicitly provided for in the architectures examined.

---

### The EUDI Wallet constitutes a European digital identity infrastructure

The European digital identity framework provides for wallets enabling natural and legal persons to identify themselves and present various digital attestations [S29].

The wallet can notably contain or enable the presentation of:

- identity data;  
- electronic attestations;  
- verifiable credentials or attributes;  
- elements necessary for authentication with public or private services.

The architecture relies on common formats and protocols enabling issuers, wallets and relying parties to cryptographically verify the information presented.

Its use is intended to be voluntary for the user.

---

### The EUDI Wallet is explicitly provided for payments

The European Commission documents a use case entitled **Payment Authentication** enabling the EUDI Wallet to be used to authenticate online or in-store payments [S29].

This architecture is designed to work with existing payment infrastructures, notably card payments and account-to-account payments.

The wallet therefore does not necessarily itself constitute the system transferring the funds.

It acts as a component notably enabling the payer to be authenticated and the evidence necessary for the transaction to be presented.

The general operation can be summarized as follows:

```
user
   ↓
EUDI Wallet
   ↓
presentation of evidence or an attestation
   ↓
bank / PSP / acquirer / merchant
   ↓
payment authentication
```

**ESTABLISHED:**

> A European digital identity infrastructure is explicitly designed to be able to intervene directly in the payment authentication process [S29].

---

### The wallet can be linked to a payer and an account

The documentation notably provides for strong authentication attestations issued by payment service providers [S29].

These attestations make it possible to establish a verifiable link between:

- the wallet;  
- a specific payer;  
- and a specific payment account or instrument.

When a payment is initiated, the wallet can present the appropriate attestation to the party responsible for verifying it, for example a bank, an acquirer or a merchant.

**ESTABLISHED:**

> The EUDI Wallet can therefore act as a cryptographically verifiable component linking the user to the authentication of a payment transaction and to the instrument or account concerned [S29].

This does not mean that all identity information contained in the wallet is transmitted with each payment.

---

### Selective disclosure makes it possible to present an attribute without transmitting the entire identity

The EUDI Wallet architecture notably relies on a principle of selective disclosure [S29].

The user can present only the information necessary for a given interaction rather than their entire identity or the entire document containing that information.

The Commission notably provides the following examples:

- age;  
- residence;  
- certain information from a driving licence [S29].

In a purchase scenario subject to an age requirement, the system can therefore verify that the user meets the required criterion without necessarily receiving their full date of birth.

The principle can be represented as follows:

```
wallet containing verifiable information
   ↓
selection of the necessary attribute
   ↓
proof of the required criterion
   ↓
verifying service or merchant
```

**ESTABLISHED:**

> The infrastructure therefore technically enables an attribute relating to a person to be verified in the context of a payment without requiring the transmission of their entire identity [S29].

---

### Age already constitutes a concrete example of a criterion associated with a purchase

The official documentation specifically provides the example of a purchase requiring age verification [S29].

In the flow presented by the Commission, the user makes an online purchase and uses their EUDI Wallet in the authentication process.

The wallet notably displays the merchant, the amount and the requested attributes.

The user can then present the necessary proof.

**ESTABLISHED:**

> A verifiable personal attribute originating from the digital identity infrastructure can therefore already be integrated into the technical flow surrounding a payment in order to verify a condition applicable to the purchase [S29].

It is, however, essential to distinguish this mechanism from a conditional payment within the meaning examined in Sections 4.5 and 4.6.

In this example, age verification responds to a requirement related to access to or the sale of the product; it does not constitute evidence that the digital euro itself applies a purchase restriction.

---

### The connection with the digital euro is explicitly provided for

The relationship between the EUDI Wallet and the digital euro is not merely a possibility resulting from the existence of two compatible European infrastructures.

The ECB documentation relating to the digital euro pilot explicitly states this [S29].

PSPs participating in the pilot will be able to support the EUDI Wallet as a strong authentication method for online transactions when the user uses the PSP's digital instruments.

PSPs remain free to choose their authentication methods, subject to compliance with the applicable regulatory requirements.

**ESTABLISHED:**

> The use of the EUDI Wallet as an authentication method in the digital euro pilot is explicitly provided for by the European Central Bank [S29].

The following connection is therefore officially documented:

```
EUDI Wallet
   ↓
strong authentication
   ↓
PSP
   ↓
digital euro payment
```

This connection is stronger than the hypothetical connections examined with other infrastructures: it is directly described by the ECB for the pilot.

---

### European pilots have already experimented with identity and payment

The use of the EUDI Wallet in payments has also been the subject of European Large Scale Pilots [S29].

European projects have notably tested:

- payment initiation;  
- strong authentication;  
- online payments;  
- in-store payments;  
- age verification associated with a payment.

**ESTABLISHED:**

> The connection between European digital identity and payment infrastructure has therefore moved beyond the stage of a mere conceptual specification: it has already been the subject of European pilots [S29].

These experiments do not, however, constitute evidence of a generalized system automatically linking all identity information to all transactions.

---

### The same infrastructure can present different types of attestations

The EUDI Wallet is not limited to basic civil identity.

Its architecture makes it possible to store and present different types of attestations issued by trusted sources.

This means that the same technical mechanism can be used to present different attributes depending on the service concerned.

**TECHNICALLY DEDUCIBLE:**

> A payment infrastructure using the EUDI Wallet for authentication or verification does not necessarily need to access all the data held by the wallet: it can request and receive only the attestation or attribute necessary for the process concerned.

From an architectural perspective, this logic is comparable to that examined for conditional payments: the component making a decision does not necessarily need to hold all the source data when the system can present it with verifiable proof.

---

### The identity → payment connection is established, but its scope must be delimited

At this stage, the following chain can be considered documented:

```
verifiable attribute or identity
   ↓
EUDI Wallet
   ↓
presentation of proof
   ↓
PSP / bank / acquirer / merchant
   ↓
authentication or verification necessary for the payment process
```

And, within the digital euro pilot:

```
EUDI Wallet
   ↓
strong authentication
   ↓
PSP participating in the pilot
   ↓
digital euro transaction
```

**ESTABLISHED:**

> There is therefore an explicitly provided institutional and technical connection between the European digital identity infrastructure and payment infrastructures, including within the digital euro pilot [S29].

---

### This connection does not mean that a complete profile accompanies each payment

The existence of this connection should not lead to the conclusion that all data held in the EUDI Wallet is automatically communicated to the PSP or merchant.

On the contrary, the wallet's design is based on principles of data minimization and selective disclosure [S29].

A verification may, for example, concern only whether a person meets an age requirement.

**NOT ESTABLISHED:**

> The sources examined do not establish that all attributes held in an EUDI Wallet can be accessed by a bank, PSP, merchant or the Eurosystem during a payment.

**NOT ESTABLISHED:**

> Nor do they establish that a general purchase history is recorded in the EUDI Wallet for individual profiling purposes.

---

### The combination with conditional payments must be distinguished from authentication

Sections 4.5 and 4.6 established that external data can contribute to the verification of a condition triggering a conditional payment.

The present section establishes that an identity wallet can provide verifiable proof within the payment process.

These two mechanisms are technically compatible in principle, but their systematic combination has not been demonstrated.

**TECHNICALLY DEDUCIBLE:**

> A verifiable attestation provided by an identity infrastructure can technically constitute one of the pieces of information used by an external service to verify that a condition necessary for an operation has been met.

The example of age verification already shows that an individual attribute can be involved in a commercial process associated with a payment.

**NOT ESTABLISHED:**

> This does not demonstrate that an environmental, tax, social or behavioral attribute can currently be imposed as a general condition for using the digital euro.

---

### The connection with the other infrastructures remains to be established

The previous chapters have now separately identified several mechanisms:

**Chapter 1**  
structured data relating to transactions and invoicing

**Chapter 3**  
identifiable products and structured environmental data

**Chapter 4.5–4.6**  
external systems and conditions that can contribute to the automated execution of a payment

**Chapter 4.7**  
verifiable identity or attribute that can directly contribute to the payment process

The separate existence of these four elements still does not demonstrate their overall interconnection.

It does, however, progressively reduce the number of purely hypothetical connections.

The connection:

> **digital identity → payment infrastructure**

is now **ESTABLISHED** [S29].

The connection:

> **EUDI Wallet → payment authentication in the digital euro pilot**

is also **ESTABLISHED** [S29].

The connection:

> **external system → condition → automated execution of a payment**

was established in the previous sections [S27][S28].

By contrast, the connection:

> **invoicing data / DPP / environmental data → individual attribute → condition applied to a payment**

remains **TO BE ESTABLISHED**.

---

### Interim conclusion

**ESTABLISHED:**

> The EUDI Wallet is explicitly designed to be used for the authentication of online and in-store payments [S29].

**ESTABLISHED:**

> Attestations issued notably by PSPs can establish a verifiable link between a wallet, a payer and a payment account or instrument [S29].

**ESTABLISHED:**

> The architecture enables the selective presentation of certain personal attributes, notably age or residence, without necessarily transmitting the user's entire identity [S29].

**ESTABLISHED:**

> European pilots have already experimented with payments using the EUDI Wallet, including scenarios combining payment and age verification [S29].

**ESTABLISHED:**

> The ECB explicitly provides for PSPs participating in the digital euro pilot to be able to use the EUDI Wallet as a strong authentication method for online payments [S29].

**TECHNICALLY DEDUCIBLE:**

> Verifiable proof or an attribute originating from an identity infrastructure can technically be used in a verification process surrounding a transaction without all the source data being communicated to the payment system.

**NOT ESTABLISHED:**

> None of the elements examined establish that the EUDI Wallet is currently intended to provide an environmental, tax or behavioral profile used to authorize or refuse digital euro payments.

**TO BE ESTABLISHED:**

> What attributes other than those currently documented for authentication may be requested in future payment services using the EUDI Wallet?

**TO BE ESTABLISHED:**

> Under what legal conditions may a merchant, bank, PSP or other service request the presentation of an attribute before the execution of a transaction?

**TO BE ESTABLISHED:**

> Are there European infrastructures or projects enabling attestations held in an identity wallet to be linked to invoicing, product or environmental data?

---

## 4.8 Limitations and safeguards provided

**Status: ESTABLISHED / ONGOING PROJECT / TO BE ESTABLISHED**

The previous sections established that the architecture envisaged for the digital euro includes significant technical capabilities: structured processing of transactions, involvement of multiple providers, funds reservation, conditional payments, use of information originating from external systems and the possibility of using a digital identity infrastructure in the payment process [S22][S24][S25][S27][S28][S29].

These capabilities cannot, however, be analyzed independently of the legal and technical safeguards provided to limit their use.

A distinction must notably be made between:

- what is explicitly prohibited;  
- what is made more difficult by the architecture;  
- what remains possible but is regulated by law;  
- and what would depend on a future change to the legal framework.

---

### The digital euro must not be programmable money

The most explicit safeguard concerns the programmability of money.

The proposed regulation excludes the digital euro being designed as money intrinsically subject to conditions limiting its use to certain goods, services, locations, persons or periods [S22].

This prohibition is also consistently affirmed by the European Central Bank [S23][S27].

**ESTABLISHED:**

> The Eurosystem must not be able to assign rules to certain digital euro units determining the goods or services for which they can be spent [S22][S23][S27].

A digital euro unit must remain fungible with other units.

This safeguard therefore prohibits a scenario in which the money itself would carry, for example, a rule such as:

"this unit cannot be used to purchase this product."

---

### This prohibition does not eliminate conditional payments

As established in 4.5 and 4.6, the prohibition of programmable money does not eliminate the possibility of building conditional services around payments [S27][S28].

The legal and technical distinction is fundamental:

**restriction attached to the money** → explicitly excluded

**condition attached to a transaction or service** → provided for in the architecture

**ESTABLISHED:**

> The safeguard against programmable money therefore does not prohibit all automated logic surrounding the execution of a payment [S22][S27].

This is precisely why the governance of the conditionality layer is important.

---

### Conditions are presented as having to be agreed between the parties

In the model presented by the ECB, conditional payments correspond to services in which the conditions are determined or accepted by the parties to the transaction [S27].

The Eurosystem provides the monetary infrastructure necessary for settlement and funds reservation but is not presented as the actor defining the commercial criteria enabling their release.

**ESTABLISHED:**

> Under the framework currently presented, the Eurosystem does not have a general power enabling it to define the goods or services that a user can purchase using the digital euro [S22][S27].

This safeguard is important.

It does not, however, fully answer another question:

**can a criterion become mandatory because it results not from the ECB but from a legal or regulatory obligation applicable to the PSP, merchant or user?**

This question then concerns less the monetary design than the law applicable to the actor executing the payment.

**TO BE ESTABLISHED:**

> Under what conditions could a rule external to the monetary system legally require a PSP or another intermediary to verify a criterion before executing a transaction?

---

### PSPs already have control and non-execution capabilities

The existence of non-programmable money does not mean that a payment service provider is technically required to execute every transaction presented to it.

As established in 4.2, PSPs remain subject to various regulatory obligations concerning notably:

- anti-money laundering and counter-terrorist financing;  
- sanctions and embargoes;  
- fraud prevention;  
- security;  
- certain tax obligations [S22][S24].

In certain circumstances provided for by law, these obligations may result in an operation being prevented, suspended or refused.

**ESTABLISHED:**

> The prohibition of programmable money therefore does not amount to an absolute technical or legal impossibility of blocking a transaction: control and non-execution mechanisms already exist where a legal basis provides for them [S22][S24].

The central question is therefore not only:

"can the payment be blocked?"

but also:

"who has the power to block it, for what reason and on what legal basis?"

---

### Holding limits are provided for

The proposed regulation also provides for the possibility of applying limits to the amount of digital euros that a user can hold [S22].

These limits are notably intended to preserve financial stability and prevent an excessive migration of bank deposits to central bank money.

PSPs participate in the application of these limits.

Mechanisms are also provided to verify that a user holding several digital euro accounts cannot circumvent the applicable overall limit [S22].

**ESTABLISHED:**

> The architecture therefore already provides for quantitative rules that can be automatically verified and applied to digital euro holdings [S22].

These limits concern the **holding** of digital euros and not the nature of the goods or services purchased.

They therefore do not constitute a restriction on consumption.

---

### The infrastructure can verify a rule without knowing its full context

The verification of holding limits nevertheless illustrates a technical principle already encountered in the previous sections.

Several components can cooperate to determine that a rule is satisfied without each of them having all the information relating to the user.

This logic is consistent with that of conditional payments and digital identity:

```
data or attribute
   ↓
verification of a rule
   ↓
result usable by another component
```

**TECHNICALLY DEDUCIBLE:**

> The architecture therefore enables the automated application of certain rules without requiring a single actor to centralize all the data used to verify them.

This characteristic constitutes both a technical capability and, when based on pseudonymization or selective disclosure, a data protection mechanism.

---

### The ECB must not be able to directly identify users from central data

The proposed regulation provides that data communicated to the ECB and national central banks must be organized in such a way as not to enable them to directly identify users [S22].

The architecture notably provides for separation, pseudonymization and cryptographic protection mechanisms.

As established in 4.3, PSPs nevertheless retain the relationship with their customers and hold the information necessary for that relationship as well as for compliance with their regulatory obligations [S22][S25].

**ESTABLISHED:**

> The current design therefore seeks to prevent the Eurosystem's central infrastructure from directly constituting a complete nominative database of individual payments [S22][S23].

This does not mean that no actor in the chain can identify the user.

The protection relies precisely on a **distribution of information among different actors**.

---

### Data separation constitutes a safeguard, but not an absence of processing

Pseudonymization does not mean that transactions cease to exist or become technically impossible to process.

It means that certain components use identifiers that do not directly enable the person concerned to be identified.

PSPs, in parallel, have the relationship enabling them to identify their own customers.

**ESTABLISHED:**

> The architecture therefore relies more on a separation of knowledge and responsibilities than on the complete absence of data [S22][S25].

This distinction is important for the analysis of interconnections.

A distributed system can enable multiple forms of processing without a single central database containing all the information.

---

### Offline mode constitutes the strongest architectural protection

The offline mode examined in 4.4 constitutes a different situation [S23][S26].

The personal details of the payment are designed to remain on the payer's and beneficiary's devices and not be transmitted to PSPs or the Eurosystem.

**ESTABLISHED:**

> Under the architecture currently envisaged, offline mode therefore prevents the central infrastructure from systematically processing the individual details of each offline transaction [S23][S26].

This protection constitutes a much greater technical obstacle to centralized matching than the mere pseudonymization of an online transaction.

Funding and defunding operations nevertheless remain visible to the PSP and subject to the corresponding regulatory controls.

---

### Data minimization is also provided for digital identity

The EUDI Wallet notably relies on selective disclosure [S29].

When a service needs to verify an attribute, the objective is to transmit only the necessary information.

For example:

"user over 18 years old: YES"

may be sufficient without transmitting the full date of birth.

**ESTABLISHED:**

> The interconnection between digital identity and payment therefore does not necessarily imply the transmission of the user's entire identity profile [S29].

This architecture limits the amount of data exposed.

It nevertheless also confirms that a decision can technically be based on a personal attribute without the system making that decision knowing all the data used to produce the proof.

---

### The safeguards rely partly on law and can therefore evolve with it

A fundamental distinction must be made between a technical impossibility and a legal prohibition.

Certain safeguards are deeply embedded in the architecture, notably the protection of offline mode.

Others rely on rules defining authorized purposes, access rights, PSP obligations or categories of permitted processing.

**TECHNICALLY DEDUCIBLE:**

> When a technical capability exists but its use is prohibited or limited by law, the safeguard depends on the continued existence of the legal framework governing that capability.

This does not mean that this framework is intended to be modified.

It simply means that a legal prohibition should not be presented as a technical impossibility.

This distinction is essential throughout this investigation.

---

### The current safeguards prevent several excessive conclusions

Based on the sources examined, it would be incorrect to claim that:

- the ECB will be able to arbitrarily decide what a citizen can purchase;  
- the digital euro will intrinsically include a carbon quota;  
- each monetary unit will be restrictable to certain products;  
- the ECB will necessarily have a complete nominative history of purchases;  
- DPP data will automatically be transmitted with each payment;  
- the EUDI Wallet will automatically transmit all personal attributes during a transaction;  
- offline payments will enable centralized tracking identical to online payments.

**NOT ESTABLISHED:**

> None of the elements examined demonstrate the current existence of a system capable of assigning an environmental quota to a person and then automatically blocking their purchases when that quota is reached.

---

### But the safeguards do not eliminate the documented technical capabilities

Conversely, it would also be incorrect to conclude that the prohibition of programmable money makes any automated decision surrounding a payment technically impossible.

The previous sections separately established:

```
structured and identifiable transactions [S25]
   ↓
funds reservation [S27]
   ↓
conditionality layer external to the Eurosystem [S27][S28]
   ↓
possible verification of events originating from external systems [S27][S28]
   ↓
market actor platforms connected through APIs in the experiments [S28]
   ↓
verifiable identity and attributes that can contribute to the payment process [S29]
```

**ESTABLISHED:**

> The safeguards surrounding the digital euro limit the authorized uses of these capabilities but do not eliminate the existence of the technical components enabling automation, condition verification and interaction with external systems [S22][S27][S28][S29].

---

### The central question therefore shifts to governance

After examining the safeguards, the question is no longer merely whether the infrastructure technically possesses the components enabling certain operations to be automated or conditioned.

Some of these components are now documented.

The question becomes:

```
who can define the rule?
   ↓
on what legal basis?
   ↓
based on what data?
   ↓
with what consent or obligation?
   ↓
which actor verifies the condition?
   ↓
which actor has the ability to act on the transaction?
```

This distinction between **technical capability** and **legal authority** will need to remain central in the chapters devoted to interconnections and legal safeguards.

---

### Interim conclusion

**ESTABLISHED:**

> The digital euro proposal prohibits programmable money in the sense of monetary units intrinsically carrying restrictions relating to the goods, services, locations, persons or periods for which they may be used [S22][S27].

**ESTABLISHED:**

> This prohibition does not prevent conditional payments, which rely on logic applied to a transaction or service rather than to the money itself [S27][S28].

**ESTABLISHED:**

> PSPs remain able and, in certain situations, legally required to perform controls that may result in the non-execution of a transaction, notably in the areas of fraud, sanctions and anti-money laundering [S22][S24].

**ESTABLISHED:**

> Digital euro holding limits can be defined and applied automatically, but they concern the amount held and not the categories of goods that can be purchased [S22].

**ESTABLISHED:**

> The architecture provides for a separation between the identity known to PSPs and the pseudonymized information processed by the central infrastructure, while offline mode benefits from stronger protection preventing the central transmission of personal transaction details [S22][S23][S26].

**ESTABLISHED:**

> The EUDI Wallet notably relies on data minimization and selective disclosure of the necessary attributes [S29].

**TECHNICALLY DEDUCIBLE:**

> Legal safeguards governing a technical capability must not be confused with the absence of that technical capability.

**NOT ESTABLISHED:**

> None of the elements examined establish the existence of a current mechanism assigning an individual environmental quota and then using that quota to authorize or refuse payments.

**TO BE ESTABLISHED:**

> To what extent do the rules governing conditional payments legally prevent a condition from being imposed other than through the voluntary agreement of the payer and the beneficiary?

**TO BE ESTABLISHED:**

> Could a regulation external to the digital euro framework legally require a PSP, merchant or other intermediary to verify an attribute or condition before executing a transaction?

**TO BE ESTABLISHED:**

> What legal safeguards prevent data originating from other digital infrastructures from being used as decision-making criteria in a payment service?

**TO BE ESTABLISHED:**

> Which safeguards arise directly from the technical architecture and which depend primarily on a legal framework that may evolve?

---

## 4.9 What this chapter establishes

The analysis of the digital euro shows that it is not merely a new means of payment reproducing the functioning of cash in digital form.

The project relies on a structured infrastructure involving the Eurosystem, payment service providers, acceptance devices, common services and various interfaces enabling market actors to develop complementary services [S22][S23][S24].

The technical documents and experiments examined also establish several important capabilities concerning data, payment automation and interaction with external systems.

These capabilities must, however, be distinguished from uses that are actually authorized or currently deployed.

---

### A centralized settlement infrastructure is provided for

**ESTABLISHED:**

> The digital euro is designed as central bank money whose settlement relies on a centralized infrastructure operated by the Eurosystem and distributed to users through payment service providers [S22][S23][S24].

This architecture does not rely on a blockchain or DLT infrastructure as the foundation of the system [S23].

The user primarily maintains a relationship with their PSP, while the Eurosystem performs the central functions necessary for settlement and the operation of the infrastructure.

---

### Online payments produce structured data

**ESTABLISHED:**

> The technical model currently published provides for structured data relating to users, accounts, devices, providers, payers, beneficiaries and transactions [S25].

Transactions notably have identifiers, an amount, a date and time, a type, an environment and a status.

Certain information also makes it possible to characterize the commercial context.

The Merchant Category Code notably makes it possible to categorize the merchant's activity and is among the information provided for in certain payment flows [S25].

This does not mean that the infrastructure systematically knows the exact product purchased or the detailed contents of the basket.

---

### Data is distributed among several actors

**ESTABLISHED:**

> The architecture does not provide for a single actor to necessarily have all the information relating to a transaction [S22][S24][S25].

PSPs know their customers in accordance with their obligations.

The central infrastructure notably uses pseudonymized identifiers and mechanisms intended to prevent the Eurosystem from directly identifying users from the information it receives [S22][S23].

The presence of data somewhere in the chain therefore does not mean that it is accessible to all participants.

---

### Offline mode constitutes a distinct architecture

**ESTABLISHED:**

> The digital euro is also designed to enable offline payments executed directly between the payer's and beneficiary's devices without real-time intervention by the central infrastructure [S23][S26].

Under the model currently presented, the personal details of these transactions remain on the devices and are accessible neither to the Eurosystem nor to PSPs.

This architecture therefore constitutes an important limitation on the possibility of systematically matching offline payments with other data at a central level.

---

### The digital euro must not be programmable money

**ESTABLISHED:**

> The proposed regulation and the European Central Bank explicitly exclude money whose units would intrinsically carry restrictions determining the goods, services, locations, beneficiaries or periods for which they may be used [S22][S23][S27].

The digital euro must remain fungible.

Under the framework currently proposed, this safeguard therefore excludes a mechanism in which certain monetary units would be directly programmed to prohibit the purchase of a category of products.

---

### Conditional payments are, however, explicitly provided for

**ESTABLISHED:**

> The prohibition of programmable money does not prevent the existence of conditional payments whose execution depends on predetermined conditions [S27].

The infrastructure notably provides for a functionality enabling funds to be reserved and then transferred when the corresponding condition is considered satisfied.

The ECB therefore distinguishes between:

**programming the money** → excluded  
**programming the conditions surrounding a transaction** → provided for

This distinction constitutes one of the central findings of the chapter.

---

### Conditional logic can be located outside the Eurosystem

**ESTABLISHED:**

> The ECB describes a separation between a settlement layer provided by the Eurosystem and a conditionality layer that can be developed by banks, PSPs and other market actors [S27][S28].

The external layer can verify that an event or condition has been satisfied and then use the functions provided by the infrastructure to continue processing the payment.

The Eurosystem therefore does not necessarily need to know all the data used to verify that condition.

---

### An external event can contribute to the execution of a payment

**ESTABLISHED:**

> The ECB's work provides for external monitoring to be able to trigger a condition used by a conditional payment service [S27].

The examples examined notably include:

- confirmation of a delivery;  
- actual use of a service;  
- completion of a milestone;  
- certain events related to transport;  
- machine-to-machine interactions [S27][S28].

The following general principle is therefore established:

```
external system or event
   ↓
verification of a condition
   ↓
conditional service
   ↓
action on the transaction
```

---

### This mechanism has been experimented

**ESTABLISHED:**

> Market actors have connected their own platforms through APIs to an environment simulating the digital euro interfaces in order to experiment with conditional services and payments [S28].

PSPs and other participants were able to develop conditional logic on top of the fundamental functionalities provided by the simulated environment.

The generic bridge between an **external system** and the **conditional processing of a payment** therefore no longer constitutes merely a theoretical architectural possibility.

It has been the subject of technical experiments.

---

### External data do not necessarily need to enter the monetary infrastructure

**TECHNICALLY DEDUCIBLE:**

> An external system can perform a verification based on its own data and then communicate only the result necessary for the conditional service.

The operation can therefore be:

```
data held in an external system
   ↓
verification of a rule
   ↓
verification result
   ↓
conditional service
   ↓
execution or non-execution of the transaction
```

This architecture means that a potential interconnection does not necessarily require the creation of a central database bringing together all the information concerned.

---

### Digital identity also has an explicit connection with payment

**ESTABLISHED:**

> The EUDI Wallet is designed to be able to contribute to payment authentication and present verifiable attestations or attributes to the actors concerned [S29].

The architecture notably enables the selective disclosure of an attribute without necessarily transmitting the user's entire identity.

Age verification already constitutes a documented example of an attribute that can contribute to a commercial process associated with a payment.

---

### The connection between the EUDI Wallet and the digital euro is explicitly provided for

**ESTABLISHED:**

> The ECB provides for PSPs participating in the digital euro pilot to be able to use the EUDI Wallet as a strong authentication method for online payments [S29].

The following chain is therefore directly documented:

```
digital identity or attestation
   ↓
EUDI Wallet
   ↓
PSP
   ↓
authentication
   ↓
digital euro payment
```

The connection between European digital identity and payment infrastructure therefore does not constitute merely a theoretical possibility.

---

### Several previously separate capabilities can now be represented together

The findings of this chapter make it possible to represent the following general architecture:

```
User
   ↓
verifiable identity / attribute
   ↓
PSP or payment service
   ↓
structured and identifiable transaction
```

in parallel:

```
external system
   ↓
verifiable data or event
   ↓
conditionality layer
```

then:

```
funds reservation
   ↓
condition satisfied or not satisfied
   ↓
settlement or absence of settlement
```

**ESTABLISHED:**

> Each of the main components of this chain is documented in the architecture or in the experiments examined [S22][S24][S25][S27][S28][S29].

**TECHNICALLY DEDUCIBLE:**

> These components technically make it possible to build services in which information originating from an external system contributes to an automated decision concerning a specific transaction, without making the money itself programmable.

---

### The connection with environmental data remains the missing link

Chapter 3 separately established:

- the existence of the Digital Product Passport;  
- the digital identification of products;  
- the possibility of associating certain structured environmental data with these products;  
- the existence of methods enabling certain environmental footprints to be quantified;  
- interoperability mechanisms, APIs and registries;  
- the technical possibility of matching a transaction with an identifiable product when the necessary identifiers and access rights exist [S15][S18][S19][S20][S21].

Chapter 4 now separately establishes:

- the existence of structured payment transactions;  
- funds reservation;  
- conditional payments;  
- an external conditionality layer;  
- the possible use of information originating from external systems;  
- APIs enabling market actor platforms to interact with the payment environment;  
- and an explicit connection between digital identity and payment [S25][S27][S28][S29].

The technical combination can therefore be represented as follows:

```
identifiable product
   ↓
external data associated with the product
   ↓
system capable of verifying a rule
   ↓
verification result
   ↓
conditionality layer
   ↓
transaction
   ↓
execution or non-execution
```

**TECHNICALLY DEDUCIBLE:**

> If environmental data relating to a product were made accessible to an authorized service and if that data became a valid criterion for a payment condition, the architecture examined would technically enable the result of that verification to be used to act on the execution of a transaction without programming the money itself.

---

### This specific connection is not, however, established

**NOT ESTABLISHED:**

> None of the elements examined in this chapter demonstrate that data originating from a Digital Product Passport, a GTIN, a carbon footprint, electronic invoicing data or an individual environmental footprint are currently used as a condition for authorizing, refusing or modifying a digital euro payment.

Nor is it established that a French or European administration has a mechanism enabling an individual environmental quota to be automatically applied to a person's purchases.

The technical possibility resulting from the combination of several components must therefore not be presented as an existing or officially planned use.

---

### The current safeguards must be incorporated into this conclusion

Several safeguards currently prevent an interpretation according to which the digital euro would directly constitute a general tool for controlling purchases:

- prohibition of programmable money [S22][S27];  
- payment conditions presented as agreed between the parties [S27];  
- pseudonymization and separation of the information accessible to the Eurosystem [S22][S23];  
- minimization and selective disclosure in the EUDI Wallet [S29];  
- enhanced privacy for offline payments [S23][S26].

**ESTABLISHED:**

> The framework currently proposed therefore does not give the Eurosystem a general power enabling it to arbitrarily determine the goods and services that a user is authorized to purchase.

---

### These safeguards must not be confused with a technical impossibility

The same sources establish, in parallel, the existence of:

- controls that may lead to the non-execution of certain transactions where a legal basis provides for them;  
- quantitative rules automatically applied to holdings;  
- conditional payments;  
- external services capable of verifying conditions;  
- APIs enabling interaction with market platforms;  
- verifiable identity attributes that can be used in the payment process [S22][S24][S27][S28][S29].

**TECHNICALLY DEDUCIBLE:**

> The current prohibition of certain uses therefore does not necessarily mean that the infrastructure would be technically incapable of implementing a comparable rule if a legal basis and the corresponding access rights existed.

The distinction between **technical capability** and **legal authority** thus constitutes one of the main conclusions of this chapter.

---

## Conclusion of Chapter 4

The analysis makes it possible to rule out two opposing conclusions.

The first would be to claim that the digital euro already constitutes programmable money enabling an authority to control individual purchases.

**The sources examined do not support this claim.**

The second would be to claim that the architecture makes it technically impossible to use external data or conditions in the execution of a payment.

**The sources examined establish, on the contrary, that such mechanisms exist in the envisaged architecture and have already been the subject of experiments.**

The result can therefore be formulated as follows:

**ESTABLISHED:**

> The digital euro is not designed as programmable money.

**ESTABLISHED:**

> The infrastructure is nevertheless designed to support conditional payments.

**ESTABLISHED:**

> The logic determining a condition can be developed outside the Eurosystem by market actors.

**ESTABLISHED:**

> Information or an event originating from an external system can contribute to the verification of a condition.

**ESTABLISHED:**

> External platforms have already been connected through APIs to an environment simulating the digital euro in order to experiment with these mechanisms.

**ESTABLISHED:**

> European digital identity has an official connection with payment infrastructures and its use is explicitly provided for in the digital euro pilot.

**TECHNICALLY DEDUCIBLE:**

> Information originating from a distinct infrastructure can be verified externally and then used in the form of a result within a conditional service without the source data necessarily being integrated into the monetary infrastructure.

**TECHNICALLY DEDUCIBLE:**

> The components examined would therefore technically enable data relating to a product or another external characteristic to be used as a criterion for a conditional transaction if an authorized actor had access to that data and a basis permitting its use.

**NOT ESTABLISHED:**

> None of the elements examined currently demonstrate the use of a DPP, carbon data, electronic invoicing data or an individual environmental profile as a criterion for authorizing or refusing a payment.

**TO BE ESTABLISHED:**

> Are there actors, projects, standards, infrastructures, calls for tenders or experiments concretely linking electronic invoicing, Digital Product Passport, digital identity and payment systems?

**TO BE ESTABLISHED:**

> Are there identifiers, APIs or intermediary infrastructures enabling information to circulate or be verified between these different systems?

**TO BE ESTABLISHED:**

> Are actors participating in the development of the digital euro also involved in DPP, electronic invoicing or environmental data processing infrastructures?

**TO BE ESTABLISHED:**

> Do European projects currently under development explicitly provide for interoperability between these different infrastructures, even when their initial purposes remain distinct?