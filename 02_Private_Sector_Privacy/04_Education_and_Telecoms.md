[← Back to Main Menu](../README.md)
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
    *   **State Law Preemption Exceptions:**
        *   **General Rule:** FCRA generally preempts state audit laws.
        *   **Credit Report Frequency:** The following 7 states are permitted to allow consumers to request free credit reports more frequently than the federal annual standard: **Colorado, Georgia, Maine, Maryland, Massachusetts, New Jersey, and Vermont**.
        *   **Credit Score usage:** Laws in **California** and **Colorado** regarding the utilization of credit scores were specifically permitted to remain in effect.
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
