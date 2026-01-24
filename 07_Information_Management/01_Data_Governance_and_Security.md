[← Back to Main Menu](../README.md)
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

