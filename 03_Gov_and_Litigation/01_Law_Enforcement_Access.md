[← Back to Main Menu](../README.md)
    *   **CalFIPA vs. GLBA:**
        *   **Non-Affiliated Third Parties:** Requires written **Opt-In** consent (GLBA only requires Opt-Out).
        *   **Affiliates:** Requires notice and an opportunity to **Opt-Out** of data sharing (GLBA generally allows affiliate sharing without opt-out, subject to FCRA limits).
            *   *Nuance:* This applies when sharing between affiliates that are **NOT in the same line of business** (insurance, banking, securities) and are regulated by a **different functional regulator**.
    *   **Notice Requirement:** Institutions must use a specific form titled **"Important Privacy Choices for Consumers"**.
        *   **Formatting:** The title must be in at least **16-point bold type**, and the body in at least 14-point type.
    *   **Preemption & The *Gould* Decision:**
        *   **Conflict:** The FCRA generally preempts state laws regarding affiliate information sharing.
        *   **Ruling:** In *American Bankers Association v. Gould*, the 9th Circuit ruled that the FCRA preempts CalFIPA's affiliate sharing rules **only** regarding information that meets the definition of a "consumer report" (creditworthiness). Sharing of non-credit data (e.g., transaction history) among affiliates can still be regulated by CalFIPA.
    *   **Relationship with CCPA/CPRA:**
        *   **Data-Level Exemption:** Personal information covered by CalFIPA is **exempt** from the CCPA/CPRA.
        *   **Entity-Level:** The financial institution *itself* is not exempt; if it collects data outside of the CalFIPA scope (e.g., website visitor data), that data is subject to CCPA.
    *   **Penalties:** Statutory damages of **$2,500** per violation, up to a **$500,000** cap for a pattern of violations.
*   **NYDFS Cybersecurity Regulation (23 NYCRR 500):**
    *   **Overview:** Mandates rigorous security programs for financial institutions operating in New York.
    *   **FTC Alignment:** The FTC's 2022 amendments to the **GLBA Safeguards Rule** were specifically designed to incorporate many of the stricter cybersecurity standards first implemented by the NYDFS (e.g., CISO requirement, MFA, encryption).
    *   **NYDFS Cryptocurrency Regulations:**
        *   **BitLicense:** It is unlawful to engage in "any virtual currency business activity" in New York without a **BitLicense**.
        *   **Personal Use Exception:** A broad exception exists for merchants and consumers using crypto for personal/purchase purposes.
        *   **The "Greenlist":** NYDFS maintains a "Greenlist" of pre-approved coins. Entities do not need a separate DFS-approved listing policy to list coins on this Greenlist.

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
    *   **State Telemarketing Prerequisites:**
        *   **Licensing & Bonds:** Over **half of U.S. states** require telemarketers to obtain a **license** or register and post a **surety bond** before calling into that state. This is a critical compliance check often missed by focusing solely on federal law.
    *   **Auto-Dialers (ATDS) & *Facebook v. Duguid* (2021):**
        *   **Ruling:** The Supreme Court narrowed the definition of an Automatic Telephone Dialing System (ATDS). To qualify, the equipment must use a **random or sequential number generator**. This excludes equipment that simply dials from a stored list of numbers.
    *   **Call Abandonment Rules:**
        *   **Rate:** Telemarketers must not abandon more than **3%** of answered calls per campaign over a 30-day period.
        *   **Connection:** Live agents must connect within **2 seconds** of the consumer’s greeting.
        *   **Safe Harbor:** If no agent is free, a **prerecorded message** must play (identifying the seller and phone number) to avoid a "dead air" violation.
    *   **Required Disclosures:**
        *   **Prompt Oral Disclosures:** Providing the **Identity of the Seller**, the **Purpose of the call** (sales), and the **Nature of the goods/services**.
        *   **Upselling:** Treated as a separate transaction requiring new disclosures.
    *   **Call Time Restrictions:**
        *   **Federal Rule:** Calls are permitted only between **8:00 a.m. and 9:00 p.m.** (local time of the recipient).
        *   **Stricter State Laws:** States may impose stricter windows.
            *   *Example:* **Alabama** prohibits telemarketing calls after **8:00 p.m.** and on **Sundays** or public holidays.
    *   **Payment Authorization:**
        *   **Express Verifiable Authorization:** Required for payments *other* than credit/debit cards (e.g., remotely created checks). Must be obtained via **audio recording** or written confirmation.
    *   **Do-Not-Call (DNC) Rules:**
        *   **National Registry:** Sellers must access the registry every **31 days** and scrub their lists.
        *   **State Registries:** While the National Registry is primary, many states maintain their own **separate, state-wide Do-Not-Call registries** that telemarketers must also consult and honor.
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
*   **Anti-Robocall Principles (2019):**
    *   **Initiative:** A set of **eight principles** agreed upon by the attorneys general of all 50 states and major telecom carriers (like AT&T, Verizon, T-Mobile) to combat illegal robocalls.
    *   **Goal:** To protect phone users from illegal calls and make it easier for law enforcement to investigate scams.
    *   **Key Provisions:**
        *   Carriers will offer **free call blocking and labeling** tools.
        *   Implement **STIR/SHAKEN** caller ID authentication to prevent "neighbor spoofing" (calls appearing to be from a local number).
        *   Monitor network traffic for suspicious patterns (high-volume bursts).
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
