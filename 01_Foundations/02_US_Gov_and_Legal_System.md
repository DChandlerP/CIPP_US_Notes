[← Back to Main Menu](../README.md)
Laws in the United States come from a variety of sources:

* **Constitutional Law:** The highest possible source of law; no other law may conflict with it.
    * *Supremacy Clause (Article VI):* Establishes the Constitution as the supreme law of the land.
    * *Privacy Protections:* The word "privacy" does not appear in the text, but protections are derived from:
        * **3rd Amendment:** Prohibition on quartering soldiers (privacy of the home).
        * **4th Amendment:** Protection against unreasonable searches and seizures.
        * **5th Amendment:** Protection against self-incrimination.
        * **14th Amendment:** Due process and liberty clauses.
        * **Penumbra Theory:** A group of rights derived by implication from other explicitly protected rights. In *Griswold v. Connecticut* (1965), the Supreme Court established this mechanism, holding that the "shadows" cast by the **1st, 3rd, 4th, 5th, and 9th Amendments** create "zones of privacy" that protect unenumerated rights, allowing for the recognition of privacy rights despite the word not appearing in the Constitution.
    * *State Constitutions:* Can provide **greater** privacy rights than the federal constitution (e.g., California), but cannot provide less (federal law sets the "floor").

* **Legislation (Statutes):** Laws passed by Congress (federal) or state legislatures.
    * **Preemption:** Federal law generally preempts state law (based on the **Supremacy Clause**).
        * **Express Preemption:** The federal law specifically states it overrides state law (e.g., **CAN-SPAM** expressly preempts most state anti-spam laws).
        * **Implied Preemption:** Courts determine that Congress intended to preempt state law even if not explicitly stated.
        * *Note on the 10th Amendment:* Powers not delegated to the federal government are reserved to the States, allowing for state-level privacy laws (like CCPA) where federal law is silent.
    * Federal laws are compiled in the *U.S. Code*.

* **Administrative Law:** Rules and regulations created by executive branch agencies to implement statutes.
    * *Formal Rulemaking:* Legally binding rules (e.g., HIPAA Privacy Rule) documented in the *Code of Federal Regulations (CFR)*.
    * *Informal Guidance:* Agency reports, speeches, and workshops that interpret law but strictly speaking are not binding.
    * - **Administrative Enforcement Actions:**
    - Considered a "third category of litigation" (alongside civil and criminal).
    - **Adjudication:** Typically litigated before an *Administrative Law Judge (ALJ)* rather than a standard court. ALJ decisions are often subject to appeal in a federal civil court.
    - **Administrative Procedure Act (APA):** The federal statute that acts as the rulebook for these actions (similar to the Federal Rules of Civil Procedure). It governs the process unless a specific statute (like the *FTC Act*) mandates different procedures.

* **Common Law (Case Law):** Legal principles developed over time through judicial decisions rather than statutes.
    * *Stare Decisis:* ("To stand by things decided") The principle that courts should follow prior *precedent* to keep the law stable.
    * *Torts:* Civil wrongs (like negligence or invasion of privacy) often stem from common law.

* **Remedies for Breach:**
        * **Monetary Damages:**
            * *Expectation Interest:* Puts the plaintiff in the position as if the contract had been performed (benefit of the bargain).
            * *Reliance Interest:* Compensates for loss suffered by relying on the contract (puts plaintiff back to pre-contract position).
            * *Restitution Interest:* Prevents unjust enrichment of the breaching party.
        * **Specific Performance:** A court orders the breaching party to perform their contractual duties (used when money damages aren't enough).
  
---

## 3. Core Legal Concepts

### Jurisdiction
A court's authority to render legal judgments has two elements:

* **Personal Jurisdiction:** A court's authority over the **person** (individual or corporation) being sued. Established through:
    * Physical presence.
    * Place of residence or business.
    * **Consent** (e.g., a clause in a contract).
    * **Minimum contacts** (conducting business within a state).
* **Subject Matter Jurisdiction:** A court's authority to hear specific types of disputes.
        * **General vs. Limited:** State courts have *general jurisdiction* (can hear almost anything), while federal courts have *limited jurisdiction* (only specific types of cases, like those involving federal laws or diversity of citizenship).
        * **Exclusive Jurisdiction:** When *only* a specific court can hear a case (e.g., bankruptcy or copyright cases *must* be heard in federal court).
        * **Removal Jurisdiction:** Under **28 U.S.C. § 1441(a)**, a defendant can "remove" a case filed in state court to federal court if the federal court would have had original jurisdiction.
            * *Note:* Under **CAN-SPAM**, State AG enforcement actions *must* specifically be filed in federal court (a unique requirement).

### Legal Definitions
* **Person:** A legal entity that can sue, be sued, own property, and sign contracts. Includes **human beings** (citizens, residents) and **legal organizations** (corporations).
* **Preemption:** Law from a **higher authority** (e.g., federal) takes precedence over law from a lower authority (e.g., state). Established by the **Supremacy Clause**.
* **Private Right of Action (PRA):** The ability for **individuals and corporations** to bring cases to court for violations of a specific law.
    * **Contains PRA:** CCPA (California Consumer Privacy Act).
    * **Lacks PRA:** FERPA, GLBA, HIPAA.

## Legal Liability
Liability is being responsible or answerable in law.

### Civil vs. Criminal Litigation
| *Feature* | *Civil Litigation* | *Criminal Litigation* |
| :--- | :--- | :--- |
| *Who brings suit?* | **Plaintiff** (Private individual, Company, or Agency like FTC) | **Prosecutor** (Government only: DOJ or State AG) |
| *Basis* | Civil wrong (Tort, Breach of Contract, Statutory violation) | Violation of Criminal Statute |
| *Standard of Proof* | **Preponderance of the evidence** (More likely than not / >50%) | **Beyond a reasonable doubt** (Highest standard; presumption of innocence) |
| *Remedy/Punishment* | Money damages, Injunctions (court orders), Declaratory judgment | Imprisonment, Criminal Fines |
| *Procedural Protections* | Standard due process | Enhanced protections (e.g., right to speedy trial, right to counsel) |

> **Key Example:** While most privacy enforcement is civil, the **Wiretap Act** (Title III) explicitly provides for criminal penalties, including fines up to $250,000 and imprisonment of up to 5 years.

### Torts and Negligence
* **Tort:** A civil wrong that involves harm to one party caused by the action or inaction of another, *not* involving a contract.
* **Negligence (A Tort):** Harm caused by a failure to act with reasonable care. Requires four elements:
    1.  **Duty of care:** An established responsibility.
    2.  **Breach of duty:** Violation of that responsibility.
    3.  **Damages:** The accuser suffered some form of harm (financial, physical, emotional).
    4.  **Causation:** The breach must be the result of the damages.
* **Four Invasion of Privacy Torts (Common Law):**
    1.  **Invasion of solitude:** Physical or electronic intrusion (e.g., accessing someone's email).
    2.  **Public disclosure of private facts:** Disclosure of truthful, non-newsworthy information that would offend a reasonable person.
    3.  **False light:** Disclosing information that causes a person to be **falsely perceived** by others.
    4.  **Appropriation:** Unauthorized use of someone’s name or likeness.

### Framework for Analyzing a Law
When determining if a law applies to a specific scenario, follow this hierarchy:
* **1. Scope (Who):** Does the law apply to the specific entity? (e.g., HIPAA applies to "Covered Entities," but not to a fitness app).
* **2. Application (What):** Does the law protect the specific type of data involved? (e.g., FCRA applies to "Consumer Reports," but not to internal marketing lists).
* **3. Preemption:** If it is a state law, has it been preempted (overridden) by a federal statute?
* **4. Enforcement:** Who has the authority to enforce it (FTC, State AG, Private Right of Action) and what are the penalties?

### Consent Models
Different privacy laws require different levels of user permission before data can be collected or shared.

| Feature | Affirmative Consent (**Opt-In**) | Implied Consent (**Opt-Out**) |
