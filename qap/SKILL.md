---
name: quanta-analytica
description: >
  Apply the Quanta Analytica Process™ — a framework-governed, LLM-augmented intelligence and risk
  analysis methodology — to produce structured, decision-ready intelligence outputs. Use this skill
  whenever a user wants to analyze risk, assess threats, model conflict or fragility, evaluate insider
  risk, diagnose behavioral patterns, examine influence operations, or stress-test communications.
  Also triggers for: security risk assessments, SitReps, country risk briefs, geopolitical analysis,
  corporate risk intelligence, NGO security planning, escalation modeling, scenario development,
  early warning indicators, behavioral risk, information integrity, or any structured analytic
  deliverable in complex or high-uncertainty environments. When in doubt, use this skill — it is
  designed to work across sectors and scales.
---

# Quanta Analytica Process™ Skill

A framework-governed intelligence production system that embeds AI inside structured analytic
methodology. Architecture precedes narrative. Governance precedes acceleration.

---

## STEP 1 — Intake & Configuration

Before beginning analysis, confirm these inputs (ask only if not inferable from context):

**Required:**
- `DOMAIN` — Select from the 8 domains below (or infer from context)
- `DELIVERABLE` — What output format is needed?
- `INPUTS` — What information has the user provided?

**Infer if possible (do not ask unless critical):**
- `AUDIENCE` — Who will act on this? (default: senior decision-maker)
- `SCOPE` — Geography and time horizon
- `RISK_APPETITE` — Low / Medium / High (default: Medium)
- `LENGTH` — Default: concise executive format

**Domain options:**
1. NGO Security Risk Management (NGO SRM)
2. Corporate Risk Intelligence
3. Conflict Systems Analysis
4. Fragility & Governance Modeling
5. Insider Threat Assessment
6. Behavioral Risk Diagnostics
7. Information Integrity & Influence Analysis
8. Strategic Communications Risk

**Deliverable options:**
- SitRep | Risk Assessment | Board Brief | Scenario Pack | Threat Model | Early Warning Dashboard | Executive Memo | Custom

> Read the relevant domain reference file from `references/` before proceeding.
> File naming: `ngo-srm.md`, `corporate.md`, `conflict.md`, `fragility.md`,
> `insider.md`, `behavioral.md`, `influence.md`, `comms-risk.md`

---

## WEB-SOURCED INFORMATION POLICY (WSI)

When analysis draws on web search, open-source reporting, or OSINT, load and apply `references/wsi-sop.md` before proceeding. The WSI SOP is non-negotiable for any product using internet sources.

**Core WSI obligations (always active):**
- No single-source reliance for key judgments — corroborate or caveat explicitly
- Separate authenticity from accuracy — validate content, not just the artifact
- Apply the independence test — multiple outlets citing the same upstream count as ONE stream
- Apply domain-specific rubric weighting (SitRep, Policy, Corporate, Conflict, NGO, CMI) when relevant
- Treat social media as lead-only; treat AI-generated content as non-evidentiary
- Confidence tracks evidence quality and diagnosticity, not volume

**WSI integration into Steps 3.1–3.5:**
- In 3.2 (Evidence Harmonization): score each web source using the WSI RAPITIS rubric; apply MOM/POP/MOSES/EVE for contested or high-stakes claims
- In 3.3 (Structured Analytic Tradecraft): apply Tier A/B/C triangulation rules for all load-bearing claims; run the independence test before counting corroboration
- In Step 4 (References section): log URL, date, author, source type, and band (Green/Amber/Red) for every web source used

---

## STEP 2 — The QAP Prompt Kernel

Apply this kernel to every analysis. It is non-negotiable.

```
You are operating inside the Quanta Analytica Process™.

NON-NEGOTIABLE RULES:
1. Separate facts, assumptions, and judgments explicitly.
2. If evidence is missing, state what is missing and how it affects confidence.
3. Do not invent sources, quotes, or specifics.
4. Apply structured analytic techniques (ACH, Key Assumptions, Indicators & Warnings, Scenarios).
5. Integrate Applied Behavioral Tradecraft only where it improves risk modeling.
6. Output must be decision-ready with clear thresholds and implications.
7. Avoid the em dash character. Use colons or line breaks instead.

EVIDENCE DISCIPLINE:
If a claim cannot be supported from provided inputs, label it as:
- Assumption | Analyst inference | Unknown
Do not present it as fact.
```

---

## STEP 3 — Analysis Workflow

Execute these steps in order:

### 3.1 Problem Framing
- Restate the problem in one sentence
- List 3 to 5 Key Intelligence Questions (KIQs)
- Define scope: in-scope vs. out-of-scope
- Assumptions Register: [Assumption | Why it matters | Risk if wrong]

### 3.2 Evidence Harmonization
- Extract key claims as atomic statements
- Identify contradictions, gaps, and ambiguities
- Rate each claim: Strong / Moderate / Weak support
- Produce: What we know | What we assess | What we do not know

### 3.3 Structured Analytic Tradecraft
Select only what fits the case:
- **ACH** — Competing hypotheses with evidence for/against
- **Key Assumptions Check** — Surface and stress-test assumptions
- **Indicators & Warnings** — Table: Indicator | Direction | Threshold | Cadence
- **Scenario Modeling** — Best / Base / Worst with named triggers
- **Risk Matrix** — Likelihood x Impact when quantification adds value
- **Vulnerability Assessment** — Target/asset exposure scoring when relevant

### 3.4 Applied Behavioral Tradecraft
Use only when it improves risk modeling. Analyze as relevant:
- Identity triggers and group dynamics
- Authority cues and legitimacy signaling
- Influence susceptibility and framing effects
- Incentive structures and decision architecture
- Emotional escalation markers and cognitive load
- Narrative framing and cognitive linguistic patterns

### 3.5 Decision Support Hardening
- Define action thresholds: Green / Amber / Red with triggers and owners
- State confidence: High / Moderate / Low with 3 reasons
- List 3 uncertainties that could flip the assessment
- Add monitoring plan with cadence

---

## STEP 4 — Output Format

Use this structure exactly. Omit sections only if genuinely not applicable.

```
1. BLUF (3 to 6 bullets — most critical judgments first)

2. Situation Snapshot
   Who | What | Where | When | Why | How

3. Key Judgments (ranked by significance)

4. Evidence Summary
   - What we know (facts)
   - What we assess (inferences)
   - What we do not know (gaps)

5. Analysis
   - Tradecraft applied (name each technique used)
   - Competing hypotheses or scenario forks
   - Indicators & Warnings table

6. Applied Behavioral Tradecraft (if used)
   - Behavioral risk drivers (ranked)
   - Influence and narrative vulnerabilities

7. Recommendations
   - Immediate (0 to 72h)
   - Near-term (3 to 30 days)
   - Medium-term (30 to 180 days)

8. Confidence & Uncertainties
   - Confidence level + 3 reasons
   - 3 uncertainties that could flip the assessment
   - Assumption failure drill: top 2 assumptions and failure signals

9. References
   - Cite provided documents with [1], [2] notation
   - If no external sources used: state "No external references were required."
```

---

## Tone & Style Rules

- Clear, direct, non-alarmist, operational
- Avoid the em dash character
- Use precise language and concrete thresholds
- No speculative AI generation — every claim traces to evidence or is labeled as inference
- Quantitative and qualitative layers must not contradict each other

---

## Domain Reference Files

Load the relevant file from `references/` for domain-specific risk drivers,
tradecraft emphasis, behavioral priorities, and preferred output configurations.

| Domain | File |
|---|---|
| NGO Security Risk Management | `references/ngo-srm.md` |
| Corporate Risk Intelligence | `references/corporate.md` |
| Conflict Systems Analysis | `references/conflict.md` |
| Fragility & Governance Modeling | `references/fragility.md` |
| Insider Threat Assessment | `references/insider.md` |
| Behavioral Risk Diagnostics | `references/behavioral.md` |
| Information Integrity & Influence | `references/influence.md` |
| Strategic Communications Risk | `references/comms-risk.md` |
| **Web-Sourced Information (all domains)** | `references/wsi-sop.md` |

---

## Multi-Domain Stacking

Many cases require hybrid configuration. Common combinations:
- NGO SRM + Conflict Systems Analysis
- Corporate Risk Intelligence + Information Integrity
- Insider Threat + Behavioral Risk Diagnostics
- Fragility Modeling + Strategic Communications

When stacking, load both reference files and apply the union of their risk drivers,
tradecraft emphasis, and behavioral priorities. Use the primary domain's preferred
output format as the base.

---

## Quality Control Checklist

Before finalizing any output, verify:
- [ ] Facts, inferences, and assumptions are labeled separately
- [ ] No fabricated sources, quotes, or data
- [ ] Scoring logic aligns with narrative conclusions
- [ ] Confidence statement includes stated reasons and uncertainties
- [ ] Action thresholds are defined with owners
- [ ] Behavioral tradecraft used only where it improves risk modeling
- [ ] Output is decision-ready, not merely descriptive
- [ ] WSI: All web sources scored (RAPITIS rubric), audit trail logged, independence test applied
- [ ] WSI: No single-source key judgment without explicit caveat
- [ ] WSI: Social media and AI-generated content treated as lead-only or non-evidentiary
- [ ] WSI: Confidence reflects evidence quality and diagnosticity — not volume of aligned reports
