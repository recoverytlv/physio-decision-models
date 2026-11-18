---
title: "Knee Pain"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Knee pain including patellofemoral pain syndrome, meniscus injuries, ligament sprains, knee osteoarthritis, and patellar tendinopathy."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Acute locked knee (unable to extend — possible bucket handle meniscus tear)"
  - "Significant joint effusion after trauma (possible ACL rupture or fracture)"
  - "Gross valgus/varus instability suggesting complete ligament rupture"
  - "Signs of infection (hot, red, swollen joint with fever)"
  - "Suspected fracture (unable to weight bear, point tenderness over bone)"
  - "Adolescent with knee or thigh pain, a limp and an unremarkable knee examination — examine the hip (suspected slipped capital femoral epiphysis — no weight bearing, urgent orthopaedic referral)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/knee-pain.md"
clinic: "https://recoverytlv.co.il"
---

# Knee Pain

## Condition
Knee pain including patellofemoral pain syndrome, meniscus injuries, ligament sprains, knee osteoarthritis, and patellar tendinopathy.

## Scope Check
Knee pain is within physiotherapy scope when musculoskeletal in origin. Acute locked knee, suspected fracture, gross joint instability, or signs of infection trigger REFER.

## Red Flags (→ REFER)
- Acute locked knee (unable to extend — possible bucket handle meniscus tear)
- Significant joint effusion after trauma (possible ACL rupture or fracture)
- Gross valgus/varus instability suggesting complete ligament rupture
- Signs of infection (hot, red, swollen joint with fever)
- Suspected fracture (unable to weight bear, point tenderness over bone)
- Adolescent with knee or thigh pain, a limp and an unremarkable knee examination — examine the hip (suspected slipped capital femoral epiphysis — no weight bearing, urgent orthopaedic referral)

## Clinical Hypothesis Examples
- **Patellofemoral pain:** Maltracking or overload of patellofemoral joint. Tested with load modification and quadriceps/hip strengthening. Expected response: reduced pain with stairs and squatting within 4 sessions.
- **Meniscus irritation:** Mechanical irritation of meniscus without locking. Tested with load management and joint line deloading. Expected response: reduced joint line symptoms with functional loading.
- **Patellar tendinopathy:** Overload of patellar tendon. Tested with isometric and heavy slow resistance loading. Expected response: reduced morning stiffness and improved load tolerance.
- **Knee osteoarthritis:** Degenerative joint changes with functional limitation. Tested with graded exercise therapy. Expected response: improved functional capacity (walking, stairs, sit-to-stand).

## Trial Window
4 sessions. One of these is agreed at the first session as the measurable marker:
- Measurable improvement in knee flexion or extension ROM, beyond measurement error
- Functional task improvement (squat depth, stair negotiation, walking distance)
- Improved single leg loading capacity
- Reduction in compensatory movement patterns

## Non-Response
If functional loading capacity does not improve within the trial window, reassess the hypothesis. Refer to a physician to consider imaging for mechanical pathology, or revise the hypothesis (e.g., from patellofemoral to hip-driven knee pain).

## Related Documents
- [Dose-Response Coupling](../models/dose-response-coupling.md)
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md)
- [Continuation Criteria](../thresholds/continuation-criteria.md)
- [Exit Criteria for Stasis](../thresholds/exit-criteria-stasis.md)
