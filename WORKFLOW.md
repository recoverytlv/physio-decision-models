# Clinical Workflow

The Recovery TLV clinical decision system operates on a repeating cycle. Every patient encounter follows the same structure.

## The Cycle

```
Listen → Evaluate → Set Goals → Treat → Re-evaluate → Decide
  ↑                                                       |
  └───────────────────────────────────────────────────────┘
```

### 1. Listen

Gather the patient's story without premature interpretation.

- Chief complaint in the patient's own words
- History of present condition (onset, duration, behavior, aggravating/easing factors)
- Previous treatments and their outcomes
- Patient's goals and expectations
- Medical history, medications, imaging

**Output:** A subjective picture of the problem, unfiltered.

### 2. Evaluate

Physical examination to generate objective data.

- Observation (posture, movement patterns, guarding)
- Active and passive range of motion (measured, documented)
- Strength testing (graded, compared bilaterally)
- Special tests (relevant to hypothesis)
- Neurological screening (if indicated)
- Functional tests (squat, gait, single leg balance, sport-specific)

**Output:** Objective baseline data. Measurable. Repeatable.

### 3. Set Goals

Define what success looks like — before starting treatment.

Goals must be:
- **Specific:** "Improve lumbar flexion ROM from 40° to 60°" not "reduce stiffness"
- **Measurable:** Linked to objective tests that can be repeated
- **Time-bound:** Evaluated within the trial window (3–5 sessions)
- **Functional:** Connected to the patient's real-world needs

**Output:** Clear criteria for CONTINUE vs DISCHARGE vs REFER.

### 4. Treat

Every intervention is a hypothesis test.

- Select intervention based on the clinical hypothesis
- Apply as a controlled perturbation (not a routine)
- Monitor immediate response (within-session change)
- Document what was done, dose, and immediate effect

The intervention answers a question: "If my hypothesis is correct, this intervention should produce X effect."

**Output:** Data. Did the intervention produce the expected response?

### 5. Re-evaluate

Repeat objective measures at defined intervals.

- Same tests as initial evaluation (consistency is critical)
- Compare to baseline: is there ≥10% improvement in ROM? Functional progress? Reduced compensation?
- Within-session changes vs between-session changes
- Patient-reported outcomes (supplementary, not sufficient alone)

**Output:** Objective comparison to baseline. Signal or noise?

### 6. Decide

Apply the decision system.

| Condition | Decision |
|---|---|
| Red flags detected | → **REFER** |
| Insufficient data to decide | → **DEFER** |
| Outside physiotherapy scope | → **DECLINE** |
| ≥10% objective improvement within trial | → **CONTINUE** |
| Goals fully met | → **DISCHARGE** |
| No improvement after trial window | → Re-evaluate hypothesis or **DISCHARGE** |
| Non-response after hypothesis revision | → **REFER** or **DISCHARGE** |

Then the cycle restarts: Listen to the patient again. What has changed? How do they feel? Re-evaluate. Decide.

## Decision Points by Session

```
Session 1-2:  Listen + Evaluate + Set Goals + Begin TRIAL
Session 3-5:  Re-evaluate → CONTINUE or revise hypothesis or DISCHARGE
Session 6-10: Re-evaluate every 2-3 sessions → CONTINUE or DISCHARGE
Session 10+:  Strong justification required for continuation
```

## The Non-Negotiables

1. **No treatment without a hypothesis.** If you don't know what you're testing, you shouldn't be treating.
2. **No continuation without objective improvement.** Subjective reports alone are insufficient.
3. **No indefinite treatment.** Every case must reach an exit: DISCHARGE, REFER, or DECLINE.
4. **Non-response is data, not failure.** It narrows the hypothesis space and drives the next decision.

## Related Documents

- [Clinical Decision System](CLINICAL_DECISION_SYSTEM.md)
- [Non-Response as Signal](models/non-response-as-signal.md)
- [Hypothesis-Driven Intervention](models/hypothesis-driven-intervention.md)
- [Trial Window Limits](thresholds/trial-window-limits.md)
- [Continuation Criteria](thresholds/continuation-criteria.md)
- [Clinical Cases](CLINICAL_CASES.md)
