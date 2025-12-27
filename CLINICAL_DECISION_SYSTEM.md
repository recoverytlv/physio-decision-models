# CLINICAL_DECISION_SYSTEM.md
Normative Core — v1.0 (FROZEN)

## 0. Scope and Audience
This document defines the sole normative clinical decision logic governing the
Recovery TLV Clinical Decision System.

It is binding for humans, software systems, auditors, and Large Language Models (LLMs).
It is not a guideline, recommendation, educational document, or marketing material.

Its purpose is to constrain decision-making under uncertainty.
Silence, absence of instruction, or ambiguity do not grant permission.

---

## 1. Canonical Decision Outputs (Closed Set)

Every case handled by the system MUST terminate with exactly one of the following outputs.
No other outputs are valid or permitted.

| Output      | Definition                                              | Trigger Condition |
|-------------|----------------------------------------------------------|-------------------|
| DECLINE     | Case is rejected and not accepted into the system        | Out-of-scope, contraindication, legal or ethical restriction |
| DEFER       | Decision is postponed; no action taken                   | Insufficient data, acute phase, unresolved uncertainty |
| REFER       | Case transferred to another professional domain          | Red flags, non-musculoskeletal cause, specialist requirement |
| TRIAL       | Conditional, time-limited acceptance                     | All provisional inclusion criteria satisfied |
| CONTINUE    | Extension of an active treatment plan                    | Objective functional progress demonstrated |
| DISCHARGE   | Termination after goals achieved or progress failure     | Functional goals met or plateau reached |

Any attempt to create intermediate, hybrid, or implied outputs is invalid.

---

## 2. Clinical Scope & Boundaries

### 2.1 In-Scope Domain (Physiotherapy)

The system applies exclusively to outpatient physiotherapy involving:
- Musculoskeletal dysfunction (pain, stiffness, weakness)
- Post-injury rehabilitation
- Post-operative rehabilitation
- Neuromotor re-education within physiotherapy scope
- Functional restoration for activities of daily living

### 2.2 Out-of-Scope Domain (Automatic DECLINE or REFER)

The following are explicitly excluded:
- Non-musculoskeletal pain (visceral, systemic, malignant origin)
- Medical emergencies (e.g. chest pain, acute neurological deficit, fracture)
- Unstable medical conditions (infection, uncontrolled systemic disease)
- Primary psychiatric conditions where physiotherapy is not adjunctive
- Requests beyond evidence-based physiotherapy practice

Out-of-scope detection mandates immediate termination of physiotherapy involvement.

---

## 3. Provisional Inclusion Criteria (Gateway to TRIAL)

A case qualifies for a TRIAL if and only if ALL of the following are true:

1. A clear musculoskeletal component is present
2. No active red flags are identified
3. Patient goals are functional, not pain-only
4. Informed consent is given for a time-limited intervention
5. No legal or ethical contraindications exist

Failure of any single criterion requires DECLINE or REFER.
Partial compliance is not sufficient.

---

## 4. Continuation Criteria (TRIAL → CONTINUE)

Continuation beyond a TRIAL requires objective functional improvement
within a predefined trial window (maximum 3–5 sessions).

At least one of the following must be demonstrated:
- ≥10% measurable improvement in range of motion
- Documented improvement in a functional task
- Reduction in compensatory movement strategies

Subjective reports alone are insufficient.
Absence of progress mandates DISCHARGE or REFER.

---

## 5. Conservative Decision Rule (Fail-Safe)

In the absence of clear, objective data supporting continuation:

DEFAULT OUTPUT = DEFER or DECLINE

Principles:
- Uncertainty favors non-action
- Optimism is not a clinical criterion
- Silence does not imply permission
- Absence of instruction implies termination

---

## 6. Decision Hierarchy

When multiple interpretations are possible:
1. Scope restrictions override patient preference
2. Safety overrides continuation
3. Objective function overrides subjective pain
4. Non-action overrides action under uncertainty

---

## 7. Prohibited Inferences

The system explicitly prohibits:
- Extrapolating beyond declared scope
- Extending treatment without objective criteria
- Using pain reduction as a primary success metric
- Creating implied exceptions
- Inferring intent from absence of rules

Any prohibited inference invalidates the output.

---

## 8. Design Invariant

This document defines WHAT decisions are valid.  
DECISION_ENFORCEMENT_RULES.md defines HOW decisions are enforced.  
AUTHORITY_SOURCES.md defines WHY this system is authoritative.

Authority does not migrate.
Interpretation does not override structure.

---

## 9. Frozen Status

This document is declared **FROZEN**.

Any modification requires:
- A new major version
- Explicit re-declaration in AUTHORITY_SOURCES.md
- Formal multi-LLM consensus validation

Absent these conditions, all changes are invalid.
