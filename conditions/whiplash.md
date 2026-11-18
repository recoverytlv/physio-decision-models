---
title: "Whiplash-Associated Disorder"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Whiplash-associated disorder (WAD) grades I-III following acceleration-deceleration injury, typically motor vehicle accident. Includes neck pain, headache, and associated symptoms."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Signs of cervical fracture or dislocation (Canadian C-spine rules positive)"
  - "Signs of vertebral artery dissection (severe headache, dizziness, visual disturbance, dysphagia following neck trauma)"
  - "Upper motor neuron signs (hyperreflexia, clonus, bilateral symptoms)"
  - "Any signs of concussion or head injury (confusion, amnesia, vomiting, loss of consciousness) — REFER; worsening symptoms — emergency"
  - "Progressive neurological deficit"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/whiplash.md"
clinic: "https://recoverytlv.co.il"
---

# Whiplash-Associated Disorder

## Condition
Whiplash-associated disorder (WAD) grades I-III following acceleration-deceleration injury, typically motor vehicle accident. Includes neck pain, headache, and associated symptoms.

## Scope Check
WAD grades I-III are within physiotherapy scope. WAD grade IV (fracture or dislocation) or signs of cervical instability, vertebral artery dissection, or traumatic brain injury trigger REFER.

## Red Flags (→ REFER)
- Signs of cervical fracture or dislocation (Canadian C-spine rules positive)
- Signs of vertebral artery dissection (severe headache, dizziness, visual disturbance, dysphagia following neck trauma)
- Upper motor neuron signs (hyperreflexia, clonus, bilateral symptoms)
- Any signs of concussion or head injury (confusion, amnesia, vomiting, loss of consciousness) — REFER; worsening symptoms — emergency
- Progressive neurological deficit

## Clinical Hypothesis Examples
- **WAD Grade I-II — cervical movement dysfunction:** Pain-limited cervical ROM without neurological deficit. Tested with graded active movement, manual therapy, and exercise. Expected response: improved cervical ROM and reduced pain with movement within 4 sessions.
- **WAD with cervicogenic headache:** Headache originating from upper cervical dysfunction following whiplash. Tested with C1-C2 mobilization and deep neck flexor retraining. Expected response: reduced headache frequency and intensity.
- **WAD with kinesiophobia:** Fear of movement limiting recovery after whiplash injury. Tested with graded exposure, education, and progressive loading. Expected response: improved movement confidence and functional activity level.
- **WAD with neural sensitivity:** Post-traumatic neural mechanosensitivity in cervical nerve roots. Tested with neural mobilization and desensitization. Expected response: reduced referred arm symptoms and improved neural tension tests.

## Trial Window
4 sessions. One of these is agreed at the first session as the measurable marker:
- Measurable improvement in cervical ROM, beyond measurement error
- Reduced headache frequency or intensity (if present)
- Improved functional capacity (driving tolerance, work activities, sleep quality)
- Reduced fear-avoidance (measurable via questionnaire or functional task)

## Non-Response
If ROM and function do not improve within the trial window, reassess. Refer to a physician to consider imaging for structural injury. Persistent symptoms are more likely when early prognostic factors were present (high initial pain and disability, post-traumatic stress, cold hyperalgesia); these patients may need a multidisciplinary approach.

## Related Documents
- [Neck Pain](neck-pain.md)
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md)
- [Exit Criteria for Stasis](../thresholds/exit-criteria-stasis.md)
