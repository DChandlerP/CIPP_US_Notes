[← Back to Main Menu](../README.md)
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
    * **State Codification:** While primarily a private contract standard, states like **Washington** and **Minnesota** have codified PCI-DSS into statute. This grants financial institutions a statutory **cause of action** to sue merchants for reimbursement if a breach occurs due to the merchant's failure to maintain PCI-DSS standards (reasonable care).
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

