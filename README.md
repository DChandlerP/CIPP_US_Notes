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

## 3. Privacy-Enhancing Technologies (PETs)
PETs are "technologies whose purpose is privacy". This field is often led by **privacy engineers** who focus on achieving "freedom from conditions" that create problems for individuals during data processing.

### Identifiability and Identifiers
* **Identifiability:** The degree to which data can be directly attributed to an individual.
* **Linkability:** The amount of effort required to link data to a specific individual.
* **Strong Identifiers:** Data that is identifying without additional context (e.g., SSN, Passport #).
* **Weak Identifiers:** General data belonging to multiple people, needed in combination for identification (e.g., height, home address).
* **Quasi-Identifiers:** Data combined with external knowledge to link it to an individual.

### Anonymization & De-Identification Techniques
* **Suppression:** Removing identifying information or values from a data set.
* **Generalization:** Reducing granularity by replacing specific info with more general elements (e.g., removing a house number from an address).
* **Top- and Bottom-Coding:** Grouping the extreme ends of a range into a single category (e.g., income brackets labeled as "< $20,000").
* **Noise Addition:** Replacing actual values with data from the same class to maintain statistical properties while hiding individuals.
* **Anonymity Metrics:** The relative success of these techniques is measured by **k-anonymity**, **l-diversity**, and **t-closeness**.

### Aggregation and Differential Privacy
* **Aggregation:** Using statistics from groups of records rather than individual data.
* **Differential Privacy:** A mathematical framework that introduces "noise" to provide a guarantee of **indistinguishability** and "plausible deniability" for individuals in a dataset.



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
* **Federal Trade Commission (FTC):** The primary federal privacy regulator. (See the [FTC Deep Dive](#5-federal-trade-commission-ftc-deep-dive) below for details).
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


## 5. Federal Trade Commission (FTC) Deep Dive
The FTC is the primary federal privacy regulator, enforcing consumer protection and antitrust laws.

### 1. Organizational Structure & Authority
* **Independent Agency Status:** Established by the FTC Act of 1914, the FTC is an independent administrative agency not under the direct authority of the President.
* **Governance:** Governed by a Chairperson and four additional Commissioners.
* **Primary Power (Section 5):** Prohibits "unfair or deceptive acts or practices in or affecting commerce." This is the most important piece of federal privacy legislation despite not explicitly mentioning data.
* **Rulemaking (Section 18 / Magnuson-Moss):** Unlike most agencies, the FTC must follow the rigorous Magnuson-Moss Act (Section 18) for rulemaking rather than the standard APA.
    * **The "Prevalence" Requirement:** The FTC can only issue rules if it has reason to believe the unfair or deceptive practices are **prevalent** (widespread), established via prior cease-and-desist orders or evidence of a widespread pattern of conduct.
    * **Commercial Surveillance Rule:** A proposed rulemaking is currently pending to govern the "commercial surveillance" industry.

### 2. Legal Standards for Section 5

* **Deceptive Trade Practices (3-Part Test):**
    1. **Material:** Likely to affect a consumer’s conduct or decision.
    2. **Statement or Omission:** A representation or failure to disclose.
    3. **Likely to Mislead:** Must be deceptive to a consumer acting reasonably under the circumstances.

* **Unfair Trade Practices (3-Part Test - Section 5(n)):**
    1. **Substantial Injury:** Causes or is likely to cause significant harm.
    2. **Not Reasonably Avoidable:** Consumers could not have reasonably prevented the injury themselves.
    3. **Not Outweighed by Benefits:** The harm is not offset by countervailing benefits to consumers or competition.


### 3. Jurisdictional Limits (Exclusions)
* **Commerce Requirement:** Authority only applies to practices "in or affecting commerce."
* **Exempt Entities:** Section 5 authority does NOT extend to:
    * Non-profit organizations.
    * Most banks and financial institutions.
    * Common carriers (communications and transportation).
* **No Private Right of Action:** Only the government can bring suits; individuals cannot sue under the FTC Act.

### 4. Enforcement Life Cycle
* **Investigatory Powers:**
    * **Section 6:** Authority to require businesses to submit written reports under oath.
    * **Section 9:** Broad subpoena power for investigations.
* **Formal Proceedings:**
    * **ALJ Hearing:** Complaints are heard by an Administrative Law Judge (ALJ). The ALJ can issue injunctions but cannot impose civil penalties.
    * **Appeals:** ALJ decisions are appealed to the five FTC Commissioners. Final adverse determinations from the Commission are appealed to a **federal Circuit Court of Appeal** (never a federal District Court).
* **Penalties and Remedies:**
    * **Civil Penalties:** While the ALJ/Commission cannot impose them directly, the FTC can seek them in federal court. As of July 2025, penalties can be up to $53,088 per violation.
    * **Section 13(b):** Allows the FTC to go directly to federal court for injunctions. Note: The Supreme Court (*AMG Capital*) ruled that this section cannot be used for "equitable monetary relief."

### 5. FTC Enforcement Remedies
The FTC uses several tools to enforce compliance and remediate harm:

* **Injunctive Relief:** Court-ordered requirements for a company to take specific actions (e.g., implementing a privacy program).
* **Civil Penalties:** Fines for violating statutes (like COPPA) or prior consent decrees. Following *AMG Capital*, the FTC cannot seek "equitable monetary relief" (like consumer restitution) under Section 13(b).
* **Algorithmic Disgorgement:** A remedy requiring companies to **delete algorithms or models** developed using improperly obtained data. (See *Everalbum* below).
    * **Specificity Requirement (Post-*LabMD*):** Following the *LabMD* ruling, the FTC must provide **concrete directives** in its orders (e.g., "Implement MFA") rather than ordering indeterminable "reasonable" programs.

### 6. Consent Decrees
The vast majority of FTC enforcement actions are settled via a Consent Decree.
* **Legal Force:** An agreement where a defendant takes specific actions to end litigation. Once court-approved, it has the force of a federal court order.
* **Key Features:**
    * Publicly posted to provide industry guidance.
    * Generally does not require an admission of guilt.
    * Usually requires the defendant to maintain and provide proof of compliance to the FTC.

### 7. FTC Security Enforcement & "Reasonableness"
Because the FTC has not issued formal security regulations, practitioners look to **consent orders** and court rulings to define "reasonable" security.

#### **Landmark Judicial Decisions**
* **FTC v. Wyndham Worldwide Corp. (2015):** Landmark 3rd Circuit case that **affirmed the FTC's authority** to regulate cybersecurity as an "unfair" trade practice.
    * **Impact:** Established that companies have "fair notice" that poor security can be a Section 5 violation.
* **LabMD, Inc. v. FTC (2018):** 11th Circuit vacated an FTC order for being **unenforceable and non-specific**.
    * **Key Finding:** The court assumed the FTC has authority over security but ruled the order to implement a "reasonable" program was too vague. The FTC must provide **concrete directives** rather than an **"indeterminable standard of reasonableness."**

#### **What the FTC Considers "Unreasonable" (2017–2020 Case Examples)**
* **Uber (2017):** Failed to use unique access keys or **multi-factor authentication (MFA)** and stored unencrypted geolocation data in the cloud.
* **Lenovo (2017):** Pre-installed **"man-in-the-middle"** software that bypassed browser encryption to show ads, creating major vulnerabilities.
* **PayPal/Venmo (2018):** Falsely claimed "bank-grade security" while lacking a written information security program.
* **VTech Electronics (2018):** The first child privacy case against an **IoT device maker**; failed to implement intrusion detection or encryption.
* **Equifax (2019):** Massive settlement ($575M+) following a breach of 147 million records; cited for failing to patch known vulnerabilities and **segment servers**.
* **Tapplock (2020):** **IoT Security:** Falsely claimed smart locks were "unbreakable" despite API vulnerabilities that allowed account bypass.
* **SkyMed (2020):** **Health Data:** Stored PHI in unsecured cloud databases and used a fake "HIPAA Compliance" seal.
* **Ascension Data & Analytics (2020):** **Vendor Oversight:** Violated the GLBA Safeguards Rule by failing to oversee a vendor that left mortgage data exposed.

#### **Modern Remedies**
* **Algorithmic Disgorgement:** Requires companies to **delete algorithms or models** developed using improperly obtained data. (e.g., *Everalbum*, 2021).


### 8. Modern FTC Enforcement Priorities
The FTC continues to evolve its enforcement strategies to address emerging technological risks and complex market behaviors.

* **2023 Office of Technology:** Created to provide the agency with specialized technical expertise. This team supports agency matters by helping investigators and attorneys understand complex technologies, data practices, and algorithmic systems.
* **Four Key Focus Areas:** Current FTC enforcement is primarily focused on:
    * **Artificial Intelligence (AI):** Monitoring deceptive claims about AI capabilities and the use of biased or improperly trained models.
    * **Healthcare Privacy:** Protecting sensitive health data, especially in non-HIPAA regulated spaces (e.g., health apps and trackers).
    * **Children's Privacy:** Continued rigorous enforcement of COPPA and expanding protections for teens.
    * **Location Data:** Cracking down on the unauthorized sale and misuse of precise geolocation information.
* **Dark Patterns:** The FTC is actively monitoring and taking action against deceptive design elements that subvert user intent. Four specific elements include:
    * **False Beliefs:** Creating deceptive impressions that lead consumers to take actions they otherwise wouldn't.
    * **Hidden Disclosures:** Burying key terms or fees in obscure locations or fine print.
    * **Unauthorized Charges:** Enrolling consumers in recurring payments without clear, informed consent.
    * **Obscured Choices:** Making it difficult for users to opt-out, cancel, or select privacy-protective settings.
* **Unfair Methods of Competition (UMC):** In 2022, the FTC issued a **Policy Statement** regarding its authority under Section 5 to regulate unfair methods of competition.
    * **Two-Part Test:** To determine if conduct is a UMC violation, the FTC looks for:
        1. **Method of Competition:** The conduct must be a type of competition (not just an individual consumer harm).
        2. **Unfair Conduct:** The conduct must be "coercive, exploitative, exclusionary, or otherwise restrictive" of competition.


## 6. Healthcare Privacy Framework
Healthcare privacy in the U.S. is governed by a complex mix of constitutional principles and specific sectoral statutes.

### 1. Constitutional Context
The U.S. legal system has historically recognized a broad **right to privacy** regarding health and medical issues, often derived from the "penumbras" of the Bill of Rights.
* **Legal Uncertainty (Post-*Dobbs*):** The 2022 Supreme Court decision in ***Dobbs v. Jackson Women's Health Organization*** has created significant legal uncertainty regarding the privacy of **reproductive health data**. This ruling narrowed the federal constitutional basis for privacy in this area, shifting many protections to a state-by-state level.

### 2. Core Federal Statutes
While the U.S. lacks a single federal health privacy law, several key statutes regulate specific domains:
* **HIPAA & HITECH:** The primary federal standards for the privacy and security of **Protected Health Information (PHI)**. (See the [HIPAA section](#medical-privacy) below for details).
* **Genetic Information Nondiscrimination Act (GINA):** Prohibits health insurers and employers from discriminating based on genetic information. (Note: Genetic info is classified as **PHI** under HIPAA).
* **21st Century Cures Act:** Focuses on accelerating medical product development and prohibiting **"information blocking"** (penalties up to $1M). Requires developers to publish APIs that allow patient data to be accessed **"without special effort."**
* **42 C.F.R. Part 2:** Provides heightened confidentiality for records of patients treated for **substance use disorders (SUD)** by a "Part 2 Program." Generally prohibits **redisclosure** of records by third-party recipients without additional consent.

### 3. Scope of Coverage & "Regulatory Gaps"
It is a common misconception that all health-related data is protected by federal privacy law.
* **Entity-Based Protection:** Laws like HIPAA apply only to **"Covered Entities"** (providers, insurers) and their **Business Associates**.
* **Unprotected Activities:** Health information generated through activities outside of these entities is often **not federally protected**.
    * *Examples:* Online health searches, fitness tracker data (not linked to a provider), and information shared on social media support groups.
* **FTC Oversight:** When sectoral health laws (like HIPAA) do not apply, the **FTC** acts as the primary regulator for health-related privacy under its Section 5 authority.

### 4. FTC Health Breach Notification Rule (HBNR)
The HBNR fills a key regulatory gap by protecting health information that is not covered by HIPAA.
* **Statutory Basis:** 16 C.F.R. Part 318.
* **Scope:** Applies to non-HIPAA covered entities, specifically **vendors of personal health records (PHRs)** and **third-party service providers** that interact with PHR data.
* **Notification Requirements:** Requires notice to **individuals** and the **FTC**.
* **The 'Media Rule':** Notification to prominent media outlets is required if a breach affects more than **500 residents** of a single state or jurisdiction.
* **Timeline:** Notifications must be sent without unreasonable delay and no later than **60 days** after the breach is discovered or "reasonably should have been known."
* **Key Precedent:** The **2023 GoodRx enforcement action** was the first case brought under this rule, resulting from the unauthorized sharing of health data with advertising platforms.
* **Preemption:** The HBNR **preempts state law** regarding health breach notifications for entities within its scope.

### 5. Consumer Medical Technology (MedTech)
The rapid growth of health-related consumer technology has created a unique regulatory landscape involving the FDA, FTC, and sectoral laws.
* **FDA/FDCA Scope:** Under the Food, Drug, and Cosmetic Act (FDCA), a **'device'** is defined as an instrument, apparatus, or similar article intended for use in the **diagnosis or treatment** of disease.
* **21st Century Cures Act Exclusion:** The Act excludes software functions from the 'device' definition if they are **'low risk'** to patient safety. The FDA categorizes 'General Wellness' products into two exclusions:
    1.  **General Health:** Products that maintain or encourage a general state of health or healthy activity (e.g., a **breathing/relaxation app**, sleep trackers, or weight management tools).
    2.  **Disease Association:** Products that associate a healthy lifestyle with helping to reduce the risk or impact of a chronic disease, provided they do not offer specific treatment advice.
* **Cybersecurity Requirements:**
    *   **Post-Market Plans:** For **'cyber devices'** (internet-connected), manufacturers must submit a plan to monitor and address post-market vulnerabilities.
    *   **Sept. 2023 Guidance:** The FDA issued final guidance emphasizing that cybersecurity is a critical part of a device's "safety and effectiveness" reviews.
* **State-Level Regulatory Framework:**
    *   **Consumer Fraud:** State Attorneys General use **"Little FTC Acts"** to prosecute health apps for misleading privacy practices or false claims.
    *   **Genetic Data:** Several states (e.g., CA, VA, UT) have enacted laws specifically governing the security and consent requirements for **Direct-to-Consumer (DTC) Genetic Testing** companies.
* **FTC Section 5 Oversight:** Even when HIPAA does not apply, **FTC Section 5** governs MedTech companies. The FTC has specifically prioritized enforcement (notably in 2022) against companies that exploit or improperly share sensitive health and location data.
* **Notice Importance:** Providing **accurate and transparent notice** is paramount in the MedTech sector, as consumers frequently mistake non-HIPAA health applications for services provided by regulated healthcare providers.


# FTC Privacy Enforcement Case Examples (UDTP)

## Unfair Practices (Security Failures)
The FTC uses the **Unfair** standard when a company fails to implement reasonable security measures, leading to substantial consumer injury. (See the [Security Enforcement Section](#7-ftc-security-enforcement--reasonableness) for Wyndham, LabMD, and modern failures like Equifax).

* **DesignerWare:** A rent-to-own company secretly installed spyware on rented computers that captured keystrokes and images. This intrusive monitoring was deemed **unfair**.
* **LifeLock (Security):** The identity theft protection service failed to implement strong security controls for its own customer data, violating its advertising claims and a prior consent decree, resulting in a **$100 million fine**.


## Deceptive Practices (Misrepresentations)
The FTC uses the **Deceptive** standard when a company makes misleading statements or omissions about how it handles, protects, or uses personal data.

* **GeoCities (1999):** The **first** privacy enforcement action based on web-based promises. The company **resold personal information** after promising not to do so.
* **Eli Lilly & Co. (2002):** The **first** action where the FTC mandated the creation of a **comprehensive information privacy and security program** after the company accidentally leaked the email addresses of 600 users.
* **Everalbum, Inc. (2021):** Introduced **Algorithmic Disgorgement**, a remedy requiring the deletion of algorithms or models developed using improperly obtained data (specifically from facial recognition features).
* **Facebook:** Charged with making deceptive claims about users' ability to control privacy, specifically allowing app developers access to user information even when users restricted access. This led to a large fine for violating a previous consent decree.
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
  
### 2. Privacy Programs and Organizational Roles

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

## 6. Vendor Management

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

## FTC-Enforced Statutes (COPPA & Teens)
The FTC lead agency for broad consumer protection in the private sector, but it also has specific enforcement authority over several key privacy statutes.

* **Children’s Online Privacy Protection Act (COPPA):** Provides special protection for children under 13.
    * **Scope:** Applies to online services (websites, apps, etc.) that are intended for, or knowingly collect data from, children under 13.
    * **Personal Information (2025 Amendments):** Now explicitly includes **government-issued identifiers** and **biometric identifiers** (e.g., fingerprints, facial geometry).
    * **Internal Procedures:** Requires:
        * **Annual security assessments** to identify and remediate risks.
        * Designation of an **oversight employee** accountable for the privacy/security program.
    * **Verifiable Parental Consent (VPC) Methods:** Operators must use one of 7 FTC-approved methods:
        1. **Signed forms** (returned via fax, mail, or electronic scan).
        2. **Credit/Debit card transactions** (providing notification of each transaction to the primary account holder).
        3. **Toll-free telephone number** staffed by trained personnel.
        4. **Video conference** with trained personnel.
        5. **Knowledge-Based Authentication (KBA)** (personalized questions).
        6. **Government-issued ID verification** (checked against databases and then deleted).
        7. **Facial Recognition** (matching a live photo against an ID photo).
    * **Safe Harbor Programs:** Companies can demonstrate compliance by joining self-regulatory programs like **Aristotle**, **iKeepSafe**, and **kidSAFE**.
    * **Requirements:** Requires operators to post a complete **Privacy Policy**, provide **Parental Notification**, obtain **Consent** before collection, and grant parents the right to review/delete data.
* **Future of Enforcement:** Addresses challenges from new technologies like **Big Data**, **Artificial Intelligence (AI)**, **Machine Learning (ML)**, and the **Internet of Things (IoT)**, which enable new business models like data brokers and cross-border data flows.
* **Teen-Specific State Protections (Ages 13–18):**
    * **California Minors "Eraser" Law:** Provides individuals under 18 the right to request removal of information they posted online.
    * **Delaware Online and Personal Privacy Protection Act:** Restricts marketing adult products (alcohol, firearms) to children and offers similar removal rights.
    * **New York Child Data Protection Act (June 2025):** Prohibits processing personal data of those aged 13–18 without informed consent.
* **CCPA Opt-in Requirements:**
    * **Ages 13–15:** Data sale/sharing requires the direct **opt-in consent** of the minor.
    * **Under 13:** Requires verifiable **parental consent**, aligning with COPPA standards.

***

## Medical Privacy
Federal laws provide special protections for personal medical information.

* **Health Insurance Portability and Accountability Act (HIPAA):** Sets standards for the privacy and security of **Protected Health Information (PHI)** and **electronic PHI (ePHI)**.
    * **Scope:** Applies to **Covered Entities** (health plans, clearinghouses, providers) and their **Business Associates** (third parties with access to PHI, bound by **Business Associate Agreements** or BAAs).
    * **"Employment Record" Exclusion:** HIPAA explicitly **excludes** employment records held by a covered entity in its role as an employer. (e.g., A hospital's HR file on its own nurses is *not* PHI under HIPAA, though it may be protected by ADA/state laws).
    * **Privacy Rule:** Governs the **use and disclosure** of PHI, requiring the **minimum necessary** amount of PHI be shared.
        * **Patient Rights:** Includes the right to access the **Designated Record Set** (medical, billing, and enrollment records). Requests must be fulfilled within **30 days**.
        * **Valid Authorizations:** To be valid, a written authorization must include six elements: (1) description of info, (2) identity of the granter, (3) identity of the recipient, (4) purpose of use, (5) expiration date/event, and (6) signature and date.
    * **Security Rule:** Applies only to ePHI, requiring safeguards for confidentiality, integrity, and availability.
        * **Required vs. Addressable:** Controls are either **Required** (must be implemented) or **Addressable** (must assess if reasonable; if not, document why and implement an equivalent alternative).
* **Health Information Technology for Economic and Clinical Health (HITECH) Act (2009):** Promoted Electronic Health Records (EHRs) and strengthened HIPAA.
    * **Key Changes:** Extended HIPAA's direct liability to **Business Associates** and introduced the **Breach Notification Rule**.
        * **Breach Standard:** A breach is **presumed** following an unauthorized use or disclosure unless the entity performs a risk assessment showing a **"low probability"** that PHI was compromised.
        * **Four Mandatory Risk Factors:** Assessments must consider: (1) The nature and extent of the PHI involved; (2) The identity of the unauthorized person who used or received it; (3) Whether the PHI was actually acquired or viewed; and (4) The extent to which the risk has been mitigated.
        * **Exceptions:** Not considered a breach if: (1) Inadvertent, good-faith access by an employee within their scope of authority; or (2) Disclosure where the recipient could not reasonably have retained the information.
        * **Tiered Notifications:**
            * **Individuals:** Must be notified within **60 days** of discovery.
            * **Media:** Must be notified within **60 days** if a breach affects more than **500 residents** of a single state or jurisdiction.
            * **HHS (Secretary):** All breaches must be reported. If >500 individuals are affected, notification must be immediate. If <500, the entity must maintain an **annual log** and report all breaches within 60 days of the end of the calendar year.
        * **Burden of Proof:** The Covered Entity or Business Associate bears the **burden of proof** to demonstrate that all required notifications were made or that the use/disclosure did not constitute a breach.
    * **Enforcement & Penalties:**
        * **DOJ Criminal Penalties (3 Tiers):**
            * *Knowing:* $50,000 fine and up to 1 year in prison.
            * *False Pretenses:* $100,000 fine and up to 5 years in prison.
            * *Malicious/Commercial:* $250,000 fine and up to 10 years in prison.
        * **Max Civil Penalty (2024):** The maximum civil penalty for a violation has been updated to **$2,067,813**.
    * **2021 Safe Harbor Bill:** Added a provision where HHS may mitigate fines or length of audits if "recognized security practices" (e.g., NIST or Cybersecurity Act 405(d) standards) were in place for at least **12 months** prior to the incident.
* **21st Century Cures Act (2016):** Encourages standardized EHRs and addresses data sharing/research.
    * **Research Protections:** Includes **Certificates of Confidentiality** (issued by NIH to prevent the use of research data in legal proceedings without consent) and a **FOIA exemption** for health data in biomedical research.
    * **Remote Access:** Researchers are permitted to remotely view PHI if they maintain appropriate privacy and security standards.
    * **Information Blocking:** Prohibits practices that interfere with access/exchange of ePHI. Penalties can be up to **$1,000,000 per violation**, with the **Inspector General** authorized to investigate claims.
    * **IT Certification & APIs:** Managed via the **ONC IT certification program**; requires developers to publish **APIs** that allow patient data to be accessed and used **"without special effort."**
* **Confidentiality of Substance Use Disorder Patient Records Rule (42 CFR Part 2):** Provides heightened confidentiality for SUD treatment records.
    * **Expanded Scope:** Applies to a **"Part 2 Program,"** which includes any individual or entity that holds itself out as providing SUD services and is federally assisted. This includes specialized units within general medical facilities or staff whose **"primary function"** is SUD diagnosis, treatment, or referral.
    * **Strict Consent Requirements:** Written consent must include: (1) Patient name; (2) Specific Part 2 program making the disclosure; (3) Description of info; (4) Identity of the recipient; (5) Purpose; (6) Revocation statement; and (7) Expiration date (not to exceed what is **"reasonably necessary"**).
    * **Third-Party Redisclosure:** Third parties receiving Part 2 records are strictly prohibited from **"redisclosing"** that information without further patient consent.
    * **Use Restrictions:** Records cannot be used to initiate **criminal charges** or as a predicate for **criminal investigations** against a patient.
    * **Administrative Duties:** Upon request, programs must provide patients with a list of entities that received their info in the past **two years**. Programs must also maintain a **formal security program** for both paper and electronic records.

***

## Financial Privacy
Regulations govern the financial sector, including credit, banking, and insurance.

* **Fair Credit Reporting Act (FCRA) (1970):** The first major federal data privacy law, regulating the collection and use of consumer credit information.
    * **Regulated Entities:**
        *   **Consumer Reporting Agencies (CRAs):** Entities that assemble/evaluate consumer credit info (e.g., Equifax, Experian, TransUnion).
        *   **Users:** Entities that purchase/use reports for decision-making (e.g., banks, employers, landlords).
            *   *Adverse Action Duty:* Any user that takes an adverse action based on a consumer report must provide the consumer with notice. This applies to all permissible purposes (credit, insurance, etc.), not just employment.
        *   **Furnishers:** Entities that provide data to CRAs (e.g., lenders, credit card issuers).
        *   **Red Flags Rule Entities:** Financial institutions and creditors required to implement identity theft prevention programs.
    *   **Definition of 'Consumer Report':** A communication by a CRA bearing on a consumer's: (1) Creditworthiness, standing, or capacity; (2) Character or general reputation; or (3) Mode of living; which is used for a **permissible purpose** (e.g., credit, insurance, employment).
    *   **Investigative Consumer Reports:** A subset of consumer reports where information on character/reputation is obtained through **personal interviews** with neighbors, friends, or associates.
        *   **Notice:** The User must notify the consumer in writing within **3 days** of requesting such a report.
    *   **Obsolescence Rules:** CRAs are prohibited from reporting negative information after a certain period:
        *   **Negative Info/Liens/Lawsuits:** 7 years.
        *   **Bankruptcies:** 10 years.
        *   *Exception:* No time limit for high-value transactions (credit/insurance >$150k, employment >$75k).
    *   **Case Law: *TransUnion LLC v. Ramirez* (2021):** Supreme Court ruled that plaintiffs must demonstrate **"actual concrete harm"** to have Article III standing to sue in federal court. A mere statutory violation or "risk of harm" without material injury is insufficient for damages.
    *   **Enforcement:**
        *   **Penalties:** The **2025 maximum civil penalty** for knowing violations is **$4,983** per violation.
        *   **State Attorneys General:** Have the authority to bring civil actions on behalf of state residents.
        *   **Private Right of Action:** Consumers can sue for **willful** (statutory + punitive damages) or **negligent** (actual damages) noncompliance.
* **Fair and Accurate Credit Transactions Act (FACTA) (2003):** Updated FCRA to combat identity theft, enhance accuracy, and address specific industry concerns.
    *   **The "Vail Letter" Overturn:**
        *   **Standard:** FACTA overturned the FTC's 1999 "Vail Letter," which had classified third-party employee misconduct investigations as "consumer reports."
        *   **Impact:** Employer investigations into suspected misconduct, compliance violations, or written disputes are now **excluded** from the broad definition of consumer reports. Employers do **not** need to notify the employee before the investigation, ensuring the process isn't compromised.
        *   **Adverse Action:** If adverse action is taken based on the report, the employer must only provide a **summary** of the report (not the full report) to the employee.
    *   **Fraud Alerts:** Consumers have the right to place alerts on their files to warn potential creditors:
        *   **Initial Fraud Alert:** Lasts for **1 year**. Can be requested if a consumer suspects they are a victim of identity theft.
        *   **Extended Fraud Alert:** Lasts for **7 years**. Requires the consumer to submit an identity theft report (e.g., police report).
        *   **Active Duty Alert:** Lasts for **12 months**. Available to active military personnel deployed away from their usual duty station.
    *   **Red Flags Rule:** Requires "financial institutions" and "creditors" to have written Identity Theft Prevention Programs containing four mandatory elements:
        1.  **Identify** relevant red flags (patterns, practices, or specific activities).
        2.  **Detect** red flags.
        3.  **Prevent** and mitigate identity theft.
        4.  **Update** the program periodically to reflect changes in risks.
    *   **Red Flag Program Clarification Act of 2010:**
        *   **Clarification:** Passed to narrow the broad definition of "creditor" which unintentionally captured professionals like attorneys and doctors.
        *   **Exclusion:** Excludes "incidental creditors" who merely bill for services after the fact. The rule now chiefly applies to entities that regularly obtain or use consumer reports in connection with a credit transaction or furnish information to CRAs.
    *   **Address Discrepancy Rule:**
        *   **Requirement:** Users of consumer reports must verify a consumer's identity if the CRA provides a **Notice of Address Discrepancy** (indicating a "substantial difference" between the address provided by the user and the address in the CRA's file).
        *   **Actions:** Users must form a "reasonable belief" that the report refers to the consumer.
    *   **Disposal Rule:**
        *   **Scope:** Applies to **any** individual or entity (not just CRAs) that uses a consumer report for a business purpose.
        *   **Standard:** Must take **"reasonable measures"** to protect against unauthorized access to or use of the information in connection with its disposal.
        *   **Methods:** Includes burning, pulverizing, or shredding papers, or destroying/erasing electronic media so that information cannot be read or reconstructed.
* **Gramm–Leach–Bliley Act (GLBA) (1999):** Regulates **financial institutions** (banks, insurers, investment firms).
    *   **Scope Expansion ("Finders"):** Under the **Revised Safeguards Rule**, the definition of "financial institution" was expanded to include **"Finders"**—companies that charge a fee to connect consumers with lenders (e.g., mortgage brokers, payday lenders).
    *   **Key Definitions (Notice Triggers):**
        *   **Consumer:** An individual who obtains a financial product/service for personal use (one-off transaction, e.g., using an ATM). *Notice Requirement:* Only required receives a "short-form" notice IF the institution shares NPI with non-affiliated third parties.
        *   **Customer:** A consumer with an **ongoing relationship** (e.g., mortgage, checking account). *Notice Requirement:* Must receive full privacy notices (**Initial** and **Annual**).
    *   **Privacy Rule (Notices):**
        1.  **Initial Notice:** Provided when the customer relationship is established.
        2.  **Annual Notice:** Provided yearly. *Exception:* Not required if the institution does not share NPI with non-affiliates (preventing opt-out rights) AND practices haven't changed.
        3.  **Revised Notice:** Required if the institution changes its data sharing practices (e.g., adding a new category of third-party sharing).
    *   **Opt-Out Rights:** Consumers must be given the right to **opt-out** of sharing **Non-Public Personal Information (NPI)** with **non-affiliated third parties**.
        *   **Exceptions (No Opt-Out Required):**
            *   **Joint Marketing:** Sharing with non-affiliates to market the financial institution's **own** products (requires a contract).
            *   **Service Providers:** Sharing necessary to process transactions or service accounts.
            *   **Legal/Compliance:** Compliance with laws, subpoenas, or fraud prevention.
    *   **Safeguards Rule (Revised 2021/2023):** Requires a written **Comprehensive Information Security Program**.
        *   **Qualified Individual:** Must designate a **single** qualified individual (employee or external affiliate) to oversee and enforce the security program.
        *   **Written Risk Assessment:** Must periodically evaluate internal/external threats and the **adequacy** of existing safeguards to control those risks.
        *   **Mandatory Testing & Monitoring:** Information systems must be monitored/tested using one of two methods:
            1.  **Continuous Monitoring:** Real-time system scanning.
            2.  **Periodic Testing:** Annual **Penetration Testing** AND Bi-annual (every 6 months) **Vulnerability Assessments**.
        *   **Technical Controls:**
            *   **Encryption:** Mandatory for all NPI held **at rest** and **in transit** over external networks.
            *   **MFA:** Multi-Factor Authentication is required for **any individual** accessing customer information systems.
        *   **Service Provider Management:** Institutions must select providers capable of maintaining appropriate safeguards and require them to do so by **contract**.
        *   **Incident Response Plan (IRP):** Establish a **written** plan designed to promptly respond to security events. It must address:
            *   Goals of the plan.
            *   Internal response processes.
            *   Definition of roles/responsibilities.
            *   External/Internal communications.
            *   Remediation of weaknesses.
        *   **Annual Board Reporting:** The Qualified Individual must report in writing, at least **annually**, to the Board of Directors (or equivalent) on the status of compliance and material matters.
    *   **Pretexting Provisions (GLBA Section 521):**
        *   **Prohibition:** Makes it illegal to obtain or attempt to obtain customer information of a financial institution by **false pretenses** (social engineering).
        *   **Penalties:** Violations can result in criminal penalties (fines and imprisonment).
    *   **2024 FTC Breach Notification:**
        *   **Rule:** Non-banking financial institutions must notify the **FTC** of a data breach.
        *   **Threshold:** Affecting **500 or more** consumers.
        *   **Timeline:** Notification must occur as soon as possible, and no later than **30 days** after discovery.

* **Consumer Financial Protection Bureau (CFPB):** Created by **Title X** of the **Dodd–Frank Act (2010)** to be the central regulator for consumer financial protection.
    *   **Consolidation of Authority:** Assumed rule-making and enforcement power from **7 other federal agencies** (including the FTC, Federal Reserve, and OCC).
    *   **Rule-Making Transition:**
        *   **Regulation P:** The CFPB now administers the GLBA Privacy Rule.
        *   **Regulation V:** The CFPB now administers broad portions of the FCRA.
    *   **Jurisdiction (Supervision & Exam):**
        *   **Banks:** Direct supervision of insured depository institutions with **assets > $10 Billion**.
        *   **Non-Banks:** Supervises mortgage brokers, payday lenders, private student lenders, and "larger participants" in consumer markets.
    *   **UDAAP Standard:** Broad authority to prevent "Unfair, Deceptive, or **Abusive** Acts and Practices."
        *   **"Abusive" Defined:** An act/practice is abusive if it:
            1.  **Materially interferes** with the ability of a consumer to understand a term or condition; OR
            2.  Takes **unreasonable advantage** of a consumer's:
                *   Lack of understanding of the risks/costs.
                *   Inability to protect their interests.
                *   Reasonable reliance on the covered person.
    *   **Enforcement Tools:**
        *   **Civil Investigative Demands (CIDs):** A powerful administrative subpoena power allowing the CFPB to demand documents, written reports, and testimony **before** commencing a legal proceeding.
    *   **Recent Enforcement Trends (2023–2024):**
        *   **"Junk Fees":** Aggressive action against illegal surprise fees (e.g., overdrafts, unexpected service charges).
        *   **Algorithmic Fairness:** Focus on preventing discrimination in automated models used for credit decisions, tenant screening, and home valuations.
*   **California Financial Information Privacy Act (CalFIPA / SB 1):** Provides stricter privacy protections for California residents than federal law.
    *   **Scope:** Applies to financial institutions doing business in California; **"Consumer"** is defined specifically as a **California resident**.
    *   **CalFIPA vs. GLBA:**
        *   **Non-Affiliated Third Parties:** Requires written **Opt-In** consent (GLBA only requires Opt-Out).
        *   **Affiliates:** Requires notice and an opportunity to **Opt-Out** of data sharing (GLBA generally allows affiliate sharing without opt-out, subject to FCRA limits).
    *   **Notice Requirement:** Institutions must use a specific form titled **"Important Privacy Choices for Consumers"**.
        *   **Formatting:** The title must be in at least **16-point bold type**, and the body in at least 14-point type.
    *   **Preemption & The *Gould* Decision:**
        *   **Conflict:** The FCRA generally preempts state laws regarding affiliate information sharing.
        *   **Ruling:** In *American Bankers Association v. Gould*, the 9th Circuit ruled that the FCRA preempts CalFIPA's affiliate sharing rules **only** regarding information that meets the definition of a "consumer report" (creditworthiness). Sharing of non-credit data (e.g., transaction history) among affiliates can still be regulated by CalFIPA.
    *   **Relationship with CCPA/CPRA:**
        *   **Data-Level Exemption:** Personal information covered by CalFIPA is **exempt** from the CCPA/CPRA.
        *   **Entity-Level:** The financial institution *itself* is not exempt; if it collects data outside of the CalFIPA scope (e.g., website visitor data), that data is subject to CCPA.
    *   **Penalties:** Statutory damages of **$2,500** per violation, up to a **$500,000** cap for a pattern of violations.

*   **Online Banking and Government Access:**
    *   **Dodd-Frank Section 1033 ("Open Banking"):**
        *   **Rule (2024/2025):** Grants consumers the right to access their financial data in a machine-readable format and share it with third parties.
        *   **Shift to APIs:** Mandates a transition away from **screen scraping** (risky sharing of login credentials) toward secure, standardized **APIs** for data sharing.
    *   **Right to Financial Privacy Act (RFPA) of 1978:**
        *   **Restricts Federal Access:** Prohibits federal government authorities from accessing bank records without a warrant, subpoena, or specific exception.
        *   **Requirements:** To access records, the government must generally provide:
            1.  A formal written request or **subpoena**.
            2.  **Prior notice** to the customer.
            3.  An opportunity for the customer to challenge the request in court.
    *   **Bank Secrecy Act (BSA) & Anti-Money Laundering (AML):**
        *   **Suspicious Activity Reports (SARs):** Financial institutions must file a SAR for any transaction (>$5,000) that typically involves potential money laundering or violations of law.
        *   **Strict Confidentiality:** The institution is **prohibited** from notifying the customer (or any third party) that a SAR has been filed. This creates a tension with typical transparency principles.
    *   **Know Your Customer (KYC):**
        *   **USA PATRIOT Act:** Section 326 requires financial institutions to implement a **Customer Identification Program (CIP)**.
        *   **Impact:** They must verify the identity of any person opening an account (Name, DOB, Address, SSN). This is a mandatory exception to privacy norms (anonymity is not an option in banking).
    *   **Mobile Banking Risks:**
        *   **SMS/Text Banking:** Often lacks end-to-end encryption; vulnerable to "SIM swapping" attacks where hackers hijack the victim's phone number to intercept 2FA codes.
        *   **Geolocation:** Apps often collect precise location data for "fraud detection" (verifying the user is in a known location), but this creates a rich database of user movements that carries significant privacy risks if breached or sold.

***

## Educational Privacy
The education sector is regulated to protect student academic records.

* **Family Educational Rights and Privacy Act (FERPA) (1974):** The primary federal law protecting the privacy of **student educational records**.
    *   **Authority & Preemption:**
        *   **Spending Clause:** Enacted under Congress's power to condition the receipt of federal funds. It applies to **any** educational agency or institution receiving funding from the U.S. Department of Education (public K-12 and most higher ed).
        *   **Preemption:** FERPA does **not** preempt stricter state laws.
    *   **Key Definitions:**
        *   **"Student":** Any individual who is or has been **"in attendance"**. It explicitly **excludes applicants** who were denied admission.
        *   **"Education Record":** Any record directly related to a student and **"maintained"** by the educational agency.
    *   **Exceptions (Records NOT Covered):**
        1.  **Sole Possession Records:** Private notes (memory aids) kept by a teacher and not shared with anyone.
        2.  **Law Enforcement Unit Records:** Created by a school's internal police unit for law enforcement purposes.
        3.  **Employment Records:** Records of school employees (unless employment is contingent on student status, like a TA).
        4.  **Medical/Treatment Records:** For students 18+ (or in college); these are excluded from FERPA but are generally not covered by HIPAA either (see below).
        5.  **Alumni Records:** Records created after the student has graduated.
        6.  **Peer-Graded Papers:** In ***Owasso v. Falvo* (2002)**, the Supreme Court ruled that peer-graded papers are **not** education records because they are not "maintained" by the school until the teacher collects and records the grade.
    *   **Student Data Subject Rights:**
        *   **Access:** Schools must provide access to records within **45 days** of a request.
        *   **Correction:** Right to request correction of inaccurate/misleading information.
            *   *Process:* Request Amendment -> If denied, Right to **Hearing** -> If denied, Right to place a **Written Explanation** in the file.
    *   **Consent Exceptions (Disclosure w/o Consent):**
        *   **Directory Information:** Information not generally considered harmful if disclosed (Name, address, phone, email, honors, dates of attendance).
            *   *Condition:* School must provide public notice and an opportunity to **opt-out**.
            *   *Restriction:* **Social Security Numbers (SSNs)** and Citizenship Status are **never** directory information.
        *   **School Officials:** With a "legitimate educational interest."
        *   **Health and Safety Emergency:** Disclosure permitted to appropriate parties (parents, police) if identifying a specific threat is necessary to protect the health/safety of students or others.
        *   **Military Recruitment:** Under the **ESEA** (not FERPA directly, but related), high schools receiving federal funds **must** provide access to students' names, addresses, and phone numbers to military recruiters upon request (unless parents opt-out).
    *   **Interaction with Other Laws:**
        *   **FERPA vs. HIPAA:** Health records maintained by a school (e.g., school nurse records, immunization forms) are **Education Records** subject to FERPA, **NOT** HIPAA PHI.
        *   **IDEA:** The *Individuals with Disabilities Education Act* provides additional privacy protections for Special Education records (IEPs).
    *   **Enforcement:**
        *   **Agency:** Family Policy Compliance Office (FPCO) within the Dept. of Education.
        *   **Process:** Complaints must be filed within **180 days**.
        *   **No Private Right of Action:** Students **cannot sue** the school directly for FERPA violations (*Gonzaga University v. Doe*). The remedy is the withholding of federal funds.

*   **Protection of Pupil Rights Amendment (PPRA) (1978):**
    *   **Scope:** Applies to elementary and secondary schools receiving federal funding. Notably, it **does NOT apply to post-secondary (higher) education**.
    *   **Protected Information (The "8 Categories"):** Schools must obtain consent/provide opt-out before asking students about:
        1.  Political affiliations.
        2.  Mental/psychological problems.
        3.  Sex behavior/attitudes.
        4.  Illegal/antisocial/self-incriminating behavior.
        5.  Critical appraisals of close family members.
        6.  Privileged relationships (lawyers, doctors, ministers).
        7.  Religious practices/affiliations.
        8.  Income (unless affecting eligibility for a program).
    *   **Survey Consent Rules:**
        *   **Dept. of Ed Funded Surveys:** Requires **Prior Written Consent (Opt-In)** from parents for surveys asking about the 8 categories.
        *   **Other Federally Funded Surveys:** Requires **Notice** and an opportunity to **Opt-Out**.
    *   **Marketing & Inspection Rights:**
        *   **Instructional Materials:** Parents have the right to **inspect** all instructional materials (textbooks, software) used in the curriculum.
        *   **Commercial Use:** Schools must adopt policies regarding the collection/sale of student info for marketing. Parents must be given the right to **Opt-Out** of such collection.
    *   **Notice & Rights Transfer:**
        *   **Timeline:** Schools must provide **direct annual notice** to parents of these policies at the start of the year.
        *   **Transfer:** Rights transfer from the parent to the student when the student turns **18** or becomes an **emancipated minor**.
    *   **Enforcement:**
        *   **Process:** Complaints filed with the **Student Privacy Policy Office (SPPO)** within **180 days**.
        *   **Liability:** Like FERPA, there is **no private right of action**; the penalty is the potential loss of federal funding.

*   **Education Technology (EdTech):** The rapid adoption of remote learning tools has heightened privacy scrutiny.
    *   **EdTech as "School Officials" (FERPA Exception):**
        *   **Mechanism:** Schools can share student data with third-party vendors (EdTech) *without* parental consent if the vendor meets the **"School Official"** exception.
        *   **Requirements:** The vendor must perform a service the school would otherwise do itself, be under the **direct control** of the school regarding data use, and use the data **only** for the authorized purpose (no re-use).
    *   **FTC COPPA Policy Statement (2022):** Focused on EdTech during remote learning, emphasizing four key compliance areas:
        1.  **Prohibitions:** Bans on mandatory data collection (if not needed for the educational purpose) and using data for commercial advertising.
        2.  **Data Security:** Must implement strong security to protect children's data.
        3.  **Data Retention:** Data should only be kept as long as necessary for the educational intent.
        4.  **Limits on EdTech:** EdTech providers cannot use the "School Official" exception to bypass COPPA's parental consent requirement for *commercial* uses (like building user profiles).
    *   **K-12 School Service Provider Pledge:**
        *   **Nature:** A legally enforceable voluntary code of conduct created by the **Future of Privacy Forum (FPF)** and the **Software & Information Industry Association (SIIA)** (violation is a Section 5 UDAP).
        *   **Core Promises:** Prohibits **selling** student personal information and using it for **behavioral targeting** of advertisements.
    *   **Google Apps for Education Case (2014):**
        *   **Precedent:** Google admitted to scanning student emails in its "Apps for Education" suite for advertising purposes.
        *   **Outcome:** Google stopped the practice after a lawsuit, setting a precedent that **scanning student communications for ad targeting** violates privacy expectations and potentially FERPA/COPPA.
    *   **Intersection with Other Laws:**
        *   **GLBA:** Universities participating in federal student financial aid programs are considered "financial institutions" under GLBA for that specific data (requiring Safeguards Rule compliance).
        *   **State Laws (SOPIPA):** The **Student Online Personal Information Protection Act (SOPIPA)** (California) served as a model for many states, explicitly banning EdTech vendors from selling student data or using it for targeted advertising.

***

## Telecommunications and Marketing Privacy
Laws in this sector regulate how businesses can use personal data for marketing.

*   **Telephone Consumer Protection Act (TCPA) (1991) & Telemarketing Sales Rule (TSR):**
    *   **Regulatory Authority:** TCPA is enforced by the **FCC**; TSR is enforced by the **FTC**.
    *   **2024 TSR Updates:**
        *   **Record-Keeping:** Extends the requirement for telemarketers to retain call records (recordings, scripts, call logs) from 2 years to **5 years**.
        *   **B2B Calls:** Applies strict prohibitions on **misrepresentation** to business-to-business (B2B) calls, which were previously largely exempt.
    *   **Auto-Dialers (ATDS) & *Facebook v. Duguid* (2021):**
        *   **Ruling:** The Supreme Court narrowed the definition of an Automatic Telephone Dialing System (ATDS). To qualify, the equipment must use a **random or sequential number generator**. This excludes equipment that simply dials from a stored list of numbers.
    *   **Call Abandonment Rules:**
        *   **Rate:** Telemarketers must not abandon more than **3%** of answered calls per campaign over a 30-day period.
        *   **Connection:** Live agents must connect within **2 seconds** of the consumer’s greeting.
        *   **Safe Harbor:** If no agent is free, a **prerecorded message** must play (identifying the seller and phone number) to avoid a "dead air" violation.
    *   **Required Disclosures:**
        *   **Prompt Oral Disclosures:** Providing the **Identity of the Seller**, the **Purpose of the call** (sales), and the **Nature of the goods/services**.
        *   **Upselling:** Treated as a separate transaction requiring new disclosures.
    *   **Payment Authorization:**
        *   **Express Verifiable Authorization:** Required for payments *other* than credit/debit cards (e.g., remotely created checks). Must be obtained via **audio recording** or written confirmation.
    *   **Do-Not-Call (DNC) Rules:**
        *   **National Registry:** Sellers must access the registry every **31 days** and scrub their lists.
        *   **Established Business Relationship (EBR) Exception:**
            *   **Transaction:** Lows calls for **18 months** after a purchase/transaction.
            *   **Inquiry:** Allows calls for **3 months** after a consumer inquiry/application.
        *   **DNC Safe Harbor:** A company is not liable for an accidental call if it can prove it meets all **6 requirements**:
            1.  Written procedures.
            2.  Employee training.
            3.  Maintained an internal "do not call" list.
            4.  Accessing the National Registry.
            5.  Monitoring compliance.
            6.  The call was an error.
    *   **Enforcement:**
        *   **Private Right of Action (TCPA):** Consumers can sue directly for **$500 per violation**, or **treble damages ($1,500)** for willful violations.
        *   **Strict Liability:** The TCPA is generally a strict liability statute (intent doesn't matter unless seeking treble damages).
*   **Junk Fax Protection Act (JFPA) (2005):** An amendment to the **TCPA** specifically regulating unsolicited fax advertisements.
    *   **Scope & Exemptions:**
        *   **Market Surveys:** In *Encyclopedia Brown Productions v. HBO*, the Second Circuit ruled that market research surveys **do not** constitute "unsolicited advertisements" if there is no pretext to sell products.
        *   **Online Fax Services:** The FCC has clarified that faxes sent to an **online fax service** (received as email) are treated as **commercial email** (under CAN-SPAM), effectively exempting them from the stricter JFPA rules because they don't consume the recipient's ink/paper.
    *   **Established Business Relationship (EBR):**
        *   **Exemption:** Senders generally cannot send unsolicited faxes *unless* they have an EBR with the recipient.
        *   **Obtaining Numbers:** Unlike the TCPA (calls), for faxes you must also prove the number was obtained via:
            1.  **Voluntary Communication:** Directly from the recipient within the context of the EBR; OR
            2.  **Public Distribution:** From a directory/site where the recipient voluntarily published it for public distribution (e.g., website contact page).
    *   **Opt-Out Notice Requirements:** Every commercial fax must contain a notice that:
        1.  Appears on the **first page**.
        2.  States the recipient is entitled to opt-out.
        3.  Explains the sender must comply with a request within **30 days**.
        4.  Provides a **cost-free, 24/7 mechanism** (phone/website) to opt-out.
    *   **Enforcement:**
        *   **Private Right of Action:** Like the TCPA, allows individuals to sue for **$500 per fax** (trebled for willful violations).
        *   **State AGs:** State Attorneys General can bring suits but must provide **prior written notice** to the FCC (federal preemption consideration).
*   **Controlling the Assault of Non-solicited Pornography and Marketing (CAN-SPAM) Act (2003):** Regulates all **commercial electronic messages** (including email and social media messages).
    *   **Scope & Primary Purpose:**
        *   **Commercial vs. Transactional:**
            *   *Commercial:* Primary purpose is advertisement/promotion. Strict rules apply (opt-out, identification).
            *   *Transactional/Relationship:* Primary purpose is facilitating an existing transaction (e.g., shipping notification, warranty, statements). Uses a **"Transactional"** exemption where only header accuracy rules apply (no opt-out required).
        *   **Mixed Content (Three-Part Test):** If a message contains both commercial and transactional content, the "primary purpose" is commercial if:
            1.  A recipient would reasonably interpret the **subject line** as advertising; OR
            2.  A recipient would reasonably interpret the **body** of the message as advertising (viewed as a whole); generally, transactional content must appear at the **beginning** to avoid this.
    *   **Expanded Requirements:**
        *   **Honesty:** Header info and Subject line must be accurate and not misleading.
        *   **No Opt-Out Fees:** Senders cannot charge a fee or require more than an email address/one page visit to opt-out.
        *   **10-Day Window:** Senders must process and honor opt-out requests within **10 business days**.
        *   **"SEXUALLY-EXPLICIT" Label:** Must be included in the subject line for adult content (initially "ADV:ADLT" was proposed, but now explicit warnings are standard).
    *   **Wireless Rules (Mobile Service Commercial Messages - MSCM):**
        *   **FCC Authority:** The FCC regulates messages sent to mobile domains (e.g., text-to-email).
        *   **Strict Opt-In Requirement:** Unlike standard commercial email (opt-out), MSCMs require **express prior authorization** (oral or written consent) before sending.
        *   **Wireless Domain Registry:** Senders must check the FCC's list of wireless domains to ensure they don't treat mobile messages as standard email.
    *   **Enforcement:**
        *   **FTC:** Primary enforcer; penalties adjusted for inflation (approx. **$53,088 per violation**).
        *   **State Attorneys General:** Can sue for up to **$250 per violation** (capped at **$2 million**).
        *   **Private Right of Action:**
            *   **ISPs:** Internet Service Providers can sue for adverse effects on their networks.
            *   **Consumers:** Have **NO** private right of action.
        *   **Preemption:** CAN-SPAM preempts most state anti-spam laws, **except** those that specifically prohibit falsity or deception in headers/subject lines.
*   **Video Privacy Protection Act (VPPA) (1988):**
    *   **Background:** Enacted after a newspaper published the video rental history of Supreme Court nominee **Robert Bork**.
    *   **Scope:** Applies to "video tape service providers." Courts have expanded this to include **streaming media services** and mobile apps that share viewing history.
    *   **Consent:**
        *   **Standard:** Generally requires **informed, written consent** (at the time of disclosure) to share PII.
        *   **2012 Amendment:** Allows for a **one-time consent** (e.g., for social media sharing) that remains valid for up to **two years**.
    *   **Exceptions (Disclosure Permitted):**
        1.  To the consumer themselves.
        2.  Law enforcement (via **warrant**, grand jury subpoena, or court order).
        3.  Civil court order (with right of prior notice).
        4.  To specific persons for **debt collection**, order fulfillment, or limited marketing (names/addresses only, with opt-out).
    *   **Data Destruction:** PII must be destroyed as soon as practicable, but no later than **one year** from the date usage is no longer necessary.
    *   **Enforcement:**
        *   **Private Right of Action:** Available for unlawful **disclosure** (but generally *not* for failure to destroy data).
        *   **Damages:** Statutory damages of **$2,500** (plus punitive damages/attorneys' fees).
        *   **Limitations:** Two-year statute of limitations.
*   **Cable Communications Policy Act of 1984:**
    *   **Scope:** Applies to "cable operators" providing "cable services" (one-way transmissions). Explicitly **excludes** broadband ISPs.
    *   **Privacy Notices:** Must be "clear and conspicuous," provided at the start of service and **annually** thereafter.
    *   **Collection & Disclosure:**
        *   **Consent:** Requires **prior written or electronic consent** for collecting or disclosing PII.
        *   **Disclosure Exceptions:** (1) Necessary for business activity; (2) Court order (with notice); (3) Name/Address (with opt-out); (4) Criminal law enforcement.
    *   **Subscriber Rights:**
        *   **Access/Correction:** Right to access and correct PII.
        *   **Data Destruction:** Requirement to destroy data when it is no longer necessary for the purpose.
    *   **Enforcement:**
        *   **Private Right of Action:** Provides a **non-exclusive** private right of action (individuals do not have to choose between this and an FCC complaint).
        *   **Damages:** Statutory damages of **$100 per day** of violation or **$1,000**, whichever is higher.
*   **Driver’s Privacy Protection Act (DPPA) (1994):**
    *   **Origin & Constitutionality:**
        *   **Context:** Enacted following the 1989 murder of actress **Rebecca Schaeffer**, whose stalker obtained her address from the DMV.
        *   **Supreme Court Ruling:** In ***Reno v. Condon*** (2000), the Court upheld the DPPA as a valid exercise of Congress's power to regulate **interstate commerce**, rejecting the argument that it violated the 10th Amendment (states' rights).
            *   *Exam Tip:* DPPA is a **Commerce Clause** regulation (interstate commerce). This is a key distinction from laws like **FERPA**, which are based on the **Spending Clause** (conditioning federal funds).
    *   **Scope & Definitions:**
        *   **Personal Information (PI):** Data that identifies an individual (Name, Address, Phone Number, SSN, License Number).
        *   **Highly Restricted Personal Information:** A sensitive subset (Photograph/Image, SSN, Medical/Disability info). Disclosure of this requires express consent unless for very specific government/legal uses.
    *   **Key Exclusions:**
        *   The DPPA does **NOT** protect information regarding **vehicular accidents**, **driving violations**, or **driver's license status** (e.g., active/suspended).
    *   **Permissible Uses (Exceptions):** DMVs may generally disclose PI **only** for specific purposes, including:
        1.  **Government/Law Enforcement:** For carrying out agency functions.
        2.  **Motor Vehicle Safety:** Matters relating to vehicle theft, emissions, and product alterations/recalls.
        3.  **Business Verification:** To verify the accuracy of personal information submitted by the individual to a business (and correct it if wrong).
        4.  **Legal Proceedings:** In connection with any court or arbitral proceeding.
        5.  **Insurance:** For claims investigation and anti-fraud activities.
        6.  **Research:** For statistical/research reports (provided no contact is made with individuals).
        7.  **Private Investigators:** For any permissible use listed.
        8.  **Toll Facilities:** For the operation of toll transportation.
        9.  **Marketing:** Only if the individual has provided **express consent (opt-in)**.
    *   **Enforcement:**
        *   **Civil Action (Private Right of Action):** Individuals can sue for actual damages, but not less than **$2,500 in liquidated damages**, plus punitive damages and attorney's fees.
        *   **Regulatory (Attorney General):** The U.S. Attorney General can fine a State DMV up to **$5,000 per day** for substantial noncompliance.
        *   **Criminal:** Criminal fines apply to individuals who knowingly obtain or disclose information in violation of the Act.
*   **Customer Proprietary Network Information (CPNI) (Telecommunications Act of 1996):** Regulates the privacy of telecommunication subscribers.
    *   **Scope & Definitions:**
        *   **Covered Entities:** Telecommunications carriers and interconnected **VoIP** providers. (Does *not* typically safeguard data held by OTT apps like WhatsApp or device manufacturers).
        *   **Definition:** CPNI is **metadata** about the technical configuration, type, destination, location, and amount of use of a telecommunications service.
        *   **Exclusion:** Distinct from **"Subscriber List Information"** (Name, Address, Phone Number), which is public and not protected as CPNI.
    *   **Use and Disclosure:**
        *   **Rule:** Carriers generally need customer approval to use/share CPNI for marketing.
            *   **Opt-In:** Required for sharing CPNI with **third-party Joint Venture partners** or independent contractors for marketing.
            *   **Opt-Out:** Permitted for affiliates marketing different communication services.
        *   **Exceptions (No Consent Needed):** Billing and collection; Fraud prevention; Customer service; Protecting carrier rights/property; Emergency services (911).
    *   **Safeguards & Certification:**
        *   **Compliance:** Carriers must file an **annual officer certification** with the FCC stating compliance with CPNI rules.
        *   **Training & Records:** Must train employees and retain records of sales/marketing approvals for **1 year**.
    *   **Breach Notification:**
        *   **Timeline:** Carriers must notify Law Enforcement (USSS/FBI) within **7 business days** of discovery.
        *   **Customer Notice:** Cannot notify customers until **after** the law enforcement notification period has passed (to avoid compromising investigations).
    *   **Enforcement & Preemption:**
        *   **Choice of Action:** A person may file a complaint with the FCC **OR** bring a private lawsuit in district court (but not both).
        *   **Preemption:** The Act does **not** generally preempt stricter state privacy laws.

### Webtracking Technologies
* **Web Cookies (HTTP Cookies):** Small text files placed on a device's hard drive by a web server to "save state" (e.g., login status, language preferences).
    * **Types of Cookies:**
        * *Session:* Temporary; deleted when the browser closes.
        * *Persistent:* Remain until a pre-defined expiration date; used for authentication.
        * *First-Party:* Set by the web server of the visited site.
        * *Third-Party:* Set by another party (e.g., an ad network) to track activity across different sites.
        * *Flash (Zombie) Cookies:* Stored outside browser control via Adobe Flash; difficult to delete and can "respawn" deleted standard cookies.
* **Other Tracking Methods:**
    * **Web Beacons (Pixels):** Invisible 1x1 images that record visits and can place cookies or log HTTP request header data (OS, URL, etc.).
    * **Digital Fingerprinting:** Identifying a device based on a unique combination of browser settings, IP addresses, and hardware information.
    * **URL Rewriting:** Redirecting a user through a tracking link (e.g., "t.co") before sending them to the destination to record the interaction.
    * **Cross-Device Tracking:** Mapping users as they move between devices (e.g., phone to laptop).
        * *Deterministic:* Based on user logins to the same service.
        * *Probabilistic:* Based on algorithms and behavioral patterns.
* **Legal Standards:**
    * **E.U. Cookie Directive:** Requires informed consent for cookies unless they are "strictly necessary" (e.g., security) or solely for communication transmission.

### Digital Advertising and Behavioral Tracking
A complex ecosystem regulated primarily by self-regulation and FTC enforcement.

#### Federal Landscape
*   **No Specific Federal Law:** There is currently no federal statute explicitly regulating behavioral advertising. The FTC essentially regulates this space using its **Section 5** authority (unfair/deceptive acts).
*   **FCC Classification Saga:**
    *   **2016:** The FCC reclassified broadband as a public utility ("common carrier"), subjecting ISPs to CPNI-style privacy rules (opt-in for web browsing history).
    *   **2018:** The FCC (under new leadership) reversed this, restoring FTC jurisdiction and removing the strict opt-in requirements for ISPs.

#### State-Level Regulation
*   **California "Do-Not-Track" (DNT) Law (CalOPPA Amendment):** Does not *mandate* honoring DNT signals, but requires websites to **disclose** how they respond to them.
*   **Age-Appropriate Design Code Act (AADC):** (California) Prohibits profiling children for targeted advertising and restricts the use of **"dark patterns"** to encourage kids to provide personal info.

#### Self-Regulation (DAA & NAI)
The industry relies heavily on self-regulatory frameworks to avoid stricter federal legislation.

*   **Digital Advertising Alliance (DAA):**
    *   **The 7 Principles:**
        1.  **Education:** Educate consumers about behavioral advertising.
        2.  **Transparency:** Clear notice of data collection practices.
        3.  **Consumer Control:** Provide mechanisms to opt-out.
        4.  **Data Security:** Reasonable security measures.
        5.  **Material Changes:** Requires **consent** before applying material changes to data collection/use policies.
        6.  **Sensitive Data:** Stricter rules for health/financial data.
        7.  **Accountability:** Enforcement by the BBB and DMA.
    *   **AdChoices Icon:** The "blue triangle" icon on ads that links to privacy controls.

*   **Network Advertising Initiative (NAI):**
    *   **The 6 Code Principles:**
        1.  **Education:** Collective effort to inform the public.
        2.  **Transparency/Notice:** Clear disclosure of profiling activities.
        3.  **User Control:** Robust opt-out mechanisms.
        4.  **Use Limitations:** Restrictions on how data is used.
        5.  **Transfer Restrictions:** Limits on sharing with non-compliant third parties.
        6.  **Data Access & Security:** Ensuring data integrity and limiting access.
    *   **Membership:** Requires public representations of compliance (making failure to comply an FTC Section 5 violation).

#### Enforcement
*   **Self-Regulatory but Binding:** While joining the DAA/NAI is voluntary, failing to adhere to their principles after publicly committing to them constitutes a **Deceptive Trade Practice** under **FTC Section 5**.

### Data Ethics and Dark Patterns
As privacy laws evolve, the focus is shifting from "what is legal" to "what is ethical," particularly regarding user interface design.

#### Data Ethics Frameworks
*   **World Federation of Advertisers (WFA):** Defines 4 key themes for data ethics—**Respect**, **Fairness**, **Accountability**, and **Transparency**.
*   **Information Accountability Foundation (IAF):** Proposed 9 principles for ethical data use, emphasizing that data use must be beneficial to the individual and society.
*   **The Trust Dividend:** Studies show a tangible economic incentive: a **1% increase in customer trust** correlates to a **~3% increase in company value**.

#### Dark Patterns (U.S. Enforcement)
Regulators are increasingly targeting "dark patterns"—user interfaces designed to trick or manipulate users into making choices they didn't intend.
*   **Legal Basis:** Prosecuted as **"unfair or deceptive acts"** under **FTC Section 5**.
*   **Key Enforcement Actions:**
    *   **Epic Games (2022):** Settled for **$520 million** for using design tricks (like counterintuitive button placement) to induce unintended purchases and locking accounts of users who disputed charges.
    *   **Intuit (2022/2024):** Settled for **$141 million** for deceiving users into paying for tax services that should have been free (steering them away from the IRS Free File program).
*   **"Click-to-Cancel" (Negative Option Rule):** Updated FTC rule requiring that canceling a subscription must be **as easy as signing up** ("easy in, easy out").

#### International Context
*   **Digital Services Act (DSA Article 25):** The EU explicitly **bans** online platforms from using dark patterns to manipulate users.
*   **GDPR Interplay:** Dark patterns violate the GDPR's requirement that consent be **"freely given"**.
    *   *EDPB Guidelines 3/2022:* Specifically address deceptive design patterns in social media interfaces.

#### Data Ethics & AI
*   **Edge of Innovation:** Ethical considerations are most critical when operating at the "edge of innovation" where laws haven't caught up, particularly in **AI/ML datasets** and **third-party data sharing**.

### Mobile and IoT Device Surveillance
Beyond web tracking, mobile and Internet of Things (IoT) devices present unique surveillance risks due to their constant connectivity and sensory capabilities.

#### Mobile Device Risks
* **Always-On Sensors:** Microphones and cameras can be utilized for illicit eavesdropping or legitimate mobile assistants (e.g., "Hey Siri").
* **Broad Data Collection:** These devices store intimate details, including contacts, video, and audio recordings, often shared with a vast ecosystem of third-party applications.

#### Internet of Things (IoT)
* **Ubiquitous Computing:** Also known as pervasive computing, this is where information processing is integrated into everyday objects and activities, appearing to be everywhere at all times.
* **Privacy Intrusiveness:** IoT devices (smart TVs, wearable fitness trackers) provide a constant stream of behavioral data, often from within the private environment of a home.
* **Consent Challenges:** Many IoT devices lack a user interface, making traditional notice and informed consent difficult or "theoretical" rather than a real alternative for the user.
* **Security & Attack Surface:**
    * **Large Attack Surface:** Multiple connected devices in a single household create numerous entry points for hackers.
    * **Maintenance Issues:** Because of interface limitations, users are less likely to keep IoT software updated, increasing vulnerability.

#### Mitigation and Best Practices
* **Privacy by Design (PbD):** Due to the high risks and lack of user interfaces, PbD is critical during development to ensure security is "front and center."
* **Data Minimization:** Controllers should account for personal data across the entire life cycle, implementing Fair Information Practices even when specific legal rules are absent.
* **Privacy Impact Assessments (PIAs):** Essential for identifying and remediating risks associated with these cutting-edge, pervasive technologies.

### Location Tracking
Location data is personal data under nearly any definition. It is particularly invasive because it can reveal sensitive inferences about an individual's private life, such as religious or political affiliations.

#### Types of Location Tracking
* **GPS (Global Positioning System):** Functional equivalent to the European **Galileo** system. GPS devices **only receive data**; they do not transmit it. An additional transmitter is required to share the location externally.
* **Wi-Fi Tracking:** Routers identify the unique **MAC address** of mobile devices searching for networks. Because Wi-Fi has a limited range, it can pinpoint a device to a specific building or store.
* **Cell Tower Triangulation:** Uses the signal strength and "time of arrival" of messages across multiple towers to calculate a phone's relative location.
* **Bluetooth Beaconing:** A low-energy signal sent from a beacon to a mobile device. This "reverses" Wi-Fi logic—the beacon sends the message and the device receives it.
* **RFID (Radio-Frequency Identification):**
    * **Passive:** No internal power; requires an external reader to activate the chip.
    * **Active:** Contains its own power source and can transmit signals outwardly.
* **Other Sources:** Metadata (Exif) in photos, location-specific search queries, and IP addresses (though IP is considered **unreliable** for precise location due to VPNs and spoofing).

#### Location-Based Services (LBS)
The IAPP defines LBS as services that utilize location information to deliver applications in various contexts (social networking, gaming, advertising).
* **Privacy Risks:** Geolocation is extremely difficult to anonymize.
* **Best Practices:** Due to its invasive nature, **opt-in consent** is the preferred standard for LBS, even when not strictly required by law.

#### Prevention and Control
* **Physical Protections:** RFID signals can be blocked using specialized **blocking sleeves**.
* **User Control:** Users can toggle Wi-Fi and Bluetooth off, though emergency features may still transmit signals even when a device is powered down.

### Web Scraping (Section 5.9)
Extremely relevant in 2026, web scraping sits at the intersection of privacy, property rights, and AI training.

*   **Definition & FIPs:**
    *   **Activity:** Automated extraction of large volumes of data from public websites without the explicit permission of the data controller.
    *   **Privacy Tension:** Violates core **Fair Information Practices (FIPs)**, specifically:
        *   **Purpose Limitation:** Data posted for one reason (e.g., social networking) is scraped for another (e.g., facial recognition training).
        *   **Transparency:** Users are unaware their data is being harvested.
        *   **Data Minimization:** Scrapers often collect "everything" rather than what is needed.
*   **Legal Landscape (CFAA & *Van Buren*):**
    *   **Computer Fraud and Abuse Act (CFAA):** Historically used by companies to sue scrapers for "unauthorized access."
    *   ***Van Buren v. United States* (2021):** The Supreme Court narrowed the CFAA, ruling that accessing information one is **authorized** to see (like public web pages) is **not** a crime, even if the purpose (scraping) violates the Terms of Service.
        *   *Result:* Scraping public data is generally **not** a CFAA violation (though it may be a civil breach of contract).
*   **Selective Enforcement (*hiQ v. LinkedIn*):**
    *   **Finding:** Courts ruled that LinkedIn could *not* use the CFAA to block a competitor (hiQ) from scraping public profiles, suggesting that selective enforcement of anti-scraping bans could be **unfair competition**.
*   **State Law Variations:**
    *   **CCPA/CPRA:** Amended the definition of "publicly available" information to include data from **widely distributed media** and government records (if used for the purpose it was made public). This generally **exempts** public social media posts from CCPA deletion requests, although interpretations vary by state.
*   **Controller Responsibilities:**
    *   **Privacy by Design:** Controllers are expected to implement technical safeguards (CAPTCHAs, rate limiting) to prevent unauthorized scraping.
    *   **Enforcement:** The DPC fined Facebook **€265 million** for failing to prevent a massive scraping incident, establishing that allowing data to be easily scraped is a failure of **security measures**.
*   **AI Training Context (2026):**
    *   **Litigation:** Whether scraping copyrighted or personal data to train Large Language Models (LLMs) constitutes **"Fair Use"** is the central legal battle of the decade.

# Government and Court Access to Private Sector Information Notes

## 🏛️ Constitutional Foundation

### The Fourth Amendment
Protects U.S. citizens from **"unreasonable searches and seizures"** by the government. It safeguards "persons, houses, papers, and effects."

*   **Evolution of the Standard:**
    *   **Physical Trespass Doctrine (1928):** In ***Olmstead v. U.S.***, the Supreme Court originally ruled that wiretapping was *not* a search because there was no physical entry into the home.
    *   **"Reasonable Expectation of Privacy" (1967):** In ***Katz v. United States***, the Court overturned *Olmstead*, establishing that the Fourth Amendment "protects people, not places."
        *   **The Katz Test:** A search occurs if: (1) The individual has a **subjective expectation** of privacy; and (2) That expectation is one that society accepts as **objectively reasonable**.

### Key Digital Privacy Cases
Recent jurisprudence has adapted the Fourth Amendment to modern technology.

*   ***United States v. Jones* (2012):**
    *   **Issue:** Police attached a GPS tracker to a suspect's car without a valid warrant.
    *   **Holding:** Violating a person's physical property (the car) to gather information is a search. It revived the "physical trespass" theory alongside *Katz*.
*   ***Riley v. California* (2014):**
    *   **Issue:** Police searched the contents of a smartphone during an arrest ("search incident to arrest").
    *   **Holding:** A **warrant is required** to search a cell phone. Providing the "digital contents of a life" deserves higher protection than physical objects found in a pocket.
*   ***Carpenter v. United States* (2018):**
    *   **Issue:** Police obtained months of historical **Cell Site Location Information (CSLI)** without a warrant.
    *   **Holding:** Accessing deep, historical location records requires a **warrant**, recognizing that CSLI provides an intimate window into a person's life (associations, religion, politics).

### The Exclusionary Rule
*   **Definition:** Evidence obtained in violation of the Fourth Amendment (i.e., without a warrant or exception) is **inadmissible** in criminal court.
*   **"Fruit of the Poisonous Tree":** This doctrine extends the ban to **secondary evidence** derived from the initial illegal search. If a warrantless wiretap leads to finding physical contraband, the contraband is also excluded.

### The Third-Party Doctrine
*   **The Rule:** Established by ***United States v. Miller* (1976)** and ***Smith v. Maryland* (1979)**.
    *   **Principle:** An individual has **no reasonable expectation of privacy** in information they voluntarily turn over to a third party (e.g., bank records, dialed phone numbers).
    *   **Impact:** The government traditionally only needed a **subpoena** (lower standard), not a warrant, to access business records.
*   **Modern Exception (*Carpenter*):** The *Carpenter* ruling created a significant crack in this doctrine. It held that because cell phones are essential for modern life, sharing location data with a cell tower is **not truly "voluntary,"** and the data is too invasive to lose constitutional protection.

---

## 🚔 Law Enforcement and Privacy

### Access to Financial Data

### Access to Financial Data

*   **Right to Financial Privacy Act (RFPA) of 1978:**
    *   **Scope:** Regulates federal government access to financial records.
        *   **"Customer":** Defined as individuals or partnerships of **5 or fewer** people.
        *   **Exclusion:** Explicitly **excludes corporations** and larger partnerships.
    *   **Permissible Access Methods (5 Exceptions):**
        1.  **Customer Authorization:** Voluntary consent (valid for **3 months**; revocable at any time).
        2.  **Administrative Subpoena:** Issued by a federal agency. Customer has **10 days** (if served in person) or **14 days** (if mailed) to move to quash.
        3.  **Judicial Subpoena:** Issued by a court. Same 10/14-day quash window apply.
        4.  **Search Warrant:** Issued by a judge/magistrate. Notice to the consumer can be delayed up to **90 days** *after* access (unlike subpoenas where notice is prior).
        5.  **Formal Written Request:** Used by agencies without subpoena power.
    *   **Institutional Duties:**
        *   **Certification:** The financial institution must receive a **written certification** of compliance from the government agency before releasing records.
        *   **Reimbursement:** Institutions generally have a right to be reimbursed by the government for costs of assembling/copying records.
    *   **Enforcement:**
        *   **Private Right of Action:** Available against government agencies or financial institutions.
        *   **Damages:** Actual damages, punitive damages (for willful violations), and a **statutory minimum of $100**.
        *   **Statute of Limitations:** **3 years**.

*   **Bank Secrecy Act (BSA) of 1970:** (a.k.a. Currency and Foreign Transactions Reporting Act)
    *   **Scope & Authority:**
        *   **Regulator:** The **Financial Crimes Enforcement Network (FinCEN)** (part of the U.S. Treasury) has authority over the BSA.
        *   **Covered Entities:** Applies to **26 different types** of entities, including banks, securities brokers, telegraph companies, **casinos**, and card clubs.
    *   **Reporting Requirements:**
        *   **Currency Transaction Reports (CTRs):** Must be filed for currency transactions of **> $10,000** (deposits, withdrawals, exchanges).
        *   **Transportation of Monetary Instruments:** Must report transportation of currency/instruments **> $10,000** into or out of the U.S.
        *   **Purchase of Monetary Instruments:** Must maintain logs of purchases of bank checks, drafts, cashier's checks, money orders, or traveler's checks for **$3,000 – $10,000** (inclusive).
        *   **Suspicious Activity Reports (SARs):** Must be filed in 4 situations:
            1.  Suspected criminal violation involving an insider (any amount).
            2.  Suspected criminal violation > $5,000 (suspect identified).
            3.  Suspected criminal violation > $25,000 (suspect unidentified).
            4.  Suspicious activity > $5,000 (potential money laundering/evasion).
            *   **Strict Prohibition:** The financial institution is **strictly prohibited** from notifying the customer that an SAR has been filed (an exception to RFPA notice).
    *   **Record Retention:** Records generally must be kept for **5 years**.
    *   **Enforcement:**
        *   **Civil Penalties:** Fines up to **$25,000** (or the amount of the instrument, capped at $100,000).
        *   **Statute of Limitations:** **6 years**.
    *   **USA PATRIOT Act Impact (2001):** Strengthened the BSA by requiring:
        1.  **Information Sharing:** Facilitated sharing between government and financial institutions.
        2.  **"Know Your Customer" (KYC):** Mandatory **Customer Identification Programs (CIP)** to verify identity (Name, DoB, Address, ID number).
        3.  **AML Program Pillars:** Every institution must have an AML program with 4 pillars:
            *   Internal policies and controls.
            *   Designated compliance officer.
            *   Ongoing employee training.
            *   Independent audit function.

### Access to Communications

### Electronic Communications Privacy Act (ECPA) of 1986
Primary legislation regulating government eavesdropping, divided into three titles.

*   **Title I: The Wiretap Act**
    *   **Scope:** Prohibits the unauthorized interception of "real-time" communications.
    *   **Technical Definitions:**
        *   **Wire Communication:** Must involve the human voice (aural transfer) and travel through wire/cable facilities (e.g., phone call).
        *   **Oral Communication:** "In-person" conversations where there is a reasonable expectation of privacy (e.g., bugging a room).
        *   **Electronic Communication:** Non-voice data, signs, or signals (e.g., email, text logs).
    *   **The 4 Hurdles (Requirements for a Court Order):** Obtaining a wiretap requires a "super-warrant" with four strict criteria:
        1.  **Predicate Crime:** Can only be issued for specific serious crimes (e.g., racketeering, drug trafficking).
        2.  **Particularity:** Must describe the specific location, device, and type of communication to be intercepted.
        3.  **Necessity:** Law enforcement must show that normal investigative procedures have failed or are too dangerous.
        4.  **Minimization:** Must minimize the interception of non-relevant conversations (e.g., stopping recording when the target talks to their spouse about dinner).
    *   **Consent Rules:**
        *   **Federal Rule:** **One-Party Consent** (interception is legal if one party to the call consents).
        *   **State Variation:** Many states (e.g., CA, MA) require **Dual-Consent** (all parties must consent).
    *   **Exception:** **Ordinary Course of Business** exception allows employers/service providers to monitor communications for quality assurance or service maintenance.
    *   **Enforcement:**
        *   **Civil Remedies:** Victims can sue for the *greater* of: (1) Actual damages; (2) **$100 per day** of violation; or (3) **$10,000**.
        *   **Punitive Damages:** Available for willful violations.
        *   **Statute of Limitations:** **2 years**.
        *   **Suing the U.S. Government:** Damages are actual damages or **$10,000** (whichever is greater). Punitive damages and attorney's fees are **NOT** available against the government.

*   **Title II: Stored Communications Act (SCA)**
    *   **Scope & Definitions:**
        *   **Electronic Communication Service (ECS):** A service that provides users the ability to send or receive wire or electronic communications (e.g., Gmail, Telephone, ISP).
        *   **Remote Computing Service (RCS):** A service that provides computer processing or storage services to the public (e.g., Cloud storage, AWS).
    *   **Government Access Standards:**
        *   **ECS Content (<= 180 Days):** Government requires a **Search Warrant** to access ECS messages stored for 180 days or less.
        *   **ECS Content (> 180 Days) & RCS Content:** Technically accessible via **Administrative Subpoena** (with prior notice) or a 2703(d) Court Order.
            *   *Note:* The 6th Circuit (*Warshak*) ruled that a warrant is constitutionally required for **all** email content, making the 180-day rule largely unenforceable.
        *   **Non-Content Records (Metadata):** Accessible via a **Court Order (2703(d))** if the government offers **"specific and articulable facts"** that the info is relevant and material.
        *   **Basic Subscriber Information (BSI):** Name, address, logs, etc., accessible via a simple **Subpoena**.
    *   **Voluntary Disclosure Rules:**
        *   **Content:** Providers are generally **prohibited** from voluntarily disclosing content to the government or third parties.
        *   **Non-Content:** Providers may generally disclose non-content records (metadata) to non-government entities without restriction.
    *   **Exceptions (Disclosure Permitted):**
        *   **Provider Exception:** To protect the rights or property of the provider (e.g., investigating a hack).
        *   **Emergency:** If the provider believes there is an immediate danger of death or serious physical injury.
    *   **Enforcement:**
        *   **Civil Action:** Violations result in actual damages, but with a **statutory minimum of $1,000**.
        *   **Statute of Limitations:** **2 years**.

*   **Title III: Pen Registers and Trap-and-Trace Devices**
    *   **Scope & Definitions:**
        *   **Pen Register:** A device/process that records **outgoing** dialing, routing, addressing, or signaling information (e.g., the phone number dialed).
        *   **Trap and Trace Device:** A device/process that captures the **incoming** electronic or other impulses that identify the originating number/source of a communication.
        *   **Crucial Distinction:** These devices capture **metadata only** (the "envelope"); they are strictly prohibited from collecting the **content** of the communication.
    *   **Legal Standard ("Relevant to an Investigation"):**
        *   **Certification:** The government does **not** need to show probable cause (Warrant) or specific facts (2703(d)). Instead, they must merely **certify** to a judge that the information likely to be obtained is **"relevant to an ongoing criminal investigation."**
        *   **Judicial Role:** If the certification is present, the judge **must** issue the order (they have no discretion to deny it based on merits).
    *   **Time Limits:**
        *   **Order Duration:** Orders are valid for a maximum of **60 days**.
        *   **Extensions:** Can be extended for additional 60-day periods.
    *   **Emergency Provision:**
        *   Law Enforcement can install a pen/trap device **without a prior court order** if there is an immediate danger of death, serious injury, or threat to national security.
        *   **Requirement:** An order must be sought within **48 hours** after installation.
    *   **Provider Obligations:**
        *   **Cooperation:** ISPs/Telecom providers must provide all information, facilities, and technical assistance necessary to complete the trace unobtrusively.
        *   **Gag Order:** Providers are typically ordered **not to disclose** the existence of the pen/trap to the subscriber.
        *   **Immunity:** Providers who cooperate in accordance with a court order are **immune from civil liability**.

* **CLOUD Act (2018):** Amends the SCA to compel U.S.-based companies to provide data stored on servers, regardless of the data’s **physical, overseas location**.
*   **Communications Assistance for Law Enforcement Act (CALEA) (1994):** (a.k.a. the **"Digital Telephony Bill"**)
    *   **Scope:** Applies to **"Telecommunications Carriers."**
        *   **FCC Expansion:** While the act originally excluded "Information Services" (like the early internet), the FCC ruled in 2005 that CALEA applies to **Broadband Internet Access (ISPs)** and **VoIP providers** because they function as replacements for traditional telephone service.
    *   **Design Mandates:** Carriers must design their systems with **"baked-in" surveillance capabilities** that allow law enforcement (with a court order) to:
        1.  Intercept communications unobtrusively.
        2.  Isolate call content and metadata independently.
        3.  **Human Intervention:** Activation of the surveillance capability must generally be controlled by a human employee of the carrier (not remotely by the police).
    *   **Encryption Duty:**
        *   Carriers are required to decrypt communications **only if** they possess the encryption key (i.e., they provided the encryption).
        *   They are **not** responsible for decrypting messages if the user employs their own third-party encryption.
    *   **Enforcement:**
        *   **Civil Penalty:** Fines up to **$10,000 per day** for non-compliance.
        *   **Court Order Test:** A court can order a carrier to adopt a specific surveillance solution only if: (1) No other manufacturer's equipment is available; and (2) The specific solution is **"reasonably achievable"** (considering cost and impact).

---

## 🔒 National Security and Privacy

* In national security, the stakes are higher, often leading lawmakers to grant the government **more power** than for regular law enforcement.

*   ***United States v. U.S. District Court* (1972) ("The Keith Case"):**
    *   **Holding:** The Fourth Amendment's **warrant requirement** applies to government surveillance of **domestic** threats to national security (i.e., the President cannot authorize warrantless wiretaps of domestic groups).
    *   **Significance:** Rejected the idea of unlimited executive power for domestic security and served as the direct precursor/impetus for the enactment of **FISA** in 1978.

### Foreign Intelligence Surveillance Act (FISA) of 1978

*   **Purpose:** Provides a legal framework for the government to track **foreign targets** and agents spying on the U.S. while setting due process and oversight.
*   **The Foreign Intelligence Surveillance Court (FISC):**
    *   **Structure:** Composed of **11 federal district court judges** appointed by the Chief Justice.
    *   **Terms:** Judges serve staggered, non-renewable **7-year terms**. (At least 3 must reside near D.C.).
    *   **Amicus Curiae:** The **USA FREEDOM Act** (2015) introduced a panel of "friends of the court" (privacy advocates/experts) to advise the FISC on novel legal interpretations, adding an adversarial element to the secret proceedings.
*   **Legal Standards:**
    *   **Target:** Must be a "foreign power" or "agent of a foreign power." Surveillance is easier if the target is **not a "United States person"**.
    *   **"Significant Purpose":** The **USA PATRIOT Act** lowered the threshold. The government no longer needs to show that foreign intelligence is the *primary* purpose, only a **"significant purpose"** of the surveillance.
*   **Key Provisions & Amendments:**
    *   **Section 217 (Computer Trespassers):** Allows interception of communications from a "computer trespasser" (hacker) if the **owner of the computer consents** and the interception is relevant to the investigation (no warrant needed).
    *   **Section 702 (FISA Amendments Act of 2008):**
        *   **Scope:** Authorized mass surveillance of **non-U.S. persons located abroad**.
        *   **Collection Methods:**
            *   *Downstream (PRISM):* Collecting stored data (emails/photos) directly from U.S. service providers (Google, Facebook).
            *   *Upstream:* Intercepting data "in transit" as it flows through the internet backbone cables.
        *   **Status:** Renewed in 2024 (Reforming Intelligence and Securing America Act) through **2026**.
    *   **USA FREEDOM Act (2015):** Ended the bulk collection of phone metadata (Section 215) by requiring "specific selection terms" and introduced transparency reports.
*   **Penalties for Misuse:**
    *   **Criminal:** Fines up to **$10,000** and/or imprisonment for up to **5 years**.
    *   **Civil:** Actual damages, punitive damages, and a statutory range of **$100 per day** or **$1,000** (whichever is greater).

*   **National Security Letters (NSLs):**
    *   **Definition:** A type of **administrative subpoena** (issued directly by the FBI without judicial oversight) used to compel the production of records in national security investigations.
    *   **Statutory Basis (Authorized by 4 Laws):**
        1.  **Right to Financial Privacy Act (RFPA):** For financial records.
        2.  **Electronic Communications Privacy Act (ECPA):** For telephone and email transactional records.
        3.  **Fair Credit Reporting Act (FCRA):** For consumer credit agency records (identity/financial institutions).
        4.  **National Security Act:** For financial/travel records of government employees (to detect leaks).
    *   **The Standard (USA PATRIOT Act Section 505):**
        *   **Lowered Threshold:** The Patriot Act removed the requirement for "specific and articulable facts." Now, the FBI need only certify that the information is **"relevant"** to an authorized investigation to protect against international terrorism or spying.
    *   **Gag Orders & Reforms:**
        *   **Secrecy:** NSLs typically prohibit the recipient from disclosing that they have received one.
        *   **2006 Reform:** Allowed recipients to petition a court to **modify or quash** the order/gag order. Secrecy is only required if disclosure would result in danger to life, flight from prosecution, or destruction of evidence.
    *   **Judicial Review:** Recipients have the explicit right to challenge an NSL in federal district court.

*   **Section 215 Orders ("Any Tangible Thing"):**
    *   **Scope:** Allows the FISC (Foreign Intelligence Surveillance Court) to issue an order compelling the production of **"any tangible thing"** (including books, records, papers, documents, and other items) relevant to a foreign intelligence, international terrorism, or clandestine intelligence investigation.
    *   **Use Case:** This widespread authority was the legal basis for the NSA's bulk collection of telephone metadata (later constrained by the USA FREEDOM Act).

### Cybersecurity Information Sharing Act (CISA) of 2015

*   **Purpose:** Incentivizes the **voluntary sharing** of threat intelligence between private entities and the federal government (via DHS) and among private entities by removing legal barriers.
*   **Key Definitions:**
    *   **Cyberthreat Indicator:** Information necessary to describe or identify malicious reconnaissance, intrusion methods, or exploitation techniques.
    *   **Defensive Measure:** Actions taken on an information system to protect rights/property and mitigate known threats.
*   **Privacy Protections (De-identification):**
    *   Entities must possess the **"technical capability"** to scrub data.
    *   **Requirement:** Must remove any personal information (PII) of specific individuals not relevant to the threat *before* sharing.
*   **Liability Protection (Immunity):**
    *   **Scope:** Provides broad immunity from civil/criminal liability for **monitoring** systems and **sharing** indicators in accordance with CISA protocols.
    *   **Immunity Nuance (Exclusion):** Immunity does **NOT** extend to the implementation of **defensive measures** (e.g., "hacking back" or actions that harm another network).
*   **Legal Privileges:**
    *   **Privilege Preservation:** Sharing does *not* waive attorney-client privilege or trade secret protections.
    *   **FOIA Exemption:** Information shared with the government is **exempt** from Freedom of Information Act disclosures.
*   **Government Usage Limits:**
    *   The government can use shared data for cybersecurity, terrorism, or serious violent felonies.
    *   **Restriction:** Data **cannot** be used for regulatory enforcement actions (e.g., antitrust, consumer protection) unrelated to cybersecurity.

---

## 🧑‍⚖️ Civil Litigation and Privacy

*   **Right of Public Access:** Derived from the **First Amendment**, this right ensures that the public and the press have access to government proceedings, most notably **criminal trials** (established in ***Richmond Newspapers, Inc. v. Virginia*** (1980)). This creates a tension between public transparency and individual privacy in court records.

### Compelled Disclosure of Media Information

*   **Background Case Law:**
    *   ***Branzburg v. Hayes* (1972):** The Supreme Court ruled that the First Amendment does **not** create a general "reporter's privilege" to refuse to testify before a grand jury.
    *   ***Zurcher v. Stanford Daily* (1978):** The Court ruled that the Fourth Amendment does **not** protect newsrooms from valid search warrants, even if the journalists are not suspects.
    *   **Legislative Response:** Congress passed the **Privacy Protection Act (PPA) of 1980** to directly overrule *Zurcher* and establish statutory protections.

*   **Privacy Protection Act (PPA) of 1980:**
    *   **The Core Rule:** Law enforcement is generally **prohibited** from using a search warrant to seize materials intended for public dissemination. Instead, they must use a **subpoena** (which allows the journalist to challenge the request in court).
    *   **Protected Categories:**
        *   **Work Product:** Materials created by the journalist (e.g., notes, drafts, mental impressions) in anticipation of communication to the public. (Higher protection).
        *   **Documentary Material:** Materials upon which information is formally recorded (e.g., photos, audio tapes, films) obtained from others.
    *   **Exceptions (When a Warrant IS Allowed):**
        1.  **Probable Cause of Criminality:** If the journalist themselves is suspected of committing a crime (other than just possessing the materials).
        2.  **Imminent Danger:** To prevent death or serious bodily injury.
        3.  **Risk of Destruction:** If giving notice via subpoena would likely result in the destruction of evidence (documents only).
    *   **Enforcement:**
        *   **Private Right of Action:** Victims can sue the government unit.
        *   **Damages:** Minimum liquidated damages of **$1,000**, actual damages, and **reasonable attorney's fees**.
        *   *Note:* The PPA's exclusionary rule is limited; evidence seized in violation of the PPA is **not** automatically excluded from trial (unlike the 4th Amendment exclusionary rule).

### Discovery and E-Discovery (FRCP)
Civil discovery is the pre-trial phase where parties exchange information. It is governed by the **Federal Rules of Civil Procedure (FRCP)**.

*   **Legal Scope (FRCP Rule 26):**
    *   **The Standard:** Parties may obtain discovery regarding any nonprivileged matter that is **relevant** to any party's claim or defense and **proportional** to the needs of the case.
    *   **Proportionality Factors:** Importance of issues, amount in controversy, access to information, and whether the burden outweighs the benefit.
*   **The 5 Primary Discovery Devices:**
    1.  **Requests for Production (RFP):** Demands to inspect/copy documents, ESI (Electronically Stored Information), or tangible things.
    2.  **Depositions:** Sworn out-of-court oral testimony.
    3.  **Interrogatories:** Written questions answered in writing under oath.
    4.  **Requests for Admission:** Written requests to admit the truth of facts (to narrow issues for trial).
    5.  **Subpoenas:** Orders compelling third parties (non-litigants) to testify or produce documents.
*   **E-Discovery Governance:**
    *   **The Sedona Conference:** An influential think-tank whose publications (e.g., *The Sedona Principles*) guide courts on handling **Electronically Stored Information (ESI)**.
    *   **Information Governance:** The holistic approach to managing information assets, balancing value against risk (privacy, security) and cost (e-discovery). Good governance reduces the "data debris" that complicates discovery.
*   **International Conflicts:**
    *   **The Conflict:** U.S. discovery is broad; EU/foreign privacy laws (like GDPR) are restrictive. This creates a "Rock and a Hard Place" scenario for multinationals.
    *   ***Societe Nationale v. U.S. District Court* (1987):** The Supreme Court established a **5-factor balancing test** to determine if U.S. discovery overrides foreign blocking statutes:
        1.  Importance of the documents to the litigation.
        2.  Specificity of the request.
        3.  Origin of the information (U.S. vs. Abroad).
        4.  Availability of alternative means.
        5.  Weighing U.S. interests vs. Foreign national interests.
*   **Privacy in Court Filings:**
    *   **Protective Orders:** Courts can issue orders to protect trade secrets or sensitive information (e.g., "Attorney's Eyes Only" designations).
    *   **FRCP Rule 5.2 (Redaction):** Mandates the redaction of sensitive data in court filings:
        *   **SSN/Tax ID:** Last 4 digits only.
        *   **Birth Date:** Year only.
        *   **Minors:** Initials only.
        *   **Financial Account Numbers:** Last 4 digits only.
    3.  **Collection:** Gathering the preserved records and securely transferring them to legal counsel.
    4.  **Processing:** Converting data to reviewable formats.
    5.  **Review:** Attorneys examine the records to **redact or remove** information that is irrelevant, protected by privilege, or protected by statute.
    6.  **Production and Presentation:** Sharing the finalized information with the opposing parties or court.

## I. Introduction to Workplace Privacy
Workplace privacy in the U.S. is not governed by a single comprehensive law but by a "patchwork" of federal and state statutes, tort law, and contracts. The primary drivers of federal workplace privacy legislation are **antidiscrimination** and **labor rights**, rather than privacy for privacy's sake.

*   **Foundational Legal Sources:**
    *   **Constitutional Law (The "State Action" Requirement):** The Fourth Amendment protects against unreasonable searches, but it requires **"State Action."** Therefore, it protects **government employees** but generally **does not apply** to the private sector.
    *   **Contract Law:** Employment agreements and **Collective Bargaining Agreements (CBAs)** can create or waive privacy expectations.
    *   **Tort Law:** Common law civil wrongs (e.g., intrusion on seclusion, defamation) provide remedies for privacy invasions where statutes don't exist.
    *   **Statutory Law:** Specific federal and state laws (e.g., ADA, FCRA, EPPA) create targeted privacy rights.

### A. Key Regulatory Agencies
* **Federal Trade Commission (FTC):** Regulates background screening via the Fair Credit Reporting Act (FCRA). Under the FCRA, a **consumer report** includes info on an individual's character or general reputation when used to determine eligibility for **"employment purposes."**
* **Consumer Financial Protection Bureau (CFPB):** Shares FCRA enforcement with the FTC; targets background check companies for inaccuracies.
* **Department of Labor (DOL):** Enforces fair labor standards under the **Fair Labor Standards Act (FLSA)** and protects benefits privacy under the **Employee Retirement Income Security Act (ERISA)**. Also administers FMLA and EPPA.
* **Equal Employment Opportunity Commission (EEOC):** Enforces antidiscrimination laws (ADA, ADEA, Title VII, GINA).
    *   **Structure:** Led by **five members** appointed by the President for **five-year terms** (no more than three from the same political party).
    *   **Litigation:** A **General Counsel** (appointed for a 4-year term) oversees litigation.
* **National Labor Relations Board (NLRB):** Protects workers' rights to organize and bargain collectively; regulates employer surveillance that might intimidate union activities.
    *   **Case Examples:**
        *   ***Colgate-Palmolive Co.:*** Ruled that covert video surveillance is a mandatory subject of collective bargaining.
        *   ***Purple Communications, Inc.:*** Restricted an employer's right to monitor/ban union-related emails sent on company systems during non-work hours.
* **Occupational Safety and Health Administration (OSHA):** Established by the **Occupational Safety and Health Act of 1970**. Ensures workplace safety and protects the confidentiality of employee complaints and medical records related to workplace safety.
* **Securities and Exchange Commission (SEC):** Under the authority of the **Securities Exchange Act of 1934**, the SEC requires public companies to disclose **top-level executive salaries** and human capital metrics relevant to investors.

### B. The Nature of the Employment Relationship
*   **"At-Will" Doctrine:** The default rule in the U.S. is that employment is "at-will," meaning employers can hire, fire, or change terms (including privacy-invasive policies) for any reason (unless illegal) or no reason. This grants employers broad authority to structure the workplace.
*   **Modifying the Relationship:**
    *   **Employment Contracts:** Can define specific privacy rights or limits on monitoring.
    *   **Collective Bargaining Agreements (CBAs):** Union contracts often restrict monitoring or require "just cause" for discipline based on surveillance.

## II. U.S. Antidiscrimination Laws
Federal laws restrict the collection and use of personal data to prevent bias.

### A. Key Statutes
*   **Civil Rights Act of 1964 (Title VII):** Prohibits discrimination in hiring, promotion, and termination based on **race, color, religion, national origin, or sex**.
    *   **Disparate Treatment:** Intentional discrimination against an individual based on a protected trait.
    *   **Disparate Impact:** A policy that is facially neutral (unintentional) but falls more harshly on a protected group (e.g., a physical strength test that disproportionately excludes women).
*   **Age Discrimination in Employment Act (ADEA):** Prohibits discrimination against applicants and employees who are **40 years of age or older**.
*   **Pregnancy Discrimination Act (PDA):** Amends Title VII to prohibit discrimination based on **pregnancy, childbirth, or related medical conditions**.
*   **Equal Pay Act of 1963:** Prohibits **wage disparity** based on sex for equal work performed under similar conditions.
*   **Bankruptcy Act:** Prohibits employers from firing or discriminating against an employee solely because they have filed for **bankruptcy**.
*   **Americans with Disabilities Act (ADA):**
    *   Prohibits discrimination based on disability if the person is qualified and can perform essential functions with **reasonable accommodation**.
    *   **Medical Exams:** Pre-employment medical exams are banned before a conditional job offer. Medical info must be kept in separate, confidential files.
    *   **Undue Hardship:** Employers are not required to provide accommodations that cause significant difficulty/expense.
*   **Genetic Information Nondiscrimination Act (GINA):**
    *   **Framework:** Functions by amending existing statutes, including **ERISA** and **HIPAA**. Genetic information is explicitly classified as **PHI** under HIPAA.
    *   **Employment Protections:** Prohibits using genetic info (including family medical history) for hiring, firing, or promotion. Generally prohibits collecting genetic info (exceptions for accidental acquisition, FMLA, wellness programs).
    *   **Health Insurer Restrictions:** Health plans cannot use genetic info for **underwriting** purposes or discriminate based on a **predisposition** to disease.
    *   **Genetic Testing:** Insurers are prohibited from requesting or requiring individuals to undergo genetic tests, except for limited, voluntary research purposes.
    *   **Exam Note:** For CIPP/US purposes, GINA is primary classified under **Workplace Privacy**.

### B. EEOC Enforcement Procedures
*   **Charge Filing:** An individual usually cannot sue immediately; they must first file a charge with the EEOC.
*   **Timeline:** The employer receives notice of the charge within **10 days**.
*   **"Reasonable Cause":** The EEOC investigates to determine if there is reasonable cause to believe discrimination occurred.
*   **Administrative Exhaustion:** A private lawsuit can only be filed **after** the EEOC process is exhausted and the agency issues a **"Right to Sue" letter**.

## III. Privacy Before Employment (Screening)
### A. Automated Employment Decision Tools (AEDT)
Use of AI/algorithms in hiring creates risks of unintentional bias (e.g., facial analysis penalizing certain groups).

1.  **Regional AEDT Regulations:**
    *   **Illinois (Artificial Intelligence Video Interview Act):** Employers must notify applicants that AI analysis is used, explain how it works, and report demographic data to the state (for race/ethnicity).
    *   **Maryland:** Prohibits the use of **facial recognition** during pre-employment interviews unless the applicant signs a specific **waiver**.
    *   **New York City (Local Law 144):** Employers cannot use AEDT for hiring/promotion unless the tool has undergone an **annual bias audit** and the results are publicly summarized. Also requires **10-day advance notice** to candidates.

2.  **Federal Oversight & EEOC Guidance (ADA & AI):**
    *   **Vendor Liability:** Employers are responsible for their use of AI tools, even if the tools are designed/administered by a third-party vendor.
    *   **3 Types of ADA Violations:**
        1.  **Reasonable Accommodation:** Failing to provide an alternative way to be assessed if the AI tool requires abilities the candidate lacks due to disability.
        2.  **"Screening Out":** Tools that unintentionally filter out qualified individuals with disabilities.
        3.  **Medical Inquiries:** Tools that inadvertently ask questions likely to elicit information about a disability (illegal pre-offer).

3.  **Case Example:** ***iTutorGroup, Inc.*** (2022)
    *   **Facts:** The company's hiring software automatically rejected female applicants over 55 and male applicants over 60.
    *   **Outcome:** The EEOC settled for $365,000, enforcing the **ADEA** and highlighting that "checking the box" on software settings can lead to direct liability for algorithmic age discrimination.

*   **National Child Protection Act (1993):**
    *   **Purpose:** Allows state officials to access the FBI’s **National Crime Information Center (NCIC)** database.
    *   **Scope:** Used to screen potential employees/volunteers who will work with children, the elderly, or individuals with disabilities.

### B. Background Screening & The FCRA
Background checks by third parties are usually considered **Consumer Reports** under the FCRA.
* **Employer Obligations (The "Certification" Rule):** Before a CRA provides a report, the employer must certify:
    1.  **Written Notification/Permission:** That they have notified the consumer and obtained written permission.
    2.  **Compliance with Adverse Action:** That they will comply with the statutory adverse action notice requirements if they deny employment.
    3.  **Non-Discrimination:** That the information will **not** be used in violation of any applicable federal or state equal employment opportunity law.
*   **Investigative Consumer Reports:** If interviewing neighbors/associates about character, specific notice of the "investigative" nature is required.
*   **Adverse Action Procedures:** Before taking "adverse action" (e.g., denying a job, promotion, or terminating employment) based on a report:
    *   **Pre-Adverse Action:** The employer must first provide the individual with a copy of the report and a written summary of their rights under the FCRA.
    *   **Final Adverse Action:** If the employer proceeds with the decision, they must then send a formal adverse action notice.
    *   *Note:* See Financial Privacy section for general FCRA adverse action duties.

1.  **State-Specific Screening Laws:**
    *   **California (ICRAA):** The **Investigative Consumer Reporting Agencies Act** imposes stricter rules than the FCRA (e.g., stricter disclosure, right to receive a copy of the report). CA and many other states limit the use of **credit information** for employment decisions.
    *   **Other Restrictive States:** Colorado, Connecticut, Hawaii, Illinois, Maryland, Nevada, Oregon, Vermont, and Washington (plus major cities) have adopted similar laws restricting credit checks or criminal history inquiries.

### C. Other Screening Methods
* **Polygraphs:** The **Employee Polygraph Protection Act (EPPA)** bans most private employers from using lie detectors for pre-employment screening.
    *   **4 Exempt Categories:**
        1.  Government (federal, state, local).
        2.  National defense/security contractors.
        3.  Security services (armored car, alarm, guard) protecting vital facilities.
        4.  Pharmaceutical manufacturers/distributors of controlled substances.
    *   **"Ongoing Investigation" Exception:** Private employers *can* use polygraphs if:
        *   There is a specific economic loss (theft).
        *   The employee had access to the property.
        *   There is **"reasonable suspicion."**
        *   The employer provides a **signed statement** detailing the incident and suspicion.
    *   **Limitation:** A test result **cannot** be the sole basis for an adverse employment action.
* **Drug/Alcohol Testing:** Regulated by a mix of state laws and federal requirements (e.g., DOT). The **Drug-Free Workplace Act** encourages, but doesn't always mandate, testing.
* **Social Media:** Employers often check profiles but risk seeing protected class info (race, religion). Best practice is using a third party to redact protected info.
    *   **Emerging Statutory Trend:** A growing number of states have passed laws **prohibiting employers** from requesting or requiring employees/applicants to disclose their **usernames or passwords** for private social media accounts.

### D. "Ban the Box" and The Fair Chance Act
*   **Concept:** Removal of the checkbox asking about criminal history from initial job applications to prevent automatic disqualification.
*   **Federal Law:** The **Fair Chance to Compete on Jobs Act (Fair Chance Act) of 2019**.
    *   **Restriction:** Prohibits federal agencies and defense contractors from requesting criminal background information **prior to extending a conditional job offer**.
    *   **Implementation:** Final rulemakings were published in September 2023.

## IV. Privacy During Employment (Monitoring)
Employees generally have **no expectation of privacy** using company equipment. To be legally defensible, a formal monitoring policy should include **6 Key Components**:
1.  **Purpose:** Why the monitoring is occurring (e.g., safety, quality control).
2.  **Scope:** Specific conduct/activities being tracked.
3.  **Methods:** How the monitoring is conducted (e.g., video, keystroke logging).
4.  **Records:** Types of records maintained.
5.  **Use:** How those records are utilized and who accesses them.
6.  **Disclosure:** To whom records are disclosed.

### A. Monitoring Technologies
* **Computer/Phone Usage:** Employers own the equipment and can monitor use.
* **Location Tracking:** GPS monitoring of company vehicles/phones is generally permitted, though some states require notice.
* **Biometrics:** Collecting fingerprints/face scans for timekeeping is common. States like IL, TX, and WA have specific laws requiring notice/consent/retention policies.
* **Wellness Programs:** Employers can offer incentives for health programs. Collection of health data must be voluntary and not penalized if opted out (EEOC rules).
*   **Consumerization of IT (COIT) & BYOD:**
    *   **Trend:** Employees using personal devices for work ("Bring Your Own Device") blurs privacy lines.
    *   **Data Loss Prevention (DLP):** Strategies to prevent data breaches (like remote wipe or keystroke logging) must strictly balance security against the employee's **higher expectation of privacy** on personal devices compared to company-owned ones.

### B. Electronic Communications Privacy Act (ECPA)
Regulates interception of wire, oral, and electronic communications.
* **The "Business Purpose" Exception:** Employers can monitor calls/emails if there is a legitimate business reason.
    * *Limitation:* Monitoring must stop if the communication is determined to be personal.
* **Consent:** Monitoring is legal if one party consents (federal law). Some states require all-party consent.
* **Stored Communications Act (SCA):** accessing stored emails (on company servers) is generally easier than intercepting real-time calls, as company ownership usually negates privacy expectations.
*   **State-Specific Notice Laws:**
    *   **Delaware:** Requires both **prior written notice** and **daily electronic notice** (e.g., a login banner) for email/internet monitoring.
    *   **Connecticut:** Requires **prior written notice** informing employees of the types of monitoring that may occur.

### C. Physical and Location-Based Monitoring
*   **Postal Mail:** In the U.S., a business can generally **open all mail** delivered to its address/office, even if it is marked "Personal" or "Private."
*   **Location Tracking (GPS):**
    *   **Vehicle Tracking:** Generally permissible (especially for company-owned fleets) to track the **vehicle**.
    *   **Person Tracking:** Tracking the **individual person** directly (e.g., via a badge or phone app outside of work hours) is widely prohibited without consent (California model).

### D. Investigation of Misconduct
*   **Fairness:** Investigations must be evenhanded to avoid discrimination claims.
    *   **Regulatory Note (EEOC "Reasonable Care"):** Even if an employer has a perfect written policy, they can still be held liable if the specific official assigned to the case fails to conduct an effective investigation of a harassment complaint.
*   **FACTA Amendment:** The Fair and Accurate Credit Transactions Act amended the FCRA so that **misconduct investigation reports** by third parties are **not** treated as standard consumer reports (overturning the *Vail* letter).
    *   **3 Statutory Conditions for Exclusion:**
        1.  **Scope:** Communication must relate to suspected misconduct, compliance with laws, or compliance with employer policies.
        2.  **No Credit Info:** The investigation cannot involve providing information on the employee's **credit worthiness** or credit standing.
        3.  **Limited Sharing:** The report cannot be shared with anyone except the employer/management, government agencies, or self-regulatory bodies (e.g., FINRA).
    *   **Impact on Consent & Disclosure:**
        *   **No Prior Consent:** Employers do *not* need to notify the employee or get permission before starting the investigation.
        *   **Post-Action Summary:** If the employer takes adverse action based on the report, they are **required** to provide the employee with a **summary** of the nature and substance of the communication (though not the full report/sources).

### E. Workplace Torts (Common Law)
*   **Intrusion on Seclusion:** Liability arises if an employer intentionally intrudes into a private area (e.g., bathroom, locker room) in a way that would be **highly offensive** to a reasonable person. **Surveillance** in these private areas is a key risk.
*   **Publicity Given to Private Life:** Liability for publicly disclosing highly sensitive private facts (e.g., medical details) that are not of legitimate public concern.

### F. Health and Leave Privacy (Confidentiality)
*   **FMLA Confidentiality:**
    *   **Rule:** The Department of Labor (DOL) requires that health information obtained for **Family and Medical Leave Act (FMLA)** purposes be kept in a **separate file** from the general personnel file and treated as confidential (similar to ADA).
    *   **Enforcement:** The FMLA provides a **private right of action** for violations. Courts are distinctively split on whether this extends to confidentiality breaches (some say actual harm is needed).
*   **Workers' Compensation:** While laws vary strictly by state, they almost universally require **confidentiality** for employee records related to workplace injuries/claims.
    *   **Interaction with HIPAA:** Workers' Compensation insurers and administrative agencies are generally *not* HIPAA covered entities, but providers treating the injured worker *are*. HIPAA allows providers to disclose PHI to employers/insurers *without authorization* to the extent necessary to comply with Workers' Comp laws.

## V. Privacy After Employment
### A. Termination Procedures
* **Transition Management:** Securely ending the relationship.
* **Access Control:** Immediate revocation of physical (keys, badges) and digital (email, network) access.
* **Administrative Procedures (Data & IP):**
    *   **Personal Devices:** Since physical return of data on personal devices is impossible, employers should request/require written confirmation of data deletion.
    *   **Ongoing Obligations:** Employers should formally remind departing employees of their **continuing confidentiality obligations** regarding trade secrets and intellectual property.

### B. Records Retention
*   **General Rule:** Employers must follow retention schedules for personnel files (performance reviews, disciplinary records, medical info) to comply with laws and prepare for potential litigation (eDiscovery).
*   **FACTA Disposal Rule:**
    *   **Applicability:** Applies to background checks or credit reports kept in a former employee's file.
    *   **Requirement:** Employers must take **"reasonable measures"** to protect against unauthorized access to or use of the information in connection with its disposal (e.g., burning, pulverizing, or shredding papers; destroying or erasing electronic files).

### C. References
* No federal requirement to provide references.
* **Service Letter Acts (e.g., Kansas):**
    *   **Kansas Requirement:** Upon written request from a former employee, employers **must** provide a letter stating the individual's (1) length of employment, (2) job classification, and (3) rate of pay.
* **Defamation Risk:** Employers face liability for **defamation** (libel/slander) if they make false, damaging statements about a former employee.
    *   **Qualified Privilege:** Some states provide employers a "qualified privilege" to give honest references without liability, provided there is no malice.
    *   **Pro-Tip for Exam:** Many employers adopt a **"Neutral Reference" Policy** (confirming only dates of employment and job title) as the standard middle ground to mitigate defamation liability while satisfying verification requests.

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
* **Data Protection Authority (DPA) Powers:** National-level agencies (except Germany, which has 16 state-level DPAs for the private sector) with investigatory, corrective, and advisory authority, including the power to:
    1. Demand records of processing activities and proof of compliance.
    2. Impose temporary bans on data processing.
    3. Require additional data breach notifications.
    4. Order the erasure of personal information.
    5. Suspend cross-border data flows.

#### Data Subject Rights
The GDPR grants extensive rights to individuals, requiring opt-in consent that is clear and distinguishable.
* **Right to Erasure (Right to be Forgotten):** Subjects can demand the deletion of their data.
* **Right to Access:** Subjects can request to know what data is collected and why.
* **Right to Rectification:** Ability to correct inaccurate data.
* **Right to Data Portability:** Right to receive data in a machine-readable format.
* **Right to Object:** Ability to opt-out of processing or direct marketing.
* **Automated Decision-Making:** Restrictions on AI making significant legal decisions about people.
* **Operational Standards for Rights:**
    * **Transparency:** Communications must be concise, transparent, intelligible, and in plain language.
    * **Timeline:** Actions must be taken "without undue delay" and no later than **one month** (extendable by two additional months for complex requests).
    * **Burden of Proof:** If a data subject objects to processing, the controller has the burden to demonstrate "compelling legitimate grounds" that override the subject's interests.

#### GDPR Breach Notification Framework
The GDPR defines a breach more broadly than most U.S. state laws, covering accidental or unlawful destruction, loss, or unauthorized access. It imposes three distinct reporting duties:
1. **Controller-to-DPA:** Must notify within **72 hours** of discovery unless the breach is unlikely to result in a risk to individuals.
2. **Processor-to-Controller:** Must notify "without undue delay" after becoming aware of the incident.
3. **Controller-to-Subject:** Required "without undue delay" only if the breach is likely to result in a **high risk** to the rights and freedoms of individuals.
    * *Exemptions:* Notice is not required if the data was unintelligible (encrypted), the risk was immediately mitigated, or notice would require "disproportionate effort."

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

### **U.S.–EU Data Frameworks**
The history of U.S.-EU data transfer is defined by legal challenges to U.S. government surveillance and the requirement for "essential equivalence" in data protection.

* **Past Agreements (Invalidated):**
    * **Safe Harbor:** The first framework, invalidated by the CJEU in *Schrems I*.
    * **Privacy Shield:** Invalidated by the CJEU in *Schrems II* (2020) because U.S. surveillance laws (like FISA 702) were found to override EU privacy protections.

* **Transfer Impact Assessments (TIA):**
Following *Schrems II*, TIAs became a mandatory procedural requirement for any organization relying on safeguards like SCCs or BCRs.
    * **Note:** A TIA is a **risk assessment step**, not a valid legal transfer mechanism itself.
    * **Purpose:** To verify on a case-by-case basis if the laws of the destination country undermine the protections of the chosen transfer tool.
    * **EDPB 6-Step Roadmap for TIAs:**
        1. **Map all transfers:** Identify data destinations and any downstream transfers.
        2. **Verify transfer tools:** Identify the legal basis used (SCC, BCR, etc.).
        3. **Assess local law:** Determine if destination laws (e.g., U.S. surveillance) impinge on safeguards.
        4. **Adopt supplementary measures:** Implement technical (encryption), organizational, or legal safeguards if gaps are identified.
        5. **Formalize steps:** Document the assessment and measures taken to meet accountability requirements.
        6. **Re-evaluate:** Monitor protection levels and legal developments at appropriate intervals.

* **Current Framework: EU–U.S. Data Privacy Framework (DPF):**
    * **Basis:** Established in 2023 following a new EU adequacy decision.
    * **Enforcement:** U.S. companies self-certify compliance via the Department of Commerce; oversight is handled by the FTC.
    * **Key Requirements:** Participating companies must update privacy policies, provide independent dispute resolution, limit data retention, and ensure third-party accountability.

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
### Multinational Compliance Strategies
* **"Rationalizing" Requirements (Most Restrictive Law Approach):** To manage overlapping global laws, organizations often "key" their data practices to the most restrictive jurisdiction in which they operate, implementing those higher standards globally.
* **Global Cross-Border Privacy Rules (Global CBPR) Forum:** Established in **2022** by the U.S., Canada, Japan, and others to create an international certification system that allows non-APEC members to participate.
* **Legal Compliance Conflicts:**
    * **U.S. Discovery Conflicts:** U.S. court discovery standards often require the disclosure of data that the GDPR prohibits sharing.
    * **The Reasonableness Standard:** U.S. courts and agencies generally review conduct based on whether it was **reasonable under the circumstances**, provided the party made good faith efforts to reconcile the conflicting legal requirements.


> **Pro-Tip for Exam:** If a tool like reCAPTCHA is legally required for site security (e.g., to prevent fraud), but violates EU transfer rules, U.S. courts may view a "good faith effort" to implement supplementary measures (like a TIA) as meeting the reasonableness standard during a discovery dispute.

***

# Privacy in Mergers, Acquisitions, and Divestitures

Corporate transactions introduce significant privacy risks that must be managed throughout the deal lifecycle.

### 1. Pre-Deal Due Diligence
*   **Process:** Similar to third-party vendor vetting but more intensive. The acquiring company must identify the target's privacy risks before assuming liability.
*   **Key Reviews:**
    *   **Data Processing Obligations:** Assessing the target’s compliance with privacy laws (GDPR, CCPA) and its own privacy policies.
    *   **Contracts:** Reviewing cloud contracts and data processing agreements (DPAs) to ensure transferable rights and adequate security measures.

### 2. The Transaction & Controller Change
*   **Asset Transfer:** In many M&A deals, customer lists and databases are key assets being purchased.
*   **Controller Liability:** The transfer of personal data to a new owner (the acquirer) constitutes a **change of controller**. The new controller instantly assumes responsibility for complying with all applicable laws and existing third-party agreements.

### 3. Transition & Integration
*   **Unifying Systems:** Merging legacy databases with new systems creates vulnerability.
*   **Documentation:** Critical to maintain strict accountability and logs during the migration of data to ensure no records are lost or exposed.
*   **Culture Clash:** Integrating teams with different risk appetites and privacy cultures can lead to compliance gaps if not managed via training and policy alignment.

### 4. Post-Integration Assessment
*   **Updated Assessments:** The combined entity is effectively a "new" organization. It requires a fresh **Privacy Impact Assessment (PIA)** to evaluate the new data flows and technologies.
*   **Policy Harmonization:** Privacy notices and internal policies must be updated to reflect the practices of the unified entity.

### 5. Divestitures (Selling Off Units)
*   **Data Separation:** Requires "untangling" shared infrastructure (e.g., HR systems, CRM).
*   **Risks:**
    *   **Data Left Behind:** Failing to completely scrub sensitive data from sold assets (servers/laptops) creates ongoing liability for the seller.
    *   **Ongoing Compliance:** If the seller retains a copy of the data (e.g., for transition services), they remain a controller/processor with continued legal obligations.
