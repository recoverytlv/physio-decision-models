---
title: "Post-Concussion Syndrome — Physiotherapy Role"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 1.0.0
status: frozen
license: MIT
author: "Alejandro Zubrisky, PT"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Persistent symptoms following concussion (mild traumatic brain injury) lasting beyond the expected recovery period (>10-14 days in adults). Symptoms may include headache, dizziness, neck pain, balance deficits, exercise intolerance, and visual disturbance. Physiotherapy addresses the cervical, vestibular, and exercise tolerance components."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "3-5 sessions"
continuation_threshold: ">=10% objective functional improvement"
red_flags:
  - "Worsening neurological symptoms (confusion, repeated vomiting, seizures, worsening headache) — emergency"
  - "Suspected intracranial hemorrhage (worst headache of life, altered consciousness) — emergency"
  - "Acute concussion in the first 48 hours (medical management first)"
  - "Significant cognitive or psychological symptoms (memory loss, personality change, depression, anxiety)"
  - "Symptoms not improving after 4+ weeks of multidisciplinary management"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/post-concussion.md"
clinic: "https://recoverytlv.co.il"
---

# Post-Concussion Syndrome — Physiotherapy Role

## Condition
Persistent symptoms following concussion (mild traumatic brain injury) lasting beyond the expected recovery period (>10-14 days in adults). Symptoms may include headache, dizziness, neck pain, balance deficits, exercise intolerance, and visual disturbance. Physiotherapy addresses the cervical, vestibular, and exercise tolerance components.

## Scope Check
The cervicogenic, vestibular, and exercise tolerance components of post-concussion syndrome are within physiotherapy scope. Cognitive, psychological, and medical management of concussion requires a multidisciplinary team. Physiotherapy is one component of post-concussion care, not the sole treatment.

## DECLINE or REFER Triggers
- Acute concussion in the first 48 hours (medical management first)
- Worsening neurological symptoms (confusion, repeated vomiting, seizures, worsening headache — emergency)
- Suspected intracranial hemorrhage (worst headache of life, altered consciousness — emergency)
- Significant cognitive or psychological symptoms (memory loss, personality change, depression, anxiety) — REFER to neuropsychologist
- Symptoms not improving after 4+ weeks of multidisciplinary management — REFER to concussion specialist

## What Physiotherapy Can Address

### 1. Cervicogenic Component
Neck pain and cervicogenic headache following head/neck trauma (the same mechanism that causes concussion often injures the cervical spine).

- Assessment: cervical ROM, segmental mobility, deep neck flexor endurance, cervicogenic headache provocation
- Treatment: cervical mobilization, deep neck flexor training, neck strengthening
- Expected response: reduced headache frequency and neck pain

### 2. Vestibular Component
Dizziness, balance deficits, and motion sensitivity following concussion.

- Assessment: vestibulo-ocular reflex (VOR), balance testing (BESS), motion sensitivity quotient
- Treatment: vestibular rehabilitation (gaze stabilization, habituation exercises, balance training)
- Expected response: reduced dizziness, improved balance scores, reduced motion sensitivity

### 3. Exercise Tolerance
Exercise intolerance (symptoms worsen with physical exertion) is common in post-concussion syndrome.

- Assessment: Buffalo Concussion Treadmill Test or modified exercise tolerance test — identify symptom threshold
- Treatment: sub-symptom threshold aerobic exercise, gradually progressed
- Expected response: increasing exercise tolerance without symptom exacerbation

## Clinical Hypothesis Examples
- **Cervicogenic headache post-concussion:** Upper cervical dysfunction contributing to persistent headache. Tested with C1-C2 assessment and treatment. Expected response: if cervicogenic, headache reduces with cervical treatment.
- **Vestibular dysfunction:** Peripheral vestibular injury or central vestibular processing deficit. Tested with VOR exercises and habituation. Expected response: reduced dizziness and improved gaze stability within 3–5 sessions.
- **Exercise intolerance — autonomic dysfunction:** Autonomic nervous system dysregulation causing symptoms with exertion. Tested with sub-threshold aerobic exercise program. Expected response: gradual increase in symptom-free exercise intensity over 2–4 weeks.
- **Combined cervicogenic + vestibular:** Both systems contributing (common). Tested with combined cervical and vestibular rehabilitation. Expected response: improvement in both headache and dizziness metrics.

## Trial Window
5 sessions. Objective criteria:
- Improved exercise tolerance (higher threshold on treadmill test)
- Reduced dizziness scores (DHI or similar)
- Improved balance (BESS score)
- Reduced headache frequency or intensity
- Improved cervical ROM (if cervicogenic component)

## Return to Sport Protocol (After Concussion)
Physiotherapy guides the graded return to sport:

| Stage | Activity | Minimum Duration |
|---|---|---|
| 1 | Symptom-limited activity (daily activities that don't provoke symptoms) | 24 hours |
| 2 | Light aerobic exercise (walking, cycling at mild intensity) | 24 hours |
| 3 | Sport-specific exercise (running drills, no contact) | 24 hours |
| 4 | Non-contact training drills (complex drills, resistance training) | 24 hours |
| 5 | Full contact practice (after medical clearance) | 24 hours |
| 6 | Return to competition | — |

Each stage must be completed symptom-free before progressing. If symptoms return, drop back to the previous symptom-free stage.

## Non-Response
If cervicogenic, vestibular, or exercise tolerance symptoms do not improve within the trial window, reassess. Persistent symptoms may require referral to concussion specialist, neuropsychologist, or neuro-ophthalmologist. Post-concussion syndrome lasting >3 months with minimal improvement despite multidisciplinary care requires specialist team management.

## Related Documents
- [Neck Pain](neck-pain.md)
- [Whiplash](whiplash.md)
- [Cervical Radiculopathy](cervical-radiculopathy.md)
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md)
- [Red Flag Referral](../thresholds/red-flag-referral.md)
