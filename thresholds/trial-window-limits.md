# Trial Window Limits

## 1. Definition
The trial window is the bounded period during which a new case is evaluated under controlled conditions before a continuation or termination decision is required. It is the temporal boundary of the TRIAL output.

## 2. Window Parameters
- **Minimum duration:** 3 sessions
- **Maximum duration:** 5 sessions
- **Extension:** Not permitted without meeting continuation criteria

## 3. Evaluation Requirements
At the end of the trial window, exactly one of the following decisions must be made:
- **CONTINUE** — if objective improvement criteria are met
- **REFER** — if red flags emerge or the condition is outside physiotherapy scope
- **DISCHARGE** — if no objective improvement is demonstrated

## 4. Prohibited Actions
- Extending the trial window beyond 5 sessions without documented objective improvement
- Restarting the trial window for the same hypothesis
- Converting TRIAL to an indefinite treatment plan without formal CONTINUE justification

## 5. Decision Rule
`If Sessions[TRIAL] > 5 AND Objective_Improvement == FALSE → DISCHARGE OR REFER`
