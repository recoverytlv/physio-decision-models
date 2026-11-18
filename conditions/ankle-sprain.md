---
title: "Ankle Sprain"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 1.3.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Lateral ankle sprain (anterior talofibular ligament, calcaneofibular ligament), medial ankle sprain (deltoid ligament), and high ankle sprain (syndesmosis). Acute, subacute, and chronic ankle instability."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "3-5 sessions"
continuation_threshold: ">=10% objective functional improvement"
red_flags:
  - "Unable to bear weight for four steps both immediately after the injury and at assessment (Ottawa ankle rules — refer to a physician to consider radiographs)"
  - "Bone tenderness at the posterior edge or tip of the lateral or medial malleolus, at the base of the fifth metatarsal, or at the navicular (Ottawa ankle rules — refer to a physician to consider radiographs)"
  - "Gross instability with visible deformity"
  - "Signs of vascular compromise (absent pedal pulse, severe swelling with tight compartment)"
  - "High ankle sprain with positive squeeze test and external rotation test (syndesmosis — may need surgical fixation)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/ankle-sprain.md"
clinic: "https://recoverytlv.co.il"
---

# Ankle Sprain

## Condition
Lateral ankle sprain (anterior talofibular ligament, calcaneofibular ligament), medial ankle sprain (deltoid ligament), and high ankle sprain (syndesmosis). Acute, subacute, and chronic ankle instability.

## Scope Check
Ankle sprain rehabilitation is within physiotherapy scope. Suspected fracture (Ottawa ankle rules positive), syndesmosis disruption requiring surgical fixation, or vascular compromise triggers REFER.

## Red Flags (→ REFER)
- Unable to bear weight for four steps both immediately after the injury and at assessment (Ottawa ankle rules — refer to a physician to consider radiographs)
- Bone tenderness at the posterior edge or tip of the lateral or medial malleolus, at the base of the fifth metatarsal, or at the navicular (Ottawa ankle rules — refer to a physician to consider radiographs)
- Gross instability with visible deformity
- Signs of vascular compromise (absent pedal pulse, severe swelling with tight compartment)
- High ankle sprain with positive squeeze test and external rotation test (syndesmosis — may need surgical fixation)

## Clinical Hypothesis Examples
- **Acute lateral ankle sprain (Grade I-II):** Ligament sprain with pain and swelling but functional stability. Tested with early weight bearing, progressive balance training, and strengthening. Expected response: improved weight bearing tolerance and reduced swelling within 3–5 sessions.
- **Chronic ankle instability:** Recurrent sprains with functional instability and giving way. Tested with proprioceptive training, peroneal strengthening, and progressive agility. Expected response: improved single leg balance time and reduced giving way episodes.
- **Ankle stiffness post-sprain:** Restricted dorsiflexion after ankle sprain limiting gait and squat. Tested with joint mobilization and stretching. Expected response: ≥10% improvement in dorsiflexion ROM.

## Trial Window
3–5 sessions. Objective criteria:
- Improved weight bearing tolerance
- Improved single leg balance (time or quality)
- ≥10% improvement in dorsiflexion ROM (if restricted)
- Functional improvement (walking, stairs, running)

## Non-Response
If weight bearing tolerance and balance do not improve within the trial window, reassess. Refer to a physician to consider imaging to rule out osteochondral lesion, undiagnosed fracture, or peroneal tendon injury. Chronic instability not responding to rehabilitation may require orthopaedic consultation for surgical stabilization.

## Related Documents
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md)
- [Trial Window Limits](../thresholds/trial-window-limits.md)
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Red Flag Referral](../thresholds/red-flag-referral.md)
