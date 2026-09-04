# Chapter 1 — Invoicing Data Transmitted to the Administration

> **Navigation:** [← Back to the table of contents](#documentation)

This first chapter documents the invoicing, transaction and payment data transmitted to the administration as part of the French electronic invoicing reform.

The purpose of this repository is to document, based on official sources, the data collected, transmitted and processed as part of the French electronic invoicing reform.

The objective is not to present as established future uses that have not been established.

The method consists of documenting each component of the system separately, then examining the technical and legal possibilities for cross-referencing or further development of these infrastructures.

Each element is classified according to four levels:

- **ESTABLISHED**: explicitly established by an official source.  
- **TECHNICALLY DEDUCIBLE**: made possible by the architecture or available data, without a corresponding officially established use.  
- **HYPOTHESIS**: potential scenario requiring additional evidence to be demonstrated.  
- **TO BE ESTABLISHED**: identified question for which the sources examined do not yet allow a sufficiently solid conclusion to be drawn.

---

## Table of Contents

- [1.1 — The principle of transmission](#11-the-principle-of-transmission-is-officially-established)  
- [1.2 — Role of the Public Invoicing Portal](#12-role-of-the-public-invoicing-portal)  
- [1.3 — Domestic B2B data](#13-domestic-b2b-invoicing-data-transmitted-to-the-administration)  
- [1.4 — International B2B e-reporting](#14-international-b2b-e-reporting)  
- [1.5 — Specific case of B2C](#15-specific-case-of-b2c)  
- [1.6 — Payment data](#16-payment-data)  
- [1.7 — Transmission architecture](#17-transmission-architecture)  
- [1.8 — Conclusion of the first chapter](#18-what-this-first-chapter-establishes)

---

# 1. Transmission of invoicing data to the administration

## 1.1 The principle of transmission is officially established

**Status: ESTABLISHED**

The French electronic invoicing reform does not merely replace paper or PDF invoices with electronic documents.

It also organizes the transmission of data to the tax administration.

The DGFiP distinguishes three mechanisms:

1. electronic invoicing between businesses concerned;  
2. electronic transmission of transaction data;  
3. electronic transmission of payment or receipt data.

As part of electronic invoicing, approved platforms extract from the invoice the regulatory data intended for the administration [S1].

For transactions subject to e-reporting, transaction or payment data are also transmitted to the administration [S2][S3].

---

## 1.2 Role of the Public Invoicing Portal

**Status: ESTABLISHED**

Following the refocusing of the Public Invoicing Portal (PPF), it notably retains a role as a central hub for transmitting invoicing and transaction data to the tax administration [S4].

The architecture can therefore be represented, in simplified form, as follows:

```
Business
   ↓
Approved platform
   ↓
Extraction / transmission of regulatory data
   ↓
Public Invoicing Portal
   ↓
Tax administration
```

The PPF is therefore not merely a directory enabling invoice routing.

It also constitutes a point of concentration for data intended for the administration [S4].

---

## 1.3 Domestic B2B invoicing data transmitted to the administration

**Status: ESTABLISHED**

The DGFiP publishes a summary table of the invoice data that must be transmitted to the administration for domestic transactions carried out between two VAT-liable businesses established in France [S1].

These data are introduced progressively in two stages.

### From September 1, 2026

| Data                                                   | Granularity |
|--------------------------------------------------------|-------------|
| Supplier's SIREN                                       | Invoice     |
| Supplier's country of establishment                    | Invoice     |
| Customer's SIREN                                       | Invoice     |
| Customer's country of establishment                    | Invoice     |
| Transaction category: goods, services or both          | Invoice     |
| Issue date                                             | Invoice     |
| Unique invoice number                                  | Invoice     |
| Amount excluding VAT by VAT rate                       | Invoice     |
| VAT amount by rate                                     | Invoice     |
| Applicable VAT rate                                    | Invoice     |
| Total amount excluding VAT                             | Invoice     |
| Total VAT amount                                       | Invoice     |
| Currency                                               | Invoice     |

Depending on the transaction, other information must also be transmitted:

- supplier's intra-Community VAT number;  
- customer's intra-Community VAT number;  
- identification of any tax representative;  
- reference to the initial invoice in the event of a correction;  
- option for payment of VAT on debits;  
- reason for VAT exemption;  
- self-billing;  
- special VAT scheme;  
- reverse charge;  
- membership of a VAT group;  
- actual date of delivery of the goods or performance of the service;  
- date of payment of a deposit in the situations provided for.

### From September 1, 2027

The granularity of the data transmitted increases.

The following notably become mandatory:

| Data                                                           | Granularity                     |
|----------------------------------------------------------------|---------------------------------|
| Precise description of the goods supplied or services provided | Invoice line                    |
| Quantity of goods or services                                  | Invoice line                    |
| Unit price excluding VAT                                       | Invoice line                    |
| Discounts, rebates and reductions                              | Line or document, as applicable |
| Fees and charges, for example transport costs                  | Line or document, as applicable |
| Delivery address when different from the customer's address    | Line or document, as applicable |
| Date of the corrected invoice                                  | Invoice                         |
| Early payment discount information                             | Invoice                         |
| Eco-contribution                                               | Line or document, as applicable |

From September 1, 2027, the administration therefore no longer receives only accounting and tax totals for domestic B2B invoices.

The regulatory transmission also includes information identifying the precise nature of the goods or services invoiced, their quantity and their unit price excluding VAT [S1].

---

## 1.4 International B2B e-reporting

**Status: ESTABLISHED**

Transactions carried out with a VAT-liable business not established in France are also subject to data transmission to the administration [S2].

From September 1, 2026, the information transmitted includes, in particular:

- identification of the French business;  
- identification of the foreign business, notably through its intra-Community VAT number or a foreign identifier where one exists;  
- supplier's country;  
- customer's country;  
- transaction category;  
- invoice date;  
- invoice number;  
- amount excluding VAT by VAT rate;  
- VAT amount by rate;  
- VAT rates;  
- total amount excluding VAT;  
- total VAT amount;  
- currency.

Depending on the transaction, other tax or transaction-related data are also transmitted.

From September 1, 2027, the following are notably added:

- precise description of the goods or services;  
- quantity;  
- unit price excluding VAT;  
- price reductions;  
- fees and charges;  
- delivery address in the cases provided for;  
- certain information relating to corrective invoices;  
- eco-contribution.

The line-by-line granularity provided for certain data in 2027 therefore also applies to international B2B transactions falling within the scope of e-reporting.

---

## 1.5 Specific case of B2C

**Status: ESTABLISHED**

The processing of transactions carried out with non-taxable persons, particularly individuals, must be distinguished from B2B.

For these transactions, the DGFiP currently provides for aggregated transmission on a daily basis.

For each category of transactions concerned, the following are notably transmitted:

- date of the day;  
- total taxable amount excluding VAT for the day's transactions;  
- corresponding VAT amount;  
- breakdown by VAT rate where several rates apply.

The documented regulatory framework therefore does not support the conclusion that, under the general B2C e-reporting framework, the administration receives individual details of each product purchased by each individual.

This distinction is essential:

**B2B: data that may reach invoice-line level from 2027.**

**B2C: transaction data currently provided in aggregated form on a daily basis [S2].**

This distinction must be preserved in any subsequent analysis.

---

## 1.6 Payment data

**Status: ESTABLISHED**

The reform also includes e-reporting of payments for transactions where VAT becomes chargeable upon receipt of payment, notably certain supplies of services [S3].

The data transmitted include:

- the date of actual receipt of payment;  
- the amount received;  
- the breakdown of the amount by VAT rate where necessary.

Where an electronic invoice exists, the transmission may be linked to it through its “paid” status.

The information then includes, in particular:

- the invoice number;  
- the payment date;  
- the amount received by VAT rate.

For certain international B2B transactions without the submission of an electronic invoice, payment data are also transmitted on an invoice-by-invoice basis.

For B2C, payment data follow the same logic as transaction e-reporting: they are aggregated on a daily basis.

---

## 1.7 Transmission architecture

**Status: ESTABLISHED**

Version 3.2 of the external specifications describes the Public Invoicing Portal as a central hub [S4].

Its role includes the centralization of:

- invoicing data;  
- transaction data;  
- payment data;  
- certain information relating to the invoice life cycle.

These data are then transmitted to the tax administration.

The architecture can therefore be represented in simplified form as follows:

```
Business
   ↓
Approved platform
   ↓
Regulatory data
   ↓
Public Invoicing Portal
   ↓
Tax administration
```

The complete invoice and the regulatory data transmitted to the administration must not be confused.

The administration receives the data provided for by the applicable legislation and specifications.

---

## 1.8 What this first chapter establishes

**Status: ESTABLISHED**

At this stage, the official documents establish that the reform creates a national infrastructure enabling the automated collection and transmission of structured economic data to the tax administration.

These data notably make it possible to identify:

- the businesses participating in a transaction;  
- the date and number of the invoice;  
- the general nature of the transaction;  
- amounts excluding VAT;  
- VAT rates and amounts;  
- certain information relating to delivery;  
- certain information relating to payment.

From September 1, 2027, for the B2B transactions concerned, this granularity also includes:

- the precise description of the goods or services;  
- their quantity;  
- their unit price excluding VAT.

It is therefore established that, for the B2B transactions concerned, the infrastructure enables structured data precisely describing the economic content of certain invoice lines to be transmitted to the administration.

However, the documents examined at this stage do not establish:

- that every purchase made by an individual is individually transmitted to the administration;  
- that an individual consumption profile is created;  
- that these data are currently used to calculate an individual carbon footprint;  
- that they are cross-referenced with environmental data;  
- that they are linked to a payment system or a digital currency;  
- that a mechanism for individually restricting purchases is planned.