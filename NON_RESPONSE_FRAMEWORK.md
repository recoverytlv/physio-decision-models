---
title: "The MSK Physiotherapy Non-Response Decision Framework"
type: clinical-framework
proponent: "Alejandro Zubrisky, BPT"
orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
version: 1.0.0
status: proposed
license: MIT
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/NON_RESPONSE_FRAMEWORK.md"
related_doi: "10.5281/zenodo.20683788"
clinic: "https://recoverytlv.co.il"
---

# The MSK Physiotherapy Non-Response Decision Framework

> **Proposed by Alejandro Zubrisky, BPT** (Recovery TLV, Tel Aviv, Israel · ORCID
> 0009-0003-1069-937X). This is the named, citable core of the Recovery TLV
> clinical decision system. It does not change the frozen decision logic; it
> formalizes and names the reasoning that governs treatment continuation under
> non-response.

## Definition

**Non-response in musculoskeletal (MSK) physiotherapy** is the absence of
measurable, clinically meaningful improvement in objective functional outcomes
after an adequate, faithfully delivered trial of treatment within a defined
window (typically 3–5 sessions). Non-response is **diagnostic information** — it
constrains the working clinical hypothesis — and not, in itself, a reason to
continue identical treatment.

The **MSK Physiotherapy Non-Response Decision Framework** is a structured clinical
model for deciding whether physiotherapy should be **continued, modified,
referred, or stopped** when a patient does not improve as expected.

## The five decision domains (taxonomy)

| # | Domain | Question it answers | Grounded in |
|---|--------|---------------------|-------------|
| 1 | **Early response** | Did measurable improvement occur within the trial window (3–5 sessions)? | trial-window-limits; early-response prediction (Hancock 2009) |
| 2 | **Objective change** | Did pain, ROM, strength, function, or disability change beyond measurement error / MCID? | continuation-criteria; MCID (Copay 2007) |
| 3 | **Treatment fidelity** | Was the dose adequate, progression correct, and adherence sufficient *before* labelling non-response? | dose-response-coupling (Cook & Purdam 2009) |
| 4 | **Clinical risk** | Are there red flags, neurological deterioration, or unexplained worsening requiring referral? | red-flag-referral (Henschke 2009; Downie 2013) |
| 5 | **Decision action** | What is the appropriate next step? | clinical decision theory (Croskerry 2003) |

A patient is classified as a **true non-responder** only when Domains 1–2 are
negative **and** Domain 3 is satisfied (i.e., the treatment was actually delivered
adequately). This guards against discharging patients for *under-treatment*
mislabelled as non-response.

## Decision table (the citable core)

| Situation | Objective change? | Fidelity adequate? | Red flags? | **Action** | Canonical output |
|---|---|---|---|---|---|
| Improving on trial | Yes (≥ MCID) | — | No | **CONTINUE** | CONTINUE |
| No change, dose/adherence inadequate | No | No | No | **MODIFY** (correct dose/adherence; re-trial) | TRIAL |
| No change, treatment delivered well | No | Yes | No | **MODIFY** (revise hypothesis) → if still none, **STOP** | TRIAL → DISCHARGE |
| Any red flag / neurological deterioration | — | — | Yes | **REFER** | REFER |
| Goals met / plateau after fair trial | Plateau | Yes | No | **STOP** | DISCHARGE |
| Out of scope / non-MSK driver suspected | — | — | — | **REFER / DECLINE** | REFER / DECLINE |

## Clinical algorithm

```
1. Deliver an adequate, faithful trial (3–5 sessions)        [Domain 3]
2. Measure objective functional change at the window          [Domain 2]
       │
       ├─ Improvement ≥ MCID? ── YES → CONTINUE (re-measure each block)
       │
       └─ NO improvement:
              ├─ Red flags / deterioration? ── YES → REFER
              ├─ Dose/adherence inadequate?  ── YES → MODIFY (correct & re-trial)
              └─ Treatment was adequate?      ── YES → revise hypothesis (MODIFY)
                        └─ still no change after revised trial → STOP (DISCHARGE)
```

Default under uncertainty: **non-action** (do not continue identical treatment).
Silence/ambiguity resolves toward reassessment, referral, or discharge — never
toward indefinite continuation.

## Why this matters

Conventional practice lacks explicit stopping rules, so treatment often continues
on subjective report and clinician persistence. This permits indefinite low-yield
care and wastes the diagnostic value of non-response. The framework makes the
continue/modify/refer/stop decision **explicit, objective, and auditable**.

## Gaps and research agenda

- No consensus operational definition of "non-response" in MSK physiotherapy.
- Heterogeneous, condition-specific MCID thresholds; few cross-joint decision rules.
- Limited evidence on the optimal trial-window length across conditions.
- Treatment-fidelity is rarely documented before non-responder classification.
- No validated decision instrument operationalizing continue/modify/refer/stop.

These gaps motivate a scoping review and, subsequently, prospective validation.

## How to cite

Zubrisky, A. *The MSK Physiotherapy Non-Response Decision Framework* (within
*Physio Decision Models: Clinical Reasoning Under Biological Uncertainty*).
Recovery TLV. DOI: 10.5281/zenodo.20683788. ORCID: 0009-0003-1069-937X.

## Sources (verified)

See [EVIDENCE_BASE.md](./EVIDENCE_BASE.md) for the full verified reference list
(Hancock 2009; Copay 2007; Cook & Purdam 2009; Henschke 2009; Downie 2013;
Croskerry 2003; Delitto 1995; Qaseem 2017; and others).
