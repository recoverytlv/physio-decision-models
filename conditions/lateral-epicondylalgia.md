---
title: "Lateral Epicondylalgia (Tennis Elbow)"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Lateral epicondylalgia (tennis elbow) and medial epicondylalgia (golfer's elbow). Tendinopathy of the common extensor or flexor origin at the elbow."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Elbow instability after trauma (suspected ligament rupture)"
  - "Progressive hand weakness or numbness (nerve entrapment)"
  - "Elbow locking or catching (loose body)"
  - "Suspected fracture (point tenderness over bone after trauma)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/lateral-epicondylalgia.md"
clinic: "https://recoverytlv.co.il"
---

# Lateral Epicondylalgia (Tennis Elbow)

## Condition
Lateral epicondylalgia (tennis elbow) and medial epicondylalgia (golfer's elbow). Tendinopathy of the common extensor or flexor origin at the elbow.

## Scope Check
Epicondylalgia is within physiotherapy scope when musculoskeletal in origin. Elbow instability, suspected fracture, or neurological involvement (cubital tunnel, radial tunnel) may require additional investigation or REFER.

## Red Flags (→ REFER)
- Elbow instability after trauma (suspected ligament rupture)
- Progressive hand weakness or numbness (nerve entrapment)
- Elbow locking or catching (loose body)
- Suspected fracture (point tenderness over bone after trauma)

## Clinical Hypothesis Examples
- **Tendon overload (extensor origin):** Common extensor tendinopathy from repetitive gripping. Tested with eccentric wrist extension loading. Expected response: improved grip strength and reduced pain with gripping within 4 sessions.
- **Tendon overload (flexor origin):** Common flexor tendinopathy from repetitive wrist flexion/pronation. Tested with eccentric wrist flexion loading. Expected response: improved forearm strength and reduced medial elbow pain.
- **Cervical contribution:** Referred pain or neural sensitivity from cervical spine contributing to lateral elbow pain. Tested with cervical mobilization. Expected response: if cervical-driven, elbow pain reduces with cervical treatment.
- **Radial nerve sensitivity:** Neural mechanosensitivity contributing to lateral elbow pain. Tested with neural mobilization targeting radial nerve. Expected response: improved radial nerve tension tests.

## Trial Window
4 sessions. One of these is agreed at the first session as the measurable marker:
- Improved pain-free grip strength (measured with dynamometer)
- Functional improvement (lifting, gripping, turning objects)
- Reduced pain with resisted wrist extension or flexion
- Measurable improvement in grip strength measurement, beyond measurement error

## Non-Response
If grip strength does not improve after eccentric loading protocol, reassess. Consider a cervical contribution (common in lateral epicondylalgia), or refer to a physician to consider imaging for structural tendon changes.

## Related Documents
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md)
- [Dose-Response Coupling](../models/dose-response-coupling.md)
- [Exit Criteria for Stasis](../thresholds/exit-criteria-stasis.md)
- [Non-Response as Signal](../models/non-response-as-signal.md)
