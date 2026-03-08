---
name: clinical-decision-system
description: Formal clinical decision system for physiotherapy under biological uncertainty. Use this skill when building health applications, clinical decision support tools, physiotherapy software, patient management systems, or any system that needs structured clinical reasoning with explicit treatment boundaries and exit criteria. Triggers on tasks involving clinical decision logic, treatment planning, patient evaluation workflows, or rehabilitation software.
license: MIT
metadata:
  author: recoverytlv
  version: "1.1.0"
---

# Recovery TLV — Clinical Decision System for Physiotherapy

A formal epistemic framework for clinical reasoning that treats physiotherapy as a continuous adaptive decision system. Every patient case must terminate with exactly one of six valid outputs.

Source: https://github.com/recoverytlv/physio-decision-models

## Canonical Decision Outputs (Closed Set)

Every case MUST terminate with exactly one of these outputs. No other outputs are valid.

| Output | Definition | Trigger Condition |
|---|---|---|
| **DECLINE** | Case rejected — not accepted into the system | Out-of-scope, contraindication, legal or ethical restriction |
| **DEFER** | Decision postponed — no action taken | Insufficient data, acute phase, unresolved uncertainty |
| **REFER** | Transferred to another professional domain | Red flags, non-musculoskeletal cause, specialist requirement |
| **TRIAL** | Conditional, time-limited acceptance (3–5 sessions) | All provisional inclusion criteria satisfied |
| **CONTINUE** | Extension of active treatment plan | Objective functional progress demonstrated |
| **DISCHARGE** | Termination — goals achieved or progress failure | Functional goals met or plateau reached |

No intermediate, hybrid, or implied outputs are permitted.

## Core Principles

1. **Interventions are hypothesis tests** — controlled perturbations designed to probe hypothesis viability, not routines to repeat indefinitely.
2. **Non-response is diagnostic data** — absence of improvement constrains the hypothesis space more strongly than partial improvement.
3. **Uncertainty favors non-action** — when in doubt, default to DECLINE or DEFER. Optimism is not a clinical criterion.
4. **Decision integrity over session volume** — correct decisions and explicit exit conditions over indefinite continuation.
5. **Silence does not imply permission** — absence of instruction implies termination.

## Clinical Scope

**In scope (physiotherapy):**
- Musculoskeletal dysfunction (pain, stiffness, weakness)
- Post-injury and post-operative rehabilitation
- Sports injury recovery and return-to-sport
- Chronic pain management (evidence-based)
- Neuromotor re-education within physiotherapy scope

**Out of scope (automatic DECLINE or REFER):**
- Non-musculoskeletal pain (visceral, systemic, malignant)
- Medical emergencies
- Unstable medical conditions
- Primary psychiatric conditions

## Provisional Inclusion Criteria (Gateway to TRIAL)

A case qualifies for TRIAL if and only if ALL are true:
1. A clear musculoskeletal component is present
2. No active red flags are identified
3. Patient goals are functional, not pain-only
4. Informed consent is given for a time-limited intervention
5. No legal or ethical contraindications exist

Failure of any single criterion requires DECLINE or REFER.

## Continuation Criteria (TRIAL → CONTINUE)

Continuation beyond TRIAL requires objective functional improvement within a trial window of 3–5 sessions. At least one:
- ≥10% measurable improvement in range of motion
- Documented improvement in a functional task
- Reduction in compensatory movement strategies

Subjective reports alone are insufficient. Absence of progress mandates DISCHARGE or REFER.

## Conservative Decision Rule (Fail-Safe)

In the absence of clear, objective data supporting continuation:

**DEFAULT OUTPUT = DEFER or DECLINE**

- Uncertainty favors non-action
- Optimism is not a clinical criterion
- Silence does not imply permission
- Absence of instruction implies termination

## Decision Hierarchy

When multiple interpretations are possible:
1. Scope restrictions override patient preference
2. Safety overrides continuation
3. Objective function overrides subjective pain
4. Non-action overrides action under uncertainty

## Clinical Workflow Cycle

```
Listen → Evaluate → Set Goals → Treat → Re-evaluate → Decide
  ↑                                                       |
  └───────────────────────────────────────────────────────┘
```

### 1. Listen
Gather patient story: chief complaint, history, previous treatments, goals, medical history, psychosocial context.

### 2. Evaluate
Red flag screening first. Then: ROM (measured in degrees), strength testing, special tests based on hypothesis, neurological screening, functional tests, palpation. Formulate testable hypothesis.

### 3. Set Goals
Specific, measurable, time-bound, functional, agreed upon. Define exit criteria at the same time: CONTINUE criteria, DISCHARGE criteria, REFER criteria.

### 4. Treat
Every intervention tests a hypothesis. Before treating: What is my hypothesis? What intervention tests it? What response do I expect? What does non-response mean?

### 5. Re-evaluate
Same tests as initial evaluation. Compare to baseline. Document: "Baseline: 40° flexion. Today: 48°. Change: +20%."

### 6. Decide
Apply the decision system based on re-evaluation data:
- Red flags → REFER
- Insufficient data → DEFER
- Outside scope → DECLINE
- ≥10% objective improvement → CONTINUE
- Goals met → DISCHARGE
- No improvement after trial → Revise hypothesis or DISCHARGE

## Clinical Models

### Hypothesis-Driven Intervention
Every intervention is a hypothesis test. If the system responds as predicted, hypothesis is consolidated. If not, hypothesis is weakened or falsified. Repeating an intervention without revising the hypothesis is epistemic inertia.

### Non-Response as Signal
Non-response is the most informative clinical situation. It constrains the hypothesis space and drives the next decision. If two revised hypotheses both fail, the case is likely beyond current treatment scope → REFER or DISCHARGE.

### Dose-Response Coupling
If increasing dose produces no proportional response, the dose-response relationship is decoupled. This challenges the working hypothesis and may indicate the intervention target is incorrect.

### Subjective Report Insufficiency
Subjective reports ("I feel better") without objective change do not justify continuation. Patient-reported outcomes are supplementary, not sufficient alone.

## Decision Thresholds

### Trial Window: 3–5 sessions maximum
### Continuation: ≥10% ROM improvement OR documented functional progress OR reduced compensatory strategies
### Exit (Stasis): No measurable change for 3+ consecutive sessions → DISCHARGE
### Red Flag Referral: Progressive neurological deficit, cauda equina signs, unexplained weight loss, night pain, fever with spinal pain, history of malignancy → immediate REFER

## Enforcement Rules

- Non-action outputs (DECLINE, DEFER, REFER, DISCHARGE) are enforced immediately
- No overrides from patient preference, commercial pressure, or operational convenience
- TRIAL: maximum 5 sessions with auto-evaluation at trial end
- CONTINUE: maximum 3 extensions total, metrics logged per extension
- All enforcement actions are logged and auditable

## When to Apply This Skill

- Designing clinical decision support systems for physiotherapy
- Building patient management or rehabilitation tracking software
- Implementing treatment planning algorithms
- Creating physiotherapy workflow automation
- Developing health applications that need structured clinical reasoning
- Reviewing code that handles clinical decisions or treatment logic
