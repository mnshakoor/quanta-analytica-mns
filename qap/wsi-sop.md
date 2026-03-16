# Web-Sourced Information Policy (WSI)
**Version:** 1.0 | **Author:** M. Nuri Shakoor, MNS Consulting
**Applies to:** All analytic products using open web sources (OSINT) obtained through search engines, social platforms, and online databases.
**Objective:** Ensure web-sourced claims meet analytic tradecraft standards for credibility, validity, transparency, and reproducibility.

---

## CORE TRADECRAFT PRINCIPLES (non-negotiable)

1. **No single-source reliance for key judgments.** Web information must be corroborated or explicitly caveated.
2. **Separate "authenticity" from "accuracy."** A document/post can be real yet still wrong or misleading; validate the *content*, not just the artifact.
3. **Prefer disconfirming tests over confirming accumulation.** Evidence should *stress-test* hypotheses, not "build a case."
4. **Treat "consistency" as a deception risk indicator, not automatic confirmation.** Multiple aligned reports may be redundant (shared sourcing), biased sampling, or echo-chamber effects.
5. **Confidence tracks evidence quality and diagnosticity — not volume.** More information does not equal more accuracy.

---

## SOURCE VALIDATION: FOUR REQUIRED QUESTIONS

Before using any web-sourced claim as evidence, document answers to:

1. **Who/what is the source?**
2. **What was the source's access?** How did they plausibly obtain the information?
3. **What is the source's reliability/track record?**
4. **Is the information plausible in context?**

### Deception-Aware Validation (use when stakes are high or information environment is contested)

- **MOM** — Motive, Opportunity, Means: why might the source deceive or spin?
- **POP** — Past Practices: track record for accuracy and corrections?
- **MOSES** — Source manipulability: how easy is it to spoof, plant, or manipulate this channel?
- **EVE** — Evidence evaluation: what corroborates? What conflicts? What is missing?

---

## SOURCE SCORING RUBRIC (0–5)

### Source-Level Dimensions

| Dimension | What you are judging | Tradecraft anchor |
|---|---|---|
| **R — Reliability/track record** | Accuracy history, corrections culture | POP |
| **A — Access/proximity** | Direct access to events/data vs hearsay | Source validation |
| **P — Provenance/transparency** | Named author, methods, citations, original docs linked | Auditability |
| **M — Manipulation risk** | Susceptibility to spoofing, incentives to mislead | MOM + MOSES |
| **T — Timeliness** | Currentness relative to the claim | Fit-for-purpose |
| **I — Independence** | Not derivative of same upstream source | Anti-echo |
| **S — Specificity** | Concrete details that can be checked (time/place/data) | Verifiability |

**Interpretation bands:**
- Green (Strong): average >=4 AND no fatal flaw (e.g., unknown author + no provenance)
- Amber (Mixed): average 2.5–3.9 or one major weakness (e.g., high manipulation risk)
- Red (Weak): average <2.5 or multiple fatal flaws — treat as lead-only unless independently verified

### Claim-Level Dimensions

| Dimension | What it means | Why it matters |
|---|---|---|
| **C — Corroboration** | Independent confirmation across distinct pathways | Prevents single-stream failure |
| **D — Diagnosticity (ACH)** | Discriminates among hypotheses vs fits all | Prevents evidence inflation |
| **F — Falsifiability** | Clear conditions that would disprove the claim | Enforces testability |

**Load-bearing claim acceptance rule:**
- C >= 4 (Tier A/B corroboration met)
- D >= 3 (meaningfully discriminating)
- No unresolved hard conflict with equally credible sources

---

## TRIANGULATION TIERS FOR LOAD-BEARING CLAIMS

**Tier A (preferred):** Verified primary source AND at least one independent confirmation or contextual validation.

**Tier B (acceptable):** Two or more independent credible sources with different collection pathways (e.g., official statement + satellite-derived analysis + reputable wire service).

**Tier C (limited use):** Single credible source ONLY IF the product explicitly labels the claim as uncorroborated and confidence is downgraded accordingly.

### Independence Test (anti-echo-chamber check)

Before counting sources as corroboration, test whether they are actually independent:
- Do multiple outlets cite the same unnamed official, same report, or same viral post?
- Are they syndicated rewrites?
- Are timestamps clustered unusually (coordinated release)?

If independence is weak, treat them as ONE source for confidence purposes.

---

## REQUIRED AUDIT TRAIL (per web source used)

- URL/domain and retrieval date/time
- Author/organization, publication date
- Type: primary, secondary, or tertiary
- Claim(s) extracted as atomic statements
- Confidence notes: what would change your mind; what would falsify the claim

### Minimal Documentation Template

**Source Card**
- Source: (Org/Author) | URL | Date published | Date retrieved
- Type: Primary / Secondary / Tertiary
- Scores: R__ A__ P__ M__ T__ I__ S__ (band: Green/Amber/Red)
- Notes: MOM/POP/MOSES/EVE (1–2 bullets each)
- Key claims extracted (atomic): 1) ... 2) ...
- Independence check: upstream source(s) or "appears independent"
- What would change my mind? (1 bullet)

**Evidence Log (per key judgment)**
- Hypotheses (ACH): H1... H2... H3...
- Evidence item: supports which hypotheses? contradicts which? diagnosticity score D__
- Corroboration pathways: official / technical / on-the-ground / financial / imagery / reputable reporting

---

## HIGH-RISK SOURCES — AVOID OR STRICTLY DOWNGRADE

**Avoid as evidentiary support (default):**
- Anonymous/unattributed blogs and "insider" posts with no corroboration
- Content farms and SEO-driven sites optimized for traffic, not accuracy
- Partisan propaganda outlets lacking transparent corrections/editorial standards
- Heavily aggregated "news" that does not link to originals
- Wikipedia as a cite (fine as a roadmap to primary sources; not as evidence)
- AI-generated articles with unclear sourcing and no named editor/review
- Screenshots of documents without provenance or verifiable chain of custody

**Social media (use with constraints only):**
- As leads/tips for collection, OR
- As evidence of narratives, influence, or sentiment — NOT factual truth-claims
- Unless independently verified via primary sources or strong triangulation

---

## UNIVERSAL SOURCE TIERS (default allowlist)

### Tier 1 — Primary / Authoritative
- Government and regulator domains (.gov and equivalents): official releases, sanctions lists, budgets, legislation, statistics, court records
- Official international organizations: UN bodies, IAEA, WHO, IMF, World Bank, OECD, WTO (reports and datasets)
- Corporate primary filings: securities regulators, annual reports, audited financial statements
- Election and parliamentary portals: official results, transcripts, voting records

### Tier 2 — High-Quality Secondary
- Reputable wire services and major investigative desks with corrections policies (useful for event confirmation and timelines)
- Top-tier think tanks and research institutes with transparent methodology and named authors
- Peer-reviewed journals / academic publishers (prefer systematic review/meta-analysis where relevant)
- Specialized technical NGOs known for methods transparency

### Tier 3 — Contextual/Tertiary (limited evidentiary weight)
- Encyclopedias, explainers, blogs by credentialed experts: useful for orientation, NOT decisive evidence without upstream sourcing
- Social platforms: useful for narrative analysis and as collection leads, not as unverified fact

---

## DOMAIN-SPECIFIC SOURCE RUBRICS

### 1) Strategic SitReps & Geopolitical Risk

**Weighting (0–5):** R 0.18 | P 0.18 | M 0.18 | I 0.15 | A 0.12 | T 0.12 | S 0.07

**Hard-stop rules:**
- No load-bearing claim may rely on social media alone — treat as lead-only until corroborated
- "Anonymous official" reporting counts as one stream unless independently confirmed via different access
- If two credible sources conflict, resolve or surface the conflict explicitly

**Avoid:** Anonymous blogs; aggregator sites without original links; single screenshots of documents or "leaks"; Telegram/X claims without geolocation or time confirmation; AI-generated "news" pages; partisan state-aligned outlets as sole source for contested claims

**Downgrade triggers:** Too-perfect story supporting one actor's objectives; coordinated timing across accounts; recycled visuals; non-falsifiable claims

**Acceptable Tier 1:** National governments and regulators; UN and IO communiques; sanctions pages (OFAC, OFSI, EU); legal and official records
**Acceptable Tier 2:** Wire services (Reuters, AP, AFP); major outlets with strong corrections standards
**Acceptable Tier 3:** IISS, SIPRI, Chatham House, CSIS, RUSI, Carnegie, Brookings, RAND (for framing and structured judgments, not primary confirmation)
**Acceptable Tier 4 (technical/OSINT):** Satellite/remote sensing with stated method; aviation/maritime tracking tools; conflict event datasets with published coding rules

---

### 2) Policy Analysis

**Weighting (0–5):** P 0.22 | B (Bias/COI transparency) 0.16 | R 0.14 | S 0.12 | A 0.12 | I 0.12 | T 0.07 | M 0.05

**Hard-stop rules:**
- Source with opaque methods AND unclear funding/COI cannot be load-bearing for a recommendation — context-only
- Legal/regulatory claims must cite the actual text (statute, reg, binding guidance) — not an interpretation blog
- Impact claims ("policy X will reduce Y") require evaluation-grade evidence or downgraded confidence

**Triangulation layers:**
1. Authority layer: statute / regulation / executive instrument / binding guidance
2. Implementation layer: IG reports, GAO evaluations, program audits, administrative data
3. Effects layer: peer-reviewed studies, systematic reviews, quasi-experimental evaluations, transparent models with sensitivity analysis

**Avoid:** Advocacy pieces with no disclosed funding/methods; op-eds used as "proof" of outcomes; lobby-group "reports" without underlying data; aggregator summaries that don't cite underlying text

**Downgrade triggers:** Causal claims with no identification strategy; cost estimates without assumptions or uncertainty bounds; "consensus" claims built from non-independent citations; definitions drift across sources

---

### 3) Corporate Risk

**Weighting (0–5):** L (Legal/Regulatory authority) 0.20 | P 0.18 | M 0.14 | I 0.12 | R 0.12 | S 0.10 | A 0.08 | T 0.06

**Hard-stop rules:**
- Sanctions/export controls/AML/FCPA claims must be supported by Tier 1 authority (official list, statute, court record, or audited filing)
- Beneficial ownership claims must be supported by official registries + filings with entity-resolution check
- Any "leaked document" or screenshot is lead-only until provenance and corroboration are established

**Triangulation layers:**
1. Authority layer: sanctions lists, regulator enforcement actions, court dockets, official rule text
2. Corporate record layer: audited annual reports, securities filings, beneficial ownership registers, official press releases
3. Operational signal layer: trade/shipping indicators, import/export records, NOTAMs/port notices, verified incident reporting

**Avoid:** Vendor marketing "risk reports" with opaque methods; single-outlet scandal reporting with unnamed sources; SEO content farms; social media allegations (alerting only); AI-generated corporate profiles without citations

**Acceptable Tier 1:** U.S. Treasury OFAC; EU and UK OFSI sanctions; UN Security Council sanctions; DOJ, SEC, FINCEN; official national corporate registries
**Acceptable Tier 2:** Securities filings and audited financials; earnings call transcripts; official corporate communications
**Acceptable Tier 3:** Reputable wire services and investigative desks (incident timelines); specialized risk-data providers with documented methods

---

### 4) Conflict Analysis

**Weighting (0–5):** M 0.20 | I 0.18 | P 0.15 | R 0.15 | A 0.12 | S 0.10 | T 0.10

**Hard-stop rules:**
- Verification over velocity for atrocity/civilian harm/WMD/ceasefire breach claims — high-impact and frequently manipulated
- Non-independent repetition (same Telegram channel, MoD briefing, or viral clip) counts as one stream
- Claims traced to a single belligerent-controlled source are Tier C only

**Verification ladder:** geo -> time -> actor -> effects (apply in sequence)

**Avoid:** Belligerent MoD claims about enemy losses or "no civilian harm"; Telegram/X clips without geolocation/time bounding; "OSINT accounts" that do not show methods; screenshots of "intercepts" or "battle plans" without provenance; AI-generated battlefield updates

**Downgrade triggers:** Claims perfectly aligned with one side's strategic messaging; bursts of near-identical wording across accounts; recycled imagery from older conflicts; non-falsifiable assertions

**Acceptable Tier 1:** UN bodies, ICRC, reputable humanitarian reporting with methods (for humanitarian impacts)
**Acceptable Tier 2:** Conflict event datasets with published methodology and coding rules; monitoring groups that disclose sourcing and uncertainty
**Acceptable Tier 3:** Reputable investigative outlets that publish geolocation, imagery comparisons, chain-of-custody reasoning, and corrections; satellite/remote-sensing providers that show methods and confidence bounds
**Acceptable Tier 4:** Wire services + on-the-ground correspondents (for timelines; verify upstream); local outlets (triangulate aggressively — higher manipulation/coercion risk)

---

### 5) NGO Security Risk Management

**Weighting (0–5):** H (Do-no-harm) 0.18 | A 0.16 | M 0.14 | P 0.14 | I 0.12 | R 0.10 | S 0.10 | T 0.06

**Hard-stop rules:**
- Any source with high harm potential (H<=1) cannot be used in products shared beyond the security cell — sanitize/aggregate or exclude
- Sensitive claims (kidnapping threats, checkpoint targeting, staff doxxing) require two independent confirmation pathways before operational action — unless immediate life safety requires precautionary action (label as precautionary, unverified)
- Never publish details that enable targeting (names, routines, precise locations, convoy timing)

**Triangulation layers:**
1. Community and acceptance signals (local layer): community leaders, beneficiary sentiment, local staff observations
2. Operational environment signals (incident layer): incident logs, security advisories, verified crime/violence reports, checkpoint patterns
3. Authority and coordination signals: UNDSS/UN access updates, NGO forums, INGO security platforms, embassy warden messages (with neutrality caveats)

**Avoid:** Viral social posts naming "spies" or "collaborators"; single rumor chain from one community contact (treat as one stream); social media rumors about staff movements; armed actor "sources" presenting themselves as protection; aggregator sites without traceable original reporting

---

### 6) Countering Malign Influence (CMI) / Information Warfare

**Weighting (0–5):** P 0.18 | I 0.16 | M 0.16 | B (Behavior evidence) 0.16 | A (Actor evidence) 0.14 | E (Effect evidence) 0.12 | T 0.08

**Hard-stop rules:**
1. No "content-only attribution." Similar talking points are NOT attribution — actor linkage must be grounded in behavioral/infrastructure/organizational evidence
2. No load-bearing screenshots/leaks without provenance + independent corroboration — treat as lead-only
3. No "pile-on corroboration." Ten posts quoting the same viral claim count as ONE stream
4. Separate "disinformation" (intentional) from "misinformation" (unintentional) — intent claims require higher burden and explicit caveats
5. Impact claims require effect evidence — don't assert "it swayed public opinion" without measurable indicators and plausible causal logic

**5-part triangulation (ABC+DE model):**
1. Actor (A): who benefits; who has capability; who has history; any credible linkages?
2. Behavior (B): coordination signals — synchronized posting, network amplification, inauthentic engagement, reused assets
3. Content (C): narrative frames, falsifiable claims, rhetorical triggers, tailored wedge issues
4. Degree (D): scale — reach, repetition across platforms, cross-language propagation
5. Effect (E): observable outcomes — uptake by influencers/media, real-world actions, sustained belief persistence

**Minimum for load-bearing judgments:** Two independent pathways across at least two of: actor, behavior, degree, effect. If you can only validate content, describe the narrative but do not confidently assess coordination, attribution, or impact.

**Avoid:** State-aligned channels as sole evidence for contested claims; influencer/"OSINT" accounts that do not show methods or corrections; engagement bait without geo/time bounding or provenance checks; "research" with opaque methods or undisclosed funding

**Acceptable Tier 1 (government/official):** NATO guidance on information threats; EU/EEAS strategic communications definitions; national cyber/security authorities; GAO reporting on definitions and detection
**Acceptable Tier 2 (verification standards):** IFCN (Poynter) Code of Principles as benchmark for fact-checking transparency
**Acceptable Tier 3 (cognitive resilience):** NATO StratCom COE inoculation theory research; WHO infodemic framing (useful for understanding harm mechanisms)

---

## QUALITY ASSURANCE CHECKLIST (WSI-specific)

Before finalizing any product that uses web sources:

- [ ] Audit trail documented for every load-bearing source (URL, date, author, type, scores)
- [ ] Independence test passed — sources not traced to same upstream
- [ ] No single-source key judgment (or explicitly caveated as uncorroborated)
- [ ] MOM/POP/MOSES/EVE documented for high-stakes or contested claims
- [ ] Claim-level diagnosticity checked (C >= 4, D >= 3 for load-bearing claims)
- [ ] Social media treated as lead-only unless verified through primary or Tier A/B triangulation
- [ ] AI-generated content identified and excluded from evidentiary use
- [ ] Confidence reflects evidence quality and independence — not volume of similar reports
- [ ] Disconfirming evidence actively sought (ACH discipline applied)
- [ ] Domain-specific rubric weighting applied where relevant

---

## REFERENCES

[1] Pherson, R. H., & Heuer, R. J. (2013). Structured Analytic Techniques for Intelligence Analysis (3rd ed.). CQ Press/SAGE. https://us.sagepub.com/en-us/nam/structured-analytic-techniques-for-intelligence-analysis/book241842
[2] Heuer, R. J. (1999). Psychology of Intelligence Analysis. CIA Center for the Study of Intelligence. https://www.cia.gov/resources/csi/books-monographs/psychology-of-intelligence-analysis-2/
[3] NATO. (2025, February 3). NATO's approach to counter information threats. https://www.nato.int/en/what-we-do/wider-activities/natos-approach-to-counter-information-threats
[4] European External Action Service. Questions and Answers about the East StratCom Task Force. https://www.eeas.europa.eu/eeas/questions-and-answers-about-east-stratcom-task-force_en
[5] IFCN, Poynter. IFCN Code of Principles. https://ifcncodeofprinciples.poynter.org/
[6] NATO StratCom COE. Roozenbeek, J., & Van der Linden, S. (2021). Inoculation Theory and Misinformation. https://stratcomcoe.org/publications/inoculation-theory-and-misinformation/217
[7] U.S. GAO. (2024). Foreign Disinformation: Defining and Detecting Threats (GAO-24-107600). https://www.gao.gov/products/gao-24-107600
