---
title: "Lumbar Spinal Stenosis"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Narrowing of the spinal canal or intervertebral foramina in the lumbar spine, causing neurogenic claudication (leg pain, heaviness, or numbness with walking that eases with sitting or flexion). Most common in adults over 60. May coexist with degenerative disc disease and spondylolisthesis."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Cauda equina syndrome (bilateral leg symptoms, saddle anaesthesia, bowel/bladder dysfunction — emergency)"
  - "Progressive motor weakness in lower extremities"
  - "Rapidly worsening walking tolerance (weeks, not months)"
  - "Neurogenic claudication with no measurable change after 4 sessions and one revised trial (surgical consultation)"
  - "Severe stenosis with myelopathic signs (if thoracic/cervical involvement suspected)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/lumbar-spinal-stenosis.md"
clinic: "https://recoverytlv.co.il"
---

# Lumbar Spinal Stenosis

## Condition
Narrowing of the spinal canal or intervertebral foramina in the lumbar spine, causing neurogenic claudication (leg pain, heaviness, or numbness with walking that eases with sitting or flexion). Most common in adults over 60. May coexist with degenerative disc disease and spondylolisthesis.

## Scope Check
Lumbar spinal stenosis is within physiotherapy scope for conservative management. Severe stenosis with progressive neurological deficit, cauda equina syndrome, or failure of conservative management requires surgical consultation (REFER).

## Red Flags (→ REFER)
- Cauda equina syndrome (bilateral leg symptoms, saddle anaesthesia, bowel/bladder dysfunction — emergency)
- Progressive motor weakness in lower extremities
- Rapidly worsening walking tolerance (weeks, not months)
- Neurogenic claudication with no measurable change after 4 sessions and one revised trial (surgical consultation)
- Severe stenosis with myelopathic signs (if thoracic/cervical involvement suspected)

## Differentiating Neurogenic from Vascular Claudication

| Feature | Neurogenic (Stenosis) | Vascular (Peripheral Artery Disease) |
|---|---|---|
| Relieved by | Sitting, flexion, leaning forward | Standing still |
| Onset | Variable walking distance | Consistent walking distance |
| Pulses | Normal | Diminished |
| Skin | Normal | Pale, cool, hairless |
| Shopping cart sign | Yes (leaning forward on cart relieves symptoms) | No |

If vascular claudication is suspected → REFER to vascular specialist.

## Clinical Hypothesis Examples
- **Flexion-biased stenosis:** Canal narrowing relieved by lumbar flexion, worsened by extension. Tested with flexion-based exercises, stationary cycling, and posture modification (avoiding sustained extension). Expected response: improved walking tolerance within 4 sessions.
- **Dynamic stenosis with deconditioning:** Narrowing exacerbated by poor general fitness. Tested with cardiovascular conditioning in flexion-biased positions (stationary cycling) and lower limb strengthening. Expected response: improved walking distance and reduced leg symptoms.
- **Stenosis with co-existing hip pathology:** Hip stiffness (especially extension deficit) increasing lumbar extension demand during gait. Tested with hip mobilization and hip flexor stretching. Expected response: improved gait mechanics and reduced stenotic symptoms.
- **Fear-avoidance in stenosis:** Patient avoiding walking due to fear of symptoms, leading to further deconditioning. Tested with graded walking exposure and education. Expected response: improved confidence and walking tolerance.

## Trial Window
4 sessions; at their end, either a documented revision with ONE new trial, or DISCHARGE/REFER (stenosis may respond more slowly). One of these is agreed at the first session as the measurable marker:
- Improved walking distance or duration before symptom onset
- Improved standing tolerance
- Reduced frequency or intensity of neurogenic claudication symptoms
- Improved lower extremity strength

## Non-Response
If walking tolerance does not improve despite flexion-based management and conditioning, refer to a physician to consider imaging (MRI) and surgical consultation. Decompressive surgery (laminectomy) may be indicated for severe stenosis with significant functional limitation.

## Related Documents
- [Low Back Pain](low-back-pain.md)
- [Sciatica](sciatica.md)
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Red Flag Referral](../thresholds/red-flag-referral.md)
