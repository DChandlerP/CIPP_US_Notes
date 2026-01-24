[← Back to Main Menu](../README.md)
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

*   **Case Study: *City of Ontario v. Quon* (2010):**
    *   **Holding:** The Supreme Court ruled that a police department's search of an officer's pager text messages was reasonable.
    *   **Public Sector Fourth Amendment Application:**
        1.  **Assumed Privacy:** The Court *assumed* (without deciding) that the employee had a reasonable expectation of privacy in the messages.
        2.  **"Legitimate Work-Related Purpose":** Established that a search is reasonable if it is motivated by a legitimate work-related purpose (e.g., auditing usage limits) and is not excessive in scope.
        3.  **No "Least Intrusive Means":** Explicitly **rejected** the argument that the employer must use the "least intrusive means" possible to conduct the search.

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
