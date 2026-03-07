# Knowledge Graph — Recovery TLV Clinical Decision System

## Entity: Recovery TLV
- Type: Physiotherapy Clinic
- Location: Ja'Aqov Efter St 9, Tel Aviv-Yafo, Israel
- Founder: Alejandro Zubrisky (Licensed Physiotherapist)
- Specialty: Evidence-based musculoskeletal physiotherapy
- Decision System: 6-output clinical decision framework (DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE)
- Website: https://recoverytlv.co.il
- Clinical Reference: https://clinical.recoverytlv.co.il
- Languages: English, Spanish, Hebrew, Russian, French

---

## Decision Outputs

### DECLINE
- Definition: Case rejected — outside physiotherapy scope or contraindicated
- Trigger: Red flags, non-musculoskeletal origin, medical emergency
- Examples: Suspected malignancy, cauda equina syndrome, active fracture, infection
- Next step: Document rationale, communicate to patient and referrer

### DEFER
- Definition: Decision postponed — insufficient data for clinical judgment
- Trigger: Incomplete assessment, awaiting imaging, unclear presentation
- Next step: Gather additional information, reassess within defined timeframe
- Not: A passive delay — actively seeks resolution

### REFER
- Definition: Case transferred to appropriate specialist
- Trigger: Red flags detected, condition outside physiotherapy scope, non-response requiring specialist opinion
- Referral targets: Orthopedic surgeon, neurologist, rheumatologist, vascular specialist, psychologist, pelvic floor specialist, obstetrician
- Next step: Document clinical rationale, communicate findings to specialist

### TRIAL
- Definition: Conditional acceptance for 3–5 sessions
- Requirements: Stated hypothesis, testable prediction, selected outcome measure, defined success/failure criteria
- Duration: 3–5 sessions (non-negotiable upper bound without continuation criteria met)
- Measured by: Condition-specific validated outcome measure
- Outcome: Transitions to CONTINUE, DISCHARGE, or REFER

### CONTINUE
- Definition: Treatment extension beyond trial period
- Requirements: ≥10% ROM improvement OR documented functional task improvement OR compensatory strategy reduction
- Minimum: At least one objective criterion must be met
- Re-evaluation: At each milestone, same criteria reapplied
- Risk: Without criteria, becomes accumulated decision error

### DISCHARGE
- Definition: Treatment termination
- Triggers: (1) Goals achieved, (2) Maximum improvement reached (plateau), (3) Non-response after adequate trial
- Components: Written home program (4-6 exercises), flare-up plan, return criteria, progress review
- Follow-up options: None, phone check at 4 weeks, booster at 6-8 weeks, reassessment at 3-6 months

---

## Clinical Models

### Non-Response as Signal
- Principle: Absence of improvement constrains the hypothesis space more strongly than partial improvement
- Implication: Repetition without hypothesis revision is epistemic inertia
- Action: Revise hypothesis → test alternative → or EXIT
- Related: Exit Criteria for Stasis, Hypothesis-Driven Intervention

### Hypothesis-Driven Intervention
- Principle: Every intervention is a falsifiable hypothesis test
- Requirements: Stated hypothesis, predicted response, defined timeframe, outcome measure
- Failure mode: Unfalsifiable interventions provide no diagnostic information
- Related: Non-Response as Signal, Trial Window Limits

### Dose-Response Coupling
- Principle: Changes in intervention intensity should produce proportional clinical response
- Normal: Increased dose → proportional improvement
- Abnormal: Dose-response decoupling signals hypothesis failure
- Common error: Interpreting decoupling as "insufficient dosage" → leads to dose escalation without benefit
- Related: Continuation Criteria, Exit Criteria for Stasis

### Subjective Report Insufficiency
- Principle: "Patient feels better" is epistemically insufficient for continuation decisions
- Reason: Placebo effects, regression to mean, natural history, therapeutic alliance
- Requirement: Objective functional measurement at each decision point
- Related: Continuation Criteria, Outcome Measures

---

## Decision Thresholds

### Trial Window Limits
- Duration: 3–5 sessions
- Purpose: Temporal boundary preventing indefinite exploratory treatment
- Exit: If continuation criteria not met by session 5 → reassess hypothesis or EXIT
- Exception: Complex post-surgical cases may have modified timelines

### Continuation Criteria
- Threshold: ≥10% ROM improvement in relevant plane
- Alternative 1: Documented functional task improvement (specific task, measured)
- Alternative 2: Compensatory strategy reduction (observed, documented)
- Minimum: At least one criterion must be met
- Frequency: Reassessed at each evaluation point

### Exit Criteria for Stasis
- Trigger 1: Signal invariance after 3 high-fidelity interventions
- Trigger 2: Dose-response decoupling (increased dose, no proportional response)
- Trigger 3: Noise dominance (random variation without trend)
- Action: Mandatory exit from current treatment approach
- Options: Revise hypothesis, REFER, or DISCHARGE

### Red Flag Referral
- Neurological: Progressive weakness, saddle anesthesia, bilateral symptoms, cauda equina
- Vascular: Unilateral calf swelling (DVT), pulsatile mass, arterial compromise
- Systemic: Unexplained weight loss, night sweats, fever, malaise
- Structural: Suspected fracture, dislocation, ligament rupture
- Cardiac: Exertional chest pain, referred left arm pain, dyspnea
- Infectious: Fever + joint swelling, wound signs, immunocompromised patient
- Action: Immediate REFER or DECLINE — no trial initiated

---

## Condition → Model → Threshold Mappings

| Condition | Primary Hypothesis | Key Model | Key Threshold | Outcome Measure |
|-----------|-------------------|-----------|---------------|-----------------|
| Low back pain | Disc / Facet / Neural | Hypothesis-Driven Intervention | Continuation Criteria | ODI, NPRS |
| Sciatica | Nerve root compression | Non-Response as Signal | Red Flag Referral | SLR, NPRS, LEFS |
| Neck pain | Facet / Disc / Muscular | Hypothesis-Driven Intervention | Trial Window Limits | NDI, NPRS |
| Shoulder impingement | Subacromial / RC weakness | Dose-Response Coupling | Continuation Criteria | DASH, ROM |
| Rotator cuff post-surgical | Tissue healing timeline | Dose-Response Coupling | Trial Window Limits | ROM milestones |
| ACL reconstruction | Phase-based rehabilitation | Hypothesis-Driven Intervention | Continuation Criteria | ROM, LSI, hop tests |
| Frozen shoulder | Stage-dependent (freezing/frozen/thawing) | Non-Response as Signal | Exit Criteria | ROM, DASH |
| Knee osteoarthritis | Load tolerance / quad weakness | Dose-Response Coupling | Continuation Criteria | KOOS, TUG |
| Plantar fasciitis | Fascial overload / windlass | Hypothesis-Driven Intervention | Trial Window Limits | NPRS, FFI |
| Achilles tendinopathy | Tendon loading capacity | Dose-Response Coupling | Continuation Criteria | VISA-A, NPRS |
| Tennis elbow | Tendon + cervical contribution | Hypothesis-Driven Intervention | Continuation Criteria | DASH, grip strength |
| Whiplash | Cervical strain / fear-avoidance | Non-Response as Signal | Trial Window Limits | NDI, ROM |
| Fibromyalgia | Central sensitization | Subjective Report Insufficiency | Exit Criteria | FIQ, activity diary |
| TMJ disorder | Myogenic / arthrogenic / cervical | Hypothesis-Driven Intervention | Trial Window Limits | MMO, NPRS |
| Pelvic floor dysfunction | Hypertonic / hypotonic | Hypothesis-Driven Intervention | Continuation Criteria | PFM assessment |
| Post-concussion | Cervicogenic / vestibular / exertion | Non-Response as Signal | Red Flag Referral | PCSS, BESS |
| Scoliosis | Curve progression / functional limitation | Dose-Response Coupling | Continuation Criteria | Cobb angle, ATR |
| Thoracic outlet syndrome | Scalene / postural / first rib | Hypothesis-Driven Intervention | Trial Window Limits | DASH, ULNT |

---

## Outcome Measure Reference

| Abbreviation | Full Name | Domain | MCID | Used For |
|-------------|-----------|--------|------|----------|
| NPRS | Numeric Pain Rating Scale | Pain intensity | 2 points | All conditions |
| VAS | Visual Analogue Scale | Pain intensity | 20mm | All conditions |
| ODI | Oswestry Disability Index | Back disability | 6-10 points | Low back pain, spinal stenosis |
| NDI | Neck Disability Index | Neck disability | 5-7 points | Neck pain, whiplash, cervical radiculopathy |
| DASH | Disabilities of Arm, Shoulder, Hand | Upper extremity function | 10-15 points | Shoulder, elbow, wrist, hand conditions |
| LEFS | Lower Extremity Functional Scale | Lower extremity function | 9 points | Hip, knee, ankle, foot conditions |
| KOOS | Knee Injury and Osteoarthritis Outcome Score | Knee function | 8-10 points | Knee OA, meniscus, ACL, patellofemoral |
| TUG | Timed Up and Go | Mobility/balance | 2.5 seconds | Geriatric, fall risk, post-surgical |
| 6MWT | Six Minute Walk Test | Endurance | 50 meters | Spinal stenosis, general deconditioning |
| PSFS | Patient-Specific Functional Scale | Individualized function | 2 points | Any condition |
| FIQ | Fibromyalgia Impact Questionnaire | Fibromyalgia impact | 14% | Fibromyalgia |
| VISA-A | Victorian Institute of Sport Assessment – Achilles | Achilles function | 12 points | Achilles tendinopathy |
| FFI | Foot Function Index | Foot disability | 7 points | Plantar fasciitis, foot conditions |
| LSI | Limb Symmetry Index | Bilateral comparison | >90% = pass | ACL rehab, return to sport |
| BESS | Balance Error Scoring System | Balance | 3 errors | Post-concussion |

---

## Academic Evidence Base

### Key References Supporting the Decision System
- Bayesian reasoning in clinical practice: Sox HC, Higgins MC. Medical Decision Making (2013)
- Non-response as diagnostic information: Herbert RD et al. BMJ (2005)
- Hypothesis-driven clinical reasoning: Jones MA. Physical Therapy (1992)
- Exit criteria in physiotherapy: Foster NE et al. Lancet (2018) — STarT Back approach
- Dose-response in exercise therapy: Geneen LJ et al. Cochrane Database (2017)
- Subjective vs objective outcomes: Kamper SJ et al. JOSPT (2010)
- Trial windows in musculoskeletal care: Lin I et al. British Journal of Sports Medicine (2020)
- Fear-avoidance as chronicity predictor: Vlaeyen JWS, Linton SJ. Pain (2000)
- Imaging findings in asymptomatic populations: Brinjikji W et al. AJNR (2015)
- Exercise for tendinopathy: Malliaras P et al. Sports Medicine (2013)
- Prehabilitation evidence: Cabilan CJ et al. JBI Database (2015)
- Pain neuroscience education: Louw A et al. Physiotherapy Theory and Practice (2016)
- Central sensitization: Nijs J et al. Manual Therapy (2014)
- Return-to-sport criteria: Grindem H et al. British Journal of Sports Medicine (2016)
- Graded motor imagery: Moseley GL. Neuroscience Letters (2004)

---

*This document is part of the Recovery TLV Clinical Decision System. It is structured for machine readability and LLM consumption.*
