[← Back to Main Menu](../README.md)
| Feature | Opt-In Regime | Opt-Out Regime |
| :--- | :--- | :--- |
| **Definition** | Data processing is **prohibited** unless the consumer explicitly says "Yes." | Data processing is **permitted** unless the consumer explicitly says "No." |
| **Default State** | **Privacy-Protective:** The default is *no collection/sharing*. | **Business-Friendly:** The default is *collection/sharing is allowed*. |
| **Action Required** | Consumer must take an **affirmative action** (e.g., checking a box, signing a form). Silence is **NOT** consent. | Consumer must take action to **stop** the processing (e.g., unchecking a box, clicking "Unsubscribe"). Silence **IS** consent. |
| **Key Examples** | • **COPPA** (Data from kids <13)<br>• **HIPAA** (Use of PHI for marketing)<br>• **GDPR** (General processing)<br>• **FCRA** (Sharing medical info for credit)<br>• **Biometric Laws** (BIPA, CUBI)<br>• **State Laws** (Sensitive Data) | • **GLBA** (Sharing with non-affiliated 3rd parties)<br>• **CAN-SPAM** (Email marketing)<br>• **CCPA/CPRA** (Sale of data for adults)<br>• **FCRA** (Affiliate sharing for marketing)<br>• **State Laws** (Targeted Advertising) |

> **Nuance:** Some laws act as hybrids. For example, **CPRA** is generally **Opt-Out** for data selling/sharing but switches to **Opt-In** for minors (13-16) and uses strict Opt-In for consumers under 13.

### Enforcement Models: Who Can Sue?
Understanding whether a law allows individuals to sue ("Private Right of Action") is critical for assessing liability risk.

| Feature | Private Right of Action (PRA) | Government Enforcement Only (No PRA) |
| :--- | :--- | :--- |
| **Who Brings Suit?** | Individual consumers, employees, or class action attorneys. | Federal agencies (FTC, HHS, OCC) or State Attorneys General. |
| **Damages/Remedies** | **Statutory Damages** (e.g., $500–$1,500 per violation), actual damages, and attorney's fees. | Civil penalties (fines paid to the gov), injunctions, consent decrees, disgorgement. |
| **Litigation Risk** | **High:** Class actions can lead to massive aggregate liability (e.g., Facebook's $650M BIPA settlement). | **Moderate:** Depends on agency priorities (though fines can be large, they are less frequent than class actions). |
| **Key Examples** | • **TCPA** (Robocalls)<br>• **FCRA** (Credit Reporting)<br>• **BIPA** (Biometrics - very strict)<br>• **VPPA** (Video Rentals)<br>• **Cable Comm. Policy Act** | • **FTC Act** (Section 5)<br>• **HIPAA** (Health)<br>• **GLBA** (Financial)<br>• **COPPA** (Children)<br>• **FERPA** (Education) |
| **Special Rules & Caveats** | **CCPA/CPRA:** Limited PRA **only** for data breaches (security failures), NOT for general privacy violations.<br><br>**State UDAP:** Most have a PRA, except **Iowa** (AG enforcement only). | **"Standard of Care":** While HIPAA has no PRA, a plaintiff can sue for "Negligence" in state court and use HIPAA standards to prove the defendant failed to meet the necessary duty of care. |

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
    - **Broader Scope:** Many state UDAP laws expand on Section 5 of the FTC Act by also prohibiting **"unconscionable"** trade practices.
    - **Private Right of Action (PRA):** Every state provides a PRA under their UDAP statute *except for Iowa*. This serves as a critical **gap-filler** for the lack of a federal PRA under the FTC Act.
* **California Privacy Protection Agency (CPPA):** The first dedicated state-level privacy agency in the U.S. (created by CPRA).
    * **Board Independence & Restrictions:** The 5-member board cannot delegate its authority for **rulemaking** or **enforcement resolutions**.
        * *Post-Employment Bans:* Members face a **1-year ban** on working for companies subject to potential enforcement and a **2-year ban** on representing any entity before the board.
    * **Enforcement Lifecycle:**
        1. **Probable Cause Hearing:** The first step is a private hearing requiring at least **30 days' notice**.
        2. **Public Hearing:** If probable cause is found, the matter proceeds to a public hearing under the **California Administrative Procedures Act**.
* **State Departments of Insurance:**
    * Insurance is regulated at the **state level** (not federal).
    *   **NAIC:** The National Association of Insurance Commissioners sets standards (e.g., Insurance Data Security Model Law).
* **Massachusetts Minimum Security Standards (201 CMR 17.00):**
    *   **Overview:** Considered the "gold standard" for state-level data security regulations.
    *   **Scope:** Applies to **any person** (regardless of location) that owns or licenses personal information of a **Massachusetts resident**.
    *   **WISP Mandate:** Requires the implementation of a **Written Information Security Program (WISP)** that notably includes:
        1.  Designating a specific employee to be **accountable** for the program.
        2.  Identifying and assessing risks (internal/external).
        3.  Developing policies for data storage, access, and transportation (e.g., encryption on laptops).
        4.  Imposing disciplinary measures for policy violations.
        5.  Limiting access for terminated employees.
        6.  Overseeing **service providers** (by contract).
        7.  Restricting physical access to records.
        8.  Regular monitoring and reviewing of the program (at least **annually**).
        9.  Documenting responsive actions taken after any incident.
* **California Data Security (AB-1950):**
    *   **Significance:** The **first** state-wide data security law.
    *   **Standard:** Requires businesses to maintain "reasonable security procedures and practices" appropriate to the nature of the information.
    *   **Guidance:** The CA Attorney General has stated that the **CIS Critical Security Controls** represent the *minimum* level of reasonable security.
    *   **Data Disposal:** Requires records to be disposed of by (1) **shredding**, (2) **erasing**, or (3) **modifying** the data to make it unreadable/undecipherable.

### Self-Regulatory Organizations (SROs)
Industry bodies that create and enforce their own privacy standards.
- **Theory of Self-Regulation:**
    - *Benefits:* Utilizes industry expertise, efficient, flexible, and quicker to adapt to technology changes than government regulation.
    - *Critiques:* Can be anti-competitive, enforcement may be lax ("fox guarding the henhouse"), and may lack diverse stakeholder input.
