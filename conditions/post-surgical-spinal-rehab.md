---
title: "Post-Surgical Spinal Rehabilitation"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Post-operative rehabilitation following spinal surgery including laminectomy, discectomy, spinal fusion, and decompression procedures."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "protocol stage (post-operative)"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "New or worsening neurological deficit post-surgery (weakness, numbness, bowel/bladder changes)"
  - "Wound infection signs (increasing redness, warmth, drainage, fever)"
  - "Sudden severe pain different from surgical pain"
  - "Loss of bowel or bladder control (cauda equina)"
  - "Progressive deformity or instability at surgical level"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/post-surgical-spinal-rehab.md"
clinic: "https://recoverytlv.co.il"
---

# Post-Surgical Spinal Rehabilitation

## Condition
Post-operative rehabilitation following spinal surgery including laminectomy, discectomy, spinal fusion, and decompression procedures.

## Scope Check
Post-surgical spinal rehabilitation is within physiotherapy scope when cleared by the surgeon. Signs of surgical complication (infection, hardware failure, new neurological deficit) trigger immediate REFER.

## Red Flags (→ REFER)
- New or worsening neurological deficit post-surgery (weakness, numbness, bowel/bladder changes)
- Wound infection signs (increasing redness, warmth, drainage, fever)
- Sudden severe pain different from surgical pain
- Loss of bowel or bladder control (cauda equina)
- Progressive deformity or instability at surgical level

## Clinical Hypothesis Examples
- **Post-laminectomy deconditioning:** Weakness and reduced endurance from surgical recovery and pre-operative deconditioning. Tested with graded mobility and core stabilization. Expected response: improved walking distance and tolerance to upright postures within the first stage of the protocol.
- **Post-fusion stiffness and deconditioning:** Reduced hip/thoracic mobility and trunk endurance after fusion; the levels adjacent to the fusion carry increased motion and load. Tested with hip and thoracic mobility work, graded trunk endurance and conditioning within surgeon restrictions (no targeted mobilization of the adjacent levels). Expected response: improved functional mobility and activity tolerance.
- **Post-discectomy neural sensitivity:** Residual neural irritability following disc surgery. Tested with neural mobilization and graded loading. Expected response: reduced radicular symptoms and improved activity tolerance.
- **Fear-avoidance after spinal surgery:** Kinesiophobia limiting functional recovery. Tested with graded exposure and progressive loading. Expected response: improved movement confidence and functional capacity.

## Trial Window
Measured against the stage of the rehabilitation protocol, not a fixed number of sessions (initiated after surgical clearance). If progress stalls at a stage, the surgeon is consulted. Stage criteria:
- Improved walking distance or duration
- Reduced reliance on assistive devices
- Improved functional independence (sit-to-stand, stair negotiation, dressing)
- Measurable improvement in available ROM, beyond measurement error

## Non-Response
If functional capacity stalls at a protocol stage despite surgical clearance, reassess. Consider surgeon follow-up for evaluation of hardware position, incomplete decompression, or adjacent segment pathology.

## Related Documents
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Continuation Criteria](../thresholds/continuation-criteria.md)
- [Low Back Pain](low-back-pain.md)
- [Sciatica](sciatica.md)
