# **QAP Standard Operating Procedures for Source Validation and Best Practices for Internet Sources**

*By M. Nuri Shakoor, Founder and Senior Consultant for Project Quanta Analytic by MNS Consulting*

This white paper outlines a **standard, tradecraft-rigorous policy** to adopt for using internet sources obtained via web search, including what to avoid and how to triangulate/verify within the Quanta Analytic systems analysis architecture. This policy is built around structured analytic tradecraft: **explicit source validation, bias resistance, and an auditable reasoning trail**. Structured techniques are designed to externalize and scrutinize analytic logic precisely because analysts often operate with incomplete, ambiguous, and sometimes deceptive information. \[1\]

---

## **Web-Sourced Information Policy (WSI)**

**Version:** 1.0  
**Applies to:** All analytic products using open web sources (OSINT) obtained through search engines, social platforms, and online databases.  
**Objective:** Ensure web-sourced claims meet analytic tradecraft standards for **credibility, validity, transparency, and reproducibility**.

---

## **1\) Core Standards**

### **1.1 Tradecraft principles (non-negotiable)**

1. **No single-source reliance for key judgments.** Web information must be corroborated or explicitly caveated. \[2\]  
2. **Separate “authenticity” from “accuracy.”** A document/post can be real yet still wrong or misleading; validate the *content*, not just the artifact. \[3\]  
3. **Prefer disconfirming tests over confirming accumulation.** Evidence should be used to *stress-test* hypotheses, not to “build a case.” \[4\]  
4. **Treat “consistency” as a deception risk indicator, not automatic confirmation.** Multiple aligned reports may be redundant (shared sourcing), biased sampling, or echo-chamber effects. \[5\]

### **1.2 Required recordkeeping (audit trail)**

For every web source used:

* **URL/domain and retrieval date/time**  
* **Author/organization, publication date**  
* **Type:** primary, secondary, tertiary  
* **Claim(s) extracted as atomic statements**  
* **Confidence notes:** what would change your mind; what would falsify the claim

(Tradecraft intent: create a transparent trail others can critique and reproduce.) \[1\]

---

## **2\) Source Evaluation Standard**

### **2.1 Minimum source validation questions**

Before using a web-sourced claim as evidence, answer (and document) four questions:

1. **Who/what is the source?**  
2. **What was the source’s access?** How did they plausibly obtain the information?  
3. **What is the source’s reliability/track record?**  
4. **Is the information plausible in context?** \[3\]

### **2.2 Deception-aware validation (recommended baseline)**

Use a deception-informed checklist when stakes are high or the information environment is contested:

* **MOM** (motive/opportunity/means)  
* **POP** (past practices)  
* **MOSES** (source manipulability)  
* **EVE** (evidence evaluation and cross-source checks) \[6\]

---

## **3\) Verification and Triangulation Requirements**

### **3.1 Triangulation rule for “load-bearing” claims**

A claim may support a key judgment only if it meets **one** of the following:

**Tier A (preferred):**

* Verified **primary source** (official record/data/filing/transcript) **and** at least **one** independent confirmation or contextual validation.

**Tier B (acceptable):**

* Two or more **independent** credible sources **with different collection pathways** (e.g., official statement \+ satellite-derived analysis \+ reputable wire service reporting).

**Tier C (limited use):**

* Single credible source **only if** the product explicitly labels the claim as **uncorroborated** and downgrades confidence accordingly.

**Why:** Analysts can be misled by redundancy and small samples that appear internally consistent but are not representative or independent. \[5\]

### **3.2 Independence test (anti-echo-chamber check)**

Before counting sources as corroboration, test whether they are **actually independent**:

* Do multiple outlets cite the **same unnamed official**, same report, or same viral post?  
* Are they syndicated rewrites?  
* Are timestamps clustered unusually (coordinated release)?  
  If independence is weak, treat them as **one** source for confidence purposes. \[5\]

### **3.3 Hypothesis-driven verification (reduce confirmation bias)**

For contested claims, use **Analysis of Competing Hypotheses (ACH)** logic:

* List plausible hypotheses (including deception where appropriate).  
* Evaluate *diagnosticity* (which evidence discriminates).  
* Actively seek evidence that would **disprove** the favored explanation. \[4\]

---

## **4\) High-Risk Web Sources to Avoid (or strictly downgrade)**

Use the categories below as a **do-not-use** list for key judgments unless independently validated.

### **4.1 Avoid as evidentiary support (default)**

* **Anonymous / unattributed blogs** and “insider” posts with no corroboration.  
* **Content farms** and SEO-driven sites optimized for traffic, not accuracy.  
* **Partisan propaganda outlets** lacking transparent corrections/editorial standards.  
* **Heavily aggregated “news”** that does not link to originals.  
* **Wikipedia as a cite** (fine as a roadmap to primary sources; not as evidence).  
* **AI-generated articles** with unclear sourcing and no named editor/review.  
* **Screenshots of documents** without provenance or verifiable chain of custody.

### **4.2 Social media (use with constraints)**

Social posts may be used only as:

* **Leads/tips** for collection, or  
* **Evidence of narratives, influence, or sentiment**, not factual truth-claims,  
  unless independently verified via primary sources or strong triangulation.

**Rationale:** Deception and disinformation exploit cognitive bias; analysts should not reject deception merely because direct evidence is absent and should avoid “good enough” acceptance. \[2\]

---

## **5\) Practical Verification Techniques (web context)**

Use as appropriate to the claim type:

**For documents/data**

* Prefer the **original hosting authority** (issuer’s site, official repository).  
* Check versioning, publication dates, and whether the issuer later corrected/withdrew it.  
* Distinguish document authenticity from content accuracy (a real doc can contain flawed intelligence). \[3\]

**For imagery/video**

* Reverse image lookup; check first appearance date.  
* Cross-check geolocation/time cues (weather, shadows, landmarks).  
* Validate against independent reporting streams.

**For numerical claims**

* Identify base rates and sample size; downgrade confidence when data are sparse even if consistent. \[5\]

---

## **6\) Quality Assurance and Review**

### **6.1 Mandatory analytic self-critique**

Before publication, conduct:

* **Key Assumptions Check** (make implicit assumptions explicit)  
* **Structured self-critique / peer review** to challenge logic and sourcing

Structured approaches exist to leave an audit trail and make disagreements visible early. \[1\]

### **6.2 Confidence discipline**

Analysts commonly become more confident with more information even when accuracy does not improve; confidence should track **evidence quality and diagnosticity**, not volume. \[7\]

---

## **7\) Credible Web Source Types Acceptable for Tradecraft-Rigorous Products**

Below is a **starter allowlist** (examples, not exhaustive). The tradecraft rule is: **prefer primary and methodologically transparent sources**.

### **Tier 1: Primary / authoritative**

* **Government and regulator domains** (generally “.gov” and equivalents): official releases, sanctions lists, budgets, legislation, statistics, court records.  
* **Official international organizations:** UN bodies, IAEA, WHO, IMF, World Bank, OECD, WTO (reports and datasets).  
* **Treaty/arms control and national statistical agencies:** official datasets, methodological notes.  
* **Corporate primary filings:** securities regulators (e.g., EDGAR-style repositories), annual reports, audited financial statements, procurement records.  
* **Election and parliamentary portals:** official results, transcripts, voting records.

### **Tier 2: High-quality secondary**

* **Reputable wire services and major investigative desks** with corrections policies (useful for event confirmation and timelines).  
* **Top-tier think tanks and research institutes** with transparent methodology and named authors (e.g., defense, conflict, economics).  
* **Peer-reviewed journals / academic publishers** (prefer systematic review/meta-analysis where relevant).  
* **Specialized technical NGOs** known for methods transparency (e.g., conflict event datasets, arms transfer databases).

### **Tier 3: Contextual/tertiary (limited evidentiary weight)**

* Encyclopedias, explainers, blogs by credentialed experts: useful for orientation, **not** decisive evidence without upstream sourcing.  
* Social platforms: useful for **narrative analysis** and as collection leads, not as unverified fact.

---

## **References (APA)**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). CQ Press/SAGE.  
\[2\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). (Deception Detection “rules of the road”; MOM/POP/MOSES/EVE). CQ Press/SAGE.  
\[3\] Jones, M. D. (1998). *The Thinker’s Toolkit*. Three Rivers Press.  
\[4\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. Center for the Study of Intelligence.  
\[5\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. (Oversensitivity to consistency; “law of small numbers”). Center for the Study of Intelligence.  
\[6\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). (EVE: corroboration and cross-source conflicts). CQ Press/SAGE.  
\[7\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. (Information volume vs accuracy; overconfidence). Center for the Study of Intelligence.

Below are two ready-to-use artifacts you can drop into an analytic SOP binder: **(A) a one-page Web Source SOP checklist** and **(B) a source scoring rubric** aligned to **MOM/POP/MOSES/EVE** (deception-aware evaluation) and **ACH** (competing hypotheses discipline). These reflect the core tradecraft themes of structured techniques and cognitive-bias mitigation. \[1\]\[2\]

---

## **A) One-Page SOP Checklist: Web Sources for Analytic Products**

### **0\) Scope gate (before you collect)**

* **Define the decision question** (what decision will this inform?).  
* Identify **“load-bearing” claims** (claims that directly drive key judgments).  
* Set **minimum corroboration standard** for load-bearing claims (see Step 4).

### **1\) Collection discipline (don’t “Google until convinced”)**

* Use **purpose-driven queries** (keywords tied to specific uncertainties).  
* Capture **full citation metadata** at time of collection:  
  * URL, title, author/organization, publication date, retrieval date/time, and any document IDs.  
* **Save the evidence** (PDF download or archived copy) when feasible—web pages change.

### **2\) Source triage (initial acceptability)**

* Classify each item:  
  * **Primary** (official record/data/filing/transcript), **Secondary** (reporting/analysis), **Tertiary** (aggregation/explainers).  
* Apply red-flag screen (auto-downgrade unless independently verified):  
  * No author/editor; no date; no sources; sensational headline; heavy affiliate/SEO behavior; “insider” claims with no access explanation.

### **3\) Source validation (MOM/POP/MOSES/EVE “quick test”)**

Document answers (one line each is enough):

* **MOM (Motive/Opportunity/Means):** Why might the source deceive or spin? What leverage exists?  
* **POP (Past Practices):** Track record for accuracy/corrections?  
* **MOSES (Source manipulability):** How easy is it to spoof/plant/manipulate this channel?  
* **EVE (Evidence evaluation):** What corroborates? What conflicts? What is missing? \[1\]

### **4\) Claim extraction (turn prose into testable statements)**

* Convert content into **atomic claims** (“X happened at Y time in Z location”).  
* Separate:  
  * **Observation** (what is reported) vs **Inference** (what it implies) vs **Assessment** (your judgment).  
* Tag each claim as:  
  * **Load-bearing / Supporting / Context-only / Lead-only**.

### **5\) Independence & echo-chamber check (required for corroboration)**

Before counting multiple sources as confirmation, test independence:

* Are they citing the **same unnamed official**, the **same report**, the **same viral post**, or syndication?  
* If yes, count them as **one** corroborative stream.

### **6\) Verification & triangulation (minimum standards)**

**For load-bearing claims, require one of:**

* **Tier A (preferred):** primary source **\+** independent confirmation/context check.  
* **Tier B (acceptable):** ≥2 independent sources **with different collection pathways** (e.g., official \+ reputable wire \+ technical/forensic).  
* **Tier C (limited):** single credible source only if explicitly labeled **uncorroborated** and confidence reduced. \[2\]

### **7\) ACH alignment (bias-resistant reasoning)**

* List plausible hypotheses (including deception where relevant).  
* For each key piece of evidence, ask:  
  * Does it **fit multiple hypotheses** (weakly diagnostic) or **discriminate** (strongly diagnostic)?  
* Actively seek **disconfirming evidence** against the favored hypothesis. \[2\]

### **8\) Confidence assignment (evidence-quality driven)**

Confidence should track:

* **Source quality \+ independence \+ diagnosticity**, not the volume of similar reports. \[2\]

### **9\) Product hygiene (publication standard)**

* Every key judgment must have:  
  * Evidence chain (citations), counterpoints/conflicts, and stated assumptions.  
* Flag any:  
  * Single-source claims, contested claims, or unresolved conflicts in the sourcing.

---

## **B) Web Source Scoring Rubric (0–5) \+ Use Rules**

### **How to use (fast)**

1. Score each source **once** (source-level) using the table below.  
2. Score each **claim** separately for **corroboration** and **diagnosticity**.  
3. For load-bearing claims, **do not rely on composite scores alone**—use Tier A/B/C corroboration rules \+ ACH diagnosticity check.

### **Source-level scoring (0–5 each)**

Use 0=unusable, 3=usable with caveats, 5=highly reliable.

| Dimension (0–5) | What you’re judging | Tradecraft anchor |
| ----- | ----- | ----- |
| **R – Reliability / track record** | Accuracy history, corrections culture, consistency over time | **POP** |
| **A – Access / proximity** | Direct access to events/data vs hearsay | Source validation |
| **P – Provenance / transparency** | Named author, methods, citations, original docs linked | Auditability |
| **M – Manipulation risk** | Susceptibility to spoofing/planting, incentives to mislead | **MOM \+ MOSES** |
| **T – Timeliness** | Currentness relative to the claim | Fit-for-purpose |
| **I – Independence** | Not derivative of same upstream source | Anti-echo |
| **S – Specificity** | Concrete details that can be checked (time/place/data) | Verifiability |

**Interpretation bands (source-level)**

* **Green (Strong):** average ≥4 **and** no “fatal flaw” (e.g., unknown author \+ no provenance).  
* **Amber (Mixed):** average 2.5–3.9 or one major weakness (e.g., high manipulation risk).  
* **Red (Weak):** average \<2.5 or multiple fatal flaws → *lead-only* unless verified.

### **Claim-level scoring (0–5 each)**

| Claim dimension (0–5) | What it means | Why it matters |
| ----- | ----- | ----- |
| **C – Corroboration** | Independent confirmation across distinct pathways | Prevents single-stream failure |
| **D – Diagnosticity (ACH)** | Discriminates among hypotheses vs fits all | Prevents “evidence inflation” |
| **F – Falsifiability** | Clear conditions that would disprove the claim | Enforces testability |

**Claim acceptance rule (recommended)**

* **Load-bearing claim can support a key judgment only if:**  
  * **C ≥ 4** (Tier A/B corroboration met), **and**  
  * **D ≥ 3** (meaningfully discriminating), **and**  
  * No unresolved “hard conflict” with equally credible sources (must be addressed if present).

### **Minimal documentation template (copy/paste)**

**Source Card**

* Source: (Org/Author) | URL | Date published | Date retrieved  
* Type: Primary / Secondary / Tertiary  
* Scores: R\_\_ A\_\_ P\_\_ M\_\_ T\_\_ I\_\_ S\_\_ (band: Green/Amber/Red)  
* Notes: MOM/POP/MOSES/EVE (1–2 bullets each)  
* Key claims extracted (atomic): 1\) … 2\) …  
* Independence check: upstream source(s) or “appears independent”  
* What would change my mind? (1 bullet)

**Evidence Log (per key judgment)**

* Hypotheses (ACH): H1… H2… H3…  
* Evidence item: supports which hypotheses? contradicts which? diagnosticity score D\_\_  
* Corroboration pathways: official / technical / on-the-ground / financial / imagery / reputable reporting

---

## **References**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). SAGE Publishing. [https://collegepublishing.sagepub.com/products/structured-analytic-techniques-for-intelligence-analysis-3-255432](https://collegepublishing.sagepub.com/products/structured-analytic-techniques-for-intelligence-analysis-3-255432) ([Sage College Publishing](https://collegepublishing.sagepub.com/products/structured-analytic-techniques-for-intelligence-analysis-3-255432?utm_source=chatgpt.com))  
\[2\] Heuer, R. J., Jr. (1999). *Psychology of Intelligence Analysis*. CIA Center for the Study of Intelligence. [https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/](https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/) ([CIA](https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/?utm_source=chatgpt.com)) (PDF: [https://www.cia.gov/resources/csi/static/Pyschology-of-Intelligence-Analysis.pdf](https://www.cia.gov/resources/csi/static/Pyschology-of-Intelligence-Analysis.pdf) ([CIA](https://www.cia.gov/resources/csi/static/Pyschology-of-Intelligence-Analysis.pdf?utm_source=chatgpt.com)))

## **1\) Strategic SitReps & Geopolitical Risk Intelligence Analysis**

**Use case:** time-sensitive updates, executive decision support, high-noise information environment, elevated deception/propaganda risk.

### **Mission-specific tradecraft priorities**

1. **Speed with controlled uncertainty:** publish fast **but label what is confirmed vs plausible vs unverified**.  
2. **Independence over volume:** 10 outlets repeating one upstream source is still **one** stream.  
3. **Deception-aware by default:** assume active narrative shaping in crises; test for manipulation and coordinated amplification. \[1\]\[2\]  
4. **Hypothesis discipline:** evidence should *differentiate* between plausible explanations, not just “fit” the favored story. \[2\]

---

## **A. Rubric weighting for SitReps (recommended)**

Use the same 0–5 scoring dimensions (R, A, P, M, T, I, S), but weight them for crisis reporting:

* **R – Reliability/track record:** **0.18**  
* **P – Provenance/transparency:** **0.18**  
* **M – Manipulation risk:** **0.18**  
* **I – Independence:** **0.15**  
* **A – Access/proximity:** **0.12**  
* **T – Timeliness:** **0.12**  
* **S – Specificity/verifiability:** **0.07**

**Why these weights:** SitReps fail most often due to *manipulated narratives*, *non-independent confirmation*, and *thin provenance*—not because they were one hour late. The goal is to move fast **without** letting urgency override validation. \[1\]\[2\]

**Hard-stop rules (SitRep gates):**

* **No load-bearing claim** may rely on **social media alone**. Treat as **lead-only** until corroborated.  
* “**Anonymous official**” reporting counts as **one stream** unless another outlet independently confirms via different access.  
* If **two credible sources conflict**, you must either resolve the conflict or surface it explicitly in the SitRep.

---

## **B. SitRep triangulation standards (fast, operational)**

**Tier A (preferred):** primary record \+ one independent confirmation  
**Tier B (acceptable):** two independent streams with different collection pathways  
**Tier C (limited):** single credible stream → allowed only as **uncorroborated**, with reduced confidence and explicit caveat. \[1\]

### **Quick “pathway menu” for independence**

Count corroboration only when it comes from distinct pathways, e.g.:

* **Official/primary:** government, regulator, IO communiqués; legal/filing records  
* **Professional journalism:** reputable wire \+ named reporting chain  
* **Technical/forensic:** satellite imagery providers; geolocated video; maritime/aviation tracking; seismology/meteorological data where relevant  
* **Market/administrative signals:** exchange/central bank actions; port closures; NOTAMs; shipping advisories; corporate disclosures

---

## **C. What to avoid or downgrade in geopolitical SitReps**

**Avoid as evidence for key judgments (unless independently verified):**

* Anonymous blogs / Substack-like posts with no methods, no sourcing, no editor  
* “Aggregator” sites that don’t link originals  
* Single screenshots of “documents,” “orders,” or “leaks” without provenance  
* Telegram/Twitter/X claims presented as fact without geolocation/time confirmation  
* AI-generated “news” pages with unclear authorship and no corrections policy  
* Partisan state-aligned outlets when they are the *sole* source for a contested claim

**Downgrade triggers (red flags):**

* **Too-perfect story** that neatly supports one actor’s objectives  
* **Coordinated timing**: many accounts post same phrasing within minutes  
* **Recycled visuals** (old images/video reintroduced as current)  
* Claims that are **non-falsifiable** (“sources say something big is coming”)

These practices mitigate common cognitive traps—especially premature closure and confirmation bias under time pressure. \[2\]

---

## **D. Acceptable web sources for SitReps (credible examples)**

Below are **source types \+ example sites** typically acceptable in tradecraft-rigorous SitReps, assuming you still apply the rubric and corroboration rules.

### **1\) Primary / authoritative (highest value)**

* **National governments & regulators:** foreign ministries, defense ministries, election commissions, central banks, statistical agencies  
* **Sanctions/controls:** U.S. Treasury OFAC, EU sanctions pages, UK OFSI  
* **International organizations:** UN (and agencies), IMF, World Bank, IAEA, OSCE (where relevant), NATO, OECD  
* **Legal/official records:** gazettes, court filings, procurement portals (where accessible)

### **2\) High-quality journalism (event confirmation & timelines)**

* **Wire services:** Reuters, Associated Press (AP), Agence France-Presse (AFP)  
* **Major outlets with strong corrections standards:** Financial Times, Wall Street Journal, BBC, etc. (use as secondary confirmation; still check upstream sourcing)

### **3\) High-quality research/analysis (context, scenarios; not “fact engines”)**

* IISS, SIPRI, Chatham House, CSIS, RUSI, Carnegie, Brookings, RAND  
  (Use for framing, indicators, and structured judgments; don’t substitute for primary confirmation.)

### **4\) Technical/observational OSINT (verification enablers)**

* **Satellite/remote sensing** providers and reputable analytic shops (esp. when they show method)  
* **Aviation/maritime tracking** tools (treat as technical indicators; confirm with official advisories when possible)

---

## **E. SitRep format requirement (to enforce rigor)**

For every SitRep item, present:

* **Claim (atomic):** what happened / where / when  
* **Status:** Confirmed | Probable | Unverified  
* **Sources:** list \+ independence note (“same upstream” if applicable)  
* **Alt explanation(s):** 1 line (ACH-lite)  
* **Confidence:** High/Med/Low \+ why \[2\]

---

## **References**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). SAGE/CQ Press. [https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842](https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842)  
\[2\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. CIA Center for the Study of Intelligence. [https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/](https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/)

## **2\) Policy Analysis/Shop**

**Use case:** advising decision-makers on **policy options**, **legal/regulatory feasibility**, **budget/implementation**, and **second-order effects**. Compared to SitReps, the tradecraft center of gravity shifts from “what happened?” to **“what will work, under what constraints, at what cost, with what risks?”**

### **Mission-specific tradecraft priorities**

1. **Primary-source supremacy:** statutes, regulations, official guidance, budgets, oversight reports, and authoritative datasets outrank commentary.  
2. **Separate fact from advocacy:** policy spaces are crowded with persuasive narratives; analysts must label **normative claims** vs **empirical claims**.  
3. **Method transparency over reputational glow:** use sources that show **how** they reached conclusions (data, assumptions, model, uncertainty).  
4. **Bias resistance:** actively test favored options; seek disconfirming evidence and compare alternatives (ACH discipline). \[1\]\[2\]

---

## **A) Rubric weighting for Policy Analysis (recommended)**

Keep the 0–5 scoring approach but **reweight** toward provenance, method, and bias/COI transparency.

**Dimensions (0–5):**

* **P** Provenance & method transparency  
* **R** Reliability/track record (corrections, rigor)  
* **A** Access/proximity to primary information (e.g., official record vs hearsay)  
* **I** Independence (not derivative/syndicated; different upstream)  
* **B** Bias/advocacy & COI transparency (funding, agenda clarity, lobbying ties)  
* **S** Specificity/verifiability (data, citations, reproducible claims)  
* **T** Timeliness (relevance window)  
* **M** Manipulation risk (lower than crisis settings, but not zero)

**Suggested weights:**

* **P 0.22 | B 0.16 | R 0.14 | S 0.12 | A 0.12 | I 0.12 | T 0.07 | M 0.05**

**Hard-stop rules (policy gates):**

* A source with **opaque methods** *and* **unclear funding/COI** cannot be load-bearing for a recommendation (it may be used as context only).  
* If the claim is about what the law/rule “does,” **cite the actual text** (statute/reg, official rulemaking docket, or binding guidance) — not an interpretation blog.  
* For impact claims (“policy X will reduce Y”), require **evaluation-grade evidence** (see triangulation below) or downgrade confidence. \[1\]\[2\]

---

## **B) Triangulation standards tailored to policy work**

Policy conclusions should be supported by **three distinct validation layers** when feasible:

### **1\) Authority layer (what is allowed/required)**

* **Statute / regulation / executive instrument / binding guidance**  
* Implementation authorities: appropriations language, delegated authorities, enforcement mechanisms

### **2\) Implementation layer (what actually happens in practice)**

* Inspector General reports, GAO-style evaluations, program audits  
* Administrative data and performance reports  
* Procurement/contracting records (where relevant)

### **3\) Effects layer (what outcomes are likely)**

* Peer-reviewed studies, systematic reviews, quasi-experimental evaluations  
* High-quality datasets with documented methodology  
* Transparent models with sensitivity analysis

**Policy independence test:** your “corroboration” doesn’t count if two sources are both recycling the same white paper, same press release, or same advocacy memo (echo-chamber problem). \[2\]

---

## **C) What to avoid (or strictly downgrade) in policy shops**

**Avoid as load-bearing evidence:**

* Advocacy pieces with **no disclosed funding**, **no method**, and **no data trail**  
* Op-eds and think pieces used as “proof” of outcomes  
* Lobby-group “reports” that do not provide underlying data or methods  
* Aggregator summaries of bills/rules that don’t cite the underlying text  
* Single-study claims with no replication and unclear external validity (unless clearly bounded)

**Downgrade triggers (policy red flags):**

* Causal claims with no identification strategy (“X caused Y” with correlation only)  
* Cost estimates without assumptions, time horizon, or uncertainty bounds  
* “Consensus” claims built from non-independent citations  
* Definitions drift (metrics or categories change across sources)

---

## **D) Analyst workflow (policy-grade, fast enough for real shops)**

1. **Frame the policy question** (decision, timeframe, jurisdiction, constraints).  
2. **Define evaluation criteria** (effectiveness, cost, legality, equity, implementability, political feasibility, risk).  
3. **Generate options** (including status quo and a “minimal change” option).  
4. **Evidence map**: for each option, fill Authority / Implementation / Effects layers.  
5. **ACH-lite**: test competing explanations for why outcomes would (or wouldn’t) occur; look for disconfirming evidence. \[2\]  
6. **Sensitivity checks**: what assumptions dominate results? what breaks first?  
7. **Write recommendations** with explicit confidence tied to evidence quality (not volume). \[1\]\[2\]

---

## **E) Credible web source material commonly acceptable (policy context)**

Use these as **starting allowlists**—they still get scored and triangulated.

### **Tier 1 — Primary legal/regulatory and official records**

* Official legislative portals (bills, statutes, voting records, committee reports, hearing transcripts)  
* Official registers/gazettes (rulemaking, notices, final rules)  
* Budget/appropriation documents, agency performance plans, official datasets  
* Court opinions and dockets (where relevant)

### **Tier 2 — Oversight and evaluation-grade sources**

* Supreme audit institutions / inspector generals / official evaluators  
* Nonpartisan budget/scoring bodies (where applicable)  
* National academies / standards bodies where methods are transparent

### **Tier 3 — Research-grade secondary**

* Peer-reviewed journals, university centers, replication repositories  
* Top-tier think tanks **with transparent methods and funding disclosure** (useful for scenarios and structured arguments, not as “primary truth”)

### **Tier 4 — Context-only (use with care)**

* Major media reporting (good for timelines and stakeholder positions; do not treat as policy impact evaluation)  
* Expert commentary (helpful for hypothesis generation and framing)

---

## **References**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). CQ Press/SAGE. `https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842`  
\[2\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. CIA Center for the Study of Intelligence. `https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/`

## **3\) Corporate Risk**

**Use case:** decision support for **material risk** (financial, legal/compliance, operational, reputational) tied to **assets, people, suppliers, markets, and transactions**. Tradecraft emphasis shifts toward **materiality, auditability, and defensible sourcing** (what you can stand behind to Legal/Compliance/Audit).

### **Mission-specific tradecraft priorities**

1. **Primary records and auditable trails first** (regulators, courts, sanctions lists, corporate filings, official registries).  
2. **Materiality-driven collection** (avoid “nice-to-know” noise; focus on what changes exposure).  
3. **KYC/third-party rigor:** provenance \+ independence checks are mandatory because corporate risk is highly vulnerable to fraud, shell structures, and narrative manipulation.  
4. **Bias resistance in judgments:** explicitly test competing explanations and avoid “evidence stacking” from non-independent sources. \[1\]\[2\]

---

## **A) Rubric weighting for Corporate Risk (recommended)**

Keep 0–5 scoring, but reweight around **legal defensibility, provenance, independence, and manipulation/fraud risk**.

**Dimensions (0–5):**

* **L – Legal/Regulatory authority:** does it originate from a competent authority (regulator, court, official list)?  
* **P – Provenance/method transparency:** can you trace it back to original records or methods?  
* **R – Reliability/track record:** corrections culture, accuracy history.  
* **I – Independence:** not derivative/syndicated; distinct upstream.  
* **M – Manipulation/fraud susceptibility:** spoofing risk, planted docs, commercial incentives.  
* **A – Access/proximity:** direct record vs hearsay.  
* **S – Specificity/verifiability:** identifiers, dates, entity resolution, citations.  
* **T – Timeliness:** current enough for the decision.

**Suggested weights:**

* **L 0.20 | P 0.18 | M 0.14 | I 0.12 | R 0.12 | S 0.10 | A 0.08 | T 0.06**

**Hard-stop rules (corporate gates):**

* If a claim affects **sanctions/export controls/AML/FCPA/privacy/labor** exposure, it must be supported by **Tier 1 authority** (official list, statute/regulation, regulator guidance, court record, or audited filing). Secondary commentary can’t be load-bearing.  
* Beneficial ownership / corporate identity claims must be supported by **official registries \+ filings** (or equally authoritative records) and pass an **entity-resolution check** (name variants, addresses, officers, registration IDs).  
* Any “leaked document” or screenshot is **lead-only** until provenance is established and corroborated.

---

## **B) Triangulation standards tailored to corporate risk**

For **load-bearing claims**, use a 3-layer validation model:

### **1\) Authority layer (what’s legally true / enforceable)**

* Sanctions lists, regulator enforcement actions, court dockets/opinions, official rule text, procurement debarment lists.

### **2\) Corporate record layer (what the entity officially represents)**

* Audited annual reports, securities filings, corporate registry filings, beneficial ownership registers (where accessible), official press releases, earnings call transcripts.

### **3\) Operational signal layer (what is happening in practice)**

* Trade/shipping indicators, import/export records where lawful, NOTAMs/port notices, insurance/claims indicators, plant closures, verified incident reporting, workforce actions, supply chain disruptions.

**Independence test:** two vendor profiles that ingest the same registry and the same press stories are not independent corroboration—treat as one stream. \[2\]

---

## **C) What to avoid or downgrade (corporate risk context)**

**Avoid as load-bearing evidence:**

* Vendor marketing “risk reports” with opaque methods or undisclosed data sources  
* Single-outlet scandal reporting with unnamed sources (use as a lead, not proof)  
* SEO content farms, listicles, and aggregator “sanctions check” pages  
* Social media allegations (use for **alerting** only unless verified)  
* “Corporate registry mirrors” that don’t clearly map to official registries  
* AI-generated corporate profiles with no citations/provenance

**Downgrade triggers (fraud/narrative red flags):**

* Identity ambiguity (similar names; transliteration variants) with weak identifiers  
* Unverifiable claims about ownership changes, seizures, or insolvency  
* Too-clean narratives that conveniently support one stakeholder’s objective  
* Claims that cannot be falsified or checked against authoritative records

---

## **D) Corporate-risk analyst workflow (practical SOP)**

1. **Define exposure**: jurisdiction(s), transaction type, counterparties, thresholds, time horizon.  
2. **Map risk taxonomy**: legal/compliance, financial, operational, cyber, reputational, ESG, geopolitical.  
3. **Identify load-bearing claims**: the few claims that drive the go/no-go or mitigation decision.  
4. **Collect Tier 1 → Tier 3** (below), scoring each source and logging provenance.  
5. **ACH-lite**: list plausible explanations (benign vs adverse vs deception) and test which evidence is diagnostic. \[2\]  
6. **Mitigation design**: contractual controls, enhanced due diligence, monitoring KRIs, alternative suppliers, exit triggers.  
7. **Confidence statement**: tie confidence to evidence quality/independence—avoid confidence inflation from repeated non-independent reporting. \[2\]

---

## **E) Credible web source material acceptable for corporate risk (starter allowlist)**

### **Tier 1 — Authority / primary (best for compliance and “defensible” claims)**

* **Sanctions & watchlists:** U.S. Treasury OFAC; EU sanctions; UK OFSI; UN Security Council sanctions  
* **Regulators/enforcers:** DOJ, SEC, FINCEN, Commerce/BIS, State, equivalent national authorities  
* **Courts:** official dockets, judgments, bankruptcy/insolvency registries (where public)  
* **Company registries:** official national corporate registries / gazettes / beneficial ownership registers (where available)

### **Tier 2 — Corporate records (strong for financial/ownership/representation)**

* **Securities filings** (issuer filings and regulator repositories)  
* **Audited financials** and annual reports  
* **Earnings call transcripts** (prefer those that reference the original call and date/time)  
* **Official corporate communications** (press releases; procurement notices)

### **Tier 3 — High-quality secondary (context and early warning; not “legal truth”)**

* Reputable wire services and investigative desks (for incident timelines; verify upstream)  
* Methodologically transparent think tanks / academic studies (for country/sector baseline risk)  
* Specialized, reputable risk-data providers **only when methods \+ sources are documented** (treat as accelerators, not arbiters)

### **Tier 4 — Lead-only (use for alerting, narrative monitoring)**

* Social platforms, forums, anonymous whistle sites, Telegram channels (must be independently verified before use as evidence)

---

## **References**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). SAGE/CQ Press. [https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842](https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842)  
\[2\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. CIA Center for the Study of Intelligence. [https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/](https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/)

## **4\) Conflict Analysis**

**Use case:** assess **armed actor behavior, battlefield dynamics, civilian harm, escalation risk, and likely trajectories** in a deliberately contested information environment. Tradecraft emphasis shifts toward **deception resistance, technical verification, and source independence** under conditions of propaganda, fog of war, and rapid narrative cycling. \[1\]\[2\]

### **Mission-specific tradecraft priorities**

1. **Verification over velocity for “atrocity / civilian harm / WMD / ceasefire breach” claims.** These are high-impact and frequently manipulated.  
2. **Independence is everything:** many “confirmations” are repackaged from the same battlefield feed. Treat non-independent repetition as **one** stream. \[2\]  
3. **Technical corroboration as a default:** geolocation, chronolocation, platform/weapon ID, crater/BDA logic, and multi-angle imagery validation.  
4. **Hypothesis discipline:** evidence must discriminate among competing explanations (combat loss vs accident vs false-flag vs misattribution). \[2\]

---

## **A) Rubric weighting for Conflict Analysis (recommended)**

Keep 0–5 scoring but weight toward manipulation risk, provenance, and independence.

**Dimensions (0–5):** R Reliability | A Access | P Provenance/method | M Manipulation risk | I Independence | S Specificity/verifiability | T Timeliness

**Suggested weights:**

* **M 0.20 | I 0.18 | P 0.16 | A 0.14 | S 0.12 | R 0.12 | T 0.08**

**Hard-stop rules (conflict gates):**

* **Casualty figures**: never load-bearing from a single belligerent, single outlet, or single NGO without methodological transparency; require triangulation and define “killed” vs “dead,” civilians vs combatants, inclusion rules.  
* **Atrocity allegations** (mass killing, sexual violence, use of banned weapons): treat as **unconfirmed** until supported by (a) credible on-the-ground investigators with methods, (b) corroborating forensic/medical/imagery evidence, and/or (c) multiple independent reporting streams.  
* **Frontline maps**: do not treat as factual unless tied to verifiable geolocated changes; many maps are interpretive.

---

## **B) Conflict-specific triangulation standards (what “good” looks like)**

For **load-bearing event claims** (“X struck Y at time Z”):

1. **What/Where/When (Event layer):** geolocated \+ time-bounded evidence (imagery/video metadata is not enough; verify by landmarks, shadows, weather, cross-post timing).  
2. **Who (Actor layer):** platform/munition ID, directionality, launch envelope, known order of battle, claimed responsibility with credibility scoring.  
3. **Effect (Impact layer):** BDA indicators (crater type, structural damage patterns), medical/evac signals, secondary fires, subsequent operational changes.

**Minimum corroboration (recommended):**

* **Tier A (preferred):** technical verification (geo/time) **\+** an independent reporting/investigation stream.  
* **Tier B (acceptable):** ≥2 independent streams with distinct pathways (e.g., local journalist \+ satellite-derived analysis; hospital logs \+ imagery).  
* **Tier C (limited):** single credible stream → allowed only as *uncorroborated*, confidence reduced, and explicitly caveated. \[1\]\[2\]

**Independence test (mandatory):** if sources ultimately trace to the same Telegram channel, MoD briefing, or viral clip, that’s **one** stream. \[2\]

---

## **C) What to avoid or downgrade (conflict environment)**

**Avoid as load-bearing evidence (unless independently verified):**

* Belligerent MoD claims about enemy losses, precision strikes, or “no civilian harm”  
* Telegram/X clips without geolocation/time bounding  
* “OSINT accounts” that do not show methods, uncertainty, or corrections  
* Screenshots of “orders,” “intercepts,” “battle plans,” or “leaks” without provenance  
* AI-generated “battlefield updates,” synthetic maps, or unlabeled simulations

**Downgrade triggers (common deception cues):**

* Claims that are perfectly aligned with one side’s strategic messaging at a key moment  
* Sudden bursts of near-identical wording across accounts (coordination/amplification)  
* Recycled imagery from older battles presented as current  
* Non-falsifiable assertions (“sources say a major offensive is imminent”) with no observable indicators

---

## **D) Analyst workflow (conflict-grade SOP)**

1. **Define the analytic frame:** theater, timeframe, actors, and key decision questions.  
2. **Build a chronology** (time-series event log) with confidence tags per event.  
3. **Decompose claims** into atomic statements (event/actor/impact).  
4. **Apply verification ladder:** geo → time → actor → effects.  
5. **ACH-lite:** test alternatives (combat vs accident vs mis-ID vs deception). Seek disconfirming evidence. \[2\]  
6. **Pattern analysis:** distinguish isolated incidents from systematic trends (rules of engagement shifts, targeting patterns, escalation thresholds).  
7. **Confidence discipline:** tie confidence to independence \+ diagnosticity, not volume of similar claims. \[2\]

---

## **E) Credible web source material acceptable (conflict context)**

Use these as **starting allowlists**; still score them and test independence.

### **Tier 1 — Primary / authoritative (with known limitations)**

* UN bodies and humanitarian coordination products (situation reports, displacement, access constraints)  
* ICRC and reputable medical/humanitarian reporting with methods (for humanitarian impacts)  
* National statistical / civil defense data **only with caveats** (often politicized; use for baselines and trend signals, not precise truth)

### **Tier 2 — Methodologically transparent conflict datasets / monitoring**

* Conflict event datasets (where methodology and coding rules are published)  
* Monitoring groups that disclose sourcing, coding, and uncertainty

### **Tier 3 — High-quality investigative and technical verification**

* Reputable investigative outlets/teams that publish geolocation, imagery comparisons, chain-of-custody reasoning, and corrections  
* Satellite/remote-sensing providers and analytic shops that show methods and confidence bounds

### **Tier 4 — Media and local reporting (valuable but must be corroborated)**

* Reputable wire services \+ on-the-ground correspondents (good for timelines; verify upstream sourcing)  
* Local outlets (often closest to events, but higher manipulation/coercion risk—triangulate aggressively)

---

## **References**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). SAGE/CQ Press. [https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842](https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842)  
\[2\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. CIA Center for the Study of Intelligence. [https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/](https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/)

## **5\) NGO Security Risk Management**

**Use case:** protect **people, programs, and partners** in high-risk environments while maintaining **humanitarian principles, duty of care, and access**. Tradecraft emphasis shifts toward **actionable risk decisions**, **context fidelity**, and **safe sourcing** (collect only what you need; avoid endangering sources/communities).

### **Mission-specific tradecraft priorities**

1. **Do-no-harm sourcing:** minimize collection that could expose staff/beneficiaries/partners; limit sensitive personal data; treat comms intercept “leaks” as high-risk.  
2. **Operational usability:** analysis must translate into **thresholds, triggers, and mitigations** (not just narrative).  
3. **Local context \+ independence:** local reporting is invaluable but vulnerable to coercion; corroborate through multiple pathways.  
4. **Bias resistance:** avoid “normalization of deviance” and complacency; actively test assumptions and challenge routine risk narratives. \[1\]\[2\]

---

## **A) Rubric weighting for NGO Security Risk (recommended)**

Use 0–5 scoring, weighted toward **access, harm risk, and manipulation risk**, since NGO environments are often rumor-rich and threat actors shape narratives.

**Dimensions (0–5):**

* **H – Harm potential (do-no-harm):** could citing/using this source endanger people or compromise neutrality?  
* **A – Access/proximity:** on-the-ground knowledge vs hearsay.  
* **P – Provenance/method transparency:** traceable collection and clarity of how claims were obtained.  
* **M – Manipulation risk:** propaganda, coercion, intimidation, planted stories.  
* **I – Independence:** distinct upstream; not a single rumor chain.  
* **R – Reliability/track record:** accuracy history.  
* **S – Specificity/verifiability:** checkable details (time/place/actors).  
* **T – Timeliness:** relevance to current operations.

**Suggested weights:**

* **H 0.18 | A 0.16 | M 0.14 | P 0.14 | I 0.12 | R 0.10 | S 0.10 | T 0.06**

**Hard-stop rules (NGO gates):**

* Any source with **high harm potential** (H≤1) cannot be used in products shared beyond the security cell; sanitize/aggregate or exclude.  
* Sensitive claims (kidnapping threats, checkpoint targeting, staff doxxing) require **two independent confirmation pathways** before operational action—unless immediate life safety requires precautionary action (then label as *precautionary, unverified*).  
* Never publish details that enable targeting (names, routines, precise locations, convoy timing).

---

## **B) Triangulation standards tailored to NGO operations**

For load-bearing security judgments (route viability, program suspension, evacuation posture), require triangulation across:

### **1\) Community & acceptance signals (local layer)**

* Community leaders/committees feedback, beneficiary sentiment (captured safely), local staff observations

### **2\) Operational environment signals (incident layer)**

* Incident logs, security advisories, verified crime/violence reports, medical facility capacity, checkpoint patterns

### **3\) Authority & coordination signals (coordination layer)**

* UNDSS/UN access updates (where relevant), NGO forums, INGO security platforms, official notices, embassy warden messages (with neutrality caveats)

**Independence check:** ensure local-layer sources are not all relaying the same rumor; treat a single community rumor chain as **one stream**. \[2\]

---

## **C) What to avoid or downgrade (NGO risk context)**

**Avoid as load-bearing evidence:**

* Viral social posts naming “spies,” “collaborators,” or accusing NGOs (often incitement)  
* Belligerent statements about “humanitarian corridors” or “safe zones” without independent verification  
* Anonymous “insider” tips that push you toward risky movements  
* Screenshots of threat messages without provenance (can be fabricated)

**Downgrade triggers (NGO red flags):**

* Threat reporting that includes **unnecessary specificity** (often engineered)  
* Reports that arrive through **new/unvetted intermediaries** requesting urgency  
* Claims that align perfectly with attempts to deny access or discredit a neutral actor  
* Sudden policy “changes” at checkpoints not reflected in any other operational signal

---

## **D) NGO security analyst workflow (operational SOP)**

1. **Define the decision:** move/no-move, suspend/continue, relocate/evacuate, accept/mitigate, or redesign activity.  
2. **Identify critical vulnerabilities:** staff travel, compounds, distributions, partner sites, comms, cash handling.  
3. **Build an incident baseline:** 30/60/90-day trend by area and modality.  
4. **Map threats by actor and intent:** criminal, political-militia, state security, community backlash.  
5. **ACH-lite:** competing explanations for incidents (targeted vs opportunistic; rumor vs real; coercion vs policy shift). Seek disconfirming evidence. \[2\]  
6. **Set triggers & thresholds:** objective indicators for posture changes (e.g., 2 verified incidents on Route X in 7 days; credible threat \+ independent corroboration).  
7. **Mitigation plan:** acceptance actions, movement protocols, comms checks, hibernation/relocation, partner assurance, contingency medical.  
8. **Review cadence:** daily crisis cell if needed; weekly baseline refresh.

---

## **E) Credible web source material acceptable for NGO security risk**

Use as starting allowlists; still score them and protect sensitive details.

### **Tier 1 — Coordination / authoritative operational context**

* UN security/access coordination products (where accessible and appropriate)  
* Official government travel/security notices (use with bias caveats)  
* Formal incident reporting channels and vetted INGO security networks (platform-dependent)

### **Tier 2 — Humanitarian and protection-focused reporting**

* Reputable humanitarian situation reporting with methods and aggregation  
* Human rights organizations with clear methodology (use for trend/context; verify time/place specifics)

### **Tier 3 — High-quality journalism and local reporting**

* Wire services and reputable local outlets (triangulate; consider coercion pressures)  
* Specialized crisis-monitoring groups that disclose sourcing and uncertainty

### **Tier 4 — Lead-only (do-no-harm constraints)**

* Social media, rumor channels, messaging apps: use for **alerting** and narrative awareness; verify independently before action.

---

## **References**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). SAGE/CQ Press. [https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842](https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842)  
\[2\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. CIA Center for the Study of Intelligence. [https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/](https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/)

## **6\) Academic Research**

**Use case:** produce **valid, reproducible, theory- and evidence-grounded** findings. Tradecraft emphasis shifts toward **methodological transparency, inferential strength, replication, and citation hygiene**—with explicit controls against confirmation bias and premature closure. \[1\]\[2\]

### **Mission-specific tradecraft priorities**

1. **Methods \> reputation:** prioritize sources that disclose **data, methods, uncertainty, and limitations** over “prestige-only” credibility.  
2. **Causal claims require causal designs:** distinguish **correlation**, **mechanism**, and **causation**; downgrade claims without identification strategies or credible inference.  
3. **Replication and convergence:** treat single studies as provisional; elevate conclusions supported by **systematic reviews/meta-analyses** and multi-method convergence.  
4. **Bias-resistant reading:** actively seek disconfirming evidence; do not “stack” confirmatory papers that share the same dataset, model family, or theoretical priors. \[2\]

---

## **A) Rubric weighting for Academic Research (recommended)**

Use 0–5 scoring, but align the dimensions to research quality and reproducibility.

**Dimensions (0–5):**

* **P – Method & provenance transparency:** methods, measures, codebooks, assumptions explicit  
* **D – Data availability & integrity:** accessible dataset/code; provenance documented  
* **R – Research reliability:** peer review quality, corrections/retractions handled, track record  
* **I – Independence:** different datasets/teams/approaches; not a single “citation family”  
* **B – Bias/COI transparency:** funding, conflicts, advocacy alignment disclosed  
* **S – Statistical/analytic validity:** design fit, robustness checks, uncertainty reporting  
* **T – Timeliness/relevance:** current enough for the question (secondary to rigor)

**Suggested weights:**

* **P 0.22 | S 0.18 | D 0.15 | I 0.14 | R 0.12 | B 0.12 | T 0.07**

**Hard-stop rules (research gates):**

* Strong causal claims **cannot be load-bearing** without an appropriate design (natural experiment, RCT, IV, DiD, matched cohort, etc.) and transparent assumptions.  
* If data/code are unavailable and methods are insufficiently described, the work is **context-only** unless independently replicated.  
* Multiple papers using the **same dataset/model lineage** do **not** count as independent corroboration.

---

## **B) Triangulation standards tailored to academic work**

For a load-bearing proposition (theory claim or policy-relevant effect), aim for **three-lens convergence**:

1. **Design convergence:** results observed via more than one credible design (e.g., DiD \+ panel model \+ qualitative process tracing).  
2. **Data convergence:** results reproduced across **different datasets** or collection contexts.  
3. **Analyst/team convergence:** independent research groups reach similar conclusions.

**Evidence hierarchy (practical):**

* **Highest:** systematic reviews/meta-analyses \+ replicated findings  
* **High:** well-identified single studies with transparent data/code  
* **Moderate:** peer-reviewed but limited identification or incomplete transparency  
* **Low:** preprints/op-eds/blogs without methods (use as leads/theory prompts)

---

## **C) What to avoid or downgrade (academic context)**

**Avoid as load-bearing evidence:**

* Predatory journals, paper-mill indicators, or venues with no credible editorial standards  
* “Review” articles that are narrative-only with no search strategy/selection criteria  
* Claims resting on p-values alone with no effect sizes/uncertainty or robustness  
* Single-study sensational claims without replication or plausibility checks

**Downgrade triggers:**

* Unclear sampling frames; shifting definitions/constructs; non-reproducible measures  
* HARKing signs (hypothesizing after results) without disclosure  
* Heavy overgeneralization beyond the study’s population/context  
* COI not disclosed where it plausibly exists

---

## **D) Research-grade analyst workflow (SOP)**

1. **Define the research question** (scope, unit of analysis, causal vs descriptive).  
2. **Map competing explanations** (ACH-lite): what else could explain the outcome? \[2\]  
3. **Build an evidence map**: systematic search plan \+ inclusion/exclusion logic.  
4. **Extract atomic claims** from each paper (what exactly is being asserted?).  
5. **Score each source** (P/D/S/I/B/R/T) and record why.  
6. **Check independence** (dataset overlap, author networks, shared priors, shared instruments).  
7. **Synthesize by diagnosticity:** which findings discriminate among hypotheses? \[2\]  
8. **State conclusions with calibrated confidence:** tie confidence to replication, convergence, and inferential strength—not citation volume. \[1\]\[2\]

---

## **E) Credible web source material acceptable (academic research)**

Use these as starting allowlists; still apply scoring and independence checks.

### **Tier 1 — Primary scholarly infrastructure**

* Publisher journal sites (final versions, corrections, retractions)  
* Cross-publisher DOI infrastructure and citation registries  
* Retraction/corrections trackers (as quality-control signals)

### **Tier 2 — Indexing and discovery**

* Scholarly databases (discipline-appropriate: biomedical, social science, engineering)  
* Library guides and university databases (strong for provenance and version control)

### **Tier 3 — Preprints (valuable but provisional)**

* Major preprint servers (use for timeliness; require extra skepticism and corroboration)

### **Tier 4 — Data/code repositories (for reproducibility)**

* Institutional repositories, OSF-style registries, reputable open-data archives  
* Domain datasets with published codebooks and collection methodology

### **Tier 5 — Context-only sources**

* Expert blogs, newsletters, and commentary (useful for hypothesis generation; not evidence)

---

## **References**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.). CQ Press/SAGE.  
\[2\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*. Center for the Study of Intelligence.

\[1\] https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842

\[2\] https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/

## **7\) Countering Malign Influence (CMI), Information Warfare, Cognitive Resilience**

**Use case:** detect, attribute (appropriately), and blunt **coordinated, manipulative information activity** while strengthening audience resilience. This domain is uniquely vulnerable to *echo-chambers, coordinated amplification, forged “evidence,” and narrative laundering*, so your sourcing standard must prioritize **provenance \+ independence \+ manipulation resistance**. \[1\]\[2\]

---

### **A) Rubric weighting for CMI / Info Warfare (0–5 scoring)**

Use these dimensions (score each 0–5), then apply weights.

**Dimensions**

* **P — Provenance & method transparency:** can you trace to original data and reproduce the analytic steps?  
* **I — Independence:** distinct upstreams/collection pathways (not the same meme repeated).  
* **M — Manipulation risk:** susceptibility to spoofing, planted content, coerced testimony, or adversary-controlled channels.  
* **B — Behavior evidence:** observable coordinated behavior (timing, network patterns, inauthentic engagement), not just content.  
* **A — Actor evidence:** credible linkage to an actor (not “it sounds like them”).  
* **E — Effect evidence:** measurable reach/engagement/uptake (not assumed impact).  
* **T — Timeliness:** relevance to the decision window.

**Recommended weights**

* **P 0.18 | I 0.16 | M 0.16 | B 0.16 | A 0.14 | E 0.12 | T 0.08**

**Why:** NATO’s “information threats” framing emphasizes coordinated, manipulative activity and resilience functions (understand/prevent/contain/recover), which aligns well to a behavior-and-effects-aware evidence model. ([NATO](https://www.nato.int/en/what-we-do/wider-activities/natos-approach-to-counter-information-threats))

---

### **B) Hard-stop rules (CMI gates)**

1. **No “content-only attribution.”** Similar talking points are *not* attribution. Actor linkage must be grounded in **behavioral/infrastructure/organizational evidence**, not vibes. \[2\]  
2. **No load-bearing screenshots/leaks** without provenance \+ independent corroboration. Treat as **lead-only** until verified.  
3. **No “pile-on corroboration.”** Ten posts quoting the same viral claim count as **one stream** (echo/laundering risk). \[2\]  
4. **Separate “disinformation” from “misinformation.”** Intent matters; treat intent claims as higher-burden and explicitly caveated. (EU and NATO both stress precision in definitions.) ([European External Action Service](https://www.eeas.europa.eu/eeas/questions-and-answers-about-east-stratcom-task-force_en))  
5. **Impact claims require effect evidence.** Don’t assert “it swayed public opinion” without measurable indicators and plausible causal logic.

---

### **C) Triangulation model for campaign assessment (ABC+DE discipline)**

Use a **5-part triangulation** aligned to the way NATO describes assessing information threats (actor/behavior/content/degree/effect). ([NATO](https://www.nato.int/en/what-we-do/wider-activities/natos-approach-to-counter-information-threats))

1. **Actor (A):** who benefits; who has capability; who has history; any credible linkages?  
2. **Behavior (B):** coordination signals—synchronized posting, network amplification, inauthentic engagement, reused assets.  
3. **Content (C):** narrative frames, falsifiable claims, rhetorical triggers, tailored wedge issues.  
4. **Degree (D):** scale—reach, repetition across platforms, cross-language propagation.  
5. **Effect (E):** observable outcomes—uptake by influencers/media, real-world actions, sustained belief persistence.

**Minimum standard for load-bearing judgments**

* **Two independent pathways** across *at least two* of: actor, behavior, degree, effect.  
* If you can only validate **content**, you may describe the narrative **but not** confidently assess coordination, attribution, or impact.

---

### **D) What web sources to avoid (or strictly downgrade) in CMI work**

* **State-aligned channels** used as sole evidence for contested claims (they are often campaign instruments).  
* **Influencer/“OSINT” accounts** that do not show methods, uncertainty, or corrections.  
* **Engagement bait** (viral clips, rage posts) without geo/time bounding or provenance checks.  
* **“Research” with opaque methods** or undisclosed funding/COI (common in influence ecosystems).  
* **Wikipedia** as evidence (fine as a pointer, not a source-of-record).

---

### **E) Credible web source material (acceptable starting allowlist)**

These are **credible source families** typically acceptable under tradecraft standards, assuming you still apply the rubric and independence tests:

**1\) Government / official threat & definition baselines**

* **NATO** guidance on “information threats” and resilience functions. ([NATO](https://www.nato.int/en/what-we-do/wider-activities/natos-approach-to-counter-information-threats))  
* **EU/EEAS** strategic communications and disinformation definitions/policy framing (and explicit caveats about what is/isn’t an official position). ([European External Action Service](https://www.eeas.europa.eu/eeas/questions-and-answers-about-east-stratcom-task-force_en))  
* **National cyber/security authorities** that publish practical identification guidance (e.g., Canada’s Centre for Cyber Security guidance on MDM and deepfakes).  
* **Oversight bodies** describing state efforts/authorities and threat landscape (e.g., GAO reporting on definitions/detection efforts). ([GAO](https://www.gao.gov/products/gao-24-107600))

**2\) Standards for verification and correction discipline**

* **IFCN (Poynter) Code of Principles** as a benchmark for transparency and methodology in fact-checking. ([ifcncodeofprinciples.poynter.org](https://ifcncodeofprinciples.poynter.org/?utm_source=chatgpt.com))

**3\) Cognitive resilience / inoculation and “prebunking”**

* NATO StratCom COE work on **inoculation theory** and psychological resilience against misinformation. ([StratCom COE](https://stratcomcoe.org/publications/inoculation-theory-and-misinformation/217))  
* WHO’s “infodemic” framing (health domain, but useful for understanding harm mechanisms in overloaded information environments). ([World Health Organization](https://www.who.int/health-topics/infodemic/understanding-the-infodemic-and-misinformation-in-the-fight-against-covid-19?utm_source=chatgpt.com))

---

## **References (numbered, with URLs in code block)**

\[1\] Pherson, R. H., & Heuer, R. J. (2013). *Structured Analytic Techniques for Intelligence Analysis* (3rd ed.).  
\[2\] Heuer, R. J. (1999). *Psychology of Intelligence Analysis*.  
\[3\] NATO. (2025, February 3). *NATO’s approach to counter information threats*. ([NATO](https://www.nato.int/en/what-we-do/wider-activities/natos-approach-to-counter-information-threats))  
\[4\] European External Action Service. *Questions and Answers about the East StratCom Task Force*. ([European External Action Service](https://www.eeas.europa.eu/eeas/questions-and-answers-about-east-stratcom-task-force_en))  
\[5\] EUvsDisinfo / East StratCom Task Force. *EUvsDisinfo (About / homepage; FIMI explained listing)*. ([EUvsDisinfo](https://euvsdisinfo.eu/about/?utm_source=chatgpt.com))  
\[6\] Canadian Centre for Cyber Security. (2024, May). *How to identify misinformation, disinformation and malinformation (ITSAP.00.300)*.  
\[7\] International Fact-Checking Network (IFCN), Poynter. *IFCN Code of Principles*. ([ifcncodeofprinciples.poynter.org](https://ifcncodeofprinciples.poynter.org/?utm_source=chatgpt.com))  
\[8\] World Health Organization. *Infodemic / misinformation resources*. ([World Health Organization](https://www.who.int/health-topics/infodemic/understanding-the-infodemic-and-misinformation-in-the-fight-against-covid-19?utm_source=chatgpt.com))  
\[9\] U.S. Government Accountability Office. (2024, September 26). *Foreign Disinformation: Defining and Detecting Threats (GAO-24-107600)*. ([GAO](https://www.gao.gov/products/gao-24-107600))  
\[10\] Roozenbeek, J., & Van der Linden, S. (2021). *Inoculation Theory and Misinformation*. NATO StratCom COE. ([StratCom COE](https://stratcomcoe.org/publications/inoculation-theory-and-misinformation/217))

\[3\] https://www.nato.int/en/what-we-do/wider-activities/natos-approach-to-counter-information-threats

\[4\] https://www.eeas.europa.eu/eeas/questions-and-answers-about-east-stratcom-task-force\_en

\[5\] https://euvsdisinfo.eu/about/

\[5b\] https://euvsdisinfo.eu/

\[6\] https://www.cyber.gc.ca/sites/default/files/misinformation-mesinformation-itsap.00.300-en.pdf

\[7\] https://ifcncodeofprinciples.poynter.org/

\[8\] https://www.who.int/health-topics/infodemic/understanding-the-infodemic-and-misinformation-in-the-fight-against-covid-19

\[9\] https://www.gao.gov/products/gao-24-107600

\[10\] https://stratcomcoe.org/publications/inoculation-theory-and-misinformation/217

