[← Back to Main Menu](../README.md)

Before diving into the legal framework, it is important to understand the four broad categories of privacy that U.S. law and the CIPP/US exam cover:

* **Information Privacy:** The claim of individuals to determine for themselves when, how, and to what extent information about them is communicated to others.
    * *Examples:* Financial data, medical records, personal marketing data.
* **Bodily Privacy:** The protection of a person's physical being against invasive procedures.
    * *Examples:* Genetic testing, drug testing, body cavity searches.
* **Communication Privacy:** The security and privacy of mail, telephones, email, and other forms of communication.
    * *Examples:* Wiretapping, opening mail, intercepting email.
* **Territorial Privacy:** Limits on intrusion into domestic and other environments (the "right to be left alone").
    * *Examples:* Home searches, workplace monitoring, video surveillance.

## 1. Personal vs. Non-Personal Information
* **Scope:** U.S. privacy laws generally protect "personal information" (PI) or "personally identifiable information" (PII). Non-personal info is usually not regulated.
* **Key Factor:** The distinction often depends on how easily the data can be associated with a specific person.

### Identified vs. Identifiable
* **Identified Individual:** Someone who can be ascertained with certainty (e.g., via Social Security Number).
* **Identifiable Individual:** Someone who can be indirectly identified through a combination of factors (e.g., combining a city, street address, and gender).
    * *Note:* This is a sliding scale. The more data you combine, the more "identifiable" a person becomes.
    * **IP Addresses:** Historically considered non-personal by U.S. courts, but the FTC increasingly views static IP addresses as identifiable PI.

## 2. Sensitive Personal Information
* Some laws only regulate specific subsets of sensitive data rather than all PI.
* **Examples:**
    * **HIPAA:** Regulates personal health records, not all data held by a facility.
    * **FCRA:** Places tighter restrictions on medical records within consumer reports.

## 3. Privacy-Enhancing Technologies (PETs)
PETs are "technologies whose purpose is privacy". This field is often led by **privacy engineers** who focus on achieving "freedom from conditions" that create problems for individuals during data processing.

### Identifiability and Identifiers
* **Identifiability:** The degree to which data can be directly attributed to an individual.
* **Linkability:** The amount of effort required to link data to a specific individual.
* **Strong Identifiers:** Data that is identifying without additional context (e.g., SSN, Passport #).
* **Weak Identifiers:** General data belonging to multiple people, needed in combination for identification (e.g., height, home address).
* **Quasi-Identifiers:** Data combined with external knowledge to link it to an individual.

### Anonymization & De-Identification Techniques
* **Suppression:** Removing identifying information or values from a data set.
* **Generalization:** Reducing granularity by replacing specific info with more general elements (e.g., removing a house number from an address).
* **Top- and Bottom-Coding:** Grouping the extreme ends of a range into a single category (e.g., income brackets labeled as "< $20,000").
* **Noise Addition:** Replacing actual values with data from the same class to maintain statistical properties while hiding individuals.
* **Anonymity Metrics:** The relative success of these techniques is measured by **k-anonymity**, **l-diversity**, and **t-closeness**.

### Aggregation and Differential Privacy
* **Aggregation:** Using statistics from groups of records rather than individual data.
* **Differential Privacy:** A mathematical framework that introduces "noise" to provide a guarantee of **indistinguishability** and "plausible deniability" for individuals in a dataset.



## 4. Sources of Information
* **Public Records:** (e.g., court filings) - generally less protected.
* **Publicly Available:** (e.g., social media) - broadly accessible.
* **Non-Public Information:** This is the primary focus of privacy protection laws.

## 5. Key Data Roles (GDPR & Industry Standard)
* **Data Subject:** The individual whose information is being processed.
* **Data Controller:** The entity that **decides** how and why data is processed (has the ultimate authority).
* **Data Processor:** The entity that processes data **on behalf of** the controller.
    * *Limit:* Can only do what the controller authorizes.
    * *Synonyms:* "Business Associate" (HIPAA), "Service Provider" (GLBA).

**Key Terminology:**
* **Processing:** Any operation performed on data (collection, storage, deletion, etc.).

* **Fair Information Practices (FIPs/FIPPs)**
    * **Definition:** Principles guiding data collection, storage, and management for fairness, privacy, and security.
    * **Role:** Foundation for data privacy laws/regulations (often not legally binding themselves).

* **US Frameworks**
    * **1973 HEW Report:** First US articulation. Five principles: no secret records, individual access, limit secondary use, correction rights, data reliability.
    * **Privacy Act of 1974:** Codified FIPs for federal agencies.
    * **2012 White House Report:** Proposed "Consumer Privacy Bill of Rights" (individual control, transparency, accountability).
    * **2012 FTC Report:**
        * **Privacy by Design:** Build privacy in at development stage.
        * **Simplified Consumer Choice:** Meaningful options (e.g., Do-Not-Track).
        * **Transparency:** Clear notices and access.

* **International Frameworks**
    * **OECD Guidelines (1980):** Eight principles (Collection Limitation, Data Quality, Purpose Specification, Use Limitation, Security Safeguards, Openness, Individual Participation, Accountability).
    * **Council of Europe Convention 108 (1981):** Binding agreement requiring FIPs in domestic law.
    * **Madrid Resolution (2009):** Standards for transborder data flow (Lawfulness, Purpose Specification, Proportionality, Data Quality, Openness, Accountability).

* **Common Themes**
    * **Individual Rights:**
        * **Notice:** Informing consumers of practices.
        * **Consent:** Control over data use (Opt-in/Opt-out).
        * **Access:** Right to view/correct data.
    * **Organizational Management:**
        * **Security Controls:** Physical, technical, administrative safeguards.
        * **Data Quality:** Accuracy, completeness, relevance.
        * **Collection/Use Limits:** Data minimization and retention limits.
        * **Accountability:** Monitoring, training, and assigning responsibility.


## 6. The Accountability Principle
The **Accountability Principle** dictates that organizations must take responsibility for protecting personal information and be able to *demonstrate* that compliance to stakeholders.

* **Core Requirement:** Organizations must implement appropriate technical and organizational measures to ensure and demonstrate that data handling complies with relevant laws.
* **Demonstrating Compliance:** This requires significant documentation, such as recording attendance at all employee training events.
* **Responsibility Shift:** The ultimate responsibility for legal compliance lies with the organization (data controller), *not* government regulatory authorities.
* **Flexibility:** How an organization realizes accountability is inherently flexible, allowing them to determine the best means to meet obligations based on their specific processing activities.
* **GDPR Influence:** Under Article 5 of the GDPR, the data controller is expressly responsible for, and must be able to demonstrate compliance with, the other principles of the regulation.

---
# 1. Branches of U.S. Government

The U.S. federal government operates on a system of checks and balances with three coequal branches.

### Legislative Branch (Congress)
* **Role:** Creates new laws and revises existing ones.
* **Source of Power:** **Article I** of the U.S. Constitution (*Article I powers*).
* **Check on Executive:** Holds the **power of the purse** (controls spending) and the power of **impeachment** (requires a majority vote in the House and two-thirds conviction in the Senate).
* **Composition:**
    * **House of Representatives:** 435 voting members, based on population, elected to two-year terms.
    * **Senate:** 100 voting members (two per state), elected to six-year terms.

### Executive Branch (President, Departments, Agencies)
* **Role:** Carries out and enforces the laws created by the legislative branch.
* **Source of Power:** **Article II** of the U.S. Constitution (*Article II powers*).
* **Check on Legislative:** **Veto power** over bills passed by Congress (Congress can override with a two-thirds majority in both houses). The power to enforce (or decline to enforce) laws.

### Judicial Branch (Federal Court System)
* **Role:** Interprets the meaning of laws, resolves disputes, and determines constitutionality.
* **Source of Power:** **Article III** of the U.S. Constitution.
* **Check on Legislative & Executive:** **Judicial review**—the power to strike down laws or practices that conflict with the U.S. Constitution.
* **Court Structure (Lesser to Greater Superiority):**
    * **U.S. District Courts:** The trial courts of the federal system.
    * **U.S. Circuit Courts of Appeal:** Intermediate courts that accept cases on appeal from District Courts; decisions are binding only within their geographic circuit.
    * **U.S. Supreme Court:** Highest court; decisions are final and binding on all inferior courts. Determines which cases to accept through *certiorari*.

---

## 2. Sources of Law
Laws in the United States come from a variety of sources:
