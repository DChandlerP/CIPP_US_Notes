# Introduction to Privacy

Before diving into the legal framework, it is important to understand the four broad categories of privacy that U.S. law and the CIPP/US exam cover:

* **Information Privacy:** The claim of individuals to determine for themselves when, how, and to what extent information about them is communicated to others.
    * *Examples:* Financial data, medical records, personal marketing data.
* **Bodily Privacy:** The protection of a person's physical being against invasive procedures.
    * *Examples:* Genetic testing, drug testing, body cavity searches.
* **Communication Privacy:** The security and privacy of mail, telephones, email, and other forms of communication.
    * *Examples:* Wiretapping, opening mail, intercepting email.
* **Territorial Privacy:** Limits on intrusion into domestic and other environments (the "right to be left alone").
    * *Examples:* Home searches, workplace monitoring, video surveillance.

## 1. Personal vs. Non-Personal Information
* **Scope:** U.S. privacy laws generally protect "personal information" (PI) or "personally identifiable information" (PII). Non-personal info is usually not regulated.
* **Key Factor:** The distinction often depends on how easily the data can be associated with a specific person.

### Identified vs. Identifiable
* **Identified Individual:** Someone who can be ascertained with certainty (e.g., via Social Security Number).
* **Identifiable Individual:** Someone who can be indirectly identified through a combination of factors (e.g., combining a city, street address, and gender).
    * *Note:* This is a sliding scale. The more data you combine, the more "identifiable" a person becomes.
    * **IP Addresses:** Historically considered non-personal by U.S. courts, but the FTC increasingly views static IP addresses as identifiable PI.

## 2. Sensitive Personal Information
* Some laws only regulate specific subsets of sensitive data rather than all PI.
* **Examples:**
    * **HIPAA:** Regulates personal health records, not all data held by a facility.
    * **FCRA:** Places tighter restrictions on medical records within consumer reports.

## 3. Data Protection Techniques
Data can be transformed from "personal" to "non-personal" to avoid regulation:
* **Encryption:** Transforming data into an unrecognizable form (ciphertext).
* **Anonymization:** Stripping data of identifying information (irreversible).
* **Pseudonymization:** Replacing identifiers with a pseudonym/code.
    * *Benefit:* It is reversible (can be re-identified) if you have the key.
* **Data Life Cycle:** Typically consists of five steps: (1) collection; (2) use; (3) disclosure; (4) retention; and (5) destruction.
* **Data Life Cycle Management (DLM):** Also known as Information Life Cycle Management (ILM), this is a policy-based approach to managing the flow of information through its entire life cycle.
* **Methods of Disposal:** Electronic data can be destroyed via overwriting or **degaussing** (using magnetic fields); physical data is typically destroyed via shredding, melting, or burning.

## 4. Sources of Information
* **Public Records:** (e.g., court filings) - generally less protected.
* **Publicly Available:** (e.g., social media) - broadly accessible.
* **Non-Public Information:** This is the primary focus of privacy protection laws.

## 5. Key Data Roles (GDPR & Industry Standard)
* **Data Subject:** The individual whose information is being processed.
* **Data Controller:** The entity that **decides** how and why data is processed (has the ultimate authority).
* **Data Processor:** The entity that processes data **on behalf of** the controller.
    * *Limit:* Can only do what the controller authorizes.
    * *Synonyms:* "Business Associate" (HIPAA), "Service Provider" (GLBA).

**Key Terminology:**
* **Processing:** Any operation performed on data (collection, storage, deletion, etc.).

* **Fair Information Practices (FIPs/FIPPs)**
    * **Definition:** Principles guiding data collection, storage, and management for fairness, privacy, and security.
    * **Role:** Foundation for data privacy laws/regulations (often not legally binding themselves).

* **US Frameworks**
    * **1973 HEW Report:** First US articulation. Five principles: no secret records, individual access, limit secondary use, correction rights, data reliability.
    * **Privacy Act of 1974:** Codified FIPs for federal agencies.
    * **2012 White House Report:** Proposed "Consumer Privacy Bill of Rights" (individual control, transparency, accountability).
    * **2012 FTC Report:**
        * **Privacy by Design:** Build privacy in at development stage.
        * **Simplified Consumer Choice:** Meaningful options (e.g., Do-Not-Track).
        * **Transparency:** Clear notices and access.

* **International Frameworks**
    * **OECD Guidelines (1980):** Eight principles (Collection Limitation, Data Quality, Purpose Specification, Use Limitation, Security Safeguards, Openness, Individual Participation, Accountability).
    * **Council of Europe Convention 108 (1981):** Binding agreement requiring FIPs in domestic law.
    * **Madrid Resolution (2009):** Standards for transborder data flow (Lawfulness, Purpose Specification, Proportionality, Data Quality, Openness, Accountability).

* **Common Themes**
    * **Individual Rights:**
        * **Notice:** Informing consumers of practices.
        * **Consent:** Control over data use (Opt-in/Opt-out).
        * **Access:** Right to view/correct data.
    * **Organizational Management:**
        * **Security Controls:** Physical, technical, administrative safeguards.
        * **Data Quality:** Accuracy, completeness, relevance.
        * **Collection/Use Limits:** Data minimization and retention limits.
        * **Accountability:** Monitoring, training, and assigning responsibility.


## 6. The Accountability Principle
The **Accountability Principle** dictates that organizations must take responsibility for protecting personal information and be able to *demonstrate* that compliance to stakeholders.

* **Core Requirement:** Organizations must implement appropriate technical and organizational measures to ensure and demonstrate that data handling complies with relevant laws.
* **Demonstrating Compliance:** This requires significant documentation, such as recording attendance at all employee training events.
* **Responsibility Shift:** The ultimate responsibility for legal compliance lies with the organization (data controller), *not* government regulatory authorities.
* **Flexibility:** How an organization realizes accountability is inherently flexible, allowing them to determine the best means to meet obligations based on their specific processing activities.
* **GDPR Influence:** Under Article 5 of the GDPR, the data controller is expressly responsible for, and must be able to demonstrate compliance with, the other principles of the regulation.

---
# 1. Branches of U.S. Government

The U.S. federal government operates on a system of checks and balances with three coequal branches.

### Legislative Branch (Congress)
* **Role:** Creates new laws and revises existing ones.
* **Source of Power:** **Article I** of the U.S. Constitution (*Article I powers*).
* **Check on Executive:** Holds the **power of the purse** (controls spending) and the power of **impeachment** (requires a majority vote in the House and two-thirds conviction in the Senate).
* **Composition:**
    * **House of Representatives:** 435 voting members, based on population, elected to two-year terms.
    * **Senate:** 100 voting members (two per state), elected to six-year terms.

### Executive Branch (President, Departments, Agencies)
* **Role:** Carries out and enforces the laws created by the legislative branch.
* **Source of Power:** **Article II** of the U.S. Constitution (*Article II powers*).
* **Check on Legislative:** **Veto power** over bills passed by Congress (Congress can override with a two-thirds majority in both houses). The power to enforce (or decline to enforce) laws.

### Judicial Branch (Federal Court System)
* **Role:** Interprets the meaning of laws, resolves disputes, and determines constitutionality.
* **Source of Power:** **Article III** of the U.S. Constitution.
* **Check on Legislative & Executive:** **Judicial review**—the power to strike down laws or practices that conflict with the U.S. Constitution.
* **Court Structure (Lesser to Greater Superiority):**
    * **U.S. District Courts:** The trial courts of the federal system.
    * **U.S. Circuit Courts of Appeal:** Intermediate courts that accept cases on appeal from District Courts; decisions are binding only within their geographic circuit.
    * **U.S. Supreme Court:** Highest court; decisions are final and binding on all inferior courts. Determines which cases to accept through *certiorari*.

---

## 2. Sources of Law
Laws in the United States come from a variety of sources:

* **Constitutional Law:** The highest possible source of law; no other law may conflict with it.
    * *Supremacy Clause (Article VI):* Establishes the Constitution as the supreme law of the land.
    * *Privacy Protections:* The word "privacy" does not appear in the text, but protections are derived from:
        * **3rd Amendment:** Prohibition on quartering soldiers (privacy of the home).
        * **4th Amendment:** Protection against unreasonable searches and seizures.
        * **5th Amendment:** Protection against self-incrimination.
        * **14th Amendment:** Due process and liberty clauses.
    * *State Constitutions:* Can provide **greater** privacy rights than the federal constitution (e.g., California), but cannot provide less (federal law sets the "floor").

* **Legislation (Statutes):** Laws passed by Congress (federal) or state legislatures.
    * **Preemption:** Federal law generally preempts state law (based on the **Supremacy Clause**).
        * **Express Preemption:** The federal law specifically states it overrides state law (e.g., **CAN-SPAM** expressly preempts most state anti-spam laws).
        * **Implied Preemption:** Courts determine that Congress intended to preempt state law even if not explicitly stated.
        * *Note on the 10th Amendment:* Powers not delegated to the federal government are reserved to the States, allowing for state-level privacy laws (like CCPA) where federal law is silent.
    * Federal laws are compiled in the *U.S. Code*.

* **Administrative Law:** Rules and regulations created by executive branch agencies to implement statutes.
    * *Formal Rulemaking:* Legally binding rules (e.g., HIPAA Privacy Rule) documented in the *Code of Federal Regulations (CFR)*.
    * *Informal Guidance:* Agency reports, speeches, and workshops that interpret law but strictly speaking are not binding.
    * - **Administrative Enforcement Actions:**
    - Considered a "third category of litigation" (alongside civil and criminal).
    - **Adjudication:** Typically litigated before an *Administrative Law Judge (ALJ)* rather than a standard court. ALJ decisions are often subject to appeal in a federal civil court.
    - **Administrative Procedure Act (APA):** The federal statute that acts as the rulebook for these actions (similar to the Federal Rules of Civil Procedure). It governs the process unless a specific statute (like the *FTC Act*) mandates different procedures.

* **Common Law (Case Law):** Legal principles developed over time through judicial decisions rather than statutes.
    * *Stare Decisis:* ("To stand by things decided") The principle that courts should follow prior *precedent* to keep the law stable.
    * *Torts:* Civil wrongs (like negligence or invasion of privacy) often stem from common law.

* **Remedies for Breach:**
        * **Monetary Damages:**
            * *Expectation Interest:* Puts the plaintiff in the position as if the contract had been performed (benefit of the bargain).
            * *Reliance Interest:* Compensates for loss suffered by relying on the contract (puts plaintiff back to pre-contract position).
            * *Restitution Interest:* Prevents unjust enrichment of the breaching party.
        * **Specific Performance:** A court orders the breaching party to perform their contractual duties (used when money damages aren't enough).
  
---

## 3. Core Legal Concepts

### Jurisdiction
A court's authority to render legal judgments has two elements:

* **Personal Jurisdiction:** A court's authority over the **person** (individual or corporation) being sued. Established through:
    * Physical presence.
    * Place of residence or business.
    * **Consent** (e.g., a clause in a contract).
    * **Minimum contacts** (conducting business within a state).
* **Subject Matter Jurisdiction:** A court's authority to hear specific types of disputes.
        * **General vs. Limited:** State courts have *general jurisdiction* (can hear almost anything), while federal courts have *limited jurisdiction* (only specific types of cases, like those involving federal laws or diversity of citizenship).
        * **Exclusive Jurisdiction:** When *only* a specific court can hear a case (e.g., bankruptcy or copyright cases *must* be heard in federal court).

### Legal Definitions
* **Person:** A legal entity that can sue, be sued, own property, and sign contracts. Includes **human beings** (citizens, residents) and **legal organizations** (corporations).
* **Preemption:** Law from a **higher authority** (e.g., federal) takes precedence over law from a lower authority (e.g., state). Established by the **Supremacy Clause**.
* **Private Right of Action (PRA):** The ability for **individuals and corporations** to bring cases to court for violations of a specific law.
    * **Contains PRA:** CCPA (California Consumer Privacy Act).
    * **Lacks PRA:** FERPA, GLBA, HIPAA.

## Legal Liability
Liability is being responsible or answerable in law.

### Civil vs. Criminal Litigation
| *Feature* | *Civil Litigation* | *Criminal Litigation* |
| :--- | :--- | :--- |
| *Who brings suit?* | **Plaintiff** (Private individual, Company, or Agency like FTC) | **Prosecutor** (Government only: DOJ or State AG) |
| *Basis* | Civil wrong (Tort, Breach of Contract, Statutory violation) | Violation of Criminal Statute |
| *Standard of Proof* | **Preponderance of the evidence** (More likely than not / >50%) | **Beyond a reasonable doubt** (Highest standard; presumption of innocence) |
| *Remedy/Punishment* | Money damages, Injunctions (court orders), Declaratory judgment | Imprisonment, Criminal Fines |
| *Procedural Protections* | Standard due process | Enhanced protections (e.g., right to speedy trial, right to counsel) |

> **Key Example:** While most privacy enforcement is civil, the **Wiretap Act** (Title III) explicitly provides for criminal penalties, including fines up to $250,000 and imprisonment of up to 5 years.

### Torts and Negligence
* **Tort:** A civil wrong that involves harm to one party caused by the action or inaction of another, *not* involving a contract.
* **Negligence (A Tort):** Harm caused by a failure to act with reasonable care. Requires four elements:
    1.  **Duty of care:** An established responsibility.
    2.  **Breach of duty:** Violation of that responsibility.
    3.  **Damages:** The accuser suffered some form of harm (financial, physical, emotional).
    4.  **Causation:** The breach must be the result of the damages.
* **Four Invasion of Privacy Torts (Common Law):**
    1.  **Invasion of solitude:** Physical or electronic intrusion (e.g., accessing someone's email).
    2.  **Public disclosure of private facts:** Disclosure of truthful, non-newsworthy information that would offend a reasonable person.
    3.  **False light:** Disclosing information that causes a person to be **falsely perceived** by others.
    4.  **Appropriation:** Unauthorized use of someone’s name or likeness.

### Framework for Analyzing a Law
When determining if a law applies to a specific scenario, follow this hierarchy:
* **1. Scope (Who):** Does the law apply to the specific entity? (e.g., HIPAA applies to "Covered Entities," but not to a fitness app).
* **2. Application (What):** Does the law protect the specific type of data involved? (e.g., FCRA applies to "Consumer Reports," but not to internal marketing lists).
* **3. Preemption:** If it is a state law, has it been preempted (overridden) by a federal statute?
* **4. Enforcement:** Who has the authority to enforce it (FTC, State AG, Private Right of Action) and what are the penalties?
    
---
## 4. Regulatory Authorities
Privacy regulation in the U.S. follows a **sectoral model**, meaning different agencies regulate different industries.

### Federal Regulatory Authorities
* **Federal Trade Commission (FTC):** The primary federal privacy regulator.
    * **Authority:** Regulates "unfair or deceptive acts or practices" (Section 5 of the FTC Act).
    * **Specifics:** Enforces the Telemarketing Sales Rule and children's privacy (COPPA).
* **Federal Communications Commission (FCC):** Regulates telecommunications (e.g., TCPA).
* **Dept. of Health and Human Services (HHS):** Enforces HIPAA (Privacy and Security Rules) for healthcare.
  - **Concurrent Jurisdiction:** Multiple agencies may have authority over the same issue.
    - *Example (HIPAA):* - **HHS:** Has primary administrative enforcement authority.
        - **DOJ:** Has jurisdiction to bring *criminal* charges for certain violations.
        - **FTC:** Can simultaneously enforce under Section 5 if the violation also constitutes an "unfair or deceptive" practice.
* **Financial Regulators:**
    * **CFPB (Consumer Financial Protection Bureau):** Regulates consumer financial products and parts of FCRA.
    * **Federal Reserve & OCC:** Regulate banking institutions.
* **Department of Commerce (DOC):**
    * **Role:** Policy development and international frameworks (e.g., Data Privacy Framework).
    * **Key Note:** The DOC **does not** have enforcement authority.

### State Regulatory Authorities
* **State Attorneys General (AG):** The chief legal officers of the states.
    * **Powers:** Enforce state privacy laws (UDAP statutes).
    * **Federal Enforcement:** Uniquely, State AGs can bring enforcement actions under certain *federal* laws, specifically **HIPAA** and **FCRA**.
  - **Coordination:** States often coordinate via the *National Association of Attorneys General (NAAG)* to facilitate information exchange and multi-state actions.
- **UDAP Specifics:**
    - Every state has a UDAP statute.
    - **Private Right of Action (PRA):** Every state provides a PRA under their UDAP statute *except for Iowa*.
* **California Privacy Protection Agency (CPPA):** The first dedicated state-level privacy agency in the U.S. (created by CPRA).
* **State Departments of Insurance:**
    * Insurance is regulated at the **state level** (not federal).
    * **NAIC:** The National Association of Insurance Commissioners sets standards (e.g., Insurance Data Security Model Law).

### Self-Regulatory Organizations (SROs)
Industry bodies that create and enforce their own privacy standards.
- **Theory of Self-Regulation:**
    - *Benefits:* Utilizes industry expertise, efficient, flexible, and quicker to adapt to technology changes than government regulation.
    - *Critiques:* Can be anti-competitive, enforcement may be lax ("fox guarding the henhouse"), and may lack diverse stakeholder input.
* **PCI-DSS:** Security standards for the payment card industry (credit cards).
- *Enforcement:* The PCI Council *sets* the standards, but the individual *Card Brands* (Visa, Amex, etc.) *enforce* them.
        - Penalties can range from $5,000 to $100,000 per month.
    - *Compliance Verification:*
        - **Qualified Security Assessor (QSA):** Hired to assess security.
        - **Approved Scanning Vendor (ASV):** Hired to detect vulnerabilities.
* **DAA / NAI:** Standards for online behavioral advertising and ad-tech.
  - **AdChoices:** The DAA's specific program/icon that allows consumers to opt-out of online interest-based ads.
* **Trust Marks:** Certification programs (badges) that verify a business's privacy practices.
* - **Co-Regulatory Enforcement:**
    - Occurs when industry groups and government jointly administer regulations.
    - *Prime Example (COPPA):* The FTC allows companies to satisfy COPPA requirements by complying with the rules of an FTC-approved "Safe Harbor" program.
    - *Safe Harbor Orgs:* Aristotle, CARU, ESRB, iKeepSafe, kidSAFE, PRIVO, TrustArc.


# FTC Privacy Enforcement Case Examples (UDTP)

## Unfair Practices (Security Failures)
The FTC uses the **Unfair** standard when a company fails to implement reasonable security measures, leading to substantial consumer injury.

* **Wyndham Worldwide:** The hotel chain suffered multiple data breaches due to a failure to implement reasonable security (e.g., strong passwords, firewalls). The action was upheld, finding it **unfair** to promise security but fail to provide adequate safeguards.
* **LabMD:** The company exposed a file with patient information on a peer-to-peer network. The FTC found the lack of sufficient cybersecurity practices to be **unfair**.
* **DesignerWare:** A rent-to-own company secretly installed spyware on rented computers that captured keystrokes and images. This intrusive monitoring was deemed **unfair**.
* **LifeLock (Security):** The identity theft protection service failed to implement strong security controls for its own customer data, violating its advertising claims and a prior consent decree, resulting in a **$100 million fine**.

## Deceptive Practices (Misrepresentations)
The FTC uses the **Deceptive** standard when a company makes misleading statements or omissions about how it handles, protects, or uses personal data.

* **Facebook:** Charged with making deceptive claims about users' ability to control privacy, specifically allowing app developers access to user information even when users restricted access. This led to a large fine for violating a previous consent decree.
* **Zoom:** Misled consumers into believing its service used **end-to-end encryption** (only users see content), when it used less secure encryption that allowed Zoom to access the content.
* **Snapchat:** Informed users that messages and photos disappeared forever, while knowing that users could easily **preserve** them. This was a **material deception** about the service's core functionality.
* **GeoCities:** **Resold personal information** of customers after telling them in its privacy policy that it would **not** do so. This direct contradiction of its policy was deemed **deceptive**.
* **TRUSTe:** The privacy certification firm was found **deceptive** for failing to conduct required **annual recertifications** of its clients' privacy practices, violating the promise implied by its **Trust Mark** seal.

### Other Federal Agencies
* **Federal Communications Commission (FCC):** Regulates interstate and international communications, enforcing rules related to **Customer Proprietary Network Information (CPNI)** under the **Telecommunications Act of 1996**.
* **Department of Health and Human Services (HHS):** The lead agency for implementing and enforcing the **Health Insurance Portability and Accountability Act (HIPAA)** Privacy and Security Rules, issuing substantial fines.
* **Department of Commerce (DOC):** Manages the U.S. portion of the **Privacy Shield** and its successor, the **Data Privacy Framework (DPF)**, which govern transatlantic data transfers.
* **Banking Regulators:**
    * **Consumer Financial Protection Bureau (CFPB)** is the lead agency for consumer financial protection.
    * Other involved agencies include the Federal Reserve, FDIC, NCUA, and OCC.
* **Department of Education (ED):** Enforces the **Family Educational Rights and Privacy Act (FERPA)**, which regulates the handling of student educational records.

## State Regulatory Authorities

State governments also have significant enforcement power.

* **Attorneys General (AG):** Most enforcement actions are brought by one or more state attorneys general under state privacy laws or **Unfair and Deceptive Acts and Practices (UDAP)** laws, which are similar to the FTC Act but vary by state.
* **California Privacy Protection Agency (CPPA):** The first state-level agency specifically dedicated to privacy and data protection, established by the **California Privacy Rights Act (CPRA)** to enforce its provisions.

## Self-Regulatory Programs

These programs allow industries to develop and enforce their own privacy and/or security standards, often to preempt government regulation.

* **Payment Card Industry Data Security Standard (PCI DSS):** A highly successful self-regulatory program focusing on security and data retention for the credit card processing industry. Merchants must comply via contractual agreements with banks.
    * It contains 12 high-level security requirements (e.g., firewalls, encryption, strong passwords).
* **Network Advertising Initiative (NAI):** A self-regulatory framework for digital advertising, publishing a code of conduct covering notice, opt-out, and data security. The NAI conducts compliance reviews and can refer noncompliant companies to the FTC.
* **Trust Marks:** Symbols (e.g., the **TRUSTe** seal) displayed on a company’s website to show that an independent third party has certified the company meets specific privacy standards.
* **Safe Harbors:** Agreements like the **Privacy Shield** (and its successor, the DPF) that offer firms exemption from prosecution under certain laws if they demonstrate compliance with specified regulatory requirements, particularly for international data transfers.
* 
# Information Management

## 1. Data Governance

**Data governance** programs identify, track, and manage sensitive information to ensure consistent data handling practices across an organization.

### Building a Data Inventory
Developing an inventory is the first step in managing sensitive data. Organizations should catalog the types and locations of sensitive information they maintain:

* **Personally Identifiable Information (PII):** Broadly refers to any information that uniquely identifies an individual.
* **Protected Health Information (PHI):** Medical records subject to **HIPAA**.
* **Financial Information:** Personal financial records maintained by the organization.
* **Government Information:** Data subject to specific rules and classification requirements.

### Data Classification
**Data classification** organizes data into categories based on sensitivity and the potential impact of unauthorized disclosure. This guides the selection of security controls.

* **Government Terminology:** Uses categories like *Top Secret*, *Secret*, *Confidential*, and *Unclassified*.
* **Business Terminology:** Often uses terms like *Highly Sensitive*, *Sensitive*, *Internal*, and *Public*.
* **NIST Guidance:** The **National Institute of Standards and Technology (NIST)** publishes guides like **SP 800-53** to specify controls for low, moderate, and high-impact information.

### Data Flow Mapping
**Data flow mapping** tracks how personal information is **received, handled, shared, and disposed of** throughout the organization.

* This process produces **data flow diagrams** that vary in detail (technical vs. business process).
* Diagrams help identify potential privacy and regulatory concerns, especially with **third-party data sharing**.

### Data Assessment Practices

- Ongoing activity: Data assessments are not one-time projects. They should be revisited on a regular cadence and after major business or technology changes to keep inventories, maps, and classifications accurate.

- Core assessment questions: Key questions include where data is stored and who owns it, what information flows into and out of systems (including cross-border transfers), the volume and format of data, what it is used for, which categories of personal or sensitive data are involved, and which third parties receive or access it.

- Assessment approaches: 
  - Top-down assessments focus on legal and regulatory requirements and then evaluate whether systems and processes meet those obligations.
  - Bottom-up assessments start from specific data assets or systems (such as a local database or a cloud application) and trace how data enters, is processed, and leaves those assets.

### Balancing Privacy Risks

* **Four risk categories:** When designing a privacy program, organizations should balance four risk categories related to personal information use: legal risk, reputational risk, operational risk, and investment risk.
* **Trade-offs and constraints:** Legal risk covers regulatory and litigation exposure from non-compliance (including self-regulatory commitments), reputational risk reflects loss of consumer trust and market position, operational risk captures how privacy controls can impede or enable business processes, and investment risk asks whether the benefits of additional privacy and security investments justify their costs.

### Privacy Vision and Organizational Goals

* **Privacy vision / mission:** A privacy program should be grounded in a written privacy vision or mission statement that reflects the organization’s goals, risk appetite, regulatory environment, and intended uses of personal information.
* **Understanding goals and risk appetite:** Key questions include the organization’s tolerance for privacy risk, how it intends to use personal data, how controls affect those uses, and what peers and competitors treat as best practices in the same industry.

### Privacy Program Framework

* **Privacy program framework:** A privacy program framework (privacy framework) is the roadmap that organizes policies, standards, and operational activities so privacy decisions are made consistently and can be measured over time.
* **Two core components:** The framework typically has two main components: (1) creation of privacy policies, standards, and guidelines; and (2) establishment of privacy program activities (education, assessments, incident response, monitoring, etc.).

#### Privacy Policy (Internal Governance Document)

* **Internal vs external:** A privacy policy is an internal governance document describing how the organization manages its privacy function and handles personal information; it is distinct from an outward-facing privacy notice given to consumers.
* **High-level, testable, and living:** The policy should be clear, accessible, comprehensive yet concise, action-oriented, and designed so its effectiveness can be measured and iterated over time.

##### Core Components of a Privacy Policy

* **Purpose:** States why the policy exists and which laws, regulations, or frameworks drive the need for it.
* **Scope:** Defines which business units, processes, systems, data types, and assets are covered.
* **Designation of responsibilities:** Identifies roles or departments accountable for privacy compliance, including internal stakeholders and relevant vendors.
* **Compliance obligations:** Sets out the rules employees must follow, including data use limitations, security requirements, and how the organization will honor data subject rights.
* **Consequences of non-compliance:** Describes the potential consequences to the organization for policy failures, while detailed employee-level sanctions are usually handled in functional documents like standards and handbooks.

#### Privacy Notices (External Disclosures)

* **Definition and purpose:** A privacy notice is an external-facing statement that explains how an organization collects, uses, discloses, and stores personal information so that individuals can make informed privacy decisions. It also guides employees on how data should be handled in practice.
* **Policy vs. notice:** Unlike the internal privacy policy (governance document), the privacy notice is directed at consumers or other external audiences and may also be called a privacy statement or fair processing notice, even though some sources use “privacy policy” and “privacy notice” interchangeably.

##### Legal Implications of Privacy Notices

* **Sectoral legal requirements:** Certain U.S. sectoral laws require specific privacy notices, including content, timing, and placement. Examples:
  * **COPPA:** Requires child-directed sites and services to describe what information is collected, how it is used, and whether it is shared with third parties, and to link to the notice on the home page and every page where children’s data is collected.
  * **GLBA:** Requires financial institutions to provide customers with annual privacy notices describing their information-sharing practices.
  * **CalOPPA:** Requires websites and online services collecting personal information from California residents to conspicuously post a privacy notice and include disclosures about categories of data collected, sharing practices, how users can request changes, effective date, how updates are communicated, how Do Not Track signals are handled, and whether third parties collect data on the site.
* **FTC UDAP risk:** Even when no specific statute mandates a notice, privacy notices are treated as legal commitments. Misrepresenting practices or failing to follow the notice can be an “unfair or deceptive” act under the FTC Act, so notices should be reviewed by legal and appropriate executives before publication.

##### Maintaining and Updating Privacy Notices

* **Change management and version control:** Privacy notices should be updated through a managed process (design, test, release, review) and versioned with dates, with prior versions retained to show which terms applied at the time of collection.
* **Material changes and consent:** The FTC expects organizations to honor the notice that was in effect when data was collected unless they obtain express, affirmative consent before making material retroactive changes (for example, starting to share data with third parties after saying they would not).

##### Designing Effective Notices

* **Common elements:** Effective privacy notices typically include the effective date; scope; what data is collected (active vs. passive); how data is used; how and when data is shared; user choices and controls; access and correction mechanisms; contact information; dispute procedures; and how changes will be communicated.
* **Layered notices:** A layered notice presents a short, standardized summary of key practices up front with links or expansion to a more detailed, full notice, improving readability for typical users.
* **Just-in-time notices:** Just-in-time notices present focused information and consent prompts at the moment data is collected (for example, an in-app pop-up when requesting location data), often linking to the relevant section of the full notice.
* **Privacy dashboards:** Dashboards provide a centralized interface where users can view privacy information and manage preferences across devices and services (for example, managing ad settings, data sharing, or deletion requests).
* **Privacy icons and visualization tools:** Icons and visual cues (such as standardized symbols or the AdChoices icon for targeted advertising) can quickly communicate key processing or choice information, especially where long-form text is impractical.
* **Single vs. multiple notices:** Organizations may use a single enterprise notice when data practices are consistent across units, but multiple notices may be more appropriate where business units or subsidiaries use data in fundamentally different ways or maintain separate customer relationships.


#### Privacy Program Activities

* **Education and awareness:** Training and awareness campaigns ensure employees understand privacy policies, procedures, and their responsibilities in day-to-day operations.
* **Internal policy compliance:** Ongoing monitoring, testing, and assessments help verify that policies are being followed and that the program does not become a “paper-only” framework.
* **Data inventories, flows, and classification:** Tools such as data inventories, flow maps, and classification schemas help track personal data from collection through deletion and understand sensitivity and risk.
* **Risk assessments:** Structured assessments (including privacy assessments, PIAs, and DPIAs) evaluate how processing activities and systems affect privacy risk and regulatory obligations.
* **Incident response:** A predefined incident response program prepares the organization to detect, escalate, and remediate privacy incidents and data breaches in a way that aligns with legal requirements.
* **Internal audit and risk management:** Internal audit tests controls and reports on privacy-related risks, while risk management functions analyze and communicate business, regulatory, and operational risk relevant to privacy.

#### Workforce Training and Awareness

* **Role in accountability:** A well-trained workforce is essential to the accountability principle and to effective implementation of privacy programs, data inventories, classifications, and incident response plans.
* **Scope of training:** Employees, contractors, and relevant third parties should receive role-appropriate training and periodic refreshers on organizational policies, procedures, and security practices.

##### Employee Data Leaks and Human Error

* **Human error as a major cause:** A significant portion of security incidents and breaches arise from human error, including falling for phishing or social engineering, misconfiguring systems, or mishandling documents and devices.
* **Inadvertent disclosures:** Training should address non-malicious leaks such as leaving documents exposed, improper disposal of records, or failing to follow “clean desk” and similar physical security practices.
* **Behavioral focus:** Effective programs teach employees how to recognize and respond to phishing, social engineering, and other threats, and how to escalate incidents promptly.

##### Legal and Regulatory Training Requirements

* **HIPAA:** Covered entities must train all workforce members on policies and procedures for protected health information within a reasonable time after hire and whenever there is a material change, and must document that training.
* **GLBA Safeguards Rule:** Financial institutions must train staff to implement the information security program, including specialized training where appropriate (for example, fraud and identity theft recognition, computer security, and secure disposal of customer information).
* **FTC Red Flags Rule:** Entities that maintain “covered accounts” must establish an identity theft prevention program, including workforce training as necessary to implement the program effectively.
* **Massachusetts Data Security Regulations:** Any person or entity that owns or licenses personal information about a Massachusetts resident must maintain a written information security program that includes ongoing employee training and training on the proper use of the computer security system.
* **Self-regulatory programs (PCI-DSS):** The PCI Data Security Standard requires a security awareness program to make all personnel aware of cardholder data security, with training at hire and at least annually, and verification that training occurred.

##### Key Training Takeaways

* **Risk reduction:** Effective training can reduce both the frequency and cost of data breaches by improving detection, reporting, and prevention of incidents.
* **Documentation and metrics:** Organizations should document training completion, track participation, and treat training effectiveness as a measurable component of the privacy and security program.


### Implementation and Metrics

* **Implementation and communication:** Successfully implementing a privacy framework requires communicating it to internal and external stakeholders and embedding its requirements into processes and technology, rather than leaving it as documentation only.
* **Regulatory alignment and monitoring:** Ongoing monitoring of applicable laws and regulations is necessary to keep the privacy program aligned with current legal requirements.
* **Privacy metrics:** Privacy metrics are measurements used to evaluate whether the privacy program is meeting its objectives; examples include compliance metrics, trend and maturity analysis, ROI-related metrics, and resource utilization.

### Privacy Operational Life Cycle

* **Continuous improvement model:** The privacy operational life cycle is a continuous improvement model that structures privacy program activities into four repeating stages: assess, protect, sustain, and respond.
* **Stage definitions:**
  * **Assess:** Identify gaps and risks by comparing current practices to laws, policies, and best-practice frameworks.
  * **Protect:** Apply safeguards and privacy-by-design concepts across the data life cycle, from collection through deletion.
  * **Sustain:** Maintain the program through management oversight, audits, training, and ongoing governance activities.
  * **Respond:** Handle events such as data subject requests, incidents, and control failures in a way that reduces risk and supports compliance.

### Balancing Privacy Risks

* **Four risk categories:** When designing a privacy program, organizations should balance four risk categories related to personal information use: legal risk, reputational risk, operational risk, and investment risk.
* **Trade-offs and constraints:** Legal risk covers regulatory and litigation exposure from non-compliance (including self-regulatory commitments), reputational risk reflects loss of consumer trust and market position, operational risk captures how privacy controls can impede or enable business processes, and investment risk asks whether the benefits of additional privacy and security investments justify their costs.

### Privacy Vision and Organizational Goals

* **Privacy vision / mission:** A privacy program should be grounded in a written privacy vision or mission statement that reflects the organization’s goals, risk appetite, regulatory environment, and intended uses of personal information.
* **Understanding goals and risk appetite:** Key questions include the organization’s tolerance for privacy risk, how it intends to use personal data, how controls affect those uses, and what peers and competitors treat as best practices in the same industry.

### Privacy Program Framework

* **Privacy program framework:** A privacy program framework (privacy framework) is the roadmap that organizes policies, standards, and operational activities so privacy decisions are made consistently and can be measured over time.
* **Two core components:** The framework typically has two main components: (1) creation of privacy policies, standards, and guidelines; and (2) establishment of privacy program activities (education, assessments, incident response, monitoring, etc.).

#### Privacy Policy (Internal Governance Document)

* **Internal vs external:** A privacy policy is an internal governance document describing how the organization manages its privacy function and handles personal information; it is distinct from an outward-facing privacy notice given to consumers.
* **High-level, testable, and living:** The policy should be clear, accessible, comprehensive yet concise, action-oriented, and designed so its effectiveness can be measured and iterated over time.

##### Core Components of a Privacy Policy

* **Purpose:** States why the policy exists and which laws, regulations, or frameworks drive the need for it.
* **Scope:** Defines which business units, processes, systems, data types, and assets are covered.
* **Designation of responsibilities:** Identifies roles or departments accountable for privacy compliance, including internal stakeholders and relevant vendors.
* **Compliance obligations:** Sets out the rules employees must follow, including data use limitations, security requirements, and how the organization will honor data subject rights.
* **Consequences of non-compliance:** Describes the potential consequences to the organization for policy failures, while detailed employee-level sanctions are usually handled in functional documents like standards and handbooks.

#### Privacy Program Activities

* **Education and awareness:** Training and awareness campaigns ensure employees understand privacy policies, procedures, and their responsibilities in day-to-day operations.
* **Internal policy compliance:** Ongoing monitoring, testing, and assessments help verify that policies are being followed and that the program does not become a “paper-only” framework.
* **Data inventories, flows, and classification:** Tools such as data inventories, flow maps, and classification schemas help track personal data from collection through deletion and understand sensitivity and risk.
* **Risk assessments:** Structured assessments (including privacy assessments, PIAs, and DPIAs) evaluate how processing activities and systems affect privacy risk and regulatory obligations.
* **Incident response:** A predefined incident response program prepares the organization to detect, escalate, and remediate privacy incidents and data breaches in a way that aligns with legal requirements.
* **Internal audit and risk management:** Internal audit tests controls and reports on privacy-related risks, while risk management functions analyze and communicate business, regulatory, and operational risk relevant to privacy.

#### Privacy Risk Assessment Deep Dive
* **Risk Definition:** The combination of the consequences of an event and the associated likelihood of occurrence.
* **Privacy Assessment vs. PIA:**
    * *Privacy Assessment:* A comprehensive, holistic review of an organization’s entire privacy risk profile.
    * *Privacy Impact Assessment (PIA):* An analysis of discrete products, services, or processes to ensure legal compliance and mitigate risks. Should be forward-looking and conducted *before* implementation.
* **Privacy Threshold Analysis (PTA):** Also called an "initial privacy assessment" or "express PIA." A preliminary investigation used to determine if a full-blown PIA is required.
* **Legal Triggers for PIAs:**
    * *Federal:* The **E-Government Act of 2002** requires federal agencies to conduct PIAs when implementing programs that collect personal info.
    * *International:* Under GDPR Article 35, these are known as **Data Protection Impact Assessments (DPIA)**.
* **Privacy Harms Models:**
    * *Calo’s Harms Dimensions:* Categorizes risks as either measurable/objective or perceived/subjective.
    * *Solove’s Taxonomy of Privacy:* Identifies risk based on four activities: collection, processing, dissemination, and invasions.
    * *Nissenbaum’s Contextual Integrity:* Identifies risk based on whether data use aligns with the norms of a specific context.
* **ISO 29134 (PIA Framework) Phases:**
    1. Determining if a PIA is needed (PTA).
    2. Preparation.
    3. Performance (identifying data flows, analyzing risks/safeguards).
    4. Follow-up.


### Implementation and Metrics

* **Implementation and communication:** Successfully implementing a privacy framework requires communicating it to internal and external stakeholders and embedding its requirements into processes and technology, rather than leaving it as documentation only.
* **Regulatory alignment and monitoring:** Ongoing monitoring of applicable laws and regulations is necessary to keep the privacy program aligned with current legal requirements.
* **Privacy metrics:** Privacy metrics are measurements used to evaluate whether the privacy program is meeting its objectives; examples include compliance metrics, trend and maturity analysis, ROI-related metrics, and resource utilization.

### Privacy Operational Life Cycle

* **Continuous improvement model:** The privacy operational life cycle is a continuous improvement model that structures privacy program activities into four repeating stages: assess, protect, sustain, and respond.
* **Stage definitions:**
  * **Assess:** Identify gaps and risks by comparing current practices to laws, policies, and best-practice frameworks.
  * **Protect:** Apply safeguards and privacy-by-design concepts across the data life cycle, from collection through deletion.
  * **Sustain:** Maintain the program through management oversight, audits, training, and ongoing governance activities.
  * **Respond:** Handle events such as data subject requests, incidents, and control failures in a way that reduces risk and supports compliance.
  
### Privacy Programs and Organizational Roles

#### Privacy Programs as Organization-Wide Efforts

- Privacy program: The organizational process used to meet legal compliance obligations, market expectations, and data security goals for handling personal information. It should be tailored to the unique obligations, risk profile, and business model of each organization.

- Program purpose: Facilitate a clear understanding of how the organization collects, uses, shares, and retains personal data, while balancing business needs with data protection, auditability, and accountability.

- Cross-functional collaboration: Effective privacy programs depend on collaboration across legal, compliance, information security, information technology, risk, marketing, HR, and other business units, not just a standalone privacy team.

- Functional implementation: Even when there is a centralized privacy office, privacy policies and standards are implemented at the functional level (e.g., marketing, product, operations), so those teams must understand and support privacy goals.

- Dedicated vs distributed teams: Large organizations may have a dedicated privacy team; others rely on functional groups (e.g., IT, legal, compliance, security) to share responsibility for privacy activities as part of their broader roles.

#### Key Organizational Privacy Roles

* **Data Protection Officer (DPO):** Most common title for employees involved in the privacy function; originates in GDPR, which mandates DPOs for many organizations, but the title is widely used even where not legally required.
* **Designated privacy leader:** Laws such as the GLBA Safeguards Rule and other sectoral regulations often require a specific individual to be accountable for privacy or information security programs, increasing organizational accountability and providing a clear point of contact for regulators and data subjects.
* **Privacy Leader:** The most senior employee with oversight of the privacy program; common titles include Chief Privacy Officer, DPO, Director of Privacy, and Privacy Officer, though in some organizations the CIO, CTO, CEO, or another executive fills this role.

##### Core Privacy Team Roles

* **Chief Privacy Officer (CPO):** Senior management role that leads the privacy team, oversees compliance and training, and serves as the organization’s primary internal expert on privacy.
* **Privacy Manager:** Provides day-to-day oversight and coordination of privacy initiatives, supports business units, promotes privacy practices, and ensures alignment with applicable laws and internal policies.
* **Privacy Analyst:** Assesses privacy risks in business operations, contributes to policies and procedures, develops training content, and often reviews privacy and data-use provisions in third-party contracts and new initiatives.
* **Privacy Engineer:** Translates legal and policy requirements into technical solutions, applies privacy by design to products and services, and advises on how new technologies affect personal data processing.
* **Information Security Specialist:** Brings security expertise to the privacy program, designs and reviews technical controls, and acts as a liaison between privacy and information security functions.

##### Distributed and Support Roles

* **Line-of-Business Privacy Steward:** Embedded within a business unit as a front-line contact for privacy, responsible for spotting issues, escalating concerns, and helping the unit apply organizational privacy policies.
* **Privacy Attorney / Privacy Counsel:** Provides legal advice on privacy and data protection issues, supports the CPO and business teams, and coordinates with the organization’s broader legal or general counsel function.
* **Privacy Compliance Manager / Consultant:** Focuses on ensuring that specific business lines or regions implement privacy policies and procedures effectively and consistently.
* **incident response / privacy incident handler:** Operational role responsible for coordinating the organization’s response to privacy incidents and working within the incident response program.
* **Privacy Champion:** Executive-level sponsor or senior manager who advocates for privacy as a core organizational value and helps secure resources and support for the privacy program across the enterprise.


### Data Lifecycle Management
Data protection must be maintained from collection to disposal.

* **Data Minimization:** Collecting the **smallest possible amount** of information necessary to meet business requirements.
* **Purpose Limitation:** Information should only be used for the **purpose for which it was originally collected** and consented to.
* **Data and Records Retention:** Data should be kept only for as long as necessary.
* **Secure Disposal:** Data must be securely destroyed so a determined adversary cannot reconstruct it.
    * **Paper Records:** Shredding (cross-cut), incineration, or pulping.
    * **Electronic Media:** Electronic erasure, degaussing (magnetic fields), or physical destruction.
* **FACTA Disposal Rule:** Requires covered organizations to take **“reasonable measures to protect against unauthorized access or use of the information in connection with its disposal”** of consumer reports (e.g., shredding, using certified destruction vendors).

## 2. Workforce Training

Workforce training ensures users understand their obligations and the risks involved with handling personal information.

* **Regular Training:** Should take place on an ongoing basis, often using **computer-based training (CBT)**.
* **Role-Based Training:** Training should be customized to an individual's job responsibilities (e.g., system administrators need highly technical training; customer service needs more focus on social engineering).
* **Content:** Must include regulatory requirements and practical steps for protecting data.

## 3. Cybersecurity Threats

Threat actors are differentiated by their sophistication, resources, motivation, and whether they are **internal** or **external**.

| Threat Actor | Description | Skill/Resources | Motivation |
| :--- | :--- | :--- | :--- |
| **Script Kiddies** | Users of pre-built, automated hacking tools with limited technical skills. | Low skill, limited resources. | Thrill, proving skill, seeking convenient targets. |
| **Hacktivists** | Use hacking techniques to achieve an **activist goal** or political cause. | Varies widely; often skilled and risk-tolerant. | Greater good, political change, social justice. |
| **Criminal Syndicates** | Organized crime groups focused on cybercrime. | Moderately to highly skilled, high resources. | Illegal **financial gain**. |
| **Advanced Persistent Threats (APTs)** | Nation-state actors or highly sophisticated groups using advanced techniques over a long period. | Highly skilled, significant resources/funding. | Political objectives, traditional espionage, stealing intellectual property (economic gain). |
| **Insiders** | Employees, contractors, or vendors with authorized access who misuse it. | Varies widely. | Financial gain, revenge, activism (whistleblowing). |

### Specialized Threats
* **Zero-Day Attacks:** Exploits a security **vulnerability unknown to product vendors**, meaning no patch is available. Often used by APTs.
* **Ransomware:** Malicious software that uses strong **encryption** to render a system's data inaccessible. Ransom is demanded for the decryption key. Newer attacks include the threat of **data disclosure** if the ransom is not paid.

## 4. Incident Response

Organizations must activate a formal **cybersecurity incident response plan** immediately following a data privacy breach.

### Definitions (NIST SP 800-61)
* **Event:** Any observable occurrence in a system or network (e.g., a user accessing a file).
* **Adverse Event:** Any event with negative consequences (e.g., malware infection).
* **Security Incident:** A violation or imminent threat of a violation of security policies (e.g., accidental loss of sensitive information, intrusion).

* **Preparation Steps:** Proper response starts before an incident via: (1) developing a response plan; (2) training; (3) defining roles; (4) insurance; and (5) managing 3rd-party vendors.
* **Readiness Assessment:** A pre-incident assessment to evaluate:
    * **Risk Level:** Whether it will affect a large data set or greatly impact specific individuals.
    * **Severity:** Types of privacy harms that could arise in light of offsetting controls.

### Phases of Incident Response (NIST Model)
1.  **Preparation:** Building the foundation for the CSIRT (Computer Security Incident Response Team), including policy, procedures, training, and purchasing **cyberinsurance**.
2.  **Detection and Analysis:** Identifying that an incident is occurring. Indicators include alerts (from IDS/antivirus), logs, publicly available information (new vulnerabilities), and reports from people.
3.  **Containment, Eradication, and Recovery:** Active measures to resolve the incident, including:
    * Selecting and implementing a containment strategy.
    * Gathering evidence for potential legal action.
    * Identifying attackers and systems.
    * Eradicating the incident and **recovering normal business operations**.
4.  **Post-Incident Activity:** Activities after resolution, including:
    * **Lessons-Learned Review:** A thorough review, ideally led by an **independent facilitator**, to improve procedures.
    * **Evidence Retention:** Identifying internal and external retention requirements (U.S. federal agencies must retain records for at least **three years**).

### 4.1 FTC Data Breach Response Guidelines
The FTC framework for private sector response includes:
* **Preliminary Step - Confirm the Breach:** Verify the fact of a breach through technical analysis.
* **Step 1 - Secure Operations & Containment:** Assemble a response team, secure physical areas, take equipment offline to stop data loss, and maintain evidence.
* **Step 2 - Analyze & Fix Vulnerabilities:** Re-evaluate 3rd-party providers, review data segmentation, and create a communication plan.
* **Step 3 - Notify Appropriate Parties:**
    * **Notification Content:** Generally includes what happened, contact info, and steps the individual can take to mitigate risk.
    * **Special Cases:** If health info is involved, media and HHS may require notification.
* **Step 4 - Proactive Steps:** Conduct 3rd-party audits and analyze weaknesses to avoid future repeats.

### Incident Response Plan Documentation
* **Policy:** The high-level cornerstone, approved by top management, assigning authority and roles. It should be relatively timeless (e.g., defining scope, roles, severity scheme).
* **Procedures and Playbooks:** *Procedures* provide detailed, tactical information. *Playbooks* describe step-by-step responses for **specific types of incidents** (e.g., "Web Server Defacement," "Breach of PII"). Playbooks are not a substitute for professional judgment.

### 4.2 OMB Framework (Federal Agencies)
The 2017 OMB guidelines provide a seven-step structure for federal agency response:
1. Create a breach response team.
2. Identify applicable privacy compliance documentation.
3. Share information to understand the extent of the breach.
4. Determine reporting requirements.
5. Assess risk of harm to individuals.
6. Mitigate risk of harm.
7. Notify affected individuals.

### Data Breach Notification
* **U.S. Requirements:** The U.S. lacks a single federal law for broad breach notification, but **every state has its own data breach notification law**.
* **International:** Laws like the **GDPR** also include breach notification requirements. Organizations must untangle overlapping requirements and consult legal counsel.

## 5. Vendor Management

Managing risks posed by third-party vendors is critical, especially those handling personal information (like cloud vendors).

* **Data Controller Liability:** The principal organization (controller) remains **legally responsible** for any misuse of data by its vendors (processors).
* **Vendor Vetting Criteria:** Organizations should evaluate a vendor's:
    * **Reputation:** Ability to handle objectives securely.
    * **Financial Stability:** Includes having appropriate **cyberinsurance** to cover potential breaches or litigation.
    * **Security Controls:** Must be as good as or better than the controller's own (e.g., ISO/IEC 27001, PCI-DSS, or SOC 2 certifications).
* **Core Contract Terms (Data Processing Agreements):**
    * **Confidentiality:** Prohibition on sharing data with unauthorized parties.
    * **"No Further Use":** Vendor must not use data for any purpose other than those specified in the agreement.
    * **Audit Rights:** Controller must retain the right to audit the vendor’s security/privacy practices.
    * **Subcontractor Use (Flow-Down):** Vendors must be contractually obligated to flow the same privacy/security requirements down to any **downstream subcontractors**.
    * **End of Relationship:** Must specify whether data is **returned or deleted** at the end of the contract.
* **Master Service Agreement (MSA):** An **umbrella contract** for long-term work, including general security and privacy requirements.
* **Statement of Work (SOW):** Documents project-specific details, referencing the overarching MSA.
* **Service-Level Agreement (SLA):** Specifies the conditions of service (e.g., system availability, response time) and remedies for failure.
* **Business Associate Agreement (BAA):** Required by **HIPAA**; contractually obligates vendors (**Business Associates**) to comply with HIPAA's security, privacy, and breach rules.
* **PCI DSS:** Requires organizations to work only with vendors that are certified as compliant with **PCI DSS** requirements.
* **Vendor Incident Management:** Agreements must clearly spell out the vendor's obligation to **report known or suspected security incidents** to the customer.

## FTC Privacy Protection
The **Federal Trade Commission (FTC)** is the lead agency for broad consumer protection in the private sector, enforcing the **FTC Act** (Section 5) against **unfair and deceptive trade practices**.

* **FTC’s Role:** Regulates private sector privacy through enforcement actions based on published privacy policies versus actual business conduct, conducts studies, and advises lawmakers. The US lacks a single comprehensive federal privacy law.
* **Children’s Online Privacy Protection Act (COPPA):** Provides special protection for children under 13.
    * **Scope:** Applies to online services (websites, apps, etc.) that are intended for, or knowingly collect data from, children under 13.
    * **Requirements:** Requires online operators to post a complete **Privacy Policy**, provide **Parental Notification**, obtain verifiable **Parental Consent** before collection, grant parents the right to review/delete data, and implement **Information Security** programs.
* **Future of Enforcement:** Addresses challenges from new technologies like **Big Data**, **Artificial Intelligence (AI)**, **Machine Learning (ML)**, and the **Internet of Things (IoT)**, which enable new business models like data brokers and cross-border data flows.

***

## Medical Privacy
Federal laws provide special protections for personal medical information.

* **Health Insurance Portability and Accountability Act (HIPAA):** Sets standards for the privacy and security of **Protected Health Information (PHI)** and **electronic PHI (ePHI)**.
    * **Scope:** Applies to **Covered Entities** (health plans, clearinghouses, providers) and their **Business Associates** (third parties with access to PHI, bound by **Business Associate Agreements** or BAAs).
    * **Privacy Rule:** Governs the **use and disclosure** of PHI, requiring the **minimum necessary** amount of PHI be shared. Grants **Individual Rights** to patients (e.g., to access, correct, and request restrictions on their data).
    * **Security Rule:** Applies only to ePHI, requiring covered entities to conduct a regular **risk analysis** and implement safeguards for confidentiality, integrity, and availability.
* **Health Information Technology for Economic and Clinical Health (HITECH) Act (2009):** Promoted Electronic Health Records (EHRs) and strengthened HIPAA.
    * **Key Change:** Extended HIPAA's direct liability to **Business Associates** and introduced the **Breach Notification Rule** (requiring notice to victims and HHS within **60 days** for significant breaches).
* **21st Century Cures Act (2016):** Encourages standardized EHRs, penalizes **information blocking** (preventing appropriate sharing of ePHI), and facilitates sharing of mental health/substance abuse information with family/caregivers.
* **Confidentiality of Substance Use Disorder Patient Records Rule (42 CFR Part 2):** Provides heightened confidentiality for substance use disorder treatment records, generally requiring patient consent for disclosure.

***

## Financial Privacy
Regulations govern the financial sector, including credit, banking, and insurance.

* **Fair Credit Reporting Act (FCRA) (1970):** Regulates **Consumer Reporting Agencies (CRAs)**.
    * **Purpose:** Ensures the accuracy, fairness, and privacy of **consumer reports** used in decisions about credit, insurance, or employment.
    * **Rights:** Gives consumers the right to **access their report/score**, be informed of unfavorable decisions, and **dispute inaccurate information**. Sharing is limited to **permissible purposes**.
* **Fair and Accurate Credit Transactions Act (FACTA) (2003):** Updated FCRA to combat identity theft.
    * **Provisions:** Guaranteed the right to **free annual credit reports** and allowed consumers to place **fraud alerts** on their reports.
* **Gramm–Leach–Bliley Act (GLBA) (1999):** Regulates **financial institutions**.
    * **Privacy Rule:** Requires providing a **Privacy Notice** to **customers** (ongoing relationship) initially and annually. Allows for sharing of customer information, but the notice must inform customers of the institution's policies.
    * **Safeguards Rule:** Requires a written **information security program** to protect customer information against anticipated threats.
* **Red Flags Rule:** Mandates that financial institutions and creditors develop a written plan to proactively monitor consumer data for signs (**red flags**) of identity theft.
* **Consumer Financial Protection Bureau (CFPB):** Created by the Dodd–Frank Act (2008). Enforces against **Unfair, Deceptive, or Abusive Acts and Practices (UDAAPs)** in the financial sector.

***

## Educational Privacy
The education sector is regulated to protect student academic records.

* **Family Educational Rights and Privacy Act (FERPA) (1974):** Protects the privacy of **student educational records**.
    * **Scope:** Applies to almost all educational institutions receiving **federal funding** from the U.S. Department of Education.
    * **Requirements:** Prohibits schools from sharing educational records without the consent of the student (over 18 or in higher education) or parent/guardian (for minors), except for specific exceptions (e.g., to "school officials" with a **legitimate educational interest**). Grants the right to inspect and seek correction of records.

***

## Telecommunications and Marketing Privacy
Laws in this sector regulate how businesses can use personal data for marketing.

* **Telephone Consumer Protection Act (TCPA) (1991) & Telemarketing Sales Rule (TSR):** Regulate unsolicited telemarketing calls and text messages.
    * **Key Provision:** Established the **National Do-Not-Call (DNC) Registry**. Telemarketers must update their DNC list every 31 days and cannot call numbers on it, with exceptions for things like political calls, charities, and the **Established Business Relationship (EBR)** exemption.
* **Controlling the Assault of Non-solicited Pornography and Marketing (CAN-SPAM) Act (2003):** Regulates all **commercial electronic messages** (including email and social media messages).
    * **Requirements:** Senders must be honest (accurate header, physical address), clearly identify the message as an advertisement, and provide a simple, free **opt-out** mechanism, honoring requests within 10 business days.
* **Video Privacy Protection Act (VPPA) (1988):** Protects a consumer’s video rental/purchase history. Disclosure requires written consent (including electronic consent). Its privacy protections are now being applied to **streaming media services**.
* **Driver’s Privacy Protection Act (DPPA) (1994):** Prevents states from indiscriminately releasing personal information from **DMV driver’s licensing databases** (e.g., name, address, photo), allowing sharing only for specific permissible purposes.
* **Customer Proprietary Network Information (CPNI):** Rules under the **Telecommunications Act** governing metadata about subscriber phone calls. Carriers must implement safeguards and obtain consent before sharing CPNI outside of limited, allowed uses.

# Government and Court Access to Private Sector Information Notes

## 🏛️ Constitutional Foundation
* **Fourth Amendment:** Protects U.S. citizens from **"unreasonable searches and seizures"** by federal agencies without a legal **warrant**. It covers "persons, houses, papers, and effects."
* ***Katz v. United States* (1967):** Established that the Fourth Amendment protects an individual's "reasonable expectation of privacy," even in public places. This is crucial for electronic communications.
* ***Third-Party Doctrine:*** Established by ***United States v. Miller* (1976)**. Once a person voluntarily turns information over to a third party (e.g., banks, service providers) for transactions, that information is no longer considered the individual's property and is generally **not protected** by the Fourth Amendment.

---

## 🚔 Law Enforcement and Privacy

### Access to Financial Data

| Legislation | Purpose | Key Requirements | Privacy Impact |
| :--- | :--- | :--- | :--- |
| **Right to Financial Privacy Act (RFPA) of 1978** | Regulates how federal authorities access customer records from financial institutions (FIs) following the *Miller* ruling. | Requires the government to notify the customer and provide a chance to **object** within 10 days (14 days if mailed). Disclosure must be authorized by: **Customer Authorization**, **Administrative/Judicial Subpoena**, **Search Warrant** (90-day notification delay), or **Formal Written Request**. | Provides some due process rights, but not Fourth Amendment protection. |
| **Bank Secrecy Act (BSA) of 1970** (a.k.a. Currency and Foreign Transactions Reporting Act) | Established to combat **money laundering** and terrorist financing by creating a financial paper trail. | FIs must have an **Anti-Money Laundering (AML) program** and a **Customer Identification Program (CIP)**. Requires FIs to file: **Currency Transaction Reports (CTRs)** (transactions over \$10,000/day) and **Suspicious Activity Reports (SARs)**. | **Reduces privacy**; FIs are **prohibited from notifying customers** when filing an SAR (making SARs an exception to the RFPA). |

### Access to Communications

* **Electronic Communications Privacy Act (ECPA) of 1986:** Primary legislation regulating government eavesdropping.

| ECPA Title | Common Name | Scope | Privacy Standard |
| :--- | :--- | :--- | :--- |
| **Title I** | **Wiretap Act** | Prohibits spying on **real-time** oral, wire, or electronic communication without **consent** (one-party consent federally) or a warrant. | High protection, requiring a warrant for content. |
| **Title II** | **Stored Communications Act (SCA)** | Extends Fourth Amendment-like protection to **digital communications stored** on third-party servers (e.g., email). Requires a **search warrant** for government access. | Lower protection than real-time, due to third-party doctrine, but enhanced by the SCA. |
| **Title III** | **Pen Registers/Trap-and-Trace** | Regulates technologies that track communications **metadata** (e.g., phone numbers, date/time) but **not content**. | Lower protection; generally requires only a court order. |

* **CLOUD Act (2018):** Amends the SCA to compel U.S.-based companies to provide data stored on servers, regardless of the data’s **physical, overseas location**.
* **Communications Assistance for Law Enforcement Act (CALEA):** Requires telecommunications carriers and manufacturers to design their devices and services to **enable authorized government surveillance** capabilities (wiretapping) to be **"baked-in"** features.
    * **Limitation:** CALEA **does not compel** companies to assist the government with **decrypting** encrypted communications.

---

## 🔒 National Security and Privacy

* In national security, the stakes are higher, often leading lawmakers to grant the government **more power** than for regular law enforcement.

### Foreign Intelligence Surveillance Act (FISA) of 1978

* **Purpose:** Provides a legal framework for the government to track **foreign targets** and agents spying on the U.S. while setting due process and oversight.
* **FISC:** Established the **Foreign Intelligence Surveillance Court**, a secret court that issues warrants for surveillance under FISA.
* **Targets:** Surveillance is easier if the target is **not a "United States person"** (U.S. citizens, legal aliens, U.S. corporations, etc.).
* **Minimization Principle:** Requires the U.S. Attorney General to implement procedures to ensure that intelligence gathered and retained **pertains only to the intended investigation** and avoids collecting incidental information on U.S. persons.

| Key Amendments/Related Acts | Impact on Surveillance Power |
| :--- | :--- |
| **USA-PATRIOT Act (2001)** | **Expanded power**, lowering FISA's surveillance threshold from "primary purpose" to **"significant purpose."** |
| **FISA Amendments Act Section 702 (2008)** | Allows the government to obtain **broad certifications** (not warrants) from FISC to conduct surveillance on **non-U.S. persons located abroad**. This has led to the **mass collection** of communications data. |
| **Section 206: Roving Wiretaps** (Patriot Act) | Authorized surveillance of **any device** associated with an individual, rather than specific devices/numbers. (Expired March 2020) |
| **Section 215: Business Records Provision** (Patriot Act) | Allowed the government to order businesses to share records of any **"tangible things"** relevant to foreign intelligence, bypassing other laws (used for bulk phone record collection). (Expired March 2020) |
| **USA FREEDOM Act (2015)** | **Curtailed power** by requiring requests to list **"selection terms"** (specific criteria like phone numbers) to end the bulk data collection programs revealed by Edward Snowden. Also reformed **National Security Letters (NSLs)**. |

* **National Security Letters (NSLs):** A type of **administrative subpoena** used to compel the production of business records (stored email, phone data). Often includes a **gag order** prohibiting the recipient from disclosing the request.

### Cybersecurity Information Sharing Act (CISA) of 2015

* **Purpose:** Encourages **voluntary sharing** of **cyber-threat indicators** between private companies and the federal government by **removing legal barriers**.
* **Safe Harbor:** Provides private companies protection from certain liabilities (like those under the ECPA or antitrust laws) when sharing information **in accordance with CISA's protocols**.
* **Privacy:** Companies are required to **remove PII** before sharing unless that information is directly related to the cyber threat itself.

---

## 🧑‍⚖️ Civil Litigation and Privacy

### Compelled Disclosure of Media Information

* ***Zurcher v. Stanford Daily* (1978):** Supreme Court ruled that the Constitution **does not protect journalists** from duly authorized search warrants.
* **Privacy Protection Act (PPA) of 1980:** Prohibits law enforcement from using a **search warrant** to seize journalistic **"work product materials"** and **"documentary materials."**
    * To compel disclosure, law enforcement must generally use a **subpoena duces tecum**, which provides the journalist with **advance notice** and the opportunity to challenge the order in court.
    * PPA provides a **private right of action** against agencies that violate the law.

### Electronic Discovery (eDiscovery)

* The process of identifying, collecting, and producing electronic records for legal proceedings.
* **Key Stages (often managed by legal counsel):**
    1.  **Identification:** Determining which records are subject to discovery, often assisted by IT staff.
    2.  **Preservation:** Placing relevant records under a **legal hold** to prevent alteration or destruction.
    3.  **Collection:** Gathering the preserved records and securely transferring them to legal counsel.
    4.  **Processing:** Converting data to reviewable formats.
    5.  **Review:** Attorneys examine the records to **redact or remove** information that is irrelevant, protected by privilege, or protected by statute.
    6.  **Production and Presentation:** Sharing the finalized information with the opposing parties or court.

## I. Introduction to Workplace Privacy
Workplace privacy in the U.S. is not governed by a single comprehensive law but by a "patchwork" of federal and state statutes, tort law, and contracts. The primary drivers of federal workplace privacy legislation are **antidiscrimination** and **labor rights**, rather than privacy for privacy's sake.

### A. Key Regulatory Agencies
* **Federal Trade Commission (FTC):** Regulates background screening via the Fair Credit Reporting Act (FCRA).
* **Consumer Financial Protection Bureau (CFPB):** Shares FCRA enforcement with the FTC; targets background check companies for inaccuracies.
* **Department of Labor (DOL):** Enforces fair labor standards and laws like FMLA, OSHA, and EPPA.
* **Equal Employment Opportunity Commission (EEOC):** Enforces antidiscrimination laws (ADA, ADEA, Title VII, GINA).
* **National Labor Relations Board (NLRB):** Protects workers' rights to organize and bargain collectively; regulates employer surveillance that might intimidate union activities.
* **Occupational Safety and Health Administration (OSHA):** Ensures workplace safety; protects confidentiality of employee complaints and medical records related to workplace safety.
* **Securities and Exchange Commission (SEC):** Requires public companies to disclose human capital metrics relevant to investors.

## II. U.S. Antidiscrimination Laws
Federal laws restrict the collection and use of personal data to prevent bias.

* **Civil Rights Act of 1964 (Title VII):** Prohibits discrimination based on race, color, religion, national origin, or sex (including pregnancy/childbirth).
* **Americans with Disabilities Act (ADA):**
    * Prohibits discrimination based on disability if the person is qualified and can perform essential functions with **reasonable accommodation**.
    * **Medical Exams:** Pre-employment medical exams are banned before a conditional job offer. Medical info must be kept in separate, confidential files.
    * **Undue Hardship:** Employers are not required to provide accommodations that cause significant difficulty/expense.
* **Genetic Information Nondiscrimination Act (GINA):**
    * Prohibits using genetic info (including family medical history) for hiring, firing, or promotion.
    * Generally prohibits collecting genetic info, with narrow exceptions (e.g., accidental acquisition, FMLA requests, wellness programs).

## III. Privacy Before Employment (Screening)
### A. Automated Employment Decision Tools
* Use of AI/algorithms in hiring creates risks of unintentional bias (e.g., facial analysis penalizing certain groups).
* **Regulation:** Some jurisdictions (e.g., NYC) require bias audits and notices to candidates before using AI in hiring.

### B. Background Screening & The FCRA
Background checks by third parties are usually considered **Consumer Reports** under the FCRA.
* **Employer Obligations:**
    1.  Provide written notice to the applicant.
    2.  Obtain written authorization.
    3.  Certify compliance to the background check provider (CRA).
    4.  **Investigative Consumer Reports:** If interviewing neighbors/associates about character, specific notice of the "investigative" nature is required.
* **Adverse Action:** If not hiring based on the report, employers must follow specific pre-adverse and adverse action notice procedures.

### C. Other Screening Methods
* **Polygraphs:** The **Employee Polygraph Protection Act (EPPA)** bans most private employers from using lie detectors for pre-employment screening.
    * *Exceptions:* Government, security firms, pharmaceutical distributors, or specific theft investigations.
* **Drug/Alcohol Testing:** Regulated by a mix of state laws and federal requirements (e.g., DOT). The **Drug-Free Workplace Act** encourages, but doesn't always mandate, testing.
* **Social Media:** Employers often check profiles but risk seeing protected class info (race, religion). Best practice is using a third party to redact protected info.

## IV. Privacy During Employment (Monitoring)
Employees generally have **no expectation of privacy** using company equipment.

### A. Monitoring Technologies
* **Computer/Phone Usage:** Employers own the equipment and can monitor use.
* **Location Tracking:** GPS monitoring of company vehicles/phones is generally permitted, though some states require notice.
* **Biometrics:** Collecting fingerprints/face scans for timekeeping is common. States like IL, TX, and WA have specific laws requiring notice/consent/retention policies.
* **Wellness Programs:** Employers can offer incentives for health programs. Collection of health data must be voluntary and not penalized if opted out (EEOC rules).

### B. Electronic Communications Privacy Act (ECPA)
Regulates interception of wire, oral, and electronic communications.
* **The "Business Purpose" Exception:** Employers can monitor calls/emails if there is a legitimate business reason.
    * *Limitation:* Monitoring must stop if the communication is determined to be personal.
* **Consent:** Monitoring is legal if one party consents (federal law). Some states require all-party consent.
* **Stored Communications Act (SCA):** accessing stored emails (on company servers) is generally easier than intercepting real-time calls, as company ownership usually negates privacy expectations.

### C. Investigation of Misconduct
* **Fairness:** Investigations must be evenhanded to avoid discrimination claims.
* **FACTA Amendment:** The Fair and Accurate Credit Transactions Act amended the FCRA so that **misconduct investigation reports** by third parties are **not** treated as standard consumer reports.
    * *Result:* Employers do *not* need to get prior consent to investigate an employee for suspected misconduct, nor do they need to provide the full report (only a summary if adverse action is taken).

## V. Privacy After Employment
### A. Termination Procedures
* **Transition Management:** Securely ending the relationship.
* **Access Control:** Immediate revocation of physical (keys, badges) and digital (email, network) access.
* **Property Return:** Retrieving laptops and ensuring no company data remains on personal devices.

### B. Records Retention
* Employers must follow retention schedules for personnel files (performance reviews, disciplinary records, medical info) to comply with laws and prepare for potential litigation (eDiscovery).

### C. References
* No federal requirement to provide references.
* **Service Letter Acts:** Some states require employers to provide basic employment verification (dates, title).
* **Defamation Risk:** Many employers limit references to basic facts (dates/title) to avoid lawsuits from former employees regarding negative comments.

# State Privacy Laws

### Overview
The United States lacks a comprehensive federal privacy regulation, resulting in a "patchwork" of state laws. States fill gaps where federal law is silent (e.g., data breach notification) and often enact stricter regulations than federal statutes.

### Federal Versus State Authority
* **Preemption:** Federal laws generally preempt state laws unless otherwise specified.
* **State Enforcement:** State Attorneys General (AGs) typically enforce privacy laws. Some states (e.g., California) have dedicated privacy agencies (CPPA).
* **Jurisdiction:** AGs can seek remedies for violations affecting their state residents, even if the company is located elsewhere.

### Common Elements of State Privacy Laws
* **Applicability & Thresholds:** Laws often apply based on specific triggers, such as annual revenue, number of customers, or amount of revenue derived from selling data.
* **Exemptions:** Common exemptions include nonprofits, government agencies, and entities already regulated by federal laws like HIPAA or GLBA.
* **Data Subject Rights:**
    * **Access:** Right to view collected data.
    * **Correction/Deletion:** Right to fix errors or erase data.
    * **Portability:** Right to receive data in a usable format.
    * **Opt-out/Opt-in:** Rights regarding data sales, sharing, and targeted advertising.
* **Privacy Notices:** Requirements to disclose practices, often aligning with transparency principles.
* **Data Security:** Obligations to implement administrative, technical, and physical controls (often referencing frameworks like NIST).
* **Enforcement:** Mechanisms include cure periods (time to fix violations before penalties), civil penalties, and occasionally a **private right of action** (allowing individuals to sue).

### Data Breach Notification Laws
Every state has enacted a data breach notification law. While they share a common structure, details vary significantly.
* **Definitions:**
    * *Breach:* Varies between "unauthorized access" vs. "unauthorized acquisition."
    * *Personal Information (PI):* Typically Name + SSN, Driver’s License, or Financial info. Newer definitions include biometrics, medical info, and username/password combinations.
* **Notification Requirements:**
    * *Whom:* Affected residents, state regulators (AGs), and credit reporting agencies (based on thresholds).
    * *When:* Timelines vary (e.g., "without unreasonable delay," 30 days, 45 days).
    * *Encryption:* Historically, encrypted data was exempt. Newer laws require notification if encryption keys are also compromised.

### Comprehensive State Privacy Laws
Several states have enacted GDPR-style comprehensive laws:
* **California (CCPA & CPRA):** The most extensive U.S. law. Includes a private right of action for security breaches, established the California Privacy Protection Agency (CPPA), and protects "sensitive personal information."
    * **Vendor Contracts:** As of Jan 2023, data controllers **must** enter into contracts with *any* third party with whom they share data, featuring specific restrictive provisions.
    * **Opt-out Requirements:** CCPA/CPRA (California) and VCDPA (Virginia) require systems to restrict data sharing with vendors if a consumer exercises their right to **opt-out of data selling or targeted advertising**.
* **Virginia (VCDPA):** Grants consumer rights (access, correct, delete) and requires data protection assessments. Enforced solely by the AG.
* **Colorado (CPA):** Similar rights to Virginia; recognizes "sensitive data" requiring consent.
* **Connecticut (CTDPA) & Utah (UCPA):** Follow similar models regarding data subject rights and controller obligations.
* **Florida (FDBR):** Targeted at "Big Tech" with a high revenue threshold ($1B+).
* **Oregon, Texas, & Montana:** Recent additions largely following the model of defining controller obligations, consumer rights, and AG enforcement.

### Comparison of Key State Privacy Laws

| State Law | Effective Date | Sensitive Data | Cure Period | Private Right of Action |
| :--- | :--- | :--- | :--- | :--- |
| **California (CCPA/CPRA)** | Jan 1, 2023 | **Opt-Out** ("Limit Use") | Discretionary (Auto 30-day ended '23) | **Yes** (limited to breaches) |
| **Virginia (VCDPA)** | Jan 1, 2023 | **Opt-In** (Consent) | 30 days | No |
| **Colorado (CPA)** | July 1, 2023 | **Opt-In** (Consent) | 60 days (Sunsets 1/1/25) | No |
| **Connecticut (CTDPA)** | July 1, 2023 | **Opt-In** (Consent) | 60 days (Sunsets 12/31/24) | No |
| **Utah (UCPA)** | Dec 31, 2023 | **Notice + Opt-Out** | 30 days | No |

### Quick Reference: Jurisdictional Thresholds
A business is subject to the law if it meets **one or more** of these criteria (varies by state):

*   **California (CCPA/CPRA):**
    *   Gross Annual Revenue > **$25 Million**
    *   Buys, sells, or shares personal revenue of **100,000+** consumers/households
    *   Derives **50% or more** of annual revenue from selling/sharing personal info

*   **Virginia (VCDPA):**
    *   Controls/processes personal data of **100,000+** consumers
    *   Controls/processes personal data of **25,000+** consumers AND derives **>50%** of gross revenue from the sale of personal data

*   **Colorado (CPA):**
    *   Controls/processes personal data of **100,000+** consumers
    *   Controls/processes personal data of **25,000+** consumers AND derives **revenue or a discount** from the sale of personal data

*   **Connecticut (CTDPA):**
    *   Controls/processes personal data of **100,000+** consumers (excluding payment data)
    *   Controls/processes personal data of **25,000+** consumers AND derives **>25%** of gross revenue from the sale of personal data

*   **Utah (UCPA):**
    *   Must meet **BOTH**: Annual Revenue > **$25 Million** AND one of the following:
        *   Controls/processes personal data of **100,000+** consumers
        *   Derives **>50%** of gross revenue from the sale of personal data AND controls/processes data of **25,000+** consumers

### Subject-Specific Privacy Laws

#### Health & Genetic Information
* **Washington My Health My Data Act:** Protects non-HIPAA health data; restricts geofencing near healthcare facilities; includes a private right of action.
* **Illinois Genetic Information Privacy Act (GIPA):** Prohibits genetic discrimination in employment and insurance; has a private right of action.
* **Nevada Consumer Health Data Privacy Law:** Similar to Washington's law, protecting health data not covered by HIPAA.

#### Online Privacy & Children
* **Delaware (DOPPA):** Requires privacy policies for websites/apps; restricts marketing of adult products to children.
* **California Age-Appropriate Design Code:** Requires high privacy defaults and Data Protection Impact Assessments (DPIAs) for services likely accessed by children.
* **CalECPA:** Requires warrants for law enforcement to access electronic communications (emails, location data).

#### Biometric Information
* **Illinois (BIPA):** Strict consent requirements for collecting biometrics; includes a private right of action (resulting in major settlements).
* **Washington & Texas (CUBI):** Regulate biometric capture and sale but enforced only by AGs.
* **New York City:** Requires commercial businesses to post signs if tracking biometrics; private right of action.

#### AI & Automated Decision-Making
* **Colorado SB 24-205:** Regulates "high-risk" AI systems making consequential decisions (hiring, lending).
* **NYC Local Law 144:** Requires bias audits for AI tools used in hiring/employment.

#### Financial & Data Brokers
* **California Financial Information Privacy Act (CFIPA):** Stricter than federal GLBA; requires opt-in for sharing with unaffiliated third parties.
* **NYDFS Cybersecurity Regulation:** Mandates rigorous security programs for financial institutions in NY (CISO, encryption, MFA).
* **California Delete Act:** Creates a centralized mechanism for consumers to request data deletion from all registered data brokers.

### Marketing Laws
* **UDAP:** State "Unfair and Deceptive Acts or Practices" laws fill gaps in FTC enforcement.
* **Telemarketing:** State laws often impose stricter curfews and registration requirements than federal rules.

# International Privacy Regulation

### Overview
Multinational corporations face significant challenges in managing data across international boundaries. While U.S. state laws operate under federal preemption, international laws have no such hierarchy, leading to potential conflicts where complying with one nation's law may violate another's. The central tension lies between countries with strict privacy rights (like the EU) and the operational need for global data flow.

### European Union General Data Protection Regulation (GDPR)
The GDPR, effective May 2018, represents a progressive model of privacy protection that prioritizes individual rights over business interests. It has broad implications for U.S. companies due to its extraterritorial scope.

#### Scope and Definitions
* **Personal Data:** Broadly defined to include any information identifying a "natural person" or "data subject" (e.g., names, geolocation). It protects anyone physically in the EU, regardless of citizenship.
* **Controllers vs. Processors:**
    * *Controller:* Entity that determines the purpose and means of processing.
    * *Processor:* Entity that processes data on behalf of the controller.
    * Both parties have distinct obligations and liabilities.
* **Territorial Jurisdiction:** Applies to any organization, regardless of location, that offers goods/services to or monitors the behavior of people within the EU.

#### Data Subject Rights
The GDPR grants extensive rights to individuals, requiring opt-in consent that is clear and distinguishable.
* **Right to Erasure (Right to be Forgotten):** Subjects can demand the deletion of their data.
* **Right to Access:** Subjects can request to know what data is collected and why.
* **Right to Rectification:** Ability to correct inaccurate data.
* **Right to Data Portability:** Right to receive data in a machine-readable format.
* **Right to Object:** Ability to opt-out of processing or direct marketing.
* **Automated Decision-Making:** Restrictions on AI making significant legal decisions about people.

#### Penalties
Violations can result in steep fines: up to **€20,000,000 or 4% of a company’s annual revenue**, whichever is greater.

### Mechanisms for International Data Transfer (EU)
The GDPR generally prohibits transferring data to non-EU countries unless the recipient ensures adequate protection.
* **"Surprise Minimization" Rule:** A guiding principle that consumers should be able to assume their information is subject to the protections of their home jurisdiction, regardless of where it is processed. Individuals should not be "surprised" by processing prohibited in their home country simply because data was moved.

1.  **Adequacy Decisions:** The EU Commission reviews a non-EU country’s laws. If deemed "adequate" (commensurate with GDPR), data can flow freely.
2.  **Binding Corporate Rules (BCRs):** Complex, legally binding internal rules for multinational corporations to transfer data between their own global entities. Requires EU regulatory approval.
3.  **Standard Contractual Clauses (SCCs):** Standardized, non-negotiable contract language provided by the EU Commission. Used between a "data exporter" (EU) and "data importer" (non-EU) to contractually obligate GDPR compliance.
4.  **Derogations (Article 49 Exceptions):** Should be relied upon only as a last resort and interpreted restrictively. They include:
    * **Explicit Consent:** Subject is informed of the specific risks (absence of adequacy/safeguards).
    * **Contract Necessity:** Necessary for a contract between the subject and controller.
    * **Third-Party Contract:** In the interest of the data subject.
    * **Public Interest:** Important reasons of public interest.
    * **Legal Claims:** Establishment, exercise, or defense of claims.
    * **Vital Interests:** Protecting life when the subject is incapable of consent.
    * **Public Register:** Transfer from a register intended for public consultation.

### Case Study: The reCAPTCHA Compliance "Trap"
* **The Conflict:** Organizations use tools like Google reCAPTCHA for bot protection, but these tools collect significant personal data (IPs, cookies, mouse movements) that are transferred to U.S. servers.
* **The Consent Wall:** Under GDPR/ePrivacy, if a tool is not "strictly necessary" for the user-requested service, it requires prior opt-in consent.
* **Operational Impact:** This creates a paradox where a person cannot access a secure page without passing reCAPTCHA, but reCAPTCHA cannot be loaded until the person accesses the page to give consent. Loading it before consent is a violation; requiring consent before access may violate the principle of "freely given" consent.

### U.S.–EU Data Frameworks
The history of U.S.-EU data transfer is marked by legal challenges regarding U.S. government surveillance.

* **Past Agreements (Invalidated):**
    * *Safe Harbor:* Invalidated following the *Schrems I* case.
    * *Privacy Shield:* Invalidated by the CJEU in *Schrems II* (2020) due to concerns that U.S. surveillance laws overrode privacy protections for EU citizens.
    * **EDPB 6-Step Roadmap for TIAs:**
        1. **Map all transfers:** Know exactly where data is going and any downstream transfers.
        2. **Verify transfer tools:** Identify the legal basis used (SCC, BCR, etc.).
        3. **Assess local law:** Determine if the destination country's laws (like U.S. surveillance) impinge on safeguards.
        4. **Adopt supplementary measures:** Implement technical (encryption), organizational, or legal safeguards if needed.
        5. **Formalize steps:** Document the assessment and measures taken.
        6. **Re-evaluate:** Monitor the level of protection at appropriate intervals.
* **Current Framework: EU–U.S. Data Privacy Framework (DPF):**
    * Established in 2023 after an EU adequacy decision.
    * **Enforcement:** U.S. companies self-certify compliance via the Department of Commerce; enforcement is handled by the FTC.
    * **Requirements:** Companies must update privacy policies, provide independent dispute resolution mechanisms, limit data retention, and ensure third-party accountability.

### APEC Privacy Framework
The Asia-Pacific Economic Cooperation (APEC) promotes flexible mechanisms to facilitate digital trade among member economies (which include the U.S., Canada, Japan, and Mexico, but not India).

* **Nature:** Non-binding framework; does not override domestic laws.
* **Nine Core Principles:**
    1.  Preventing Harm
    2.  Notice
    3.  Collection Limitation
    4.  Uses of Personal Information
    5.  Choice
    6.  Integrity of Personal Information
    7.  Security Safeguards
    8.  Access and Correction
    9.  Accountability
* **Cross-Border Privacy Rules (CBPR):** A voluntary safe harbor system where companies are certified by third parties (like TrustArc in the U.S.) to demonstrate compliance with APEC principles.
- **Cross-border Privacy Enforcement Arrangement (CPEA):**
    - A framework for regional cooperation specifically for *Privacy Enforcement Authorities (PE Authorities)* to share information and conduct joint investigations.
    - *Distinction:* Unlike the CBPR (which certifies *companies*), the CPEA connects *regulators*.
    - The U.S. is a member of the CPEA.
* **FACTA Disposal Rule:** Requires any individual or entity that uses a consumer report for a business purpose to dispose of it in a manner that avoids unauthorized access and misuse.

### Global Cooperation & Enforcement
* **Global Privacy Enforcement Network (GPEN):** Created by the OECD. It is not a regulatory framework but a network to facilitate cooperation, information sharing, and training among privacy enforcement authorities globally.
  - *U.S. Participation:* The U.S. participates through the **FTC**, the **FCC**, and the **California Attorney General**.
* **Conflict Resolution:** There is no single international law to resolve conflicts. Companies must rely on data management programs and legal counsel to navigate contradictions (e.g., when U.S. law mandates disclosure that EU law prohibits).
