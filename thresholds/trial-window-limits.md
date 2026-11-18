# Trial Window Limits

## 1. Definition
The trial window is the bounded period during which a new case is evaluated under controlled conditions before a continuation or termination decision is required. It is the temporal boundary of the TRIAL output. The 4-session window is a pragmatic, author-defined review point; no study has validated a specific number of sessions.

## 2. Window Parameters
- **Length:** 4 sessions
- **Marker:** one measurable marker (pain on a validated scale, function, mobility or strength) is agreed at the first session; the first session counts
- **Extension:** Not permitted. When continuation criteria are met the output is CONTINUE, not a longer trial
- **Post-operative cases:** progress is measured against the stage of the rehabilitation protocol instead of a session count; if progress stalls at a stage, the surgeon is consulted
- **Warning signs or worsening:** immediate referral, without waiting for the window to end

## 3. Evaluation Requirements
At the end of the trial window, exactly one of the following decisions must be made:
- **CONTINUE** — if objective improvement criteria are met
- **REFER** — if red flags emerge, the condition is outside physiotherapy scope, or non-response (including a second failed TRIAL) calls for medical or specialist assessment
- **New TRIAL (once)** — after a documented revision, when the agreed marker has not changed measurably: either a different hypothesis, or the same hypothesis with a documented change of dose, technique or adherence plan
- **DISCHARGE** — if the agreed marker has not changed measurably and no revision is justified, or after a second failed TRIAL; the case is re-evaluated and, if needed, the patient is advised to see their treating or family doctor

## 4. Prohibited Actions
- Extending the trial window beyond 4 sessions
- Restarting the trial window for the same hypothesis without a documented change of dose, technique or adherence plan
- Starting a third TRIAL for the same case
- Converting TRIAL to an indefinite treatment plan without formal CONTINUE justification

## 5. Decision Rule
`If Sessions[TRIAL] >= 4 AND Objective_Improvement == FALSE → documented revision + ONE new TRIAL, OR DISCHARGE, OR REFER; if this was already the second TRIAL → DISCHARGE OR REFER` (post-operative: `If Stage_Progress == STALLED → consult surgeon`)

## Related Documents
- [Continuation Criteria](./continuation-criteria.md) — Defines the objective thresholds evaluated at trial end
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md) — The trial window is the hypothesis testing period
- [Exit Criteria for Stasis](./exit-criteria-stasis.md) — Stasis within trial window triggers early exit
- [Red Flag Referral](./red-flag-referral.md) — Red flags detected during trial override the window and mandate immediate REFER
