[← Back to Main Menu](../README.md)
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
*   **Age-Appropriate Design Code Act (AADC):** (California) Prohibits profiling children for targeted advertising and restricts the use of **"dark patterns"**.
    *   **Enforcement:**
        *   **Notice Period:** The CA Attorney General must provide a **90-day** notice period to a business to allow for compliance before filing a lawsuit.
        *   **Penalties:**
            *   **Negligent Violations:** Up to **$2,500** per affected child.
            *   **Intentional Violations:** Up to **$7,500** per affected child.

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
