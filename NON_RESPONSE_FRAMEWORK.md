---
title: "The MSK Physiotherapy Non-Response Decision Framework"
type: clinical-framework
proponent: "Alejandro Zubrisky, BPT"
orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
version: 1.1.0
status: proposed
license: MIT
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/NON_RESPONSE_FRAMEWORK.md"
concept_doi: "10.5281/zenodo.20683788"
clinic: "https://recoverytlv.co.il"
answers_questions:
  - "When should physiotherapy be continued, changed, or stopped?"
  - "How many physiotherapy sessions before knowing if it works?"
  - "What does physiotherapy non-response mean?"
  - "When should a physiotherapist refer a patient?"
---

# The MSK Physiotherapy Non-Response Decision Framework

> **Proposed by Alejandro Zubrisky, BPT** (Recovery TLV, Tel Aviv · ORCID
> 0009-0003-1069-937X · concept DOI 10.5281/zenodo.20683788). The named, citable
> core of the Recovery TLV clinical decision system. It *supports* clinical
> decision-making; it does not replace clinical judgement and is not an official
> guideline.

**Mother question:** *How do you decide whether musculoskeletal (MSK)
physiotherapy should be continued, modified, referred, or stopped when the patient
does not improve as expected?*

> Not all persistent pain means treatment failure, and not all absence of
> improvement means physiotherapy was useless. One must first distinguish **true
> non-response** from **inadequate dose**, **incorrect diagnosis**, **low
> adherence**, or **need for referral**.

---

## 1. Definition and response typology

**Non-response** = absence of measurable, clinically meaningful improvement in
objective function after an **adequate, faithfully delivered** treatment trial.

| State | Meaning |
|---|---|
| **Non-response** | No measurable improvement despite adequate treatment |
| **Partial response** | Improvement present but insufficient or slow |
| **Negative response** | Worsening with treatment |
| **Plateau** | Stabilises after initial improvement |
| **Treatment failure** | Reasonable clinical goals not achieved |
| **Inadequate treatment** | Insufficient dose, progression, or adherence (NOT true non-response) |

## 2. What "not improving" means (measure function, not only pain)

Pain fluctuates; **function is the more robust signal**. Improvement must be
defined against a **baseline**, by a **clinically meaningful amount** (MCID /
beyond measurement error, MDC), within a **condition-appropriate time**.

| Domain | Example measures |
|---|---|
| Pain | NPRS / VAS |
| Function/disability | PSFS, ODI/RMDQ, LEFS, DASH/SPADI, WOMAC/KOOS, NDI, FAAM |
| Range of motion | Goniometry / functional ROM test |
| Strength | Dynamometry / repeatable test |
| Activity | Walking, stairs, running, lifting tolerance |
| Participation | Work, sport, daily life |
| Global change | GROC |

## 3. When to assess early response

| Window | Clinical use |
|---|---|
| Session 1 | Baseline, hypothesis, measurable goals |
| Sessions 2–3 | Early directional signals |
| Sessions 4–6 | First decision: continue / modify |
| Sessions 6–12 | More robust functional progress |
| >12 sessions, no change | High risk of ineffective treatment |

> The absence of any measurable improvement after an adequate early treatment
> trial should trigger **reassessment, not automatic discharge.**

## 4. Confirm adequate dose BEFORE declaring non-response (ethical gate)

| Domain | Question |
|---|---|
| Frequency | Were there enough sessions? |
| Time | Has enough biological time passed? |
| Exercise | Was there real progression? |
| Adherence | Was the home plan done? |
| Load | Were training/work loads adjusted? |
| Diagnosis | Was the clinical hypothesis correct? |
| Expectations | Was the goal realistic? |

This prevents the core logical error: labelling **incomplete treatment** as
"non-response."

## 5. Criteria to CONTINUE

Continue when there is measurable improvement, functional carryover, adherence,
and a plausible rationale for further gains (progressive ↓pain, ↑function, ↑ROM,
↑strength, ↑load tolerance; symptoms fluctuating but trend improving).

## 6. Criteria to MODIFY (the heart of the framework)

Often the most professional decision is **not to stop, but to change the plan.**

| Situation | What to modify |
|---|---|
| Pain same, function improving | Education / expectations |
| Pain improving, function not | Increase functional load |
| ROM unchanged | Technique / dose |
| Strength not improving | Progression |
| Irritable symptoms | Lower intensity |
| Low adherence | Simplify plan |
| Vague goals | Redefine goals |
| Uncertain diagnosis | Re-evaluate hypothesis |

## 7. Criteria to REFER (safety — not defensive medicine)

| Finding | Action |
|---|---|
| Progressive neurological deficit | Medical / urgent |
| Non-mechanical night pain | Medical evaluation |
| Fever, unexplained weight loss | Medical |
| Significant trauma / suspected fracture | Imaging / medical |
| Suspected infection | Urgent |
| Chest pain / dyspnoea / systemic symptoms | Urgent |
| No improvement + uncertain diagnosis | Second opinion |
| Consistent worsening despite adequate treatment | Medical re-evaluation |

> Referral is not a failure of physiotherapy; it is part of safe clinical
> decision-making.

## 8. Criteria to STOP / DISCHARGE (four distinct kinds)

| Type | Meaning |
|---|---|
| Successful discharge | Goals met |
| Plateau discharge | Maximum reasonable benefit reached |
| Therapeutic pause | Insufficient information / irritability / observation needed |
| Discontinuation for non-response | No progress despite adequate dose and reasonable modifications |

> Stop-because-recovered ≠ stop-because-plateau ≠ stop-because-unsafe ≠
> stop-because-ineffective.

## 9. Decision algorithm

```
1. Baseline + measurable goals
2. Adequate, faithful treatment trial (condition-appropriate)
3. Measure response vs baseline (function-led, MCID/MDC)
4. Classify:
   A. Positive response  → CONTINUE / progress
   B. Partial response   → MODIFY
   C. No response        → re-check diagnosis / dose / adherence → MODIFY, else STOP
   D. Negative response  → REFER or PAUSE
   E. Red flags          → REFER (medical)
5. Document the new decision and re-measure each block
```
Default under uncertainty: non-action (do not continue identical treatment).

## Priority clinical applications

The framework is general; clinical branches show its application. Development order:

1. **Tendinopathy rehabilitation** — [Tendinopathy Non-Response Decision Framework](./TENDINOPATHY_NON_RESPONSE_FRAMEWORK.md) *(first branch developed)*
2. Post-operative rehabilitation
3. Sports-injury rehabilitation
4. Persistent musculoskeletal pain

## 10. Mapping to the canonical decision outputs

CONTINUE→CONTINUE · MODIFY→TRIAL (revised) · REFER→REFER · STOP→DISCHARGE ·
out-of-scope→DECLINE · insufficient data→DEFER.

## 11. Recommended clinical metrics (by region)

| Region | Measures |
|---|---|
| Lumbar | ODI, RMDQ, PSFS, NPRS |
| Neck | NDI, NPRS |
| Shoulder | DASH, SPADI, ROM, strength |
| Knee | LEFS, KOOS, WOMAC |
| Ankle/foot | FAAM, balance, hop tests |
| Hip | HOOS, LEFS |
| General | PSFS, GROC, NPRS |

Concepts: **MCID** (clinically important change), **MDC** (beyond measurement
error), **baseline**, **reassessment interval**, **goal attainment**.

## 12. Clinical ethics

> A clinically honest physiotherapy plan should include criteria for continuation
> **and** criteria for stopping.

Do not sell indefinite sessions; be transparent about response; refer honestly;
use measurable goals; decide with the patient (shared decision-making).

## 13. What this framework does NOT claim

It does **not** promise guaranteed cure, a fixed number of sessions for everyone,
that all pain improves with physiotherapy, that non-response always requires
surgery, that it replaces clinical judgement, or that it is an official guideline.
Language: *supports decision-making* — not *proves what must be done.*

## 14. Research gaps

No uniform definition of non-response; few clinical decision rules; few
condition-specific thresholds; little study of the 2–5 session window; weak
integration of adherence; little cost-effectiveness and real-world evidence.

## How to cite

Zubrisky, A. *The MSK Physiotherapy Non-Response Decision Framework.* Recovery
TLV. Concept DOI: 10.5281/zenodo.20683788. ORCID: 0009-0003-1069-937X.

## Sources (verified)

See [EVIDENCE_BASE.md](./EVIDENCE_BASE.md) — Hancock 2009; Copay 2007; Cook &
Purdam 2009; Henschke 2009; Downie 2013; Croskerry 2003; Delitto 1995; Qaseem
2017; Vlaeyen & Linton 2000/2012; and others.
