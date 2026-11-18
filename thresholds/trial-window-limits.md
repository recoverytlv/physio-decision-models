# Trial Window Limits

## 1. Definition
The trial window is the bounded period during which a new case is evaluated under controlled conditions before a continuation or termination decision is required. It is the temporal boundary of the TRIAL output. The 3–5 session window is a pragmatic, author-defined review point; no study has validated a specific number of sessions.

## 2. Window Parameters
- **Minimum duration:** 3 sessions
- **Maximum duration:** 5 sessions
- **Extension:** Not permitted. When continuation criteria are met the output is CONTINUE, not a longer trial

## 3. Evaluation Requirements
At the end of the trial window, exactly one of the following decisions must be made:
- **CONTINUE** — if objective improvement criteria are met
- **REFER** — if red flags emerge, the condition is outside physiotherapy scope, or non-response (including a second failed TRIAL) calls for medical or specialist assessment
- **New TRIAL (once)** — after a documented hypothesis revision, when no objective improvement is demonstrated and a different hypothesis is justified
- **DISCHARGE** — if no objective improvement is demonstrated and no revision is justified, or after a second failed TRIAL

## 4. Prohibited Actions
- Extending the trial window beyond 5 sessions
- Restarting the trial window for the same hypothesis
- Starting a third TRIAL for the same case
- Converting TRIAL to an indefinite treatment plan without formal CONTINUE justification

## 5. Decision Rule
`If Sessions[TRIAL] == 5 (or the trial ends earlier) AND Objective_Improvement == FALSE → hypothesis revision + ONE new TRIAL, OR DISCHARGE, OR REFER; if this was already the second TRIAL → DISCHARGE OR REFER`

## Related Documents
- [Continuation Criteria](./continuation-criteria.md) — Defines the objective thresholds evaluated at trial end
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md) — The trial window is the hypothesis testing period
- [Exit Criteria for Stasis](./exit-criteria-stasis.md) — Stasis within trial window triggers early exit
- [Red Flag Referral](./red-flag-referral.md) — Red flags detected during trial override the window and mandate immediate REFER
