---
title: "Calf Strain"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Acute muscle strain of the gastrocnemius or soleus (calf muscles). Gastrocnemius strains are more common and typically occur during explosive activities (sprinting, jumping). Soleus strains are more insidious and common in distance runners. Graded I-III by severity."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Calf pain with swelling, warmth, and redness without clear mechanism of injury (suspected DVT — urgent referral)"
  - "Palpable gap in the muscle with complete loss of function (grade III / complete rupture — surgical consultation)"
  - "Positive Thompson test (Achilles tendon rupture, not calf strain)"
  - "Calf pain with recent surgery, immobilization, or long-haul travel (DVT risk factors)"
  - "Exertional calf pain or cramping in a young athlete that recurs at a predictable workload and settles with rest (consider popliteal artery entrapment — refer for vascular assessment)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/calf-strain.md"
clinic: "https://recoverytlv.co.il"
---

# Calf Strain

## Condition
Acute muscle strain of the gastrocnemius or soleus (calf muscles). Gastrocnemius strains are more common and typically occur during explosive activities (sprinting, jumping). Soleus strains are more insidious and common in distance runners. Graded I-III by severity.

## Scope Check
Calf strains are within physiotherapy scope. Suspected deep vein thrombosis (DVT), complete muscle rupture requiring surgical repair, or Achilles tendon rupture must be differentiated and referred.

## Red Flags (→ REFER)
- Calf pain with swelling, warmth, and redness without clear mechanism of injury (suspected DVT — urgent referral)
- Palpable gap in the muscle with complete loss of function (grade III / complete rupture — surgical consultation)
- Positive Thompson test (Achilles tendon rupture, not calf strain)
- Calf pain with recent surgery, immobilization, or long-haul travel (DVT risk factors)
- Exertional calf pain or cramping in a young athlete that recurs at a predictable workload and settles with rest (consider popliteal artery entrapment — refer for vascular assessment)

## Differentiating Calf Strain from DVT

| Feature | Calf Strain | DVT |
|---|---|---|
| Onset | Sudden, during activity | Gradual, often at rest |
| Mechanism | Clear (sprinting, jumping, push-off) | No clear mechanism |
| Swelling | Localized to muscle | Diffuse, entire lower leg |
| Warmth | Localized | Diffuse |
| Bruising | May appear 24-48h post-injury | Rarely |
| Homans' sign | Unreliable — not used | Unreliable — not used |
| Risk factors | Athletic activity | Immobility, surgery, travel, clotting disorders |

Individual clinical features have limited value for confirming or excluding DVT (Goodacre et al. 2005, PMID 16027455).

**If DVT is suspected or cannot be confidently excluded → REFER for same-day medical assessment (probability scoring, D-dimer and ultrasound are medical decisions). Do not treat as a calf strain.**

## Clinical Hypothesis Examples
- **Gastrocnemius strain (acute):** Sudden onset during push-off or change of direction. Tested with progressive loading: isometric → eccentric → concentric → plyometric. Expected response: improved pain-free range and strength within each session, full recovery 2–8 weeks depending on grade.
- **Soleus strain:** More gradual onset, worse with knee-bent calf raises, common in runners. Tested with bent-knee calf loading and progressive running exposure. Expected response: reduced pain with soleus-specific tests and improved running tolerance.
- **Recurrent calf strain:** Repeated injury suggesting incomplete rehabilitation or biomechanical factor. Tested with eccentric strengthening, calf endurance testing (25+ single leg calf raises), and a review of training load and return-to-running progression. Expected response: improved calf endurance symmetry and reduced re-injury risk.

## Trial Window
4 sessions. One of these is agreed at the first session as the measurable marker:
- Improved pain-free range of motion (dorsiflexion)
- Improved calf strength (single leg calf raise repetitions compared bilaterally)
- Improved functional capacity (walking, jogging, sprinting progression)
- Reduced pain with provocative testing (resisted plantarflexion, stretch)

## Return to Sport Criteria
Before clearance for full sport:
- Pain-free single leg calf raise: ≥25 repetitions (matching contralateral)
- Pain-free hopping
- Pain-free sprinting at full speed
- No pain with sport-specific movements

## Non-Response
If calf symptoms persist despite appropriate loading progression, refer to a physician to consider imaging (ultrasound) to assess tear extent. Persistent symptoms at the musculotendinous junction may indicate partial Achilles involvement. Exertional calf pain in a young athlete that recurs at a predictable workload and settles with rest should raise suspicion of popliteal artery entrapment (REFER for vascular assessment).

## Related Documents
- [Achilles Tendinopathy](achilles-tendinopathy.md)
- [Hamstring Tendinopathy](hamstring-tendinopathy.md)
- [Dose-Response Coupling](../models/dose-response-coupling.md)
- [Red Flag Referral](../thresholds/red-flag-referral.md)
