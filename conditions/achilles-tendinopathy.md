---
title: "Achilles Tendinopathy"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Achilles tendinopathy including midportion tendinopathy and insertional tendinopathy. Distinct from acute Achilles tendon rupture."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Sudden onset of severe calf pain with audible pop (suspected rupture)"
  - "Palpable gap in tendon"
  - "Positive Thompson test (no plantarflexion with calf squeeze)"
  - "Inability to perform single leg heel raise"
  - "Signs of DVT (unilateral calf swelling, warmth, tenderness along the deep veins)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/achilles-tendinopathy.md"
clinic: "https://recoverytlv.co.il"
---

# Achilles Tendinopathy

## Condition
Achilles tendinopathy including midportion tendinopathy and insertional tendinopathy. Distinct from acute Achilles tendon rupture.

## Scope Check
Achilles tendinopathy is within physiotherapy scope. Suspected complete tendon rupture (positive calf-squeeze [Simmonds–Thompson] test, altered resting ankle angle with the knee flexed in prone [Matles test], palpable gap; Maffulli 1998, PMID 9548122) triggers REFER for urgent orthopaedic assessment. Some active plantarflexion is often preserved after a rupture and does not exclude it.

## Red Flags (→ REFER)
- Sudden onset of severe calf pain with audible pop (suspected rupture)
- Palpable gap in tendon
- Positive Thompson test (no plantarflexion with calf squeeze)
- Inability to perform single leg heel raise
- Signs of DVT (unilateral calf swelling, warmth, tenderness along the deep veins)

## Clinical Hypothesis Examples
- **Midportion tendinopathy with load intolerance:** Tendon overloaded beyond its capacity. Tested with isometric calf loading progressing to heavy slow resistance. Expected response: reduced morning stiffness and improved load tolerance within 4 sessions.
- **Insertional tendinopathy with compression component:** Tendon compression at calcaneal insertion. Tested with load modification (avoiding dorsiflexion compression) and progressive loading. Expected response: improved tolerance to heel loading.
- **Kinetic chain deficit:** Proximal weakness contributing to tendon overload. Tested with hip and calf strengthening. Expected response: improved single leg calf raise capacity and reduced tendon irritability.

## Trial Window
4 sessions. One of these is agreed at the first session as the measurable marker:
- Increased single leg calf raise capacity (repetitions or height)
- Reduced morning stiffness duration
- Improved walking or running tolerance
- Measurable improvement in ankle dorsiflexion ROM (if restricted), beyond measurement error

## Non-Response
Tendinopathy often requires longer loading periods. However, if load tolerance does not improve at all within 4 sessions (no change in calf raise capacity, no reduction in morning stiffness), reassess. Revise the hypothesis, or refer to a physician to consider imaging of tendon structure.

## Related Documents
- [Dose-Response Coupling](../models/dose-response-coupling.md)
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Continuation Criteria](../thresholds/continuation-criteria.md)
- [Trial Window Limits](../thresholds/trial-window-limits.md)
