# DECISION_ENFORCEMENT_RULES.md
Enforcement Layer v1.0 — FROZEN
## 1. Enforcement Principles
The enforcement layer converts normative decisions into coercive actions.
It does not interpret or modify logic — it executes.
- **Default to termination**: Non-action outputs (DECLINE, DEFER, REFER, DISCHARGE)
  are enforced immediately and irreversibly.
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
| REFER | Forced referral protocol. Generate referral note and terminate physio involvement. | Referral note logged; follow-up check in 7 days. |
| TRIAL | Time-bound initiation. Maximum 5 sessions. Auto-evaluate at trial end. | Session logs + objective metrics required. |
| CONTINUE | Conditional extension only if criteria met. Maximum 3 extensions total. | Metrics logged per extension; auto-terminate if criteria fail. |
| DISCHARGE | Immediate termination. Close case and issue discharge summary (functional only). | Summary logged; case cannot reopen without new evaluation. |
---
## 3. Coercive Triggers
- **Red flag detection**
  Automatic REFER if red-flag symptoms emerge
  (e.g., acute neurological deficit, unexplained severe pain).
- **Progress failure**
  Auto-DISCHARGE if no measurable functional change after trial
  (e.g., <10% objective improvement).
- **Scope violation**
  Immediate DECLINE if the case drifts outside defined scope
  (e.g., non-musculoskeletal request).
- **Uncertainty threshold**
  DEFER if data confidence is below 80%
  (e.g., incomplete history or conflicting findings).
---
## 4. Execution Invariants
- All actions are system-enforced; manual override is prohibited.
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
