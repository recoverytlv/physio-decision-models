---
title: "Plantar Fasciitis"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Plantar fasciitis (plantar heel pain) and plantar fasciopathy. Pain at the medial calcaneal tubercle, typically worse with first steps in the morning."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Heel pain after trauma with inability to weight bear (suspected fracture)"
  - "Bilateral heel pain with morning stiffness >30 minutes (systemic inflammatory condition)"
  - "Numbness or burning in heel distribution (nerve entrapment)"
  - "Night pain with unexplained weight loss"
  - "Pain not related to weight bearing (non-mechanical pattern)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/plantar-fasciitis.md"
clinic: "https://recoverytlv.co.il"
---

# Plantar Fasciitis

## Condition
Plantar fasciitis (plantar heel pain) and plantar fasciopathy. Pain at the medial calcaneal tubercle, typically worse with first steps in the morning.

## Scope Check
Plantar heel pain is within physiotherapy scope when musculoskeletal in origin. Suspected calcaneal stress fracture, nerve entrapment (Baxter's nerve), or systemic inflammatory conditions trigger additional investigation or REFER.

## Red Flags (→ REFER)
- Heel pain after trauma with inability to weight bear (suspected fracture)
- Bilateral heel pain with morning stiffness >30 minutes (systemic inflammatory condition)
- Numbness or burning in heel distribution (nerve entrapment)
- Night pain with unexplained weight loss
- Pain not related to weight bearing (non-mechanical pattern)

## Clinical Hypothesis Examples
- **Plantar fascia overload:** Mechanical overload of plantar fascia from increased activity or load. Tested with load modification and calf/plantar fascia stretching. Expected response: reduced first-step pain and improved walking tolerance within 4 sessions.
- **Calf tightness contributing to fascial load:** Restricted ankle dorsiflexion increasing plantar fascia strain. Tested with calf stretching and mobilization. Expected response: improved dorsiflexion ROM and reduced heel pain with walking.
- **Intrinsic foot weakness:** Weak foot intrinsic muscles increasing fascial load. Tested with intrinsic foot strengthening (short foot exercise, towel curls). Expected response: improved arch control and reduced pain with prolonged standing.

## Trial Window
4 sessions. One of these is agreed at the first session as the measurable marker:
- Reduced morning first-step pain severity
- Improved walking tolerance (distance or duration)
- Measurable improvement in ankle dorsiflexion ROM (if restricted), beyond measurement error
- Improved single leg calf raise capacity

## Non-Response
If first-step pain and walking tolerance do not improve within the trial window, reassess. Refer to a physician to consider imaging to evaluate fascial thickness or calcaneal stress fracture. Consider referral for investigation of systemic causes if bilateral.

## Related Documents
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md)
- [Trial Window Limits](../thresholds/trial-window-limits.md)
- [Continuation Criteria](../thresholds/continuation-criteria.md)
