[← Back to Main Menu](../README.md)
### Comprehensive State Privacy Laws
Several states have enacted GDPR-style comprehensive laws:
* **California (CCPA & CPRA):** The most extensive U.S. law. Includes a private right of action for security breaches, established the California Privacy Protection Agency (CPPA), and protects "sensitive personal information."
    * **Vendor Contracts:** As of Jan 2023, data controllers **must** enter into contracts with *any* third party with whom they share data, featuring specific restrictive provisions.
    * **Opt-out Requirements:** CCPA/CPRA (California) and VCDPA (Virginia) require systems to restrict data sharing with vendors if a consumer exercises their right to **opt-out of data selling or targeted advertising**.
* **Virginia (VCDPA):** Grants consumer rights (access, correct, delete) and requires data protection assessments. Enforced solely by the AG.
* **Colorado (CPA):** Similar rights to Virginia; recognizes "sensitive data" requiring consent.
    *   **Functional Role Determination:** A fact-based determination. If a processor begins determining the "purposes and means" of processing, it legally becomes a controller for that activity.
    *   **Appeals Process:** First state to require an internal appeals process for denied requests (decision mandated within **45 days**).
* **Connecticut (CTDPA):** Follows the Virginia model but with stronger privacy protections and specific exemptions.
* **Utah (UCPA):** More business-friendly with narrower consumer rights.
    *   **Narrower Rights:**
        *   **Right to Delete:** Limited to data provided *directly* by the consumer.
        *   **No Profiling Opt-Out:** The right to opt-out does NOT apply to profiling.
        *   **No Right to Correct:** The only comprehensive law lacking a right to correct inaccurate data.
    *   **2024 Amendments (S.B. 127):**
        *   **Utah Cyber Center:** Created within the Dept. of Government Operations to coordinate state response.
        *   **New Thresholds:**
            *   **AG & Cyber Center:** Must be notified if breach involves **500+** individuals and is used for fraud/ID theft.
            *   **CRAs:** Must be notified if **1,000+** individuals are affected.
* **Florida (FDBR):** Targeted at "Big Tech" with a high revenue threshold ($1B+).
    *   **Record-Keeping Mandates:** While most states require keeping records of deletion requests, **California** and **Minnesota** uniquely require controllers to maintain detailed records of **all processing activities**, modeled after the GDPR.
* **Consent Requirements (Secondary Use & Sensitive Data):**
    *   **Maryland:** Uniquely strict; generally **prohibits** the processing of sensitive data (no consent exception) with only narrow exceptions.
    *   **Secondary Use:** Most states require **Opt-In** consent for processing data for a secondary purpose (different from the original collection purpose).
        *   *Exceptions:* **California, Iowa, Rhode Island, and Utah** do not have an explicit statutory requirement for secondary use opt-in.
* **Oregon, Texas, & Montana:** Recent additions largely following the model of defining controller obligations, consumer rights, and AG enforcement.

### Comparison of Key State Privacy Laws

| State Law | Effective Date | Sensitive Data | Cure Period | Private Right of Action |
| :--- | :--- | :--- | :--- | :--- |
| **California (CCPA/CPRA)** | Jan 1, 2023 | **Opt-Out** ("Limit Use") | Discretionary (Auto 30-day ended '23) | **Yes** (limited to breaches) |
| **Virginia (VCDPA)** | Jan 1, 2023 | **Opt-In** (Consent) | 30 days | No |
| **Colorado (CPA)** | July 1, 2023 | **Opt-In** (Consent) | 60 days (**Ended** 1/1/25) | No |
| **Connecticut (CTDPA)** | July 1, 2023 | **Opt-In** (Consent) | 60 days (**Ended** 1/1/25) | No |
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
    *   **Payment Transaction Exemption:** Uniquely excludes from its scope any processing of personal data that is done **solely** to complete a payment transaction.

*   **Utah (UCPA):**
    *   Must meet **BOTH**: Annual Revenue > **$25 Million** AND one of the following:
        *   Controls/processes personal data of **100,000+** consumers
        *   Derives **>50%** of gross revenue from the sale of personal data AND controls/processes data of **25,000+** consumers

*   **Exceptions & Outliers:**
    *   **Florida:** Only applies if Global Gross Annual Revenue exceeds **$1 Billion** (targeting Big Tech).
    *   **Texas & Nebraska:** Unique in having **NO revenue or volume thresholds** for applicability (broad scope).
    *   **Lower Thresholds:**
        *   **Montana:** 50,000 consumers (or 25,000 + 25% revenue from sale).
        *   **Delaware:** 35,000 consumers (or 10,000 + 20% revenue from sale).

### Subject-Specific Privacy Laws

#### Social Security Number (SSN) Laws
*   **California (Civil Code 1798.85):** Prohibits companies from:
    1.  Publicly posting or displaying SSNs.
    2.  Printing SSNs on access cards (IDs).
    3.  Requiring SSNs for website log-ins (unless accompanied by a password).
    4.  Mailing documents with the SSN visible through the window.
    5.  Sending SSNs over the internet **without encryption**.
    6.  Selling SSNs.
*   **Colorado:** Specifically prohibits **public entities** from issuing a license, permit, or pass that contains the holder's SSN.

#### Health & Genetic Information
* **Washington My Health My Data Act:** Protects non-HIPAA health data; restricts geofencing near healthcare facilities; includes a private right of action.
* **Illinois Genetic Information Privacy Act (GIPA):** Prohibits genetic discrimination in employment and insurance; has a private right of action.
* **Nevada Consumer Health Data Privacy Law:** Similar to Washington's law, protecting health data not covered by HIPAA.
    *   **Geofencing Restrictions (New York):** Specifically prohibits geofencing around healthcare facilities for advertising or profiling, defining the restricted radius as at least **1,850 feet** (approx. 1/3 of a mile).

#### Online Privacy & Children
* **Delaware (DOPPA):** Requires privacy policies for websites/apps; restricts marketing of adult products to children.
    *   **E-Book Protections:** Uniquely regulates the disclosure of information related to the viewing of **e-books**, requiring non-government entities to obtain a court order showing a "**compelling interest**" before disclosure.
* **California Age-Appropriate Design Code:** Requires high privacy defaults and Data Protection Impact Assessments (DPIAs) for services likely accessed by children.
* **New York SAFE For Kids Act:**
    *   **Addictive Feeds:** Prohibits providing "addictive feeds" (personalized algorithms) to minors without **verifiable parental consent**.
    *   **Nighttime Ban:** restricts platform notifications to minors between **12 AM and 6 AM ET**.
* **CalECPA:** Requires warrants for law enforcement to access electronic communications (emails, location data).

#### Biometric Information
* **Illinois (BIPA):** Strict consent requirements for collecting biometrics; includes a private right of action (resulting in major settlements).
    *   **2024 Amendments (Critical Update):** Liability is now limited to **one BIPA violation per person**, overturning prior court interpretations that accrued a separate claim for every single scan/transmission.
    *   **Written Release:** The definition now explicitly includes **electronic signatures**.
* **Washington & Texas (CUBI):** Regulate biometric capture and sale but enforced only by AGs.
* **New York City:** Requires commercial businesses to post signs if tracking biometrics; private right of action.
* **Specific Facial Recognition Prohibitions:**
    *   **Maryland:** Prohibits use in the **hiring process** without applicant consent.
    *   **New York:** Prohibits use in **schools**.
    *   **Vermont / Maine / Virginia:** Various prohibitions on deployment by **law enforcement** or government agencies.

#### AI & Automated Decision-Making
* **Colorado SB 24-205:** Regulates "high-risk" AI systems making consequential decisions (hiring, lending).
* **NYC Local Law 144:** Requires bias audits for AI tools used in hiring/employment.
* **NAIC AIS Governance Guidelines (2023):**
    *   **Requirement:** Reminds insurers that AI use does **not** exempt them from existing unfair trade practice laws.
    *   **Framework:** Calls for a **written AI governance framework** covering the entire AI lifecycle (proposal to retirement).

#### Financial & Data Brokers
* **California Financial Information Privacy Act (CFIPA):** Stricter than federal GLBA; requires opt-in for sharing with unaffiliated third parties.
* **NYDFS Cybersecurity Regulation:** Mandates rigorous security programs for financial institutions in NY (CISO, encryption, MFA).
* **California Delete Act:** Creates a centralized mechanism for consumers to request data deletion from all registered data brokers.
    *   **Audit Requirement:** Beginning in **2028**, data brokers must undergo an **independent audit** every **three years**.
    *   **Penalties:** Failure to comply with a deletion request results in a penalty of **$200 per day** per request.
* **Vermont Data Broker Law (2018):**
    *   **Significance:** The **first** state law specifically regulating data brokers.
    *   **Requirements:** Brokers must:
        1.  **Register annually** with the Secretary of State.
        2.  Disclose their data collection practices, specifically regarding **minors**.
        3.  Disclose opt-out procedures.
        4.  Maintain a **comprehensive information security program**.
        5.  Eliminate fees for credit freezes (pre-dating the federal requirement).

### Marketing Laws
* **UDAP:** State "Unfair and Deceptive Acts or Practices" laws fill gaps in FTC enforcement.
* **Telemarketing:** State laws often impose stricter curfews and registration requirements than federal rules.

# International Privacy Regulation
