[← Back to Main Menu](../README.md)
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
Every state has enacted a data breach notification law. While they share a common structure, specific details and procedural requirements vary significantly.
*   **Historical Context:**
    *   **First:** **California** (SB 1386) was the first state to enact a breach law in **2003**.
    *   **Last:** **Alabama** and **South Dakota** were the last states to enact laws in **2018**, completing the 50-state map.
    *   **California SB-1386 Specifics:**
        *   **Encryption Key Exception:** Notification is triggered even for encrypted data if the **encryption key** was also acquired by the unauthorized party.
        *   **Substitute Notice:** Permitted if the cost of providing notice exceeds **$250,000** OR the number of affected individuals is greater than **500,000**.
*   **Federal Gap-Fillers:** In the absence of a single comprehensive federal breach law, agencies fill the gaps:
    *   **FTC Health Breach Notification Rule (HBNR):** Covers non-HIPAA health data.
    *   **SEC Disclosure:** Publicly traded companies must disclose **"material"** cybersecurity incidents within **4 days** of determination.
*   **Definitions:**
    *   *Breach:* Varies between "unauthorized access" vs. "unauthorized acquisition" (acquisition is a higher threshold and more favorable to business).
    *   *Personal Information (PI):* Typically Name + SSN, Driver’s License, or Financial info. Newer definitions include biometrics, medical info, and username/password combinations.
    *   *Covered Entities:* Most laws apply to any business.
        *   **Georgia Exception:** Uniquely, Georgia's law applies only to **information brokers** and **government agencies**, not to standard commercial entities.
    *   **Notification Timeline Definitions (Pennsylvania SB 696):**
        *   **Discovery:** The suspicion that a breach has occurred.
        *   **Determination:** The verification of reasonable certainty that a breach occurred.
        *   *Rule:* In PA, the notification timeline only begins upon **determination**.
*   **Notification Requirements:**
    *   **Whom to Notify:** Affected residents, state regulators (AGs), and credit reporting agencies (usually if >500-1000 affected).
        *   **The "Texas Provision":** Texas historically requires organizations to notify residents of *any* state that lacks its own data breach law covering the specific event.
        *   **Unique State AG Notification Requirements:**
            *   **Illinois (Public vs. Private):** Under HB 1260, HIPAA-regulated entities must notify the AG within **5 days** of notifying HHS. This requirement uniquely does **not** apply to other private entities in the state.
            *   **South Dakota (Accountability Model):** Entities are exempt from consumer notification if an investigation determines "no likely harm," but they **must still notify the State AG** of this determination.
    *   **Strict Jurisdictional Timelines:**
        *   Most States: "Without unreasonable delay" or 30-60 days.
        *   **Puerto Rico:** Specific strictness—notice must be provided to the **PR Department of Consumer Affairs** within **10 days**, and the Department must make it public within **24 hours**.
    *   **Prohibited Notice Content (Massachusetts):**
        *   While most states generally require a description of the incident, **Massachusetts** strictly **prohibits** including a description of the nature of the breach or the number of affected residents in the specific notice sent to consumers (to prevent further social engineering/targeting risks).
    *   *Encryption:* Historically, encrypted data was exempt. Newer laws amended this safe harbor:
        *   **Tennessee (SB 2005 / SB 547):** Was the first state to remove the absolute safe harbor; now requires notice if the **encryption key** was also compromised.
        *   **Illinois (HB 1260):** Adopted a similar provision triggering notice if the key is **reasonably believed** to have been compromised.

### State Cybersecurity Safe Harbors
*   **Concept:** A "third category" of state security law (beyond "reasonable" or "prescriptive" standards) that uses incentives to encourage better security.
*   **The Incentive:** States like **Ohio, Utah, Connecticut, and Iowa** provide an **affirmative defense** against tort lawsuits (e.g., negligence claims after a breach) if the company can prove its security program reasonably conforms to a recognized industry framework (e.g., **NIST**, **CIS Controls**, **ISO 27001**, **HIPAA**, or **GLBA**).
*   **Variations:**
    *   **Connecticut:** The safe harbor specifically protects against **punitive damages** (not actual damages).
    *   **Iowa:** Requires the cybersecurity program's cost to be appropriate to the risk, but compliance effectively presumes the company was not negligent.

