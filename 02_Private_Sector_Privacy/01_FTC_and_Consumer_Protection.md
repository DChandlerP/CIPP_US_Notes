[← Back to Main Menu](../README.md)
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
