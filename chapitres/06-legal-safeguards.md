# Chapter 6 — Legal Safeguards

> **Navigation:** [← Back to the table of contents](#documentation)

The previous chapters identified the data collected, the infrastructures concerned and several documented possibilities or mechanisms for interconnection between invoicing, taxation, products, environmental data, digital identity and payment.

However, the existence of a technical capability for interconnection does not mean that its use is legally authorized.

This chapter therefore examines the legal safeguards that may regulate, limit or prohibit certain processing operations or data cross-referencing identified during the investigation.

The analysis notably examines:

- the legal bases enabling processing;  
- the purposes for which data may be collected and reused;  
- the principle of purpose limitation;  
- the principle of data minimization;  
- the conditions applicable to cross-referencing data originating from different systems;  
- the rules relating to profiling and automated decision-making;  
- the rights of data subjects;  
- transparency obligations;  
- retention and access rules;  
- the powers and positions of supervisory authorities, notably the CNIL;  
- the requirements of necessity and proportionality;  
- any specific safeguards provided for digital identity, the DPP and payment infrastructures;  
- the possibilities and conditions for future changes to purposes or legal bases.

The objective is not to presume that a violation exists.

It is to determine, for each capability identified in the previous chapters, whether current law:

> **explicitly authorizes it;**

> **authorizes it under certain conditions;**

> **limits it;**

> **appears to prohibit it;**

> **or does not yet allow a conclusion to be reached.**

Particular attention will be paid to the difference between a protection established in current law and a technical impossibility.

A legal rule may currently limit processing that the architecture would technically enable.

Conversely, the existence of a technical infrastructure does not make it possible to presume that a legal development authorizing new uses will subsequently occur.

The chapter will therefore seek to identify both existing protections and their limitations, without transforming the possibility of legal evolution into an established institutional intention.

---

## Table of contents

- [6.1 — Applicable legal framework](#61-applicable-legal-framework)  
- [6.2 — Purposes of processing and data reuse](#62-purposes-of-processing-and-data-reuse)  
- [6.3 — Data cross-referencing, matching and interconnection](#63-data-cross-referencing-matching-and-interconnection)  
- [6.4 — Profiling and automated decision-making](#64-profiling-and-automated-decision-making)  
- [6.5 — Necessity, proportionality and minimization](#65-necessity-proportionality-and-minimization)  
- [6.6 — Data subject rights and CNIL oversight](#66-data-subject-rights-and-cnil-oversight)  
- [6.7 — Safeguards specific to the infrastructures examined](#67-safeguards-specific-to-the-infrastructures-examined)  
- [6.8 — Evolution of purposes and the legal framework](#68-evolution-of-purposes-and-the-legal-framework)  
- [6.9 — Legal vulnerabilities and limitations of the analysis](#69-legal-vulnerabilities-and-limitations-of-the-analysis)  
- [6.10 — What this chapter establishes](#610-what-this-chapter-establishes)

---

## 6.1 Applicable legal framework

**Status: ESTABLISHED LEGAL SAFEGUARDS / IDENTIFIED POINTS OF VIGILANCE**

The previous chapters focused primarily on the existence of the data, their circulation and the possibilities for interconnection between different infrastructures.

Chapter 6 raises a different question:

> **is the fact that processing is technically feasible and pursues an objective of general interest sufficient to make it legally permissible?**

The answer is no.

Several levels of law govern the processing operations examined.

---

### The GDPR applies to personal data used within the system

The General Data Protection Regulation applies when information relates to an identified or identifiable natural person [S36].

Not all data contained in an invoice therefore necessarily constitute personal data.

An invoice concerning a company may mainly contain information relating to a legal entity.

However, invoicing systems may also contain information that makes it possible to identify natural persons directly or indirectly.

This point is no longer merely theoretical with regard to the use of data originating from the reform for tax purposes.

The CNIL explicitly describes data originating from electronic invoicing and added to the CFVR processing system as **personal data collected** [S37].

**ESTABLISHED:**

> At least some of the data originating from the electronic invoicing reform fall within the scope of personal data protection.

The system therefore does not fall outside the GDPR merely because it primarily concerns economic transactions between businesses.

---

### The reform has a legal basis

A first argument must immediately be ruled out.

The transmission of data to the administration is not implemented without a legal basis.

It results notably from the French General Tax Code and from legislative and regulatory provisions governing electronic invoicing and e-reporting.

The decree governing the system itself explicitly refers to the GDPR and was adopted after consultation with the CNIL [S38].

**INSUFFICIENT ARGUMENT:**

> "The collection is mandatory and carried out without consent, therefore it necessarily violates the GDPR."

The GDPR does not rely solely on consent.

Processing may notably be based on a legal obligation or be necessary for the performance of a task carried out in the public interest provided for by law [S36].

The absence of consent from the businesses or persons concerned is therefore not, in itself, sufficient to make the reform unlawful.

---

### The existence of a legal basis does not, however, grant an unlimited right of use

This is where a first important legal distinction appears.

The GDPR requires data to be:

> collected for specified, explicit and legitimate purposes;

and:

> not further processed in a manner incompatible with those purposes [S36].

It also requires data to be:

> adequate, relevant and limited to what is necessary in relation to the purposes for which they are processed [S36].

Therefore:

```
legal basis
   ≠
general authorization for reuse
```

and:

```
legally mandatory collection
   ≠
unlimited ability to cross-reference data for any future public policy
```

**ESTABLISHED LEGAL SAFEGUARD:**

> Any subsequent reuse of personal data must remain compatible with the applicable legal framework, notably the purposes and the principles of necessity, proportionality and minimization.

This distinction becomes particularly important in light of the interconnections examined in Chapter 5.

---

### An important finding: invoicing data do in fact feed an algorithmic tax-targeting system

Chapter 2 had left open the question of the automated processing actually applied to data originating from the reform.

The documentation published in 2026 now makes it possible to provide a precise answer.

The CNIL examined the integration of data originating from electronic invoicing into the automated **CFVR — fraud targeting and query enhancement** processing system [S37].

This development was subsequently incorporated into the regulatory framework by the Order of 10 July 2026 amending the order establishing CFVR [S45].

Data originating from electronic invoicing are therefore now among the categories of data integrated into the CFVR system.

The CNIL further states that part of the CFVR data, together with data originating from electronic invoicing, are to feed the DGFiP's secure data platform so that they can be processed there, notably because of their volume [S37].

It notes that:

> their addition substantially increases the volume of data processed;

and that the volume concerned is approximately:

> **2 to 3 billion electronic invoices per year** [S37].

The results produced by the processing carried out on this platform can then feed CFVR and be cross-referenced with other information in order to contribute notably to the identification of anomalies and businesses presenting certain tax risks [S37].

**ESTABLISHED:**

> The integration of data originating from electronic invoicing into the CFVR processing system is now based on an adopted regulatory text [S45].

**ESTABLISHED:**

> These data are intended to be processed on a large scale within the DGFiP's data analysis infrastructure for purposes related to tax control and targeting [S37][S45].

**ESTABLISHED LEGAL SAFEGUARD:**

> This integration does not exempt the processing carried out from the applicable principles of purpose limitation, minimization, security, necessity and proportionality [S36][S43][S44].

---

### The data are cross-referenced with other analysis results

The CNIL opinion provides a second important element.

The data processed on the platform are intended to produce results that can be cross-referenced with other information used by CFVR in order to obtain, notably, lists of businesses considered to present certain tax risks [S37].

The CNIL also indicates that, ultimately, all data from the CFVR processing system are intended to feed the secure data platform.

The actually documented chain therefore becomes:

```
electronic invoicing data
   ↓
DGFiP secure data platform
   ↓
algorithmic processing
   ↓
cross-referencing with other data / results
   ↓
anomaly detection
   ↓
identification of businesses presenting certain risks
   ↓
possible targeting of tax audits
```

**ESTABLISHED:**

> The cross-referencing and automated analysis of data originating from electronic invoicing with other tax information are no longer merely a technical possibility.

They form part of the documented uses of the CFVR system [S37].

---

### The processing extends beyond businesses alone

The history of CFVR described by the CNIL is also worth noting.

Initially developed for business taxpayers, the system was subsequently extended to natural persons involved in the operation of businesses, and then to private individuals [S37].

This does not mean that every piece of electronic invoicing data will be associated with every individual.

But it demonstrates that the analytical infrastructure into which these data are now being integrated is not inherently limited to legal entities alone.

**POINT OF VIGILANCE:**

> The large-scale integration of data originating from electronic invoicing into an infrastructure that already uses different categories of data relating to professionals and natural persons reinforces the importance of rules governing purpose limitation, minimization, authorization and proportionality.

---

### Exchanges with other administrations are also documented

The same CNIL deliberation describes exchanges between the DGFiP and social security bodies within the framework of CFVR [S37].

These exchanges have a specific legal basis and are limited to certain purposes.

The CNIL considers these purposes legitimate under the legal framework currently provided for.

**ESTABLISHED:**

> Legal mechanisms already enable certain administrative data to circulate between public bodies for specified purposes.

However, the CNIL specifically emphasizes:

- data minimization;  
- restriction to authorized agents;  
- the need-to-know principle;  
- the retention period;  
- information provided to data subjects;  
- the proportionality of exchanges [S37].

This observation is essential for the remainder of the investigation.

**ESTABLISHED LEGAL SAFEGUARD:**

> Interconnection between administrations is not legally unrestricted: it must be based on a legal basis and comply with specified purposes and safeguards.

---

### First area of vulnerability: the progressive expansion of purposes

The reform is initially based notably on tax-related objectives: modernization of VAT collection, combating fraud, pre-filling and improving knowledge of economic activity.

The use of data for tax targeting therefore has a direct connection with several stated purposes.

**INSUFFICIENT ARGUMENT AT THIS STAGE:**

> The current use of invoicing data by CFVR necessarily constitutes purpose diversion.

The sources examined do not support this conclusion.

Combating fraud and tax control are precisely part of the framework within which this processing is organized.

However, the issue would become legally much more sensitive if the same data were subsequently reused for a substantially different purpose.

For example:

```
collection for a tax purpose
   ↓
retention of a detailed transaction infrastructure
   ↓
reuse for another public policy
   ↓
cross-referencing with other categories of data
```

Such a development would have to be examined in light of purpose limitation, its legal basis, necessity and proportionality [S36][S43].

**POTENTIAL VULNERABILITY:**

> The technical capability to reuse data does not constitute a legal basis allowing new purposes to be freely assigned to them.

---

### Second area of vulnerability: data volume and proportionality

The CNIL itself notes the substantial increase in the volume of data caused by the integration of electronic invoicing into CFVR [S37].

The announced volume reaches several billion invoices per year.

However, case law relating to the protection of privacy and personal data requires a balance to be struck between:

> the objective of general interest pursued

and:

> the nature, scope and sensitivity of the data processed, as well as the seriousness of the interference [S39][S44].

The relevant legal question is therefore not simply:

> "is combating fraud a legitimate objective?"

It is.

The question is:

> **"are the precise scope of the data collected, their level of detail, their retention period, their cross-referencing and the ways in which they are processed necessary and proportionate to that objective?"**

It is on this ground that legal scrutiny becomes genuinely relevant.

---

### Third area of vulnerability: data protection by design and by default

The principle of minimization does not apply solely to the initial choice of categories of data collected.

Article 25 of the GDPR also requires the controller to implement technical and organizational measures enabling the effective application of data protection principles by design and by default [S43].

The Regulation specifies that this requirement notably concerns:

- the amount of personal data collected;  
- the extent of their processing;  
- their retention period;  
- their accessibility.

This provision is particularly relevant to an infrastructure expected to process several billion electronic invoices per year and enable their processing within a platform with significant computing capabilities [S37].

The legal question therefore does not concern only the existence of a legal basis allowing the integration of the data.

It also concerns the concrete design of the infrastructure:

> what data are actually necessary?

> for how long?

> for what processing operations?

> accessible to which agents?

> with what level of granularity?

> and what measures technically prevent their use beyond the authorized purposes?

The CNIL specifically requires the secure data platform to maintain strict segregation, that the data transferred to it be processed solely for the intended purposes and that its use not provide access to new recipients who were not originally provided for [S37].

**ESTABLISHED LEGAL SAFEGUARD:**

> The GDPR requires data protection and minimization to be integrated into the very design of the processing and that, by default, only the data necessary for each specific purpose be processed [S43].

**POINT OF VIGILANCE:**

> An increase in technical storage, computing or cross-referencing capabilities does not in itself constitute justification for expanding the data accessible or the processing carried out.

**LEGAL QUESTION TO BE DOCUMENTED:**

> Do the technical and organizational measures actually implemented in CFVR and in the secure data platform demonstrate, with regard to data originating from electronic invoicing, the effective application of the principles of data minimization and data protection by design and by default?

---

### Fourth area of vulnerability: access control

The CNIL also emphasizes the need to restrict access to a limited number of agents and strictly on a need-to-know basis [S37].

It requires the secure platform to:

> maintain strict segregation of data;

> allow their processing only for the intended purposes;

> not provide access to new recipients who were not originally provided for.

This requirement is particularly important for our investigation.

It means that an infrastructure technically capable of hosting several categories of data cannot legally become a general-purpose environment for data reuse without a new legal framework.

**ESTABLISHED LEGAL SAFEGUARD:**

> The segregation of purposes and access currently constitutes a legally significant safeguard against generalized data reuse.

**POINT OF VIGILANCE:**

> Any extension of the categories of persons with access, the purposes or the data being cross-referenced must be examined separately in order to determine whether the existing legal basis and safeguards remain sufficient.

---

### A fundamental distinction emerges

The result of this initial analysis differs from two extreme positions.

It would be legally incorrect to claim:

> **"The reform violates the GDPR because the data are transmitted without consent."**

A legal basis exists, and consent is not the only basis on which processing may be carried out.

But it would also be incorrect to claim:

> **"Since the collection is provided for by law, the administration can then do whatever it wishes with the data."**

The GDPR and constitutional and European requirements for the protection of privacy continue to govern:

- the purposes;  
- the categories of data;  
- their necessity;  
- their proportionality;  
- their retention;  
- their recipients;  
- their cross-referencing;  
- automated decisions;  
- security measures.

---

### First legal conclusion

**ESTABLISHED:**

> The reform is based on a legal and regulatory framework and has been subject to consultation with the CNIL.

**ESTABLISHED:**

> Data originating from electronic invoicing include personal data subject to the safeguards of the GDPR.

**ESTABLISHED:**

> These data are intended to feed a DGFiP infrastructure enabling their large-scale algorithmic processing for tax targeting.

**ESTABLISHED:**

> The CNIL itself notes a substantial increase in data volume and identifies risks relating to minimization, access, retention, security, algorithmic bias and automation.

**ESTABLISHED:**

> Certain exchanges and cross-referencing between administrations are legally possible when provided for by law and when their purposes are specified.

**ESTABLISHED LEGAL SAFEGUARD:**

> Legally established data collection does not permit unlimited reuse of the data for any purpose.

**POTENTIAL VULNERABILITY:**

> Any substantial extension of the purposes, categories of data, recipients or matching mechanisms must be able to satisfy the requirements of a legal basis, necessity, minimization and proportionality.

**TO BE ESTABLISHED:**

> The exact scope of the safeguards surrounding each processing operation resulting from the reform and the possibility of legally challenging certain extensions or methods of processing must be examined in the following sections.

---

### What 6.1 changes in the investigation

An element that remained partially unresolved in the earlier chapters can now be clarified.

The following chain is documented:

```
electronic invoicing
   ↓
personal and economic data on a very large scale
   ↓
DGFiP secure data platform
   ↓
algorithmic processing
   ↓
cross-referencing / analysis
   ↓
anomaly detection and tax targeting
   ↓
possible human decision to initiate an audit
```

The legal question is therefore no longer whether invoicing data **can technically be processed and cross-referenced on a large scale**.

Such processing is now documented in the tax domain.

The question becomes:

> **how far can this processing legally go before it encounters the principles of purpose limitation, minimization, necessity, proportionality and protection against certain automated decisions?**

It is this boundary that the following sections must seek to identify.

---

## 6.2 Purposes of processing and data reuse

**Status: ESTABLISHED LEGAL SAFEGUARDS / IDENTIFIED LEGAL LATITUDE / BOUNDARIES TO BE ESTABLISHED**

The principle of purpose limitation constitutes one of the main legal safeguards applicable to the architectures examined in the previous chapters.

But its scope must be described precisely.

An overly simplistic interpretation would be to consider that:

> **"any new use of data for a purpose different from the one stated when it was collected is prohibited."**

The GDPR does not establish such an absolute prohibition.

On the contrary, it provides several mechanisms allowing, under certain conditions, certain further processing operations [S36][S43][S46].

---

### A purpose must be specified, explicit and legitimate

The initial principle remains clear.

Personal data must be collected for specified, explicit and legitimate purposes and must not be further processed in a manner incompatible with those purposes [S36][S43].

This rule prevents, in principle, an infrastructure established for a specific purpose from becoming, solely by virtue of its technical existence, a general repository of data that can be used for any future purpose.

It therefore requires a distinction between:

```
technical capability for reuse
   ↓
legally defined purpose
   ↓
legal basis
   ↓
necessity / proportionality
   ↓
authorized processing
```

The first step is never sufficient to demonstrate the subsequent ones.

**LEGAL SAFEGUARD:**

> The technical availability of data does not, in itself, constitute a purpose or a legal basis allowing its use.

---

### A new purpose is not, however, automatically prohibited

Article 6(4) of the GDPR explicitly provides for cases in which data are further processed for a purpose other than the one that justified their initial collection [S46].

Where such further processing is based neither on the data subject's consent nor on a relevant provision of Union or Member State law, the controller must notably determine whether the new purpose is compatible with the initial purpose.

The Regulation provides several criteria for this assessment:

- the link between the initial purpose and the further purpose;  
- the context in which the data were collected;  
- the nature of the data;  
- the possible consequences of the new processing for the individuals concerned;  
- the safeguards implemented, notably encryption or pseudonymization [S46].

There is therefore, in legal terms, a:

> **purpose compatibility test.**

**LEGAL LATITUDE:**

> Data collected for a specified purpose may, under certain conditions, be subject to further processing compatible with that purpose.

This means that:

```
new use
   ≠
automatic illegality
```

But also that:

```
new use
   ≠
automatic compatibility
```

Compatibility must be assessed in light of the processing actually envisaged.

---

### A second route exists: intervention through law

Article 6(4) reveals a second important possibility for this investigation.

The compatibility test mechanism it describes concerns cases in which further processing is not based, notably, on Union or Member State law constituting a necessary and proportionate measure in a democratic society to safeguard the objectives referred to in Article 23 of the GDPR [S46].

In other words, the evolution of uses does not depend solely on compatibility with the initial purpose.

The law may also provide a framework for certain new processing operations or certain restrictions under the conditions laid down by the GDPR.

**LEGAL LATITUDE:**

> The legal framework may evolve and permit certain further processing operations that do not rely solely on compatibility with the initial purpose.

This latitude is fundamental to the analysis of the architectures examined in this repository.

An existing technical infrastructure may currently be legally limited to certain purposes, without that limitation necessarily constituting a definitive legal impossibility.

A change in the law could modify the processing operations that are authorized.

This does not, however, make it possible to presume that such a change will occur.

---

### The tax domain explicitly benefits from this latitude

This possibility is not purely abstract in the domain examined.

Article 23 of the GDPR expressly provides that Union or national law may, under certain conditions, restrict the scope of several obligations and rights provided for by the Regulation in order to safeguard certain important objectives of general public interest [S47].

The areas explicitly mentioned notably include:

- important economic or financial interests;  
- monetary matters;  
- budgetary matters;  
- taxation matters;  
- social security;  
- certain monitoring, inspection or regulatory functions connected to the exercise of official authority [S47].

This possibility remains subject to conditions.

The measure must notably:

> respect the essence of fundamental rights and freedoms;

and:

> be necessary and proportionate in a democratic society [S47].

**LEGAL SAFEGUARD:**

> The GDPR does not authorize a general and uncontrolled restriction of rights in the name of tax interests.

**LEGAL LATITUDE:**

> The GDPR explicitly provides for the possibility for the legislature to adjust certain safeguards or rights where tax objectives or monitoring functions justify it, subject notably to the requirements of necessity and proportionality.

---

### This latitude is already being used within the CFVR framework

The connection with the investigation becomes particularly concrete in the Order of 10 July 2026 amending CFVR [S45][S47].

This Order:

- integrates data originating from electronic invoicing among the data processed;  
- extends or specifies several data sources used by the system;  
- organizes certain access and data transfers;  
- and explicitly refers to points (e) and (h) of Article 23(1) of the GDPR [S45][S47].

This is therefore not merely a theoretical possibility contained in the European regulation.

The current regulatory framework governing CFVR already makes use of the legal mechanisms allowing certain restrictions in the context of taxation and monitoring functions.

**ESTABLISHED:**

> The CFVR legal framework explicitly refers to the possibilities for restriction provided for by Article 23 of the GDPR for certain objectives of general public interest and certain monitoring functions [S45][S47].

---

### The law can therefore shift the boundary without removing all safeguards

This observation leads to an important distinction.

It would be incorrect to write:

> **"The purposes stated today definitively prohibit any new future use."**

The law can evolve.

It would be equally incorrect to write:

> **"It is sufficient to adopt a new legal text to make any use of the data legally possible."**

New provisions remain subject to the applicable higher-ranking legal norms.

Depending on the circumstances, these may notably include:

- the GDPR;  
- the Charter of Fundamental Rights of the European Union;  
- the right to respect for private life;  
- the necessity test;  
- the proportionality test;  
- the principle of minimization;  
- the safeguards applicable to data subjects [S39][S43][S44][S46][S47].

The actual boundary is therefore not:

```
possible
   /
impossible
```

but rather:

```
currently authorized use
   ↓
envisaged extension
   ↓
possible compatibility
   or
new legal basis
   ↓
necessity test
   ↓
proportionality test
   ↓
applicable safeguards
```

---

### First legal vulnerability: progressive expansion may be lawful

This conclusion reveals a particular vulnerability.

It does not necessarily result from a violation of the law.

On the contrary, it results from the ability of the law to progressively expand the scope of authorized processing.

An infrastructure may therefore successively undergo:

```
purpose A
   ↓
compatible extension A → A+
   ↓
new legal basis
   ↓
extension towards B
   ↓
new authorized cross-referencing
```

Each step may be legally regulated and yet, over time, lead to an architecture whose scope is much broader than when it was created.

**LEGAL VULNERABILITY:**

> Purpose limitation constitutes a safeguard against incompatible reuse that lacks a sufficient legal basis, but it does not guarantee that the legal scope of processing will remain unchanged.

**IMPORTANT:**

> This possibility of evolution demonstrates neither that a particular extension is envisaged nor that it would be legally permissible.

It demonstrates only that:

> **the legal boundary can evolve without requiring modification of the technical architecture already available.**

---

### Second vulnerability: the accumulation of extensions

The legal analysis of an extension is generally carried out in relation to a specific processing operation and purpose.

However, the investigation also examines the cumulative effect of several infrastructures and successive developments.

A succession of individually justified extensions may progressively increase:

- the amount of data available;  
- the number of sources;  
- the number of possible cross-references;  
- the number of recipients;  
- the period during which certain information remains usable;  
- the capacity for profiling or analysis.

The question then becomes:

> **at what point does the cumulative effect of several legally grounded extensions sufficiently alter the nature or intensity of the processing to require a new assessment of necessity and proportionality?**

**TO BE ESTABLISHED:**

> To what extent does the applicable law require the proportionality of not only each extension considered individually, but also the architecture resulting from their accumulation, to be reassessed?

This question must be considered alongside the analyses of necessity, proportionality and impact examined in the following sections.

---

### An essential boundary for the interconnections examined in Chapter 5

This analysis also makes it possible to preserve an essential methodological boundary regarding the chains examined previously.

Chapter 5 identified several technical or experimental capabilities connecting notably:

```
transaction
   ↓
product
   ↓
DPP
   ↓
environmental data
```

as well as:

```
external data
   ↓
condition
   ↓
conditional payment
```

The existence of the further processing mechanism provided for by the GDPR does not make it possible to transform these technical possibilities into legally authorized uses.

Nor does it make it possible to conclude that a future legal basis will be created to connect them.

**NOT ESTABLISHED:**

> No element examined in this section establishes that environmental data from the DPP can currently be used to determine the authorization, refusal or limitation of a payment.

**LEGALLY DEDUCIBLE:**

> If such an interconnection involving personal data were to be implemented, its compliance would have to be examined in light of its purpose, its legal basis and the applicable safeguards, as well as, depending on the mechanism used, the requirements of necessity, proportionality and minimization.

This distinction prevents confusion between:

```
legally possible evolution in theory
   ↓
   and
legally authorized use today
```

---

### Conclusion of 6.2

**ESTABLISHED:**

> The GDPR prohibits further processing incompatible with the initial purposes where no other relevant legal basis permits the processing [S36][S43][S46].

**ESTABLISHED:**

> The GDPR provides a mechanism for assessing the compatibility of a further purpose with the initial purpose [S46].

**ESTABLISHED:**

> Union or national law may also provide for certain restrictions or processing operations under the conditions laid down by the GDPR, notably for important objectives in the field of taxation and for certain monitoring functions [S46][S47].

**ESTABLISHED:**

> The CFVR framework as amended in July 2026 explicitly refers to points (e) and (h) of Article 23(1) of the GDPR [S45][S47].

**LEGAL SAFEGUARD:**

> An extension of uses does not become lawful merely because it is technically possible or pursues an objective of general interest.

**LEGAL LATITUDE:**

> The law nevertheless permits certain compatible forms of reuse and may evolve the scope of authorized processing, subject to the applicable conditions and safeguards.

**LEGAL VULNERABILITY:**

> Purpose limitation protects against certain forms of reuse, but does not permanently freeze the legal scope of a data infrastructure.

**TO BE ESTABLISHED:**

> How far can successive extensions of purposes, data sources and recipients accumulate before their overall effect requires a new assessment of necessity and proportionality?

**NOT ESTABLISHED:**

> Nothing in the sources examined here demonstrates that a legal development is currently envisaged to connect environmental data from the DPP to the authorization, refusal or limitation of a payment.

---

## 6.3 Data cross-referencing, matching and interconnection

**Status: ESTABLISHED INTERCONNECTIONS / DOCUMENTED SAFEGUARDS / IDENTIFIED VULNERABILITIES AND BLIND SPOTS**

The previous chapters showed that several of the infrastructures examined have cross-referencing or interconnection capabilities.

In the tax domain, this issue is now no longer merely technical.

The CFVR processing system already constitutes an architecture fed by numerous data sources and enabling their analysis or cross-referencing [S37][S45].

The legal issue therefore becomes twofold:

> **which interconnections are actually authorized?**

and:

> **what safeguards prevent a large-scale data-matching infrastructure from itself becoming a disproportionate source of risk, notably in the event of compromise, misuse or expanded access?**

---

### CFVR already constitutes a multi-source infrastructure

The Order amending CFVR in July 2026 is not limited to adding data originating from electronic invoicing [S45].

The processing system is fed by numerous other sources.

The regulatory list notably includes data originating from:

- tax records;  
- tax returns;  
- withholding tax;  
- property and housing occupancy data;  
- inheritances;  
- bank account details declared by tax households;  
- cross-border payments recorded in CESOP;  
- intra-EU VAT;  
- exchanges of goods within the European Union;  
- processing systems relating to vehicle tax clearance certificates;  
- data processing systems originating from social security bodies;  
- publicly accessible data collected from certain online platforms;  
- and, now, electronic invoicing [S45].

The Order also provides for data concerning natural persons that are necessary for certain work relating to the intensity of economic activity [S45].

**ESTABLISHED:**

> CFVR is not a database limited solely to data originating from electronic invoicing.

It constitutes an analytical infrastructure fed by a much broader range of tax, economic and administrative sources and, in certain cases, data relating to natural persons.

---

### Cross-referencing is a documented function of the system

The CNIL explicitly describes the intended processing of the new electronic invoicing data [S37].

Part of the CFVR data, together with data originating from electronic invoicing, are intended to feed the DGFiP's secure data platform.

The results of queries performed on this platform can then be cross-referenced with data originating from CFVR in order to obtain, notably, lists of businesses considered to present certain risks.

Ultimately:

> **all CFVR data are intended to feed this platform** [S37].

The documented chain therefore becomes:

```
multiple administrative / tax sources
   ↓
CFVR
   ↓
electronic invoicing data
   +
other CFVR data
   ↓
secure data platform
   ↓
queries / models / analyses
   ↓
cross-referencing of results
   ↓
anomaly detection
   ↓
selection of cases presenting certain risks
```

**ESTABLISHED:**

> The matching of multiple datasets constitutes an actual and legally organized function of CFVR [S37][S45].

It is therefore no longer merely a technically conceivable interconnection.

---

### Exchanges between administrations further broaden the scope

The documented interconnections also extend beyond the DGFiP alone.

Article L. 152 of the French Tax Procedures Code allows certain exchanges between the tax administration and social security bodies.

The CFVR system has been adapted accordingly [S37][S45].

Data may be transmitted to social security bodies for certain tasks relating to the verification of the basis for social security contributions.

Conversely, certain data communicated by these bodies may also feed CFVR.

The CNIL notably mentions information relating to:

- undeclared work;  
- remuneration;  
- the results of tax audits [S37].

**ESTABLISHED:**

> There is therefore a legally organized two-way flow of data between the tax administration and certain social security bodies.

This flow is based on a legal basis and specified purposes.

---

### The scope of persons with access to the system is also evolving

The July 2026 Order provides for several categories of authorized agents who may access the data necessary for modelling and visualization work [S45].

These notably include agents belonging to:

- the national data analysis network;  
- interregional programming structures;  
- certain specialized national services;  
- departmental public finance directorates;  
- the National Directorate of Tax Investigations.

Useful results are also accessible, on a need-to-know basis, to certain agents responsible for case management, programming and auditing, as well as to certain authorized agents of social security bodies [S45].

The CNIL indicates that members of the national network must be individually authorized, trained and supervised, and that certain queries may be approved or rejected by the competent office [S37].

**LEGAL AND ORGANIZATIONAL SAFEGUARD:**

> Access is not presented as being indiscriminately open to all public officials.

It is based on authorizations and must be limited to the need-to-know principle [S37][S45].

---

### Large-scale cross-referencing is itself a recognized risk factor

This architecture must, however, be considered in light of the criteria used by the CNIL for data protection impact assessments.

The criteria used to identify processing operations likely to result in a high risk notably include:

- large-scale processing;  
- matching or combining datasets;  
- evaluation or scoring;  
- the use of innovative technologies or methods [S49].

CFVR publicly exhibits several characteristics corresponding to these criteria:

```
massive volume
   +
data cross-referencing
   +
analysis / targeting
   +
algorithmic methods
```

The CNIL itself notes that the arrival of electronic invoicing **substantially** increases the volume of data processed and refers to several billion invoices per year [S37].

**MAJOR POINT OF VIGILANCE:**

> The simultaneous increase in data volume, the number of sources and matching capabilities increases not only the analytical power of the system, but also the potential consequences of an error, misuse or compromise.

---

### First vulnerability: concentration increases the potential impact of a compromise

A database or platform capable of matching numerous categories of data presents a different risk from several strictly segregated databases.

A compromise would not necessarily affect only a single isolated piece of information.

Depending on the access actually obtained, it could make it possible to match several categories of information.

The GDPR specifically requires the level of security to be appropriate to:

- the nature of the data;  
- their scope;  
- the context of the processing;  
- the likelihood of the risk;  
- its severity [S48].

Here, the CNIL goes much further than a general statement.

In its opinion concerning CFVR, it explicitly notes:

> the massive volume of data;

> their sensitivity;

> the evolution of the threat;

> and the evolution of cyberattack methods [S37].

**LEGAL AND TECHNICAL VULNERABILITY:**

> The more the architecture concentrates data, sources and matching capabilities, the higher the level of security that can reasonably be required.

This does not mean that CFVR is currently compromised or insufficiently secured.

It means that:

> **the change in scale also changes the level of risk over which the administration must be able to demonstrate effective control.**

---

### The CNIL itself calls for enhanced protection against compromised access

The CNIL opinion provides a particularly concrete element here [S37].

It welcomes the ministry's commitment to systematically implement:

- two-factor authentication;  
- access only from secure devices.

However, the CNIL goes further regarding connection and activity logs.

It considers that logging should be accompanied by mechanisms enabling notably:

- proactive analysis of events;  
- detection of unexpected behavior;  
- generation of alerts;  
- immediate blocking of the accounts concerned until doubts have been resolved by management [S37].

**DOCUMENTED SAFEGUARD:**

> Two-factor authentication and the use of secure devices are the subject of a commitment by the ministry that was positively noted by the CNIL.

**DOCUMENTARY BLIND SPOT:**

> In its opinion published in 2026, the CNIL specifically calls on the ministry to implement proactive mechanisms for log analysis, alerts and account blocking in the event of unexpected behavior.

The public sources examined here do not yet make it possible to establish whether all of these recommended mechanisms have actually been deployed across all the environments concerned.

**TO BE ESTABLISHED:**

> Have the proactive detection and blocking mechanisms requested by the CNIL since been effectively deployed, with what coverage and according to what procedures?

This is a very concrete question that can be addressed to the administration.

---

### Second vulnerability: the risk does not arise solely from an external attack

The security of an infrastructure of this nature does not concern only a hacker gaining access from the Internet.

Article 32 of the GDPR also covers risks of unauthorized access or disclosure [S48].

Access control therefore becomes fundamental.

An infrastructure bringing together:

```text
more data
   +
more sources
   +
more analyses
   +
several categories of persons with access
```

mechanically increases the number of situations in which an incorrect authorization, a compromised account, a misconfiguration or misuse could have significant consequences.

This is precisely why the CNIL emphasizes:

- limiting the number of agents;  
- individual authorization;  
- the strict need-to-know principle;  
- supervision;  
- logging;  
- behavioral analysis [S37][S50].

**VULNERABILITY:**

> The security of the system depends not only on protecting its IT perimeter but also on the ongoing quality of identity management, access authorizations and the detection of abnormal use.

---

### Third vulnerability: interconnection expands the trust surface

Exchanges with other administrations add another dimension.

The CNIL notes the use of a secure file-transfer tool with state-of-the-art encryption for exchanges with social security bodies [S37].

This is an important safeguard.

But an interconnection necessarily creates several environments involved:

```
organization A
   ↓
transfer mechanism
   ↓
organization B
```

Overall security therefore no longer depends solely on the original infrastructure.

It also depends on:

- the authorizations within each organization;  
- the security of each organization's equipment;  
- any copies that may be created;  
- retention periods;  
- effective deletion;  
- logging;  
- the ability to detect abnormal use or transfer.

**DOCUMENTED SAFEGUARD:**

> Exchanges between the DGFiP and social security bodies must use a secure and encrypted transfer mechanism [S37].

**STRUCTURAL VULNERABILITY:**

> Any increase in the number of recipients or environments in which the data are accessible expands the surface across which confidentiality, integrity and access-control safeguards must be maintained.

This is not evidence of a current weakness in any particular organization.

It is a consequence of the distributed architecture itself.

---

### A very concrete blind spot emerges regarding the retention of exchanged data

The CNIL opinion contains a particularly noteworthy observation concerning exchanges with social security bodies [S37].

The Commission notes that the draft Order submitted to it:

> **did not specify the retention period for data transmitted as part of these exchanges.**

It then reiterates that exchanges between administrations are permitted only if their arrangements remain proportionate to the objectives pursued and emphasizes the need to limit retention to the period necessary [S37].

**IDENTIFIED DOCUMENTARY BLIND SPOT:**

> The text submitted to the CNIL did not itself determine the retention period for data transferred between the DGFiP and social security bodies.

This does not demonstrate that the data are retained without limit.

Retention periods may be provided for in other legal texts, agreements, internal policies or recipient processing systems.

But this raises a legally verifiable question:

**TO BE ESTABLISHED:**

> For each category of data transferred between CFVR and social security bodies, what is the maximum retention period applicable at the recipient organization, by which legal text or document is it determined, and how is its effective deletion monitored?

This point may be far more relevant than a general criticism of data retention.

---

### Fourth vulnerability: a change in risk may require a new assessment

The GDPR contains a mechanism that is particularly relevant for monitoring the evolution of this type of architecture.

Article 35 provides that, where a data protection impact assessment exists, the controller must review whether the processing remains compliant with that assessment when there is a change in the risk [S48].

Several transformations are now documented:

- the arrival of a new massive category of data;  
- several billion additional invoices;  
- the use of an infrastructure with enhanced computing capabilities;  
- cross-referencing with other information;  
- the development of new learning methods;  
- organizational expansion of the analysis network;  
- new relationships with social security bodies [S37][S45].

**MAJOR LEGAL QUESTION:**

> Have these developments been incorporated into an existing DPIA, or have they resulted in a new analysis or a formal reassessment of the risk in accordance with Article 35 of the GDPR?

The public sources examined do not, at this stage, make it possible to answer this question fully.

**DOCUMENTARY BLIND SPOT:**

> The possible existence of an internal DPIA should not be confused with its absence. However, we do not yet have a public document making it possible to establish precisely which impact assessment covers the entire CFVR + secure data platform + electronic invoicing + new cross-referencing + inter-administration exchanges chain.

This distinction is essential.

---

### A DPIA would be particularly relevant in light of the CNIL's criteria

Without prejudging the legal analysis already carried out by the DGFiP, several high-risk criteria described by the CNIL objectively appear in the public documentation [S37][S49]:

```
large-scale processing             ✓
matching of datasets               ✓
evaluation / targeting             ✓
algorithmic methods                ✓
```

The presence of these characteristics makes it particularly important to be able to verify:

- the exact description of the processing examined in the DPIA;  
- the categories of data covered;  
- the interconnections taken into account;  
- the risks of compromise;  
- the risks related to access authorizations;  
- the risks of excessive correlation;  
- the measures taken to mitigate these risks;  
- successive changes to the assessment.

**TO BE ESTABLISHED:**

> Which DPIA currently covers the processing of electronic invoicing data within CFVR and the secure data platform?

> When was it last revised?

> Does it take into account the arrival of several billion invoices per year?

> Does it take into account the cross-referencing carried out on the secure data platform?

> Does it take into account exchanges with social security bodies?

> Does it take into account the evolution of algorithmic methods and the expansion of the network of analysts?

---

### Fifth vulnerability: segregation becomes a critical safeguard

The CNIL imposes a particularly strong condition regarding the secure data platform [S37].

It considers that its use requires:

- strict segregation;  
- that the data transferred to it be processed solely for the purposes currently provided for;  
- that no new unauthorized person be able to access them;  
- that technical protections be equivalent to those existing outside the secure data platform.

This wording shows that segregation is not a secondary issue.

It constitutes one of the safeguards preventing technical concentration from leading to functional opening of the data.

**LEGAL AND TECHNICAL SAFEGUARD:**

> The secure data platform must not become, solely because it hosts several datasets, an infrastructure enabling their general use by unauthorized users or for unauthorized purposes.

**POTENTIAL VULNERABILITY:**

> The legal robustness of the architecture therefore depends directly on technical segregation safeguards that cannot be fully verified from the public documentation examined.

**TO BE ESTABLISHED:**

> How are the separations between datasets, purposes, processing operations and access profiles technically implemented and audited within the secure data platform?

---

### The security issue therefore cannot be reduced to "anything can be hacked"

It would be legally insufficient to claim:

> **"Any IT system can be hacked, therefore this architecture is dangerous."**

Zero risk does not exist, and the GDPR does not require the absolute impossibility of a compromise.

The legal requirement is different.

It concerns the relationship between:

```
level of risk
   ↓
measures implemented
   ↓
state of the art
   ↓
monitoring
   ↓
regular reassessment
   ↓
ability to demonstrate compliance
```

[S48][S50]

The analysis must therefore focus on this ground.

---

### What 6.3 already makes it possible to raise

Several specific questions can now be addressed to the DGFiP, the CNIL or the legislature:

> **1. Which DPIA currently covers CFVR following the integration of electronic invoicing and its processing within the secure data platform?**

> **2. When was this DPIA last reassessed in light of the massive change in data volume and the new interconnections?**

> **3. Have the proactive mechanisms for detecting abnormal behavior and immediately blocking accounts recommended by the CNIL been fully deployed?**

> **4. What maximum retention period applies to data transferred between the DGFiP and each social security body?**

> **5. How is the effective deletion of copies received by recipient organizations monitored?**

> **6. How is segregation between datasets, purposes and categories of users technically guaranteed and audited within the secure data platform?**

> **7. What independent audits or regular tests make it possible to demonstrate that the level of security remains appropriate as threats evolve?**

These questions do not presume any violation.

They request evidence of the safeguards that the law specifically makes relevant.

---

### Conclusion of 6.3

**ESTABLISHED:**

> CFVR already cross-references numerous tax, economic, administrative and social data sources and now integrates data originating from electronic invoicing [S37][S45].

**ESTABLISHED:**

> Electronic invoicing data are intended to be processed within the secure data platform, and the resulting outputs may be cross-referenced with other information used by CFVR [S37].

**ESTABLISHED:**

> Bidirectional exchanges of certain data are legally organized between the DGFiP and social security bodies [S37][S45].

**ESTABLISHED:**

> The CNIL explicitly considers that the massive volume, the sensitivity of the data and the evolution of cyberattack methods require particular vigilance [S37].

**LEGAL SAFEGUARD:**

> The GDPR requires a level of security appropriate to the risk, as well as reassessment when changes in processing operations result in a change in risk [S48].

**DOCUMENTED SAFEGUARD:**

> The CNIL notably records commitments concerning two-factor authentication, secure devices, segregation and the limitation of access authorizations [S37].

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not yet make it possible to establish whether all the proactive detection and blocking measures recommended by the CNIL have actually been deployed.

**DOCUMENTARY BLIND SPOT:**

> The draft examined by the CNIL did not specify the retention period for data transmitted to social security bodies; the precise regime applicable to each copy held by recipients remains to be established [S37].

**DOCUMENTARY BLIND SPOT:**

> We have not yet identified a public DPIA making it possible to verify precisely how the entire CFVR + secure data platform + electronic invoicing + new cross-referencing + inter-administration exchanges architecture was assessed.

**LEGAL VULNERABILITY:**

> The simultaneous increase in data volume, the number of sources, matching capabilities and categories of persons with access increases the potential consequences of a compromise or misuse and therefore reinforces the requirements for security, segregation and risk reassessment.

**TO BE ESTABLISHED:**

> Can the administration demonstrate that the technical and organizational measures and impact assessments have been reassessed to match the change in scale introduced in 2026?

**NOT ESTABLISHED:**

> No element identified makes it possible to claim that CFVR or the secure data platform have suffered a compromise or that the security measures currently deployed are legally insufficient.

---

## 6.4 Profiling and automated decision-making

**Status: ESTABLISHED ALGORITHMIC PROCESSING / DOCUMENTED HUMAN SAFEGUARD / IDENTIFIED LEGAL BOUNDARY / VULNERABILITIES TO BE ESTABLISHED**

The previous sections established that data originating from electronic invoicing are intended to be processed on a large scale, cross-referenced with other information and used in a processing system enabling, notably, the identification of anomalies and businesses presenting certain tax risks [S37][S45].

This architecture directly raises an additional legal question:

> **at what point does processing that analyzes, classifies or selects persons or businesses cease to be merely a decision-support tool and become sufficiently determinative to fall within the safeguards applicable to automated decisions?**

This boundary is particularly important because European law does not consider only the formal existence of an algorithm.

It also considers its concrete role in the resulting decision.

---

### Profiling and automated decision-making are not synonymous

A first distinction must be maintained.

Profiling consists of using personal data to evaluate certain personal aspects relating to a natural person.

An automated decision may be based on profiling, but the two concepts are not the same [S36][S43].

Processing may therefore:

```
analyze data
   ↓
produce a score / signal / classification
   ↓
without itself making
a decision producing a legal effect
```

Conversely, a decision may be fully automated without necessarily being based on prior profiling.

**METHODOLOGICAL SAFEGUARD:**

> The existence of algorithms, models or classifications is not, in itself, sufficient to demonstrate the existence of an automated individual decision prohibited or specifically regulated by Article 22 of the GDPR.

---

### Article 22 nevertheless establishes an important boundary

Article 22 of the GDPR recognizes the data subject's right not to be subject to a decision based solely on automated processing, including profiling, where that decision:

- produces legal effects concerning them;  
- or similarly significantly affects them [S36][S43].

Exceptions exist.

Such a decision may notably be authorized where it is provided for by Union or Member State law and appropriate measures safeguard the rights, freedoms and legitimate interests of the individuals concerned [S43].

The principle is therefore not:

```
algorithm
   =
prohibition
```

The legal question is more precise:

```
automated processing
   ↓
decision
   ↓
solely automated nature
   ↓
legal or significant effect
   ↓
Article 22
```

---

### CFVR is currently upstream of this boundary according to the documented system

The public documentation relating to CFVR contains a particularly important safeguard here.

The CNIL indicates that the purpose of the processing is:

> to guide and inform the analysis carried out by agents,

and specifies that:

> **only agents can decide to initiate a tax audit procedure** [S37].

It emphasizes this separation again when examining algorithmic methods.

The alerts generated by CFVR must remain a tool enabling agents to assess whether or not it is appropriate to open an audit.

They must not replace their analysis [S37].

**ESTABLISHED:**

> The legally and organizationally documented operation of CFVR does not provide for an algorithm to decide on its own to initiate a tax audit.

**LEGAL AND ORGANIZATIONAL SAFEGUARD:**

> Human analysis must take place before an audit is initiated.

This safeguard therefore prevents claiming, on the basis of the sources currently available:

> **"CFVR automatically initiates tax audits."**

This claim is not established.

---

### But the CNIL itself considers this human intervention indispensable

The wording used by the CNIL is particularly important.

It considers it:

> **indispensable to the balance of the system**

that the alerts generated must under no circumstances replace the analysis carried out by agents [S37].

It also asks the ministry to guarantee:

> **effective human oversight and decision-making** [S37].

It notably recommends:

- appropriate documentation for analysts;  
- regular training;  
- a tax analysis of the documents in each case;  
- taking into account the latest available tax returns [S37].

The CNIL describes these measures as essential to prevent:

> **the automation of the initiation of tax audits** [S37].

This wording reveals a very clear legal and organizational boundary.

```
CFVR
   ↓
algorithmic alert
   ↓
EFFECTIVE HUMAN ANALYSIS
   ↓
possible decision
```

The robustness of the safeguard therefore depends on what actually happens at the central stage.

---

### SCHUFA prevents the issue from being reduced to the formal presence of a human

The case law of the Court of Justice provides a major element here.

In the SCHUFA case, the Court had to examine a system in which a company automatically generated a probability value concerning an individual, then transmitted that value to a third party that formally made the final decision [S51].

There were therefore two distinct stages:

```
automated system
   ↓
score
   ↓
third party
   ↓
decision
```

The Court nevertheless held that the automated establishment of the score could itself constitute an automated individual decision within the meaning of Article 22 where the third party's decision depended **in a determining manner** on that value [S51].

**PRINCIPLE ESTABLISHED BY CASE LAW:**

> The existence of a human decision-maker or a third party at the end of the chain is therefore not necessarily sufficient to exclude Article 22 where the automated result plays, in practice, a determining role in the final decision.

This case law did not concern CFVR and does not make it possible to automatically transpose its conclusion to tax audits.

But it provides a particularly relevant criterion for examining this type of architecture.

---

### First legal vulnerability: human intervention must be genuine, not merely formal

The question concerning CFVR therefore becomes more precise.

It is not merely:

> **"does a human click the final button?"**

It is:

> **"does this human genuinely have the information, time, expertise and autonomy necessary to challenge the signal produced by the system?"**

The CNIL itself appears to identify this difficulty, since it calls for **effective** human oversight and decision-making [S37].

**LEGAL VULNERABILITY:**

> If human analysis were to become purely formal and algorithmic alerts were, in practice, to determine the initiation of audits, the legal classification of the process would have to be reassessed in light notably of Article 22 and the SCHUFA case law [S43][S51].

**NOT ESTABLISHED:**

> The sources examined do not demonstrate that such de facto automation currently exists within CFVR.

**TO BE ESTABLISHED:**

> What proportion of CFVR alerts submitted to agents are ultimately accepted or rejected following human analysis?

> What elements make it possible to concretely assess the agents' ability to disregard an algorithmic recommendation?

> Are there indicators making it possible to identify near-systematic validation of alerts generated by certain models, services or categories of agents?

These data would make it possible to assess the actual effectiveness of the human safeguard.

---

### A second vulnerability emerges: the algorithmic feedback loop

The CNIL explicitly identifies another issue [S37].

The results of past tax audits are used to develop the models employed within CFVR.

This potentially creates a loop:

```
model
   ↓
selection of a population
   ↓
audits
   ↓
audit results
   ↓
new training data
   ↓
new model
   ↓
new selection
```

The issue arises when an initial bias influences the audits carried out.

Populations subject to more audits mechanically generate more data resulting from audits.

These data can then feed future models.

The CNIL specifically describes the risk of an amplification leading to a concentration of audits on certain populations or categories of entities that would no longer be justified by the current prevalence of fraud [S37].

**ESTABLISHED:**

> The CNIL explicitly identifies a risk of bias amplification within CFVR due to the reuse of past audit results to develop the models.

This is therefore not a hypothetical vulnerability invented by the investigation.

---

### The 50% safeguard is noteworthy but acknowledged as insufficient on its own

The ministry has introduced a specific safeguard.

It limits to 50% the proportion of tax audits initiated by agents following the analysis of signals originating from CFVR [S37].

The CNIL considers this measure useful for limiting the development of significant biases.

But it immediately adds that:

> **this limitation is not sufficient, on its own, to prevent all risks of significant bias** [S37].

It therefore also calls for:

- analyses concerning the explainability of algorithms;  
- critical assessments of biases that may emerge;  
- monitoring of the effectiveness of the safeguards [S37].

The ministry has committed to carrying out these studies and reporting on them in CFVR activity reports.

**DOCUMENTED SAFEGUARD:**

> The ministry limits to 50% the proportion of audits initiated following CFVR signals.

**EXPLICITLY ACKNOWLEDGED LIMITATION:**

> The CNIL itself considers that this safeguard is not sufficient to eliminate all risks of bias.

**TO BE ESTABLISHED:**

> Have the announced studies on explainability and bias been carried out?

> What results have they produced?

> What indicators make it possible to verify that certain populations or categories of entities do not become progressively overrepresented in audits solely as a result of a learning feedback loop?

---

### Unsupervised learning further increases the significance of the issue

The CNIL also notes the development of new learning methods within CFVR, notably so-called unsupervised methods [S37].

In this type of method, the model seeks notably to distinguish behaviors considered normal or abnormal without prior labelling.

The CNIL considers that:

- the massive expansion of data;  
- the development of these new methods;

have the effect of amplifying the risks associated with algorithms and bias [S37].

This development is particularly important with the arrival of data originating from several billion invoices.

The chain becomes:

```
massive datasets
   ↓
automated detection of patterns / anomalies
   ↓
classification or alert
   ↓
list of businesses considered at risk
   ↓
human analysis
   ↓
possible audit
```

**MAJOR POINT OF VIGILANCE:**

> The more complex the operation of the model becomes and the more it depends on relationships automatically detected within very large volumes of data, the more legally and operationally important the ability to understand, control and explain the reasons for an alert becomes.

---

### Third vulnerability: explainability becomes a central safeguard

European law now contains particularly precise case law concerning the explanation of automated decisions [S52].

In Case C-203/22, the Court of Justice specifies that, where the relevant regime applies, the individual must be able to obtain information enabling them to understand:

- the procedure actually used;  
- the principles applied;  
- how their data contributed to the result [S52].

The Court also specifies that:

> the complexity of the processing does not remove the obligation to provide an intelligible explanation.

A complex mathematical formula does not necessarily constitute a sufficient explanation.

Nor does an exhaustive description of all technical operations [S52].

**LEGAL SAFEGUARD:**

> Where a decision falls within the GDPR regime governing automated decisions, the complexity of an algorithm cannot be used as a justification for making its result legally inexplicable.

---

### A tension emerges with complex models

This case law raises an important question regarding the evolution of CFVR.

The CNIL specifically asks the ministry to work on:

> **the explainability of algorithms** [S37].

At the same time, CFVR is developing:

- learning methods;  
- unsupervised methods;  
- analyses involving massive volumes of data;  
- cross-referencing between multiple sources [S37][S45].

A structural tension therefore emerges:

```
increasing complexity
   ↓
increasing detection capabilities
   ↓
but
   ↓
need to preserve
understanding
control
explainability
contestability
```

**POTENTIAL LEGAL VULNERABILITY:**

> An architecture whose results became sufficiently determinative to produce or condition significant decisions would have to remain capable of providing the transparency and explanation safeguards required by applicable law.

**NOT ESTABLISHED:**

> The sources examined do not make it possible to conclude that CFVR models are currently legally inexplicable.

---

### Fourth vulnerability: data quality can directly influence targeting

The human intervention documented by the CNIL includes a revealing precaution.

Agents must notably verify:

> that the latest tax returns filed have been taken into account [S37].

This requirement shows that an algorithmic alert may be influenced by the state of the data available at the time it is calculated.

Electronic invoicing data will considerably increase the quantity and granularity of exploitable information.

An error may arise from:

```
incorrect data
   ↓
cross-referencing
   ↓
anomaly detected
   ↓
alert
   ↓
business selected
```

The human safeguard must therefore make it possible to break this chain before an erroneous algorithmic signal produces unjustified consequences.

**VULNERABILITY:**

> The greater the number of sources and data used, the more decisive control over their accuracy, currency and context becomes for the quality of the algorithmic result.

---

### The legal boundary becomes particularly important if the consequences evolve

Today, the documentation primarily establishes:

```
alert
   ↓
guidance for an agent
   ↓
human analysis
   ↓
possible tax audit
```

This architecture benefits precisely from the existence of this human stage.

But the SCHUFA case law shows that another configuration must be analyzed differently:

```
automated result
   ↓
determining result
   ↓
decision producing a significant effect
```

[S51]

The question therefore does not concern only CFVR as it exists today.

It also concerns any future development in which a score or classification produced by a public infrastructure became determinative in:

- automatically initiating a procedure;  
- denying a right or service;  
- modifying the conditions of access to a service;  
- producing a financial consequence;  
- imposing a restriction;  
- or conditioning another decision producing a significant effect on an individual.

**LEGAL BOUNDARY:**

> The more determinative the algorithmic result becomes in producing a significant individual consequence, the more central the question of the application of Article 22 and the associated safeguards becomes [S43][S51].

---

### This boundary is essential for the bridge with the other infrastructures examined in the investigation

This conclusion provides an important legal element for the architectures examined in Chapter 5.

The previous chapters separately identified capabilities concerning:

- transactions;  
- electronic invoicing;  
- identity;  
- products;  
- the Digital Product Passport;  
- environmental data;  
- certain payment conditions.

No element examined currently demonstrates the existence of a system using all of these data to automatically produce an individual decision.

But the legal framework now makes it possible to identify what would need to be examined if such infrastructures were interconnected.

The legally sensitive chain would be:

```
economic data
   +
transaction data
   +
identity data
   +
product data
   +
environmental data
   ↓
profile / score / classification
   ↓
automated result
   ↓
determining influence
   ↓
decision producing
a legal or significant effect
```

At that stage, several safeguards would then have to be examined simultaneously:

- purpose of the processing;  
- legal basis;  
- minimization;  
- proportionality;  
- data accuracy;  
- transparency;  
- explainability;  
- human intervention;  
- ability to challenge;  
- Article 22 of the GDPR where its conditions are met [S43][S44][S46][S48][S51][S52].

**LEGALLY DEDUCIBLE:**

> The technical interconnection of several infrastructures is not sufficient to make a decision resulting from their combination legally permissible.

**LEGALLY DEDUCIBLE:**

> If their combination were to produce a score or classification playing a determining role in a significant individual decision, the formal existence of a human intermediary would not necessarily be sufficient to exclude the safeguards applicable to automated decisions [S51].

**NOT ESTABLISHED:**

> No element examined currently demonstrates that an environmental score, a DPP or data originating from electronic invoicing determines the authorization or refusal of a payment or another individual right.

This boundary must be strictly maintained.

---

### A deeper vulnerability nevertheless emerges

The infrastructures examined progressively reveal three distinct phenomena:

```
1. increase in available data
2. increase in matching possibilities
3. increase in algorithmic capabilities
```

Taken separately, each may have its own legal basis and safeguards.

But their combination increases the technical possibility of producing increasingly granular classifications.

The law does not prohibit this development as a matter of principle.

It does, however, require safeguards to evolve with the nature and influence of the processing.

**STRUCTURAL VULNERABILITY:**

> An architecture may remain legally presented as a decision-support system as long as human intervention remains genuine and determinative. The boundary becomes much more sensitive if the increasing precision, volume or authority given to algorithmic results progressively transforms this human intervention into essentially formal validation.

It is precisely this development that would need to be measurable over time.

---

### Questions for testing this safeguard

The analysis now makes it possible to formulate several verifiable questions:

> **1. What is the rate at which agents reject cases proposed by CFVR following human analysis?**

> **2. Is this rate monitored model by model and alert category by alert category?**

> **3. What mechanisms make it possible to detect excessive reliance by agents on algorithmic recommendations?**

> **4. Have the studies on bias and explainability announced to the CNIL been carried out, and can their results be disclosed?**

> **5. How is any potential overrepresentation of certain categories of taxpayers or businesses in alerts measured?**

> **6. How does the administration verify that a correlation detected by a model remains linked to a real and current prevalence of fraud?**

> **7. What information can be provided to an individual seeking to understand the role played by algorithmic processing in the selection of their case?**

> **8. What safeguards prevent a future development from transforming an algorithmic recommendation into the automatic or near-automatic initiation of a procedure?**

These questions do not presume any violation.

They make it possible to test the effectiveness of the safeguards invoked.

---

### Conclusion of 6.4

**ESTABLISHED:**

> CFVR uses algorithmic methods to identify anomalies and guide tax audit programming [S37][S45].

**ESTABLISHED:**

> The development of unsupervised learning methods and the massive expansion of data lead the CNIL itself to consider that algorithmic risks and risks of bias are amplified [S37].

**ESTABLISHED:**

> The results of previous audits are used to develop the models, which, according to the CNIL, exposes the system to a risk of bias amplification over time [S37].

**DOCUMENTED SAFEGUARD:**

> CFVR alerts must not replace the analysis carried out by agents, and the initiation of a tax audit must currently result from a human decision [S37].

**DOCUMENTED SAFEGUARD:**

> The ministry limits to 50% the proportion of audits initiated following signals originating from CFVR [S37].

**EXPLICITLY ACKNOWLEDGED LIMITATION:**

> The CNIL considers that this 50% limit is not sufficient, on its own, to prevent all risks of significant bias and calls for additional work on explainability and bias [S37].

**PRINCIPLE ESTABLISHED BY CASE LAW:**

> According to the CJEU, an automated result may itself fall within the concept of an automated decision where the subsequent decision depends in a determining manner on that result [S51].

**LEGAL SAFEGUARD:**

> Where the regime governing automated decisions applies, the technical complexity of the system does not remove the requirements of transparency and explanation [S52].

**LEGAL VULNERABILITY:**

> The protection provided by human intervention depends on its actual effectiveness. Essentially formal human validation of a determinative algorithmic result could require a reassessment of the legal classification of the process.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not make it possible to precisely measure the rate at which CFVR alerts are rejected by agents or, consequently, the degree of practical influence that algorithmic recommendations have on decisions to initiate audits.

**TO BE ESTABLISHED:**

> Do the announced studies on explainability and bias make it possible to demonstrate that the massive expansion of data and the development of new methods do not lead to an unjustified concentration of audits on certain populations or categories of entities?

**TO BE ESTABLISHED:**

> What mechanisms make it possible to demonstrate that human intervention remains substantive as the predictive capabilities and complexity of the models increase?

**LEGALLY DEDUCIBLE:**

> If a future infrastructure combined economic, transaction, identity, product or environmental data in order to produce a result determinative of a significant individual decision, that chain would have to be examined in light of the safeguards applicable to automated processing, irrespective of the mere formal presence of a human at the end of the chain [S51].

**NOT ESTABLISHED:**

> No element examined currently makes it possible to claim that CFVR automatically decides to initiate a tax audit or that environmental data, a DPP or invoicing data automatically determines access to a payment, service or right.

---

## 6.5 Necessity, proportionality and minimization

**Status: ESTABLISHED LEGAL OBLIGATIONS / ESTABLISHED CHANGE IN SCALE / JUSTIFICATIONS TO BE ESTABLISHED**

The previous sections established several important elements.

Data originating from electronic invoicing are intended to feed an infrastructure enabling their large-scale algorithmic processing.

They are incorporated into a processing system already fed by numerous other sources.

Cross-referencing is carried out notably to detect anomalies and identify businesses presenting certain tax risks.

The announced volume reaches several billion electronic invoices per year [S37][S45].

The legal question then becomes different.

It is no longer merely:

> **"does the fight against fraud constitute a legitimate purpose?"**

That purpose is established.

The question becomes:

> **"are all the data collected, their granularity, their cross-referencing, their retention periods and the ways in which they are processed necessary and proportionate to that purpose?"**

This distinction is essential.

---

### A legitimate purpose is not sufficient to demonstrate the necessity of each item of data

The principle of data minimization laid down in Article 5 of the GDPR requires personal data to be:

> **adequate, relevant and limited to what is necessary in relation to the purposes for which they are processed** [S36][S43].

This requirement therefore concerns not only the existence of a legitimate purpose, but also the relationship between that purpose and the data actually used.

The legal chain is not:

```
objective of general interest
   ↓
all data that may potentially be useful
```

It is:

```
precisely defined objective
   ↓
necessary data
   ↓
necessary quantity
   ↓
necessary duration
   ↓
necessary access
   ↓
necessary processing
```

**LEGAL SAFEGUARD:**

> The potential usefulness of data is not necessarily sufficient to demonstrate its legal necessity.

---

### The CJEU applies this requirement directly to tax administrations

Case C-175/20 is particularly important for this investigation because it specifically concerns a tax administration [S53].

The Court of Justice reiterates that limitations on data protection must remain limited to what is strictly necessary.

It concludes that a controller, even when acting in the context of a task carried out in the public interest:

> **cannot collect personal data in a general and indiscriminate manner** [S53].

It must also:

> **refrain from collecting data that are not strictly necessary for the purposes of the processing** [S53].

The Court adds that the controller must seek to minimize the amount of data collected as much as possible.

**PRINCIPLE ESTABLISHED BY CASE LAW:**

> A tax administration therefore does not have, solely by virtue of its mission to combat fraud, a general right to indiscriminately collect all personal data that may be of analytical interest.

---

### The burden of demonstrating compliance is a particularly important element

The Court adds an essential requirement.

The controller must be able to demonstrate compliance with the principles laid down in Article 5 of the GDPR [S53].

Regarding minimization, it states that it is for the administration concerned to establish that it has sought to minimize the amount of data collected as much as possible.

Regarding duration, it also specifies that the period concerned cannot exceed what is strictly necessary for the objective of general interest pursued [S53].

The question is therefore not merely:

> **"can it be demonstrated that these data are useful?"**

It becomes:

> **"can it be demonstrated why this precise amount of data is necessary?"**

and:

> **"can it be demonstrated why a smaller amount, lower granularity or shorter period would not be sufficient to achieve the objective pursued?"**

**LEGAL SAFEGUARD:**

> The principle of accountability requires the controller to be able to demonstrate compliance with data minimization.

---

### This case law directly intersects with CFVR's change in scale

The CNIL notes that the arrival of data originating from electronic invoicing substantially increases the volume of data processed within CFVR [S37].

It indicates that the volume of electronic invoices is estimated at:

> **2 to 3 billion per year** [S37].

The volume is such that the ministry indicates that these data could not be processed within the existing CFVR infrastructure.

An infrastructure with enhanced computing power, the secure data platform, becomes necessary precisely to enable their processing [S37].

The documented chain is therefore:

```
new category of data
   ↓
substantial increase in volume
   ↓
2 to 3 billion invoices / year
   ↓
existing infrastructure insufficient
   ↓
secure data platform with enhanced computing power
   ↓
processing
   ↓
cross-referencing of results
   ↓
tax targeting
```

**ESTABLISHED:**

> The integration of electronic invoicing does not constitute a marginal increase in processing.

It results in a change in scale significant enough to require an infrastructure with enhanced computing power [S37].

---

### First vulnerability: the change in scale must be justifiable data by data

The change in scale does not, in itself, constitute a violation of the principle of data minimization.

Mass collection may be necessary where a legitimate task cannot reasonably be carried out otherwise.

But C-175/20 prevents reasoning solely on the basis of the general interest pursued [S53].

The data actually necessary must also be examined.

The question therefore becomes:

> **Are all categories of personal data originating from electronic invoicing that are integrated into or processed within this chain necessary for the models and analyses pursued?**

And more specifically:

> **Does each personal data field processed make a necessary contribution to a specified purpose?**

> **Could certain analyses operate with fewer fields?**

> **Could certain data be aggregated, pseudonymized or deleted before processing?**

> **Could the same effectiveness be achieved without retaining certain elements at transaction level?**

**LEGAL VULNERABILITY:**

> The more systematically an infrastructure absorbs data, the less reasonably the demonstration of necessity can be limited to the general assertion that these data may improve the fight against fraud.

**TO BE ESTABLISHED:**

> What documented demonstration justifies, category by category, the personal data originating from electronic invoicing that are actually necessary for the processing carried out within the secure data platform and CFVR?

---

### The case law also requires examining whether more limited targeting is possible

Case C-175/20 contains particularly noteworthy reasoning here [S53].

In that case, the Court specifically asks whether it would be possible to achieve the tax objective without potentially obtaining data relating to all the advertisements concerned.

It explicitly considers the possibility of:

> **targeting certain advertisements using specific criteria** [S53].

The principle is important.

Where the objective can be achieved through more targeted collection, generalized collection becomes more difficult to justify.

Applied to the architecture examined, this raises a question that is no longer theoretical:

```
processing of invoicing data
on a very large scale
   VS
prior selection
of categories / transactions / situations
presenting risk criteria
```

**MAJOR LEGAL QUESTION:**

> Is the processing of the mass of electronic invoicing data necessary for the purposes pursued, or could certain analyses be carried out on the basis of a less intrusive prior selection?

The answer requires technical and statistical information that is not present in the public sources examined.

**DOCUMENTARY BLIND SPOT:**

> We have not yet identified any public demonstration comparing the planned large-scale processing with less intrusive architectures that might produce comparable results.

---

### Second vulnerability: minimization also concerns granularity

Two processing operations may involve the same number of documents while presenting very different levels of interference.

A distinction must be made between:

```
existence of an invoice
```

and:

```
detailed content of the invoice
```

and further:

```
detailed content
   +
history
   +
counterparties
   +
cross-referencing with other databases
```

The principle of data minimization applies to the amount of data, but also to the extent of processing and their accessibility [S43].

The relevant question is therefore not merely:

> **how many invoices are processed?**

It is also:

> **what level of detail originating from each of these invoices is actually necessary for each model or query?**

**LEGAL VULNERABILITY:**

> A justification concerning the necessity of using invoices does not automatically demonstrate the necessity of using every item of personal data they contain.

---

### Third vulnerability: cross-referencing changes the intensity of processing

An isolated item of data and the same item cross-referenced with numerous other pieces of information do not necessarily involve the same level of interference.

CFVR specifically enables multiple sources to be cross-referenced [S37][S45].

The secure data platform is intended to progressively host all the data processed within CFVR [S37].

Thus:

```
data A
   +
data B
   +
data C
   +
electronic invoicing
   +
tax history
   +
other sources
   ↓
increased inference capability
```

The principle of data minimization must therefore be examined not only at the level of each database considered separately, but also in light of the processing actually carried out through their combination.

**STRUCTURAL VULNERABILITY:**

> Data that are individually necessary for several processing operations may, when cross-referenced, produce a much more intrusive analytical capability than that resulting from each source considered separately.

**TO BE ESTABLISHED:**

> How are necessity and proportionality assessed for combinations of data and not only for each source considered separately?

---

### The French Constitutional Council also requires a proportionality assessment

This requirement does not arise solely from the GDPR and European case law.

The French Constitutional Council links the protection of personal data to the right to respect for private life guaranteed by Article 2 of the Declaration of the Rights of Man and of the Citizen [S44].

It holds that:

> **the collection, recording, retention, consultation and communication of personal data must be justified by a reason of general interest and implemented in a manner that is appropriate and proportionate to that objective** [S44].

The assessment therefore concerns several successive operations:

```
collection
   ↓
recording
   ↓
retention
   ↓
consultation
   ↓
communication
```

**CONSTITUTIONAL SAFEGUARD:**

> The existence of a reason of general interest does not exempt the system from an assessment of the appropriateness and proportionality of its practical arrangements.

---

### Fourth vulnerability: retention must be justified separately

Data that are necessary today do not automatically remain necessary for the entire period during which their retention is technically possible.

The principle of storage limitation requires that data enabling individuals to be identified not be retained for longer than necessary in relation to the purposes pursued [S43].

C-175/20 also applies the logic of strict necessity to the period covered by tax-related data collection [S53].

This question becomes particularly important in an algorithmic infrastructure.

The longer the available history:

```
more historical data
   ↓
more possible comparisons
   ↓
more possible models
   ↓
greater inference capabilities
```

But:

```
analytical usefulness
   ≠
automatic legal necessity
```

**LEGAL VULNERABILITY:**

> A long retention period must be justifiable in relation to the purposes pursued and cannot be based solely on the potential value of having access to a richer historical dataset.

---

### A first concrete point already exists regarding exchanges with social security bodies

The CNIL specifically applied this reasoning to exchanges between the DGFiP and social security bodies [S37].

It notes that the draft submitted to it did not specify the retention period for the data transmitted.

It then reiterates that exchanges between administrations are permitted only where their arrangements remain proportionate to the objectives pursued.

It calls for retention to be limited to the period necessary [S37].

The ministry committed to providing for a maximum retention period of ten years.

But the CNIL also asks for something more precise:

> that the applicable retention periods be determined **category of data by category of data** in the agreements concluded with social security bodies [S37].

This clarification is particularly noteworthy.

It shows that:

```
a general maximum retention period
   ≠
individualized justification
of the necessary duration
for each category
```

**ESTABLISHED:**

> The CNIL itself calls for a more granular assessment of retention periods for data exchanged with social security bodies [S37].

---

### Fifth vulnerability: "up to ten years" does not mean "ten years are necessary"

This distinction must be maintained.

The fact that a legal framework permits retention for up to a certain period does not necessarily mean that all categories of data must actually be retained for that entire period.

The principles of data minimization and storage limitation require identifying the period necessary for the processing concerned [S43][S53].

Thus:

```
maximum legally permissible period
   ≠
necessary period for each item of data
```

**QUESTION TO BE ESTABLISHED:**

> Among the data that may be retained for up to ten years, which actually require that retention period and which could be deleted or anonymized earlier?

---

### Sixth vulnerability: progressive accumulation may shift the proportionality assessment

Section 6.2 identified a question that was deliberately left open:

> how far can successive extensions of purposes, sources and recipients accumulate before their overall effect requires a new assessment of necessity and proportionality?

This question now becomes much more concrete.

CFVR is no longer the processing system it was when it was created.

Its scope has evolved.

Its sources have evolved.

Its methods have evolved.

Its computing capabilities have evolved.

The categories of agents involved have evolved.

Inter-administration exchanges have evolved.

And several billion electronic invoices are now being added to this architecture [S37][S45].

The evolution can therefore be represented as follows:

```
initial processing
   ↓
new sources
   ↓
new cross-referencing
   ↓
new algorithms
   ↓
new persons with access
   ↓
new exchanges
   ↓
new computing infrastructure
   ↓
several billion invoices / year
```

Each extension may separately have a legal basis.

But this does not fully answer another question:

> **does the resulting architecture, as a whole, remain necessary and proportionate?**

**STRUCTURAL LEGAL VULNERABILITY:**

> Assessing each extension in isolation may not be sufficient to account for the overall intensity of the processing resulting from their accumulation.

---

### The principle of accountability shifts part of the reasoning here

One of the most important contributions of C-175/20 is that the responsibility for demonstrating data minimization lies with the controller [S53].

This changes how the questions in this investigation can be formulated.

We do not necessarily have to demonstrate:

> **"these data are unnecessary."**

The legally relevant question may be:

> **"what evidence establishes that these data are necessary?"**

Likewise, it is not necessary to claim:

> **"this retention period is excessive."**

We can ask:

> **"what evidence establishes that this retention period is necessary for this purpose?"**

Or:

> **"what evidence establishes that the same objective could not be achieved with a smaller amount of data?"**

This is a fundamental methodological difference.

---

### Seventh vulnerability: technical capabilities do not constitute the measure of necessity

The CNIL explains that the secure data platform is technically necessary because the volume of electronic invoicing data exceeds the capabilities of the existing CFVR environment [S37].

This establishes:

> **the technical necessity of a more powerful infrastructure to process the envisaged volume of data.**

However, this does not answer a different question:

> **the legal necessity of processing the entire envisaged volume.**

The two lines of reasoning must not be confused.

```
"we need the secure data platform
to process this much data"
   ≠
"we have demonstrated that it is necessary
to process this much data"
```

**DOCUMENTARY VULNERABILITY:**

> The sources examined explain why enhanced computing power is necessary to process the planned volume of data, but they do not, on their own, demonstrate why this precise volume constitutes the minimum level necessary for each purpose pursued.

This distinction is particularly important.

---

### This reasoning becomes crucial for the other infrastructures examined in the investigation

The principle of necessity does not concern CFVR alone.

It also provides a legal test for any future interconnection involving personal data.

The previous chapters identified various infrastructures relating notably to:

- transactions;  
- invoicing;  
- identity;  
- products;  
- the DPP;  
- environmental information;  
- certain payment infrastructures.

The separate existence of legal bases permitting certain processing operations within each of these infrastructures would not necessarily be sufficient to justify their combination.

The question would have to be asked again for the resulting processing:

```
data necessary in system A
   +
data necessary in system B
   +
data necessary in system C
   ≠ automatically
necessary combination of A + B + C
```

**LEGALLY DEDUCIBLE:**

> The necessity of collecting data within its original system does not automatically demonstrate the necessity of cross-referencing it with data from another infrastructure.

This is an important legal boundary for the bridge constructed in this investigation.

---

### Application to the environmental / identity / payment bridge

No element examined currently demonstrates the existence of processing combining all of these infrastructures in order to produce an individual decision.

But if a future development were to lead, for example, to:

```
identity
   +
transaction
   +
product
   +
DPP
   +
environmental information
   +
payment
   ↓
analysis / classification
   ↓
individual consequence
```

the mere existence of a legal basis specific to each component would not necessarily be sufficient to establish the necessity and proportionality of the resulting processing.

It would notably be necessary to examine:

- the precise purpose of the cross-referencing;  
- the data strictly necessary;  
- the necessary granularity;  
- the necessary duration;  
- the persons who may access it;  
- less intrusive alternatives;  
- the consequences for individuals;  
- safeguards against secondary uses [S43][S44][S53].

**LEGALLY DEDUCIBLE:**

> The more several infrastructures are interconnected, the more the justification must concern the processing resulting from their combination and not solely the individual legality of each of their components.

**NOT ESTABLISHED:**

> Nothing in the sources examined currently demonstrates that such a comprehensive interconnection is implemented or legally provided for.

---

### A genuine line of legal assessment emerges

After Sections 6.1 to 6.5, the legal reasoning can now be summarized as follows:

```
legal basis
   ↓
legitimate purpose
   ↓
   BUT
   ↓
necessary data?
   ↓
necessary quantity?
   ↓
necessary granularity?
   ↓
necessary cross-referencing?
   ↓
necessary duration?
   ↓
necessary persons with access?
   ↓
less intrusive alternative?
   ↓
overall proportionality?
```

A positive answer to the first two stages therefore does not automatically answer the subsequent ones.

---

### Questions for concretely testing proportionality

The analysis now makes it possible to ask much more precise questions:

> **1. Which exact categories of personal data originating from invoices are processed within the secure data platform for each model or query?**

> **2. What analysis demonstrates the necessity of each of these categories?**

> **3. What tests have been carried out using a smaller or less granular dataset?**

> **4. Has the administration compared the effectiveness of large-scale processing with that of collection or prior selection based on risk criteria?**

> **5. Which data are deleted before processing because they are not necessary?**

> **6. Which data are aggregated, pseudonymized or anonymized before being cross-referenced?**

> **7. For each category of data, what retention period is actually applied and why is that period necessary?**

> **8. What analysis addresses the cumulative effect of the different sources used within CFVR?**

> **9. Does the DPIA examine less intrusive alternative architectures?**

> **10. What evidence makes it possible to establish that the change in scale introduced by several billion invoices remains proportionate to the benefits obtained for the purposes pursued?**

These questions do not ask the administration to demonstrate that the processing presents zero risk.

They ask for evidence of its necessity and proportionality.

---

### Conclusion of 6.5

**ESTABLISHED:**

> The principle of data minimization requires personal data to be adequate, relevant and limited to what is necessary for the purposes pursued [S36][S43].

**PRINCIPLE ESTABLISHED BY CASE LAW:**

> A tax administration cannot collect personal data in a general and indiscriminate manner and must refrain from collecting data that are not strictly necessary [S53].

**PRINCIPLE ESTABLISHED BY CASE LAW:**

> The controller must be able to demonstrate that it has sought to minimize as much as possible the amount of data collected and the period concerned [S53].

**CONSTITUTIONAL SAFEGUARD:**

> The collection, recording, retention, consultation and communication of personal data must be justified by a reason of general interest and implemented in a manner that is appropriate and proportionate to that objective [S44].

**ESTABLISHED:**

> The integration of electronic invoicing results in a substantial increase in the volume of data processed within CFVR, estimated at several billion invoices per year, requiring the use of an infrastructure with enhanced computing power [S37].

**ESTABLISHED:**

> Regarding certain inter-administration exchanges, the CNIL already requires retention periods to be specified category of data by category of data [S37].

**LEGAL VULNERABILITY:**

> The legitimacy of the fight against fraud does not remove the requirement to demonstrate the necessity of the amount, granularity, duration and cross-referencing of the data actually used.

**STRUCTURAL VULNERABILITY:**

> The individual necessity of data originating from several systems does not automatically demonstrate the necessity of combining them.

**DOCUMENTARY VULNERABILITY:**

> The public sources examined explain why an infrastructure with enhanced computing power is necessary to process the envisaged volume, but they are not sufficient to demonstrate why processing this precise volume itself constitutes the minimum means necessary for each purpose pursued.

**DOCUMENTARY BLIND SPOT:**

> We have not identified in the public sources examined a comparison making it possible to determine whether certain CFVR purposes could be achieved with a smaller amount of data, lower granularity or more restrictive prior targeting.

**TO BE ESTABLISHED:**

> Can the administration demonstrate, in accordance with the principle of accountability, the necessity of each category of personal data processed and the absence of a reasonably less intrusive solution capable of achieving the same purposes?

**TO BE ESTABLISHED:**

> Is the cumulative effect of successive extensions of CFVR subject to an overall and regularly reassessed evaluation of necessity and proportionality?

**LEGALLY DEDUCIBLE:**

> Any future interconnection of personal data originating from invoicing, identity, products, the DPP, environmental data or payment infrastructures would have to justify the necessity of the cross-referencing itself and not merely the separate legality of each source.

**NOT ESTABLISHED:**

> The sources examined do not make it possible to conclude that the current integration of electronic invoicing data into CFVR is disproportionate or contrary to the GDPR.

---

## 6.6 Data subject rights and CNIL oversight

**Status: ESTABLISHED RIGHTS / EXPRESSLY PROVIDED RESTRICTIONS / INDEPENDENT OVERSIGHT / EFFECTIVENESS TO BE EXAMINED**

The previous sections established that a significant amount of personal data may be collected, cross-referenced and analyzed within CFVR.

They also established that:

- electronic invoicing data are intended to be incorporated into this architecture;  
- certain results are produced by algorithmic processing;  
- these results may contribute to the selection of cases;  
- exchanges exist with other administrations;  
- data and results may circulate between several environments and categories of recipients [S37][S45].

A question then becomes central:

> **What means does an individual have to know which data concerning them are being used, verify their accuracy, obtain their correction and challenge processing that would infringe their rights?**

This question concerns the effectiveness of the safeguards.

A right laid down in a legal text and a right that can actually be exercised are not necessarily the same thing.

---

### The GDPR grants important rights to individuals

The GDPR notably provides for:

- a right to information;  
- a right of access;  
- a right to rectification;  
- under certain conditions, a right to erasure;  
- a right to restriction of processing;  
- under certain conditions, a right to object;  
- safeguards relating to certain automated decisions;  
- a right to lodge a complaint with a supervisory authority;  
- a right to an effective judicial remedy [S43].

The right of access provided for in Article 15 notably makes it possible to know:

- the purposes of the processing;  
- the categories of personal data concerned;  
- the recipients or categories of recipients;  
- the retention period or the criteria used to determine it;  
- the existence of certain other rights;  
- the source of the data where they were not collected from the individual;  
- in the situations provided for by the GDPR, certain information relating to the logic of automated decision-making [S43].

**LEGAL SAFEGUARD:**

> An individual is therefore not legally deprived of means of control over the use of their data by an administration.

---

### CFVR explicitly provides for the exercise of some of these rights

Article 6 of the Order establishing CFVR expressly provides that the rights of access and rectification under Articles 15 and 16 of the GDPR may be exercised [S45].

Depending on the source of the data, these rights are exercised:

- with the SJCF-1D office;  
- or with the public finance center responsible for the individual concerned [S45].

The right to restriction provided for in Article 18 of the GDPR may also be exercised with the SJCF-1D office [S45].

**ESTABLISHED:**

> CFVR is not a processing system placed outside the rights of access, rectification and restriction.

But the Order immediately provides for several restrictions.

---

### First major restriction: the right to object does not apply to CFVR

Article 6 of the CFVR Order explicitly provides that:

> **the right to object provided for in Article 21 of the GDPR does not apply to the processing** [S45].

Since the July 2026 amendment, this exclusion has been expressly linked to the objectives referred to in points (e) and (h) of Article 23(1) of the GDPR [S45].

These provisions notably concern:

- important objectives of general public interest of the Union or a Member State, notably in tax matters;  
- monitoring, inspection or regulatory functions connected notably to those objectives [S43].

The practical consequence is significant.

An individual cannot simply decide:

```
"I object to my data
being used within CFVR"
   ↓
processing stops
```

The right to object is expressly excluded for this processing.

**LEGAL LATITUDE:**

> European law permits, subject to conditions, certain rights to be restricted in order to protect notably important tax interests and the associated monitoring functions.

**ESTABLISHED RESTRICTION:**

> Within CFVR, the right to object provided for in Article 21 of the GDPR does not apply [S45].

This restriction therefore does not, in itself, constitute a violation of the GDPR.

It nevertheless constitutes a concrete limitation on the individual's control over the use of their data.

---

### Second restriction: access and rectification may themselves be limited

The CFVR Order also provides that the rights of access and rectification may be subject to restrictions under the conditions laid down in Article 52 of the French Data Protection Act [S45][S54].

This provision specifically concerns certain processing operations used by administrations to audit or collect taxes [S54].

The rationale is understandable:

```
right of access
   ↓
but
   ↓
do not disclose information
that could compromise
the tax audit
```

An individual subject to a risk analysis may therefore not necessarily be able to immediately obtain all the information that could reveal audit methods or compromise their purpose.

**LEGAL LATITUDE:**

> The law expressly provides for the possibility of restricting certain rights in order to preserve the effectiveness of certain tax functions.

But this possibility creates an obvious tension:

```
to challenge effectively
   ↓
one must understand
what is being done
   but
to preserve the audit
   ↓
certain information
may be restricted
```

---

### The CNIL then becomes an essential intermediary

When the restrictions provided for CFVR apply, the individual exercises their rights through the CNIL under the conditions laid down in Article 118 of the French Data Protection Act [S45][S54].

The CNIL then carries out the necessary checks.

It may arrange for the necessary changes to be made.

It then informs the individual that the checks have been carried out and indicates the existence of a judicial remedy [S54].

Where certain information can be disclosed without compromising the protected purposes, it may be communicated under the conditions provided for by law [S54].

**LEGAL SAFEGUARD:**

> Restricting direct access does not therefore necessarily result in the absence of oversight.

An independent institutional third party can verify the processing.

---

### But a fundamental difference emerges between verification and personal understanding

This architecture simultaneously protects two interests:

```
effectiveness of tax audits
   ↕
individual rights
```

But it may produce a particular situation:

```
the individual suspects
incorrect data or analysis
   ↓
they request access / rectification
   ↓
certain information is restricted
   ↓
the CNIL carries out checks
   ↓
the individual may be informed
that the checks have been carried out
   ↓
without necessarily knowing
all of the protected information
```

**STRUCTURAL LEGAL VULNERABILITY:**

> The more the information necessary to understand the origin of an alert is protected against disclosure, the more the effectiveness of an individual challenge depends on the oversight exercised by the CNIL and, where applicable, by the courts.

This does not mean that the remedy becomes ineffective.

It means that individual oversight may become partly **mediated by an independent authority** rather than exercised directly by the individual.

---

### Rectification becomes particularly important in an interconnected architecture

The right to rectification makes it possible to obtain the correction of inaccurate personal data [S43].

But the architecture examined is no longer necessarily limited to data stored in a single database.

Data may follow a chain:

```
source data
   ↓
transmission
   ↓
cross-referencing
   ↓
analysis
   ↓
indicator
   ↓
algorithmic result
   ↓
case proposed
```

The GDPR also provides that where rectification, erasure or restriction takes place, the controller must in principle communicate it to the recipients to whom the data have been disclosed, unless this proves impossible or involves disproportionate effort [S43].

This safeguard becomes particularly important in a multi-source architecture.

---

### First difficult question: does correcting the data correct its consequences?

Consider a hypothetical situation:

```
incorrect data A
   ↓
cross-referencing with B and C
   ↓
indicator D
   ↓
score / classification E
   ↓
alert F
```

The correction of A is legally regulated.

But several additional questions arise:

> **Is D automatically recalculated?**

> **Is E deleted or reassessed?**

> **Is F withdrawn if it was based on the incorrect information?**

> **Are the recipients of F informed?**

> **Do derived data remain in other environments?**

The GDPR contains mechanisms for rectification, restriction and notification to recipients [S43].

But their application to complex chains of derived data must be examined in practice.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not make it possible to determine precisely the technical mechanism by which a rectification made to source data is propagated to results, indicators, classifications or alerts already produced from those data within CFVR and the secure data platform.

---

### This question is not theoretical for CFVR

The CNIL requires agents to verify notably that the latest tax returns filed have been taken into account before deciding whether to initiate an audit [S37].

This requirement constitutes an important safeguard.

But it also confirms that an algorithmic result may be affected by the state of the data used at the time it is produced.

The following chain is therefore legally relevant:

```
outdated / inaccurate / incomplete data
   ↓
algorithmic analysis
   ↓
apparent anomaly
   ↓
alert
   ↓
human verification
```

Human verification constitutes an essential barrier here.

**DOCUMENTED SAFEGUARD:**

> The agent must not treat the algorithmic signal as an autonomous truth and must analyze the case on the basis of relevant and up-to-date information [S37].

---

### The right to restriction provides an additional safeguard

Article 18 of the GDPR provides notably that an individual may request restriction of processing where they contest the accuracy of data, for the period necessary for the controller to verify their accuracy [S43].

CFVR expressly provides for the exercise of this right with the SJCF-1D office [S45].

Restriction may therefore constitute a particularly important safeguard where information capable of influencing processing is contested.

**LEGAL SAFEGUARD:**

> Contesting the accuracy of data may, under the conditions provided for by the GDPR, lead to the temporary restriction of its processing while its accuracy is being verified [S43][S45].

**TO BE ESTABLISHED:**

> How is this restriction technically propagated when the contested data have already contributed to producing results across several environments?

---

### The issue becomes more complex with derived data

An algorithmic infrastructure does not necessarily merely replicate source data.

It may produce:

- indicators;  
- categories;  
- relationships;  
- anomalies;  
- scores;  
- query results;  
- audit proposals.

CFVR notably feeds GALAXIE with certain links between individuals and entities and PILOT CF with cases proposed for audit [S45].

The question of rectification must therefore potentially be considered at several levels:

```
level 1
source data

level 2
cross-referenced data

level 3
inference / indicator

level 4
algorithmic result

level 5
operational consequence
```

**STRUCTURAL VULNERABILITY:**

> The more an architecture produces derived data from multiple sources, the more the effective correction of inaccurate information requires control not only over the initial data, but also over the results derived from it.

---

### Second difficult question: can an individual know why their case was selected?

The right of access makes it possible to obtain a wide range of information relating to the processing [S43].

But CFVR is specifically a system for detecting and programming tax audits.

Overly detailed disclosure of detection rules could compromise some of its purposes.

Hence the possibility of restricting certain rights [S45][S54].

The individual may therefore face a structural difficulty:

```
to challenge an alert
   ↓
understand why
the system produced it
   but
explaining precisely
the detection method
   ↓
may compromise
the effectiveness of the audit
```

**LEGAL VULNERABILITY:**

> The effectiveness of the right to challenge depends on the balance between the level of information accessible to the individual and the level of secrecy necessary to protect audit methods.

---

### This tension directly relates to the explainability examined in 6.4

The case law examined in 6.4 shows that, where the regime governing automated decisions applies, the complexity of a system does not exempt the controller from providing the explanations legally required [S52].

According to the current sources, CFVR does not constitute a system that automatically decides to initiate an audit.

But the question of explainability remains important because the CNIL itself asks the ministry to carry out work on explainability and bias [S37].

This produces a boundary:

```
necessary secrecy
of audit methods
   ↕
necessary understanding
to exercise rights
```

**TO BE ESTABLISHED:**

> What level of explanation can be provided to an individual regarding the role of a CFVR result in the selection of their case without compromising audit methods?

---

### Informing individuals nevertheless remains mandatory

Regarding the new exchanges between the DGFiP and social security bodies, the CNIL expressly reiterates that each of the administrations concerned must inform individuals in accordance with Articles 12 to 14 of the GDPR [S37].

The ministry indicated that the agreements governing these exchanges will reiterate this obligation [S37].

This is an important point.

The existence of legally authorized exchanges therefore does not automatically remove the obligation to provide information.

**DOCUMENTED SAFEGUARD:**

> The CNIL requires the individuals concerned to be informed of data exchanges between the DGFiP and social security bodies under the conditions provided for by the GDPR [S37].

---

### But general information does not mean individual knowledge of each use

A distinction must be made between:

```
being informed
of the existence of processing
   ≠
knowing that specific data
were used in a specific analysis
   ≠
knowing the result
of that analysis
   ≠
knowing that this result
contributed to a decision
```

These four levels of information do not have the same purpose or necessarily the same legal regime.

**DOCUMENTARY VULNERABILITY:**

> General information about the existence and purposes of CFVR does not, on its own, make it possible to determine the extent to which an individual can concretely trace the use of their data in a particular analysis.

---

### The CNIL has significant supervisory powers

The CNIL is not limited to issuing opinions when processing systems are created or modified.

The GDPR notably grants it powers to:

- require the necessary information;  
- conduct investigations and audits;  
- access the personal data necessary for its tasks;  
- access processing premises and equipment;  
- order certain measures to bring processing into compliance;  
- restrict or prohibit certain processing operations under the conditions provided for by law [S43].

An individual may also lodge a complaint with a supervisory authority where they consider that processing concerning them infringes the GDPR [S43].

**INSTITUTIONAL SAFEGUARD:**

> Oversight of the lawfulness of processing therefore does not depend solely on the administration that processes the data.

---

### The CNIL's prior opinion does not, however, constitute definitive validation of the system

CFVR has existed since 2014.

Since then, its scope has undergone numerous changes [S37][S45].

It has notably been extended:

- to professionals;  
- to individuals connected to businesses;  
- to private individuals;  
- to new sources;  
- to new algorithmic methods;  
- to data originating from platforms;  
- to new administrative exchanges;  
- to a new computing infrastructure;
- and now to data originating from electronic invoicing [S37][S45].

The CNIL has issued several successive opinions on these developments [S37].

But an opinion issued at a given point in time concerns the system presented to it at that time.

**SAFEGUARD:**

> Significant modifications to the system are subject to a legal framework, and some have resulted in new opinions from the CNIL.

**STRUCTURAL VULNERABILITY:**

> The compliance of an evolving architecture cannot be considered definitively established solely because an earlier version or a particular modification was the subject of a CNIL opinion.

Compliance with the GDPR is a continuing obligation.

---

### Ex post oversight therefore becomes essential

The CNIL may investigate an organization:

- following a complaint;  
- following an alert;  
- or on its own initiative [S43].

It may carry out on-site inspections, documentary inspections, hearings or online investigations.

In the event of non-compliance, various corrective measures may be implemented.

This distinction is fundamental:

```
opinion on a proposed system
   ≠
oversight of actual operation
   ≠
finding of permanent compliance
```

**INSTITUTIONAL SAFEGUARD:**

> The existence of a favorable opinion or an opinion containing observations does not deprive the CNIL of its subsequent supervisory powers.

---

### A particular vulnerability emerges from the continuous evolution of systems

Sections 6.3 to 6.5 showed that several characteristics may evolve simultaneously:

```
more data
   +
more sources
   +
more cross-referencing
   +
new algorithms
   +
new recipients
   +
new infrastructure
```

Each of these developments may alter the level of risk to rights and freedoms.

A safeguard designed for a given architecture may therefore become insufficient if the architecture changes substantially.

**LEGAL VULNERABILITY:**

> In an evolving processing system, the effectiveness of safeguards depends on their reassessment when the nature, scale or risks of the processing change.

This question directly relates to the obligation to review the data protection impact assessment when changes in risk justify it [S48].

---

### Judicial remedy constitutes the final safeguard

The GDPR recognizes:

- the right to lodge a complaint with a supervisory authority;  
- the right to an effective judicial remedy against certain decisions of that authority;  
- the right to an effective judicial remedy against a controller or processor where the individual considers that their rights have been infringed [S43].

The specific procedure provided for by Article 118 of the French Data Protection Act also reiterates the existence of a judicial remedy [S54].

**LEGAL SAFEGUARD:**

> Even where an individual cannot directly obtain certain protected information, the processing does not escape all external oversight.

---

### But an effective remedy requires being able to identify the problem sufficiently

A difficulty nevertheless remains.

To effectively challenge processing, an individual must generally be able to identify at least the existence of a problem.

In a complex architecture:

```
collection
   ↓
cross-referencing
   ↓
inference
   ↓
alert
   ↓
transmission
   ↓
consequence
```

an error may arise far from the initial data.

The individual may know the consequence without necessarily immediately knowing:

- the data that caused it;  
- the source of those data;  
- the cross-referencing performed;  
- the inference produced;  
- the system that generated the signal;  
- the recipients who received it.

**STRUCTURAL VULNERABILITY:**

> The more stages, controllers and derived data a processing chain involves, the more the effective exercise of rights depends on the internal traceability of the processing and the ability of supervisory authorities to reconstruct that chain.

---

### This question extends beyond CFVR and relates to the other infrastructures examined in the investigation

The previous chapters separately identified several infrastructures capable of processing information concerning:

- identity;  
- transactions;  
- invoicing;  
- products;  
- the DPP;  
- environmental characteristics;  
- payments.

No source examined currently demonstrates the existence of a single system using all of this information in order to make an individual decision.

But if several of these infrastructures were one day interconnected, the question of rights would become more complex.

```
system A
identity
       ↓
system B
transaction
       ↓
system C
product / DPP
       ↓
system D
environmental information
       ↓
system E
payment
```

The question would no longer be solely:

> **"do I have a right of access within each of these systems?"**

It would become:

> **"can I reconstruct the chain that led to the consequence affecting me?"**

---

### The right of access to each component does not automatically guarantee understanding of the resulting system

This distinction is essential.

Suppose that each infrastructure separately provides:

```
A → access possible
B → access possible
C → access possible
D → access possible
E → access possible
```

It does not automatically follow that:

```
A + B + C + D + E
   ↓
possible understanding
of the resulting decision
```

**STRUCTURAL LEGAL VULNERABILITY:**

> In an interconnected architecture, the effectiveness of rights must be assessed not only processing operation by processing operation, but also in light of the individual's ability to understand and challenge the processing chain that produces a consequence affecting them.

This conclusion constitutes a new legal bridge with the previous chapters.

---

### The connection with fundamental rights must nevertheless remain rigorous

The right to the protection of personal data is not merely a technical requirement.

It contributes to the protection of individuals' rights and freedoms.

But not every collection of data or administrative processing operation automatically constitutes an infringement of a fundamental right.

The legally relevant question is:

```
interference / processing
   ↓
legal basis
   ↓
legitimate purpose
   ↓
necessity
   ↓
proportionality
   ↓
safeguards
   ↓
effective rights
   ↓
independent oversight
   ↓
effective remedy
```

A legally problematic interference may arise when this balance is no longer respected.

---

### The real point of vulnerability is therefore effectiveness

After the previous sections, a common thread emerges.

Protection does not rely on the technical impossibility of using the data.

It relies on a succession of legal and organizational safeguards:

```
purpose limitation
   ↓
minimization
   ↓
proportionality
   ↓
security
   ↓
human intervention
   ↓
information
   ↓
access
   ↓
rectification
   ↓
restriction
   ↓
CNIL oversight
   ↓
judicial remedy
```

The more infrastructures become capable of collecting, cross-referencing and analyzing data, the more important the effectiveness of each of these safeguards becomes.

**STRUCTURAL VULNERABILITY:**

> The protection of rights and freedoms therefore does not rely solely on the formal existence of rights, but on the practical ability to exercise them and on the existence of authorities capable of overseeing processing where individual access must be restricted.

---

### Questions for testing this effectiveness

The investigation can now ask much more precise questions:

> **1. Can an individual obtain a list of the data concerning them that are actually used within CFVR and their source?**

> **2. Can they know the recipients to whom results concerning them have been transmitted?**

> **3. When data are rectified, what mechanisms ensure the correction or recalculation of results derived from those data?**

> **4. Is a restriction requested under Article 18 propagated to the environments and results in which the data have already been used?**

> **5. Is it possible to know the role played by CFVR in the selection of a case without revealing methods whose confidentiality is necessary for tax audits?**

> **6. What information is actually communicated to an individual when their right of access is exercised through the CNIL?**

> **7. What mechanisms enable the CNIL to reconstruct the complete chain when data have circulated between several processing systems or administrations?**

> **8. Are individuals informed with sufficient precision about the new exchanges between the DGFiP and social security bodies?**

> **9. How are rights exercised when several controllers intervene successively within the same chain?**

> **10. Do developments in CFVR result in regular reassessment of the effectiveness of rights and the restrictions imposed on them?**

These questions do not presume any violation.

They make it possible to test whether the safeguards are genuinely operational.

---

### Conclusion of 6.6

**ESTABLISHED:**

> CFVR provides for the exercise of the rights of access, rectification and restriction [S45].

**ESTABLISHED RESTRICTION:**

> The right to object provided for in Article 21 of the GDPR does not apply to CFVR [S45].

**ESTABLISHED RESTRICTION:**

> The rights of access and rectification may be subject to restrictions under the conditions provided for by the French Data Protection Act [S45][S54].

**LEGAL SAFEGUARD:**

> Where a restriction applies, a procedure for exercising rights through the CNIL is provided for, and a judicial remedy remains available [S54].

**LEGAL SAFEGUARD:**

> The GDPR provides mechanisms notably enabling the rectification of inaccurate data, the restriction of certain processing operations and the notification of certain rectifications or restrictions to recipients [S43].

**DOCUMENTED SAFEGUARD:**

> The CNIL reiterates that the DGFiP and social security bodies must inform the individuals concerned of the data exchanges planned between them [S37].

**INSTITUTIONAL SAFEGUARD:**

> The CNIL has investigative and supervisory powers independent of its prior opinions, and an individual may lodge a complaint where they consider that the processing of their data infringes the GDPR [S43].

**LEGAL VULNERABILITY:**

> Individual protection becomes more dependent on oversight by the CNIL and the courts where the information necessary for a direct understanding of the processing may lawfully be restricted.

**STRUCTURAL VULNERABILITY:**

> In a multi-source architecture, the effective rectification of data requires control over the results, inferences and transmissions already produced from those data.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not make it possible to determine precisely how a rectification or restriction is propagated to algorithmic results and derived data already produced within CFVR, the secure data platform or the applications fed by their results.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not make it possible to precisely measure the level of information actually obtained by an individual where certain information relating to CFVR is subject to the restrictions provided for by tax law.

**TO BE ESTABLISHED:**

> Can an individual sufficiently reconstruct the chain leading from source data to an alert or an audit proposal in order to effectively exercise their rights where several processing systems contributed to the result?

**TO BE ESTABLISHED:**

> Do traceability mechanisms enable the CNIL to reconstruct this complete chain where the individual themselves cannot directly access certain information?

**LEGALLY DEDUCIBLE:**

> If several infrastructures relating to identity, transactions, invoicing, products, environmental data or payments were one day interconnected to produce an individual consequence, the existence of separate rights within each infrastructure would not necessarily be sufficient to guarantee an effective remedy against the result produced by their combination.

**NOT ESTABLISHED:**

> The sources examined do not make it possible to conclude that the restrictions currently provided for within CFVR deprive individuals of an effective remedy or are contrary to the GDPR.

---

## 6.7 Safeguards specific to the infrastructures examined

**Status: ESTABLISHED SPECIFIC SAFEGUARDS / DOCUMENTED INTERFACES / IDENTIFIED LEGAL BOUNDARIES**

The previous sections examined the general safeguards applicable to data processing:

- purpose;  
- legal basis;  
- minimization;  
- proportionality;  
- security;  
- profiling;  
- automated decisions;  
- data subject rights;  
- oversight by independent authorities.

But the infrastructures examined in the previous chapters also have safeguards specific to them.

This section therefore examines separately:

```
electronic invoicing
   +
digital identity
   +
Digital Product Passport
   +
environmental data
   +
payment / digital euro
```

The objective is then to determine what happens to these safeguards when several infrastructures may interact.

---

### First finding: the infrastructures are not legally designed as a single database

The previous chapters identified several technical possibilities for interconnection.

But the legal texts examined instead organize several forms of separation.

These notably include:

```
tax data
→ specified tax purposes

digital identity
→ user control
→ selective disclosure
→ segregation

DPP
→ product information
→ specified access rights
→ protection of customer data

payment
→ specific purposes
→ data protection
→ specific safeguards
```

**STRUCTURAL SAFEGUARD:**

> None of the texts examined establishes a general right allowing all data originating from these infrastructures to be freely merged.

Technical interoperability therefore does not constitute a general authorization for legal interconnection.

---

### European digital identity includes particularly strong safeguards

The eIDAS 2 Regulation provides that the European Digital Identity Wallet operates under the control of the user [S55].

The user must notably be able to:

- select the data they wish to present;  
- combine different attributes;  
- use selective disclosure;  
- view the relying parties with which they have interacted;  
- know, where applicable, the data exchanged;  
- request the deletion of certain data;  
- report a suspicious request to the data protection authority [S55].

The wallet may also generate and locally store pseudonyms.

The Regulation even provides for technologies enabling a user to demonstrate that a condition is satisfied without revealing the underlying data.

Example:

```
full attribute
"date of birth: ..."
   ↓
minimal proof
"over 18: YES"
```

rather than:

```
transmission of
full identity
   +
date of birth
   +
other unnecessary attributes
```

**LEGAL AND TECHNICAL SAFEGUARD:**

> The European digital identity architecture explicitly incorporates mechanisms designed to reduce the amount of information disclosed when accessing a service [S55].

---

### The wallet provider must not become a general observer of its user

A particularly important safeguard appears in the Regulation.

The wallet provider must not collect information about its use that is not necessary for the provision of the service [S55].

It must ensure a form of "unobservability" preventing it from obtaining a general overview of the transactions carried out by the user.

It is also prohibited from combining identification data or other personal data linked to the wallet with data originating from other services where such combination is not necessary for the wallet service, unless expressly requested by the user [S55].

Attribute attestation services are also subject to separation requirements.

**MAJOR SAFEGUARD:**

> The European Digital Identity Wallet is not legally designed to allow its provider to freely reconstruct all of its user's digital activities.

This safeguard directly addresses one of the risks identified in the previous chapters.

---

### Refusing to use the wallet must not become a general ground for exclusion

The Regulation also provides that access to public and private services, the labor market and the freedom to conduct a business must not be restricted or made disadvantageous solely because an individual does not use the European Digital Identity Wallet [S55].

Alternative means must remain available.

The consequence is important.

```
use of the wallet
   ↓
possible
   but
refusal to use the wallet
   ↓
must not, by itself,
result in exclusion
```

**SAFEGUARD OF FREEDOM OF CHOICE:**

> The current framework explicitly seeks to prevent the European Digital Identity Wallet from becoming a general and mandatory condition for access to services.

This safeguard will be particularly important to monitor during the practical deployment of the system.

---

### But the wallet is also designed to combine attributes

The same infrastructure has another characteristic.

The wallet must enable its user to:

> request, obtain, select, combine, store, delete, share and present person identification data and electronic attestations of attributes [S55].

It is therefore designed to be able to present several attributes originating from distinct sources to a relying party.

```
identity
   +
attribute A
   +
attribute B
   +
attestation C
   ↓
presentation to a service
```

This capability is not, in itself, a vulnerability.

It is precisely one of the functions of the wallet.

But it creates an important boundary.

**LEGAL BOUNDARY:**

> Protection does not rely on the technical impossibility of combining attributes. It relies on user control, limitation of the data requested, the purpose of the service and the rules applicable to the relying party.

---

### Relying parties must declare the data they request

A party wishing to use the European Digital Identity Wallet must register and notably declare the intended use as well as the data it intends to request [S55].

It must then not request from the user any data other than those declared.

It must also identify itself to the user.

**LEGAL SAFEGUARD:**

> A relying party therefore does not have indiscriminate access to the attributes contained in the wallet.

The architecture operates according to a logic of specified access:

```
service
   ↓
declared purpose
   ↓
declared attributes
   ↓
request
   ↓
selective presentation
```

and not:

```
service
   ↓
access to the entire wallet
```

---

### The DPP also contains a fundamental separation

The Digital Product Passport is designed as an infrastructure for product-related data [S56].

It may notably contain information relating to:

- product characteristics;  
- its compliance;  
- its life cycle;  
- its durability;  
- certain environmental characteristics;  
- its traceability.

The DPP must be associated with a unique product identifier and operate within an open and interoperable data environment [S56].

Depending on the applicable requirements, it may be established at the level of:

```
model
   or
batch
   or
item
```

The latter possibility significantly increases the potential granularity of product traceability.

But the Regulation immediately introduces an important safeguard.

---

### The DPP is not legally an environmental record of the consumer

The ESPR explicitly provides that:

> personal data relating to customers must not be stored in the Digital Product Passport without their explicit consent [S56].

This rule breaks an association that might otherwise appear obvious:

```
identifiable product
   ↓
identifiable buyer
```

The first element does not legally produce the second.

A DPP may precisely identify a product or item without identifying its owner or user.

**MAJOR LEGAL SAFEGUARD:**

> The current DPP framework explicitly separates product identification from the personal identification of the customer.

**NOT ESTABLISHED:**

> In the texts examined, the European DPP does not constitute an "individual environmental passport" recording a citizen's purchases or personal environmental footprint.

This distinction must be strictly maintained.

---

### But the unique identifier and interoperability make another operation technically possible

The previous safeguard does not mean that a product can never be linked to an individual in another system.

A commercial transaction may already contain:

```
buyer
   +
seller
   +
product
   +
date
   +
amount
```

The DPP may, for its part, contain:

```
product identifier
   +
product characteristics
   +
environmental data
```

An external association could therefore theoretically produce:

```
transaction
   ↓
identified product
   ↓
DPP
   ↓
environmental characteristics
```

This technical possibility has already been identified in the previous chapters.

But legally:

**LEGAL BOUNDARY:**

> The protection of the DPP against the storage of customers' personal data does not constitute a general prohibition on any external cross-referencing between a product and a transaction.

Such cross-referencing would, however, constitute separate processing that would need its own purpose, its own legal basis and would have to comply with the requirements of necessity, proportionality and minimization where it involves personal data [S43][S44][S53][S56].

---

### A first asymmetry therefore emerges

The DPP protects its own content:

```
DPP
   ↓
no customer personal data
without explicit consent
```

But this safeguard concerns:

> **what is stored in the DPP.**

It does not necessarily mean:

> **that no other system can use the product identifier to perform cross-referencing authorized under another legal basis.**

**STRUCTURAL VULNERABILITY:**

> A safeguard preventing the centralization of personal data within one infrastructure does not necessarily constitute a prohibition on reconstructing the relationship between several data points through external processing.

This is an important distinction for the entire investigation.

---

### The digital euro also includes a particularly strong safeguard

The proposed framework for the digital euro contains an explicit prohibition:

> **the digital euro must not be programmable money** [S57].

A unit of digital euro must therefore not contain intrinsic logic imposing:

```
usable only
for product X
   or
prohibited for product Y
   or
usable only
before a certain date
   or
usable only
with a certain beneficiary
```

The ECB also reiterates that such limitations would be incompatible with the chosen design of the digital euro [S57].

**MAJOR MONETARY SAFEGUARD:**

> The proposed framework prohibits the digital euro from intrinsically becoming money whose use would be restricted according to goods, services, dates or beneficiaries.

This safeguard directly addresses one of the strongest concerns that may arise around a central bank digital currency.

---

### But "non-programmable money" does not mean "payments cannot be conditional"

This is where a much subtler boundary emerges.

The proposal explicitly distinguishes:

```
**PROGRAMMABLE MONEY**

logic embedded in the money
that limits its fungibility
   ↓
PROHIBITED
```

from:

```
**CONDITIONAL PAYMENT**

software
   +
predetermined condition
   +
payer / payee agreement
   +
automatic triggering
   ↓
PROVIDED FOR
```

[S57]

A conditional transaction is defined as a transaction automatically triggered when predetermined conditions agreed by the payer and the payee are met.

The proposal even allows the ECB to provide the standards and functionalities necessary for such payments, including the reservation of funds [S57].

**EXPLICIT LEGAL LATITUDE:**

> The proposed framework prohibits the intrinsic programming of the money but allows the programming of certain conditions governing the execution of a payment.

This distinction is fundamental.

---

### The protection therefore concerns the money, not the existence of any conditional logic surrounding the payment

The boundary can be represented as follows:

```
"this euro can only purchase
certain categories of products"
   ↓
programmable money
   ↓
PROHIBITED
```

but:

```
"execute this payment
if agreed condition X
is satisfied"
   ↓
conditional payment
   ↓
PROVIDED FOR
```

**LEGAL FRICTION POINT:**

> The prohibition of programmable money therefore does not constitute a general prohibition on any infrastructure capable of automatically conditioning the execution of a payment.

This is probably one of the most important distinctions identified in this investigation.

---

### This still does not mean that an environmental condition is provided for

The documentary boundary must immediately be maintained.

Official examples of conditional payments notably concern:

- payment upon delivery;  
- pay-per-use;  
- payments linked to certain milestones;  
- certain automated machine-to-machine payments [S57].

No source examined demonstrates that a digital euro payment is intended to be conditional on:

- an individual environmental score;  
- a personal carbon footprint;  
- a DPP;  
- a purchase history;  
- or an environmental classification of an individual.

**NOT ESTABLISHED:**

> No official mechanism examined currently links environmental data or a DPP to the authorization or refusal of a digital euro payment.

---

### But the condition may originate from information external to the payment

A conditional payment necessarily requires a system to be able to determine whether:

```
condition X
   =
satisfied
   or
not satisfied
```

The work examined in the previous chapters has already experimentally established the possibility for an external system to verify a condition used to trigger a payment.

The general technical structure is therefore:

```
external source
   ↓
condition verification
   ↓
condition satisfied?
   ↓
YES / NO
   ↓
payment execution
```

The nature of the external source depends on the service concerned.

**LEGAL BOUNDARY:**

> The proposed framework allows for the existence of a condition external to the payment, but the lawfulness of the condition itself would depend on its purpose, the mechanism used, the data processed, the agreement of the parties and the other applicable rules.

In other words:

> **the capability to impose conditions exists; the legal freedom to choose any condition is not established.**

---

### Digital identity and the digital euro have an explicitly provided interface

Another element is particularly important.

The proposed Regulation on the digital euro provides that front-end services must be:

> **interoperable with or integrated into European Digital Identity Wallets** [S57].

The European Digital Identity Wallet, for its part, enables the presentation of identity data and attestations of attributes to public or private services [S55].

We therefore have an interconnection here that is no longer merely technically deduced:

```
European Digital
Identity Wallet
   ↕
digital euro services
```

**DOCUMENTED INTERFACE:**

> The proposed framework for the digital euro explicitly provides for interoperability or integration with the European Digital Identity Wallet.

This interface does not mean that all attributes in the wallet become accessible to the payment system.

The safeguards of the eIDAS 2 Regulation continue to apply.

But the existence of the interface itself is documented.

---

### The identity → payment bridge is therefore established, but strictly limited in scope

The conclusion must be precise.

We can now establish:

```
digital identity
   ↕
provided interface
   ↕
digital euro
```

But not:

```
all identity attributes
   ↓
all payments
```

and even less:

```
identity
   +
environment
   ↓
payment authorization
```

**ESTABLISHED AT THE LEVEL OF THE PROPOSED FRAMEWORK:**

> An interface between the European Digital Identity Wallet and digital euro payment services is explicitly provided for [S57].

**NOT ESTABLISHED:**

> This interface does not demonstrate any use of environmental attributes or DPPs to authorize, refuse or restrict a payment.

---

### The digital euro framework also provides strong privacy safeguards

The proposal notably distinguishes between online and offline payments [S57].

For offline payments, the intended level of privacy should be close to that of cash.

The details of offline transactions must not be accessible to the ECB or national central banks under the same conditions as online payments.

For online payments, the proposal provides for technical and organizational measures designed to prevent data transmitted to the Eurosystem from enabling the direct identification of individual users [S57].

**PRIVACY SAFEGUARD:**

> The proposed architecture is not based on the idea that the ECB should have access to a general nominative history of individual payments.

---

### European data protection authorities have nevertheless called for additional safeguards

The EDPB and EDPS examined the digital euro proposal.

They acknowledge the efforts made regarding privacy protection, notably:

- the offline mode;  
- data protection by design;  
- minimization;  
- maintaining the choice between cash and the digital euro.

But they also called for the design to avoid excessive centralization of personal data by the ECB or national central banks.

**INSTITUTIONAL POINT OF VIGILANCE:**

> Even an architecture explicitly designed to provide a high level of privacy must be examined in light of the amount of data centralized and the allocation of responsibilities among the different actors.

---

### The ability to pay in cash itself constitutes an important safeguard

The proposed framework for the digital euro is not intended to eliminate cash.

The digital euro must constitute an additional means of payment.

European data protection authorities have expressly welcomed maintaining the choice between the digital euro and cash.

The ECB also states that the digital euro should complement banknotes and coins.

**SAFEGUARD OF FREEDOM OF CHOICE:**

> Under the framework currently proposed, the digital euro must not constitute the only available means of payment.

This safeguard significantly reduces the risk that a restriction specific to the digital euro would automatically result in a general inability to pay.

---

### An interesting architecture emerges when only the documented interfaces are assembled

At this stage, it is necessary to distinguish what is actually established from what remains hypothetical.

The documented elements already make it possible to write:

```
DIGITAL IDENTITY
   ↓
provided interface
   ↓
DIGITAL EURO

DIGITAL EURO
   ↓
conditional payments possible
   ↓
external condition verified

PRODUCT
   ↓
unique identifier
   ↓
DPP
   ↓
product / environmental data

TRANSACTION
   ↓
may identify a product
```

By contrast, the following link remains absent:

```
DPP / environment
   ↓
payment condition
```

**DOCUMENTARY BOUNDARY:**

> Several segments of the chain exist separately or have documented interfaces, but the connection enabling environmental data originating from the DPP to determine a payment condition is not established.

---

### The real potential weakness is therefore not the absence of safeguards

There are numerous safeguards.

These notably include:

```
IDENTITY

→ user control

→ selective disclosure

→ unobservability

→ data separation

→ alternatives to the wallet

DPP

→ access rights

→ decentralized architecture

→ no customer personal data

  without explicit consent

DIGITAL EURO

→ privacy

→ cash maintained

→ programmable money prohibited
```

But each of these safeguards primarily protects **its own scope**.

The cross-cutting question becomes:

> **What happens when information leaves its original infrastructure and becomes a legally authorized input into another processing operation?**

This is where the most interesting point of friction in 6.7 lies.

---

### A local safeguard does not necessarily constitute a global prohibition on cross-referencing

Three examples illustrate this distinction.

#### DPP

```
no customer personal data
in the DPP without consent
```

does not automatically mean:

```
impossibility of cross-referencing elsewhere
a transaction and the product identifier
```

#### Digital identity

```
wallet provider
must not observe
all transactions
```

does not mean:

```
no authorized service
may receive an attribute
presented by the user
```

#### Digital euro

```
programmable money prohibited
```

does not mean:

```
conditional payment prohibited
```

**STRUCTURAL VULNERABILITY:**

> Several strong safeguards identified in the texts are scope-specific safeguards: they limit what an infrastructure or actor may do directly, without necessarily constituting a general prohibition on any subsequent processing or any authorized interface with another infrastructure.

---

### This is where Sections 6.2 to 6.6 regain their full importance

Information leaving its silo does not enter a legal vacuum.

Its subsequent processing should still satisfy the requirements examined previously:

```
legal basis
   ↓
purpose
   ↓
compatibility / new legal basis
   ↓
necessity
   ↓
minimization
   ↓
proportionality
   ↓
security
   ↓
rights
   ↓
oversight
```

Thus, the existence of technical interfaces does not remove the general safeguards.

But conversely:

> **the safeguards specific to each infrastructure are not necessarily sufficient, on their own, to prevent any future interconnection.**

---

### A particularly important boundary emerges around consent

Several protections identified rely on an action or request by the user.

For example:

- voluntary presentation of attributes in the wallet;  
- explicit consent for certain personal data in the DPP;  
- payment conditions agreed between payer and payee.

This constitutes an important safeguard.

But consent is legally valid only where it meets the applicable requirements, notably where it must be freely given.

A question would therefore arise if access to a good, service or means of payment became, in practice, conditional on accepting the cross-referencing of data.

**LEGAL BOUNDARY:**

> The formal existence of consent or agreement would not necessarily be sufficient if the legal conditions required for it to be considered freely given and valid were no longer met.

**NOT ESTABLISHED:**

> The sources examined do not demonstrate the current existence of a system requiring an individual to share environmental data in order to access a payment or an essential service.

---

### Freedom of choice therefore constitutes a cross-cutting safeguard to monitor

Two infrastructures include particularly interesting protections in this respect.

For digital identity:

```
wallet
   ↓
must not become
the only means of access
```

For the digital euro:

```
digital euro
   ↓
complement to cash
   ↓
no mandatory replacement
```

This redundancy constitutes a strong safeguard.

It means that the current framework preserves alternative means.

**CROSS-CUTTING SAFEGUARD:**

> As long as genuine alternatives remain accessible without unjustified disadvantage, the ability of a digital infrastructure to impose, on its own, a condition on economic or administrative life as a whole remains legally and practically limited.

The important word, however, is:

> **genuine.**

An alternative existing only in law but becoming impracticable in practice would raise a different question.

---

### At this stage, the most important boundary can be identified

The investigation does not make it possible to establish:

```
identity
   +
invoicing
   +
DPP
   +
environment
   +
payment
   ↓
individual control
```

But it now makes it possible to establish something more precise:

```
each infrastructure
has its own safeguards
   ↓
certain interfaces
between infrastructures
are explicitly provided for
   ↓
certain external capabilities
can provide conditions
   ↓
local safeguards
do not necessarily amount to
a global prohibition
on future cross-referencing
   ↓
any new cross-referencing
would then have to pass
the general safeguards
examined in 6.1 to 6.6
```

This is the boundary that must be preserved going forward.

---

### Questions now open

> **1. What categories of attributes will actually be usable in the integration between the European Digital Identity Wallet and digital euro services?**

> **2. Can the data presented during this interaction be technically and legally reused for purposes other than authentication or execution of the requested service?**

> **3. How will the wallet's unobservability be audited in interactions with payment services?**

> **4. What safeguards prevent a product or transaction identifier from being used to indirectly reconstruct a relationship between an individual and a DPP without storing that relationship in the DPP itself?**

> **5. What categories of external sources will be able to provide the conditions used by future conditional payment services?**

> **6. To what extent can a payment condition relate to an attribute concerning the payer without becoming incompatible with data protection, proportionality or non-discrimination rules?**

> **7. How will the existence of genuine alternatives be guaranteed when the European Digital Identity Wallet or the digital euro are integrated into public or private services?**

> **8. Can an architecture that is legally compliant silo by silo become disproportionate when its interfaces make it possible to reconstruct information that each silo was specifically designed not to centralize?**

The last question probably constitutes the main cross-cutting research issue arising from this section.

---

### Conclusion of 6.7

**ESTABLISHED SAFEGUARD:**

> The European Digital Identity Wallet provides for user control, selective disclosure, unobservability of its use by the provider and limitations on the combination of data [S55].

**ESTABLISHED SAFEGUARD:**

> Refusing to use the European Digital Identity Wallet must not, by itself, restrict or disadvantage access to public or private services; alternatives must remain available [S55].

**ESTABLISHED SAFEGUARD:**

> The DPP must not store personal data relating to customers without their explicit consent [S56].

**ESTABLISHED SAFEGUARD:**

> The identification of a product or item in a DPP does not legally constitute, by itself, the identification of its buyer [S56].

**PROPOSED SAFEGUARD:**

> The proposed framework for the digital euro prohibits programmable money and maintains the principle of fully fungible money [S57].

**EXPLICIT LEGAL LATITUDE IN THE PROPOSAL:**

> This prohibition does not extend to conditional payments: the proposed framework expressly provides for payments automatically triggered when predetermined and agreed conditions are met [S57].

**DOCUMENTED INTERFACE IN THE PROPOSAL:**

> Digital euro front-end services must be interoperable with or integrated into European Digital Identity Wallets [S57].

**LEGAL BOUNDARY:**

> The prohibition of programmable money protects the fungibility of the money, but does not constitute a general prohibition on any conditional logic applied to the execution of a payment.

**STRUCTURAL VULNERABILITY:**

> The safeguards specific to the infrastructures examined primarily protect their respective scopes. They do not necessarily constitute a general prohibition on any external association of data where another processing operation has a valid legal basis.

**STRUCTURAL VULNERABILITY:**

> An architecture may avoid centralizing a relationship within each of its components while technically allowing that relationship to be reconstructed in a separate processing operation by cross-referencing their identifiers or data.

**TO BE ESTABLISHED:**

> Are the segregation safeguards provided separately for identity, products and payments sufficient to prevent a future interconnection from reconstructing, within another processing operation, relationships that each infrastructure considered in isolation does not retain?

**TO BE ESTABLISHED:**

> What legal limits would apply to the choice of an external condition used to trigger a conditional payment where that condition concerns data or attributes relating to an individual?

**NOT ESTABLISHED:**

> No element examined demonstrates that environmental data, a DPP, a consumption history or an individual environmental score is currently intended to authorize, refuse or restrict a digital euro payment.

**NOT ESTABLISHED:**

> The digital euro has not yet been adopted or issued as of September 3, 2026. The provisions examined concerning its legal architecture remain those of the legislative framework currently under negotiation.

---

## 6.8 Evolution of purposes and the legal framework

**Status: ESTABLISHED LEGAL EVOLUTION / NON-IMMUTABLE SAFEGUARDS / FUTURE BOUNDARIES TO BE ESTABLISHED**

The previous sections established a significant set of safeguards.

They notably show that current law:

- limits the purposes of processing;  
- requires a legal basis;  
- regulates reuse;  
- imposes necessity, proportionality and minimization;  
- protects certain individual decisions against excessive automation;  
- provides for rights and avenues of redress;  
- imposes specific safeguards on certain infrastructures;  
- currently prohibits certain uses, such as programmable money under the proposed framework for the digital euro.

One question nevertheless remains essential:

> **do these safeguards permanently fix the legally authorized purposes and uses?**

The answer is no.

A legal protection applicable today does not necessarily constitute a permanent legal impossibility.

---

### Three different situations must be distinguished

The evolution of an infrastructure may result from very different legal mechanisms.

```
1. same purpose
   +
   technical evolution

2. new use
   compatible with the initial purpose

3. new purpose
   +
   new legal basis
```

These three situations must not be confused.

The GDPR regulates further processing and notably provides for an assessment of the compatibility of a new purpose with the purpose that initially justified the collection [S43][S46].

But where new processing is based on a provision of Union or national law satisfying the applicable requirements, the law may also create or modify the legal basis allowing that processing [S43][S46][S47].

**LEGAL SAFEGUARD:**

> An administration cannot simply decide that data collected for a specified purpose may now be used for any other purpose.

**LEGAL LATITUDE:**

> The legislature or competent regulatory authority may nevertheless modify the legally authorized scope of processing where the conditions laid down by higher-ranking law are respected.

The difference is fundamental.

---

### Purpose limitation is therefore not a guarantee of immutability

An overly simplistic reading of the principle of purpose limitation would suggest:

```
data collected for X
   ↓
usable only for X
forever
```

The law operates in a more complex manner.

Depending on the circumstances, an evolution may result from:

```
initial purpose
   ↓
compatible further processing
```

or:

```
initial purpose
   ↓
new legal text
   ↓
new authorized processing
under new conditions
```

[S43][S46]

**LEGAL VULNERABILITY:**

> A safeguard based on the current purpose of processing limits present uses, but does not guarantee that the legal scope of that processing can never evolve.

This does not mean that every evolution would be authorized.

It means that the boundary is legal and not technically immutable.

---

### CFVR provides a concrete example of the gradual evolution of the same infrastructure

This possibility is not merely theoretical.

CFVR has existed since 2014 [S58].

Since its creation, its framework has been amended several times.

```
2014

creation of CFVR
   ↓
2017

modification of the processing
   +
experimental extension
to fraud involving individuals
   ↓
2021

further modification
   +
connection with the collection
of certain public data
from online platforms
   ↓
2024

further modification
   ↓
2026

further modification
   +
electronic invoicing
   +
new sources
   +
exchanges with social security bodies
   +
use within the secure data platform
```

[S37][S45][S58]

**ESTABLISHED:**

> The legal scope of CFVR has evolved through successive stages since its creation.

The processing nevertheless retains the same general identity:

> **"targeting fraud and enhancing the value of queries."**

---

### An infrastructure can therefore retain its name while changing significantly in scale

This observation is important.

The evolution of a public system does not necessarily require:

```
old system
   ↓
removal
   ↓
new system
```

It may take the form of:

```
same infrastructure
   ↓
new source
   ↓
new category of data
   ↓
new recipient
   ↓
new capability
   ↓
new legal amendment
```

CFVR provides a documented example of precisely this type of evolution [S58].

**ESTABLISHED:**

> The institutional continuity of a processing operation does not mean that its scope of data, sources, recipients or methods of use remains stable.

---

### The 2017 development is particularly revealing

In 2017, the CFVR framework explicitly distinguished between:

```
fraud involving
businesses
   ↓
permanent processing
```

and:

```
fraud involving
individuals
   ↓
two-year
experiment
```

[S58]

The processing could therefore experimentally use data concerning individuals with no connection to a business.

The current framework now covers fraud involving **both businesses and individuals** [S45][S58].

This evolution provides a particularly clear example:

```
limited / experimental capability
   ↓
evaluation and legal evolution
   ↓
integration into
a broader scope
```

**LEGAL VULNERABILITY:**

> The experimental or limited nature of processing at a given date does not guarantee that its scope will remain experimental or limited.

This does not mean that every experiment necessarily becomes permanent.

It merely demonstrates that making it permanent constitutes a legally possible evolution where a new framework authorizes it.

---

### The integration of electronic invoicing provides a second example

CFVR already existed before the reform examined in this investigation.

Electronic invoicing constitutes a distinct infrastructure, developed notably to meet its own tax and economic requirements.

In 2026, data originating from this infrastructure were expressly integrated among the categories of data used by CFVR [S37][S45].

The sequence is therefore documented:

```
infrastructure A
electronic invoicing
   +
infrastructure B
CFVR
   ↓
legal amendment
   ↓
data from A
used in B
```

**ESTABLISHED:**

> An existing data infrastructure may subsequently become a new legally authorized source for a pre-existing processing operation.

This observation is central to the entire investigation.

---

### The question is therefore no longer solely whether two infrastructures are connected today

It is necessary to distinguish:

```
CURRENT INTERCONNECTION
   ↓
factual question
```

from:

```
FUTURE INTERCONNECTION
   ↓
legal question
   +
possible evolution of the law
```

The current absence of an interconnection is important information.

But it does not make it possible to state:

> **"this interconnection can never legally exist."**

Conversely, the possibility of changing the law provides absolutely no basis for stating:

> **"this interconnection will be created."**

**LEGAL SAFEGUARD:**

> Any new interconnection involving personal data would have to comply with the legal framework applicable at the time of its implementation.

**NOT ESTABLISHED:**

> The abstract legal possibility of modifying a processing operation does not demonstrate any institutional intention to create a specific interconnection.

---

### This distinction is essential for the DPP

The current DPP framework provides strong safeguards [S56].

But the ESPR itself provides that the delegated acts applicable to the different product groups will notably specify:

```
DPP data
   +
model / batch / item level
   +
actors with access
   +
data accessible to each
   +
period of availability
```

[S56]

The Regulation also provides that where other provisions of Union law require or allow specific data to be included in the DPP, those data may be incorporated in accordance with the applicable delegated act.

**ESTABLISHED:**

> The specific content of the DPP and its access rights are not entirely fixed in the framework Regulation: they must be specified for the different product groups through delegated acts [S56].

---

### But some DPP limitations remain embedded in the Regulation itself

This capacity for evolution does not remove higher-level safeguards.

The Regulation notably provides that personal data relating to customers must not be stored in the DPP without their explicit consent [S56].

Evolution through a delegated act therefore does not mean:

```
Commission
   ↓
unlimited freedom
   ↓
any data
in the DPP
```

Delegated acts must remain within the scope of the delegation and comply with applicable higher-ranking law.

**LEGAL SAFEGUARD:**

> The ability to specify or modify the content of an infrastructure through subsequent acts does not remove the limitations laid down by the Regulation governing it.

---

### The European Digital Identity Wallet also has an evolving architecture

The eIDAS 2 Regulation establishes the fundamental safeguards of the wallet [S55].

But its practical operation also relies on implementing acts determining technical standards, specifications and procedures.

This notably concerns:

- wallet interfaces;  
- the issuance and presentation of attributes;  
- the identification of relying parties;  
- registration procedures;  
- certain certification arrangements;  
- interoperability [S55].

The Regulation also allows several attestations of attributes to be combined under the control of the user.

**ESTABLISHED:**

> The fundamental legal framework of the wallet is established by the Regulation, while a significant part of its practical operation is specified through implementing acts and technical specifications [S55].

---

### Technical evolution can therefore significantly change practical capabilities without removing legal safeguards

This is an additional distinction.

```
stable legal rule
   ↓
new specification
   ↓
new technical capability
```

is not necessarily:

```
new legal purpose
```

But the evolution of standards may increase:

- interoperability;  
- the number of available attributes;  
- the number of compatible services;  
- the ease with which certain proofs can be presented;  
- the number of possible interactions between infrastructures.

**LEGAL VULNERABILITY:**

> The evolution of an infrastructure's practical capabilities may precede or accompany the evolution of its uses, making it necessary to regularly reassess whether the initial legal safeguards remain appropriate to the capabilities actually deployed.

---

### The boundary is even more evident for the digital euro

Unlike eIDAS 2 and the ESPR, the Regulation establishing the digital euro has not yet been definitively adopted at the time of this investigation [S57].

The safeguards examined in 6.7 concerning notably:

- the prohibition of programmable money;  
- conditional payments;  
- privacy;  
- integration with the European Digital Identity Wallet;

must therefore be qualified according to their status in the legislative process.

**LEGAL SAFEGUARD:**

> Until the text is adopted, the provisions of the proposal must not be presented as a definitive and immutable framework.

**TO BE ESTABLISHED:**

> What safeguards, definitions and technical possibilities relating to conditional payments and interoperability with the European Digital Identity Wallet will appear in the text ultimately adopted?

---

### The central point now emerges: legal protection is dynamic

The previous chapters could give the impression of a static architecture:

```
system
   +
purpose
   +
safeguards
   =
definitive balance
```

The history of CFVR shows a different reality.

The balance looks more like:

```
infrastructure
   ↓
initial legal framework
   ↓
new capability
   ↓
new source
   ↓
amendment of the framework
   ↓
new safeguards
   ↓
new capability
   ↓
new amendment
   ↓
etc.
```

[S58]

**LEGAL VULNERABILITY:**

> The compliance of an infrastructure at a given date does not guarantee that its future scope will remain identical; on the contrary, it requires compliance to be reassessed when purposes, data, sources, recipients or capabilities evolve.

---

### This changes the way the safeguards identified in 6.7 should be interpreted

In 6.7, we established in particular:

```
DPP
→ no personal customer data
  without explicit consent

WALLET
→ user control
→ selective disclosure
→ limitation of requests
→ alternatives

DIGITAL EURO
→ programmable currency prohibited
→ conditional payments provided for
  within the proposed framework
```

These safeguards are real.

But they must be read as:

> **safeguards of the applicable legal framework.**

Not as:

> **eternal technical impossibilities.**

The distinction is fundamental.

---

### An evolution can also occur without physically merging the databases

This is probably the most important point for the architecture studied.

A legal evolution does not necessarily need to create:

```
CENTRAL MEGA DATABASE
identity
   +
invoices
   +
products
   +
environment
   +
payments
```

It could theoretically authorize:

```
system A
   ↓
result / attribute

system B
   ↓
result / attribute

   ↓
processing C
```

In other words, the question of freedoms does not depend solely on the existence of a centralized database.

It also depends on:

- the accessible data;  
- the identifiers enabling cross-referencing;  
- the attributes that can be presented;  
- the results that can be transmitted;  
- the conditions that can be verified;  
- the consequences attached to these results.

**LEGAL VULNERABILITY:**

> An evolution of the framework can increase the possibilities of cross-referencing without requiring the physical merger of the infrastructures concerned.

---

### This is precisely why the interfaces identified in Chapter 5 and in 6.7 are important

We have separately documented:

```
transaction
↔ product

product
↔ DPP

DPP
↔ environmental data

wallet
↔ verified attributes

wallet
↔ digital euro services
   within the proposed framework

external condition
↔ conditional payment
```

The complete chain:

```
identity
   +
economic history
   +
product
   +
environment
   ↓
condition
   ↓
authorization / refusal / limitation
of a payment
```

is **not established**.

But the relevant legal question is no longer only:

> **"does this chain exist today?"**

It also becomes:

> **"what legal changes would be needed to enable each of its junctions, and what safeguards would oppose them?"**

This is a much more precise and verifiable question.

---

### An important legal boundary appears around rights and freedoms

EU law and constitutional law do not allow the legislature to freely eliminate all protection simply by adopting a new text.

An evolution remains notably confronted with:

```
fundamental rights
   ↓
privacy
   +
data protection
   +
necessity
   +
proportionality
   +
effective safeguards
```

[S39][S44][S53]

Where a restriction on the rights protected by the GDPR falls within the scope of Article 23, it must notably respect the essence of fundamental freedoms and rights and constitute a necessary and proportionate measure in a democratic society [S47].

**LEGAL SAFEGUARD:**

> The fact that the legislature can make the law evolve does not mean it can legally authorize any surveillance, any profiling, or any restriction whatsoever.

---

### The real vulnerability therefore lies between two false claims

First excessive claim:

```
"it's forbidden today,
so it will be impossible tomorrow"
```

False.

Second excessive claim:

```
"the law can change,
so they will be able to do anything"
```

Also false.

The legally defensible position is:

```
technically capable architecture
   +
use not authorized today
   ↓
possible legal evolution
   ↓
but subject to higher-order norms
   ↓
necessity review
   +
proportionality
   +
fundamental rights
   +
safeguards
   +
judicial review
```

---

### The history of CFVR nevertheless shows why this distinction is not theoretical

Between 2014 and 2026, the same processing underwent several successive modifications [S58].

Over the course of these developments, we notably see:

```
more categories of persons
   +
more sources
   +
more data
   +
more analytical capabilities
   +
more exchanges
   +
new computing infrastructure
   +
electronic invoicing
```

[S37][S45][S58]

Each development taken in isolation may have its own justification and its own safeguards.

The cross-cutting question, however, becomes:

> **at what point should one re-examine not only each extension separately, but also the cumulative effect of all previous extensions?**

This question links directly back to 6.5.

**TO BE ESTABLISHED:**

> Is there a comprehensive, periodic assessment allowing the cumulative effect of successive modifications to a processing operation on privacy and freedoms to be measured, beyond the legal examination of each modification taken separately?

---

### The documentary risk is one of gradual normalization

Particular caution is required here.

The sources show no evidence of any strategy aimed at progressively introducing a system of generalized control.

Such an intention cannot be inferred merely from the succession of legal texts.

But an objective property can be examined:

```
extension A
→ legally authorized

extension B
→ legally authorized

extension C
→ legally authorized

extension D
→ legally authorized
```

does not automatically imply that:

```
A + B + C + D
```

was the subject of a separate, comprehensive public assessment.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not make it possible to systematically establish how the cumulative effect of all successive extensions of an infrastructure is assessed when a new modification is adopted.

This formulation is much more solid than asserting the existence of drift.

---

### A safeguard can also change in nature when the ecosystem changes

A safeguard that is effective within an isolated infrastructure can become less protective if the technical environment evolves.

Abstract example:

```
product identifier
alone
   ↓
weak capacity
for personal identification
```

then:

```
product identifier
   +
identifiable transaction
   +
identity attribute
   ↓
much greater
cross-referencing capacity
```

The rule specific to the DPP may remain exactly the same.

But the ecosystem surrounding the DPP has changed.

Same reasoning applies to:

```
wallet attribute
   +
payment service
   +
external condition
```

**LEGAL VULNERABILITY:**

> The real effectiveness of a compartmentalization safeguard must be assessed within the technical and legal ecosystem in which the infrastructure operates, not solely on the basis of the content of its own founding text.

---

### The ultimate question becomes that of a change in consequence

A system may initially serve only to:

```
inform
```

then possibly:

```
recommend
```

then:

```
classify
```

then:

```
orient
```

then, if the law permitted it:

```
condition a decision
```

This last step profoundly changes the legal analysis.

Sections 6.4 and 6.5 showed that the more an automated result becomes determinative in a decision producing a legal or similarly significant effect, the more central the safeguards relating to automated decisions, necessity, and proportionality become [S43][S51][S53].

**LEGAL SAFEGUARD:**

> The fact that a piece of data may legally be used to inform or orient does not automatically mean it can be used to produce an individual restriction.

---

### Applied to the environment, this point becomes decisive

The DPP and environmental infrastructures can produce information concerning the characteristics of a product.

An informative use could take the form of:

```
product
   ↓
environmental information
   ↓
consumer information
```

A far more intrusive architecture would be:

```
product
   +
consumption history
   +
identity
   ↓
individual environmental profile
   ↓
consequence on
payment / right / service
```

These two architectures are not legally equivalent.

**NOT ESTABLISHED:**

> No element examined currently demonstrates the existence or preparation of a European mechanism assigning individuals an individual environmental score used to limit their payments, purchases, or rights.

**LEGAL SAFEGUARD:**

> Moving from product-related environmental information to an individual restriction based on a personal profile would constitute a substantial change in processing and would need to be examined against the applicable legal bases and safeguards.

---

### The current absence of the complete chain therefore remains an important conclusion

At this stage:

```
DPP
   ↓
product / environmental information

wallet
   ↓
identity / attributes

conditional payment
   ↓
possible external condition
```

are documented separately.

But:

```
environmental DPP
   ↓
individual profile
   ↓
imposed condition
   ↓
payment refused
```

remains:

> **NOT ESTABLISHED.**

This boundary must not be weakened.

On the contrary, it makes the investigation more solid.

---

### What now needs to be monitored is therefore not an intention, but verifiable modifications

The relevant indicators would notably be:

```
new category of data
   ↓
new identifier
   ↓
new category of accessors
   ↓
new interface
   ↓
new purpose
   ↓
new cross-referencing possibility
   ↓
new individual consequence
```

A change in any one of these elements can be objectively documented.

There is no need to speculate about intentions.

---

### Open questions after 6.8

> **1. What successive modifications have precisely increased the scope of each infrastructure studied since its creation?**

> **2. When a new source is added to an existing processing operation, is the cumulative effect with all sources already present subject to a separate analysis?**

> **3. How will future developments in the DPP's delegated acts modify the available data, its granularity, and the categories of actors able to access it?**

> **4. What new categories of attestations will progressively become usable within the European Digital Identity Wallet?**

> **5. What data will actually be exchanged between the European Digital Identity Wallet and future digital euro services?**

> **6. What external sources could be used by services offering conditional payments?**

> **7. Would a new legal basis be needed if environmental data relating to a product were to be transformed into an attribute relating to a person?**

> **8. What legal basis and what safeguards would be needed if such an attribute were subsequently to influence access to a payment, a service, or a right?**

> **9. Is there a mechanism for identifying the moment when several extensions, individually legally admissible, together produce an architecture requiring a new overall assessment of proportionality?**

---

### Conclusion of 6.8

**ESTABLISHED:**

> The legal scope of a public data infrastructure can evolve over time. CFVR provides a documented example of this since 2014 [S58].

**ESTABLISHED:**

> CFVR has undergone several successive modifications concerning in particular the persons concerned, the data sources, the associated processing operations, and, in 2026, the integration of data from electronic invoicing [S37][S45][S58].

**ESTABLISHED:**

> The ESPR regulation provides that the concrete content, granularity, and access rights to the DPP are to be specified for different product groups by delegated acts [S56].

**ESTABLISHED:**

> The concrete operation of the European Digital Identity Wallet also relies on implementing acts and technical specifications, within the limits set by the eIDAS 2 regulation [S55].

**LEGAL SAFEGUARD:**

> A change in the law does not permit the higher-order requirements relating to fundamental rights, data protection, necessity, and proportionality to be freely set aside.

**LEGAL LATITUDE:**

> A purpose, data source, recipient, or interconnection that is not legally authorized today may, depending on the circumstances, subsequently become subject to a new legal basis, provided the applicable higher-order norms are respected.

**LEGAL VULNERABILITY:**

> A safeguard based on the current scope of a processing operation constitutes present protection, but not a guarantee that this scope will remain unchanged.

**LEGAL VULNERABILITY:**

> An evolution can increase the possibilities of cross-referencing between infrastructures without requiring their physical merger into a single database.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not make it possible to systematically establish how the cumulative effect of all successive extensions of an infrastructure is reassessed when a new extension is adopted.

**TO BE ESTABLISHED:**

> To what extent can several successive extensions, each individually legally regulated, alter the overall balance of an infrastructure before a new overall assessment of necessity and proportionality becomes indispensable?

**NOT ESTABLISHED:**

> No element examined demonstrates that a legal evolution is currently underway to create an individual environmental profile linked to digital identity and used to authorize, refuse, or limit a payment, a purchase, a service, or a right.

**NOT ESTABLISHED:**

> The legal possibility of subsequently modifying the purposes or interfaces of an infrastructure does not constitute proof that such a modification is being contemplated.

---

## 6.9 Legal vulnerabilities and limits of the analysis

**Status: VULNERABILITIES IDENTIFIED / HIGHER-ORDER SAFEGUARDS / FACTUAL LIMITS OF THE INVESTIGATION**

The investigation is now able to answer a more important question than whether each infrastructure studied is, taken in isolation, legally regulated.

The final question is:

> **what happens when several legally distinct infrastructures simultaneously increase their capacities for collection, identification, cross-referencing, analysis, and action?**

The preceding sections have established that the law contains numerous protections.

They have also shown that these protections do not all constitute technical impossibilities, and that the legal scope of infrastructures can evolve.

The main vulnerability identified by this investigation lies precisely in this gap.

```
TECHNICAL CAPABILITY
   ↓
broader than
   ↓
LEGALLY AUTHORIZED USE
TODAY
```

This difference currently protects against certain uses.

But it also means that the evolution of the law becomes an essential variable of the architecture.

---

### First vulnerability: functional centralization can exist without a single central database

The investigation did not identify a single European database bringing together:

```
identity
   +
invoices
   +
transactions
   +
products
   +
environmental data
   +
payments
```

Such a claim would be incorrect.

The preceding chapters have, however, documented several specialized infrastructures with their own identifiers, interfaces, registries, verification mechanisms, or cross-referencing capabilities.

French electronic invoicing provides a particularly concrete example.

Data from electronic invoices now constitutes a source for CFVR and must feed the DGFiP's secure data platform in order to be exploited at scale [S37][S45].

CFVR already cross-references numerous other tax, economic, administrative, and social sources.

**ESTABLISHED:**

> Physical centralization in a single database is not necessary to enable cross-referencing between information originating from distinct systems.

**LEGAL VULNERABILITY:**

> The separate regulation of several infrastructures is not necessarily sufficient to assess the consequences resulting from their combination when they become interoperable, or when the results produced by one can be used by another.

The determining question is therefore not only:

> **"where is the data stored?"**

but also:

> **"what information can be linked, verified, transmitted, or used to produce a consequence?"**

---

### Second vulnerability: a purpose that is legally limited today may evolve tomorrow

Section 6.8 established that CFVR already provides a historical example of successive modifications to the same processing operation [S58].

An infrastructure can retain its institutional existence while seeing the following evolve:

- its sources;  
- its categories of data;  
- the persons concerned;  
- its recipients;  
- its technical capabilities;  
- its modes of operation.

**LEGAL SAFEGUARD:**

> An administration cannot freely modify a purpose or freely reuse data outside the applicable legal framework.

**LEGAL VULNERABILITY:**

> The current absence of a given use does not necessarily constitute a definitive legal prohibition: a new text may modify the authorized scope, subject to compliance with higher-order law.

This distinction rules out two opposing conclusions.

```
"it's not authorized today
so it will always be impossible"
```

is not demonstrated.

But:

```
"the law can evolve
so this use will be authorized tomorrow"
```

is not demonstrated either.

---

### Third vulnerability: accumulation can become more significant than each extension taken in isolation

The analysis of CFVR reveals a cross-cutting difficulty.

A succession can take the form of:

```
extension A
   +
extension B
   +
new source C
   +
new exchange D
   +
new capability E
```

Each can be legally examined at the time of its introduction.

But the ultimate issue becomes:

```
A + B + C + D + E
   ↓
OVERALL CAPABILITY
```

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not make it possible to systematically establish how the cumulative effect of all successive extensions of an infrastructure is reassessed independently of the examination of each new modification.

This question becomes particularly important when the following progress simultaneously:

```
volume
   +
number of sources
   +
precision
   +
interoperability
   +
algorithmic capability
   +
number of recipients
```

---

### Fourth vulnerability: interoperability can produce a new capability without merging systems

The infrastructures studied are increasingly designed around:

- identifiers;  
- interfaces;  
- registries;  
- verifiable attestations;  
- attribute-presentation mechanisms;  
- services capable of verifying conditions;  
- common standards.

This allows for an architecture in which one infrastructure does not necessarily need to receive all the raw data from another.

```
SYSTEM A
   ↓
attribute / proof / result

SYSTEM B
   ↓
verification

SYSTEM C
   ↓
consequence
```

**LEGAL VULNERABILITY:**

> A distributed infrastructure can produce consequences comparable to those of a centralized system without requiring the creation of a database physically containing all the data concerned.

This property makes it insufficient to examine databases alone.

The interfaces must also be examined.

---

### Fifth vulnerability: the shift from information to consequence

This boundary is probably the most important in the entire chapter.

Data can be used to:

```
INFORM
```

then:

```
VERIFY
```

then:

```
CLASSIFY
```

then:

```
ORIENT
```

and possibly:

```
CONDITION
```

These functions do not produce the same legal consequences.

CFVR already provides an example of this distinction.

Algorithmic results can guide officers, but the CNIL requires that they not replace human analysis and that the human decision remain effective [S37][S51].

**LEGAL SAFEGUARD:**

> Authorization to use data to inform, detect, or verify does not automatically constitute authorization to use it to produce an individual restriction.

**LEGAL VULNERABILITY:**

> The more determinative a piece of data or an algorithmic result becomes for access to a payment, a service, a right, or another significant possibility, the more determinative the requirements relating to legal basis, proportionality, accuracy, transparency, the ability to challenge, and automated decisions become.

---

### Sixth vulnerability: an error can change in nature as it passes through several infrastructures

The preceding sections identified the rights of access and rectification.

But an interconnected architecture poses an additional difficulty.

```
erroneous data A
   ↓
processing B
   ↓
classification C
   ↓
attribute D
   ↓
decision E
```

Correcting A does not, on its own, technically guarantee that:

```
B
C
D
E
```

have all been recalculated, corrected, or neutralized.

The law provides for various obligations of rectification, restriction, and notification to recipients when the corresponding conditions are met [S43].

**LEGAL VULNERABILITY:**

> In a distributed architecture, the effectiveness of the right to rectification depends not only on correcting the source data, but also on the ability to identify and correct the derived consequences still associated with that data.

**DOCUMENTARY BLIND SPOT:**

> The public sources examined do not establish the existence of a cross-cutting mechanism allowing a person to learn of, and then have automatically corrected, all derived data or propagated consequences across several legally distinct infrastructures.

---

### Seventh vulnerability: protection sometimes depends on maintaining a functional separation

Several of the safeguards identified rest on boundaries.

For CFVR:

```
algorithm
   ↓
flagging
   ↓
human analysis
   ↓
decision
```

For the DPP:

```
product information
   ≠
personal consumer profile
```

For the digital euro within the proposed framework:

```
conditional payment
   ≠
programmable currency
```

For the European wallet:

```
presentation of a necessary attribute
   ≠
systematic disclosure
of the entire identity
```

These separations constitute genuine safeguards.

But their effectiveness depends on their being maintained.

**LEGAL VULNERABILITY:**

> When a protection rests on a separation between two functions that are technically capable of being brought closer together, any evolution reducing that separation must be subject to a new legal analysis.

---

### Eighth vulnerability: the digital euro could be created without the individual consent of each citizen

A distinction must be drawn here between the creation of a currency and an individual obligation to use it.

The proposed European framework provides for a legislative procedure enabling the digital euro to be established.

Once this framework is adopted, the decision whether or not to issue the digital euro would belong to the ECB [S57].

This is not, therefore, a mechanism based on the individual consent of each citizen to the creation of this new form of currency.

**ESTABLISHED:**

> The possible creation of the digital euro falls within the European institutional and legislative process and, subsequently, within the framework envisaged, an issuance decision by the ECB; it is not conditional on the individual agreement of each user.

But this observation does not mean:

```
digital euro created
   =
obligation for each citizen
to give up cash
```

The framework currently being negotiated instead provides for the coexistence of the digital euro with cash, together with measures intended to preserve the access to and acceptance of cash [S57].

**NOT ESTABLISHED:**

> No element examined makes it possible to assert that the current framework provides for the abolition of cash or a general obligation for each citizen to use the digital euro exclusively.

---

### Ninth vulnerability: control of a digital currency and control of the use of each unit are not legally equivalent

A central bank digital currency infrastructure necessarily entails rules concerning, among other things:

- its issuance;  
- its distribution;  
- its operation;  
- its intermediaries;  
- its possible holding limits;  
- its payment mechanisms.

The framework currently proposed does indeed envisage holding limits [S57].

But another boundary exists.

The ECB considers that intrinsically limiting:

```
where
 +
when
 +
to whom
```

a unit of digital euro can be spent would amount to creating a programmable currency incompatible with its character as a fully fungible currency and with its status as legal tender [S57].

**LEGAL SAFEGUARD:**

> The proposed framework excludes the transformation of the digital euro into a programmable currency whose units would intrinsically impose restrictions concerning the goods, services, places, times, or beneficiaries for which they could be used.

This safeguard is important.

It must not be confused with conditional payments.

---

### Tenth vulnerability: conditional payments nevertheless create an interface with external conditions

The preceding chapters documented the technical and experimental possibility of using an externally verified condition to trigger a payment.

The proposed framework for the digital euro precisely distinguishes:

```
PROGRAMMABLE CURRENCY
   ↓
intrinsic restriction
on the currency
   ≠
CONDITIONAL PAYMENT
   ↓
payment triggered
according to an agreed condition
```

[S22][S27][S28][S57]

**ESTABLISHED:**

> The proposed framework prohibits programmable currency while allowing the development of conditional payment services.

This distinction constitutes simultaneously:

```
a SAFEGUARD
   +
an INTERFACE TO MONITOR
```

The safeguard is that the currency itself cannot be restricted to certain uses.

The interface to monitor concerns the nature of the conditions used by payment services.

---

### This is where the environmental question must be formulated with maximum precision

The preceding chapters established:

```
product
   ↓
DPP
   ↓
environmental data
```

and separately:

```
external condition
   ↓
verification
   ↓
conditional payment
```

But they did not establish:

```
identity
   ↓
purchase history
   ↓
personal environmental score
   ↓
quota
   ↓
payment authorization / refusal
```

**NOT ESTABLISHED:**

> No element examined currently demonstrates the existence, deployment, or legal adoption of an individual "environmental pass" using DPP data to determine whether or not a person may make a payment.

This conclusion must remain explicit.

But it does not exhaust the legal question.

---

### The real question becomes: what protections would be activated if this boundary were crossed?

A hypothetical architecture:

```
IDENTITY
   +
TRANSACTIONS
   +
PRODUCTS
   +
ENVIRONMENTAL DATA
   ↓
INDIVIDUAL PROFILE
   ↓
CONDITION
   ↓
PAYMENT / SERVICE / RIGHT
```

could not be analyzed as a mere technical extension.

It would notably have to be examined in light of:

- its legal basis;  
- its purpose;  
- necessity;  
- proportionality;  
- minimization;  
- rights of access and rectification;  
- rules relating to profiling;  
- automated decisions, where their conditions are met;  
- the fundamental rights affected;  
- the available remedies.

[S43][S44][S47][S51][S53]

**LEGAL SAFEGUARD:**

> An infrastructure technically capable of producing a restriction is not legally authorized to produce it merely because that capability exists.

---

### And even a new law does not constitute an unlimited power

This is probably the most important legal boundary in this chapter.

A new law or a new regulation may change the authorized uses.

But:

```
NEW LAW
   ≠
UNLIMITED LEGAL POWER
```

Where a measure restricts fundamental rights protected by EU law, that restriction must notably:

```
be provided for by law
   +
respect the essential content of the right
   +
be necessary
   +
be proportionate
   +
genuinely meet
an objective of general interest
or protect the rights of others
```

[S39][S44]

**LEGAL SAFEGUARD:**

> The evolution of the law can shift certain boundaries, but it remains itself subject to higher-order legal norms and to judicial review.

This safeguard constitutes the limit to the idea that:

> **"it would be enough to change the law to be able to do anything."**

---

### The electronic invoicing reform nevertheless constitutes a major change of scale

It is worth returning here to the starting point of the investigation.

A structured electronic invoice is not merely a PDF sent by another route.

It transforms previously scattered economic information into data that is:

```
structured
   +
standardized
   +
automatically exploitable
   +
transmissible
   +
cross-referenceable
   +
analyzable at scale
```

Chapters 1 and 2 established the nature and lifecycle of this data.

Chapter 5 examined the possibilities for interconnection.

The present chapter has shown that certain electronic invoicing data are now integrated into CFVR and exploited within an algorithmic infrastructure capable of processing a volume of several billion invoices per year [S37][S45].

**ESTABLISHED:**

> The reform substantially increases the quantity of structured economic data likely to be processed automatically by the tax administration.

---

### But "centralizing everything" would be an excessive conclusion

The record does not demonstrate:

```
ELECTRONIC INVOICING
   ↓
SINGLE DATABASE
   ↓
all identity
   +
all products
   +
all the environment
   +
all payments
```

**NOT ESTABLISHED:**

> The French electronic invoicing reform does not, on the basis of the sources examined, constitute a central database bringing together all the infrastructures analyzed in this investigation.

The precise conclusion is different:

> **it creates a new, massive layer of structured economic data that can become a source for other processing operations when the law authorizes it.**

CFVR now provides a concrete example of this.

---

### This is precisely what makes electronic invoicing a structuring infrastructure

The critical point is therefore not:

> **"electronic invoicing already controls everything."**

The documented point is:

```
ECONOMIC ACTIVITY
   ↓
STRUCTURED DATA
   ↓
TRANSMISSION
   ↓
LARGE-SCALE PROCESSING
   ↓
CROSS-REFERENCING
   ↓
ALGORITHMIC ANALYSIS
```

This chain now exists within the tax domain studied [S37][S45].

**LEGAL VULNERABILITY:**

> The more an infrastructure transforms diffuse economic activity into structured, standardized, and interoperable data, the more decisive the evolution of its purposes, its recipients, and its cross-referencing possibilities becomes for freedoms.

---

### The fundamental vulnerability is therefore not a hidden function

At the conclusion of the investigation, no source revealed:

```
secret button
"total control"
```

The vulnerability identified is more structural.

```
DIGITIZATION
   ↓
STRUCTURING
   ↓
IDENTIFICATION
   ↓
INTEROPERABILITY
   ↓
CROSS-REFERENCING
   ↓
ANALYSIS
   ↓
POSSIBLE CONDITION / DECISION
```

At each stage, safeguards exist.

But each stage also increases the potential capability of the next.

---

### The protection of freedoms therefore depends less on the existence of capabilities than on the boundaries imposed on their use

This investigation ultimately shows that two realities can be true simultaneously.

First reality:

> **the infrastructures studied do not today constitute a legally authorized system of general control over purchases, identity, the environment, and currency.**

Second reality:

> **they objectively increase the technical capabilities for identification, structuring, cross-referencing, verification, and automation available within the European digital ecosystem.**

There is no contradiction between these two findings.

It is precisely the space between them that the law must protect.

---

### The red lines then become identifiable

The investigation now makes it possible to define changes that would require a particularly rigorous reassessment:

> **1. use of a common identifier systematically linking identity, purchases, products, and payments;**

> **2. transformation of environmental information relating to products into an individual environmental profile;**

> **3. use of this profile to produce a consequence on a payment, a service, or a right;**

> **4. transformation of algorithmic assistance into a mechanism practically determining the human decision;**

> **5. disappearance or substantial reduction of the possibility of using a means of payment not associated with the same level of traceability;**

> **6. extension of purposes allowing the cross-use of data initially collected within distinct infrastructures;**

> **7. practical impossibility for a person to know, correct, or challenge the data and derived results used with respect to them;**

> **8. multiplication of separately justified extensions without sufficient public assessment of their cumulative effect.**

None of these points should be presented as having occurred when it has not.

They constitute verifiable monitoring criteria.

---

### What the investigation does not allow us to assert

**NOT ESTABLISHED:**

> It is not established that the European Union or France are currently setting up a system intended to assign an individual environmental score to citizens.

**NOT ESTABLISHED:**

> It is not established that DPP data will be used to determine the authorization or refusal of a person's purchases.

**NOT ESTABLISHED:**

> It is not established that the digital euro will allow the ECB to authorize or prohibit a person's purchases depending on the products they wish to buy.

**NOT ESTABLISHED:**

> It is not established that electronic invoicing, the DPP, the European Digital Identity Wallet, and the digital euro will be brought together within a single control infrastructure.

**NOT ESTABLISHED:**

> It is not established that cash will be abolished upon the possible introduction of the digital euro.

These limits do not diminish the investigation.

They define its solidity.

---

### What it does allow us to establish

**ESTABLISHED:**

> Electronic invoicing transforms a significant portion of economic activity into structured data that can be exploited automatically.

**ESTABLISHED:**

> Some of this data is now intended to feed CFVR and the DGFiP's secure data platform [S37][S45].

**ESTABLISHED:**

> CFVR already combines numerous sources and uses algorithmic methods to detect anomalies and guide tax audits [S37].

**ESTABLISHED:**

> The DPP makes it possible to associate structured information with products, which may notably include environmental information [S56].

**ESTABLISHED:**

> The European Digital Identity Wallet enables the presentation and verification of electronic attributes according to the framework studied [S55].

**ESTABLISHED:**

> The proposed framework for the digital euro distinguishes and prohibits programmable currency while allowing conditional payment services [S57].

**ESTABLISHED:**

> The purposes, sources, and scope of certain public infrastructures can evolve legally over time, as the history of CFVR demonstrates [S58].

**LEGAL SAFEGUARD:**

> These technical capabilities cannot be freely combined to produce any individual consequence whatsoever: their use remains subject to legal bases, authorized purposes, fundamental rights, and the requirements of necessity and proportionality.

---

### Conclusion of 6.9

The result of the investigation is therefore neither:

```
"everything is already connected"
```

nor:

```
"current safeguards make
any evolution impossible"
```

The result is more precise.

```
DISTINCT INFRASTRUCTURES
   ↓
GROWING CAPABILITIES
   ↓
GROWING INTEROPERABILITY
   ↓
CROSS-REFERENCING POSSIBILITIES
   ↓
USES LIMITED BY
CURRENT LAW
   ↓
BUT A LEGAL FRAMEWORK
LIKELY TO EVOLVE
   ↓
UNDER THE CONTROL OF
FUNDAMENTAL RIGHTS
```

**LEGAL VULNERABILITY:**

> The main risk identified is not the demonstrated existence of a single control system, but the possibility that successive extensions of purposes, access, interfaces, or consequences progressively bring initially separate infrastructures closer together.

**DOCUMENTARY BLIND SPOT:**

> Public sources generally make it possible to study each infrastructure and each legal modification separately, but make it much less easy to assess the cumulative effect of the entire ecosystem on the capabilities for identification, cross-referencing, and decision-making.

**LEGAL SAFEGUARD:**

> Even where an evolution is decided by the legislature, restrictions placed on fundamental rights remain subject to the requirements of legality, respect for the essential content of rights, necessity, and proportionality.

**NOT ESTABLISHED:**

> The investigation currently demonstrates neither the existence of an individual "environmental pass," nor the use of an environmental profile to control payments, nor a single architecture automatically linking electronic invoicing, digital identity, the DPP, and the digital euro in order to restrict citizens' rights or purchases.

**CONCLUSION:**

> **The determining question is therefore not whether the infrastructure already allows for generalized control. It is whether the legal boundaries that today separate collection, information, identification, cross-referencing, profiling, and decision-making will continue to evolve at the same pace as the technical capabilities that make it possible to cross them.**

And it is precisely for this reason that the analysis must remain evolving:

> **every new data source, every new identifier, every new interface, every new purpose, and every new consequence attached to these infrastructures must be examined not only in isolation, but also for what it enables when combined with what already exists.**