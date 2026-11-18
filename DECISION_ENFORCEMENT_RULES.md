# DECISION_ENFORCEMENT_RULES.md
Enforcement Layer v2.0 — FROZEN
## 1. Enforcement Principles
The enforcement layer converts normative decisions into coercive actions.
It does not interpret or modify logic — it executes.
- **Default to termination**: DECLINE, REFER and DISCHARGE are enforced immediately.
  DEFER is a temporary hold, enforced immediately and lifted only on explicit resolution.
- **No overrides**: Patient preference, commercial pressure, or operational
  convenience do not supersede system outputs.
- **Traceability**: All enforcement actions are logged and auditable
  (see AUTHORITY_SOURCES.md).
---
## 2. Enforcement Mechanisms by Output
| Output | Enforcement Action | Audit Requirement |
|------------|-------------------------------------------------------------------------------------|-------------------|
| DECLINE | Immediate block on case acceptance. System logs rejection rationale. | Full rationale logged; no patient access. |
| DEFER | Temporary hold on progression pending explicit resolution (e.g., additional data). | Timestamped hold; re-trigger if unresolved after 48 hours. |
| REFER | Referral protocol. The patient is told in person, at once: emergency signs → emergency department now; otherwise the treating or family doctor (the surgeon, after an operation); physio involvement ends. | Referral recorded in the clinical file; follow-up check in 7 days. |
| TRIAL | Time-bound initiation. 4 sessions, with one measurable marker agreed at the first session. Evaluate at session 4 (post-operative cases: at each protocol stage). | Session logs + objective metrics required. |
| CONTINUE | Conditional extension only if criteria met; criteria re-checked at each documented review. | Metrics logged per review; extension ends if criteria fail. |
| DISCHARGE | Immediate termination. Close case and record functional outcomes in the clinical file; a written summary goes to the treating physician only if they request it. | Outcomes recorded; case cannot reopen without new evaluation. |
---
## 3. Coercive Triggers
- **Red flag detection**
  Automatic REFER if red-flag symptoms emerge
  (e.g., acute neurological deficit, unexplained severe pain).
- **Progress failure**
  If the agreed marker has not changed measurably after 4 sessions, treatment stops and the case is re-evaluated:
  a documented revision (a different hypothesis, or the same hypothesis with a documented change of dose, technique or adherence plan) followed by ONE new TRIAL, or DISCHARGE, or REFER (advice to see the treating or family doctor).
  A second failed TRIAL requires DISCHARGE or REFER.
- **Scope violation**
  Immediate DECLINE if the case drifts outside defined scope
  (e.g., non-musculoskeletal request).
- **Uncertainty**
  DEFER when the data are insufficient for a decision
  (e.g., incomplete history or conflicting findings).
---
## 4. Execution Invariants
- Outputs follow the rules above. A clinician may depart from them only with a documented clinical rationale, which is logged for audit.
- Enforcement logs are immutable and traceable to AUTHORITY_SOURCES.md.
- No grace periods for continuation: criteria must be met strictly.
- Metric evaluation may use automated calculation tools when applicable
  (e.g., progress threshold computation).
---
## 5. Design Invariant
This document defines **HOW** decisions are enforced.
CLINICAL_DECISION_SYSTEM.md defines **WHAT** decisions are valid.
AUTHORITY_SOURCES.md defines **WHY** this system is authoritative.
The enforcement layer has no independent authority.
---
