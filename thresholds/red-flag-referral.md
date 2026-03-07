# Red Flag Detection and Mandatory Referral

## 1. Definition
Red flags are clinical signs or symptoms that indicate a potentially serious underlying pathology requiring assessment beyond physiotherapy scope. Detection of any red flag triggers mandatory REFER or DECLINE.

## 2. Red Flag Categories

### 2.1 Neurological Red Flags
- Progressive neurological deficit (worsening weakness, numbness, or coordination)
- Cauda equina syndrome signs (saddle anaesthesia, bladder/bowel dysfunction)
- Upper motor neuron signs inconsistent with musculoskeletal origin

### 2.2 Systemic Red Flags
- Unexplained weight loss (>5% body weight in 3 months)
- Night pain unrelated to mechanical loading
- Fever or systemic illness concurrent with musculoskeletal complaint
- History of malignancy with new onset pain

### 2.3 Vascular Red Flags
- Signs of deep vein thrombosis (unilateral swelling, warmth, tenderness)
- Pulsatile mass or vascular bruit in the region of complaint
- Acute limb ischaemia signs

### 2.4 Structural Red Flags
- Suspected fracture (trauma mechanism, point tenderness, deformity)
- Joint instability suggesting ligamentous rupture requiring surgical assessment
- Suspected infection (local warmth, erythema, swelling with systemic signs)

## 3. Decision Consequences
- Red flag detection overrides all other decision logic
- No trial period is initiated when red flags are present
- The system output is REFER (to appropriate medical specialist) or DECLINE
- Documentation must specify the red flag identified and the referral destination

## 4. Decision Rule
`If Red_Flag_Detected == TRUE → REFER OR DECLINE (immediate)`

## Related Documents
- [Trial Window Limits](./trial-window-limits.md) — Red flags override trial window and prevent TRIAL initiation
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md) — Red flags invalidate the musculoskeletal hypothesis entirely
- [Exit Criteria for Stasis](./exit-criteria-stasis.md) — Red flags are distinct from stasis — they demand immediate action, not observation
- [Continuation Criteria](./continuation-criteria.md) — Red flags override continuation criteria regardless of objective improvement
