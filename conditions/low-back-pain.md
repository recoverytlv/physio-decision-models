---
title: "Low Back Pain"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Low back pain including mechanical low back pain, lumbar disc herniation, chronic low back pain, and lumbar facet-related pain."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Progressive lower limb weakness or numbness"
  - "Bladder or bowel dysfunction (cauda equina)"
  - "Saddle anaesthesia"
  - "Unexplained weight loss with back pain"
  - "Night pain unrelated to position"
  - "History of malignancy with new back pain"
  - "Fever with spinal pain"
  - "Sudden back pain after a fall or minor trauma in an older adult, or with osteoporosis or prolonged corticosteroid use (suspected vertebral fracture)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/low-back-pain.md"
clinic: "https://recoverytlv.co.il"
---

# Low Back Pain

## Condition
Low back pain including mechanical low back pain, lumbar disc herniation, chronic low back pain, and lumbar facet-related pain.

## Scope Check
Low back pain is within physiotherapy scope when the presentation is musculoskeletal in origin. Cases with progressive neurological deficit, cauda equina signs, unexplained weight loss, fever, or history of malignancy trigger REFER.

## Red Flags (→ REFER)
- Progressive lower limb weakness or numbness
- Bladder or bowel dysfunction (cauda equina)
- Saddle anaesthesia
- Unexplained weight loss with back pain
- Night pain unrelated to position
- History of malignancy with new back pain
- Fever with spinal pain
- Sudden back pain after a fall or minor trauma in an older adult, or with osteoporosis or prolonged corticosteroid use (suspected vertebral fracture)

## Clinical Hypothesis Examples
- **Segmental hypomobility:** Restricted intersegmental motion at a specific level. Tested with mobilization. Expected response: improved ROM within 2–3 sessions.
- **Disc-related radiculopathy:** Nerve root involvement with dermatomal pattern. Tested with directional preference loading. Expected response: centralization of symptoms.
- **Motor control deficit:** Poor lumbopelvic control under load. Tested with graded motor control exercises. Expected response: improved movement quality and reduced compensatory patterns.
- **Neural sensitivity:** Heightened mechanosensitivity of neural structures. Tested with neural mobilization. Expected response: improved nerve mobility tests.

## Trial Window
4 sessions. One of these is agreed at the first session as the measurable marker:
- Measurable improvement in lumbar ROM (flexion, extension, or lateral flexion), beyond measurement error
- Documented functional task improvement (e.g., sit-to-stand, walking tolerance, lifting capacity)
- Reduction in compensatory movement strategies

## Non-Response
If no objective improvement after the trial window, the working hypothesis is revised or the case is exited. Persistent non-response is diagnostic data — it constrains the hypothesis space and may indicate non-musculoskeletal drivers.

## Related Documents
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md)
- [Trial Window Limits](../thresholds/trial-window-limits.md)
- [Continuation Criteria](../thresholds/continuation-criteria.md)
- [Red Flag Referral](../thresholds/red-flag-referral.md)
