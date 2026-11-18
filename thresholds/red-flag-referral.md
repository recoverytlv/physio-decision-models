# Red Flag Detection and Mandatory Referral

## 1. Definition
Red flags are clinical signs or symptoms that indicate a potentially serious underlying pathology requiring assessment beyond physiotherapy scope. In acute low back pain, some red flags have very high false-positive rates and, used in isolation, little diagnostic value (Henschke 2009); only a small subset are informative for fracture or malignancy, and the probability of fracture is higher when several are present (Downie 2013). These data concern low back pain; they do not lower the weight of emergency signs, where a single finding is enough to act. A clinically significant red flag, or a combination of flags, that raises suspicion of serious pathology in context triggers mandatory REFER.

## 2. Red Flag Categories

### 2.1 Neurological Red Flags
- Progressive neurological deficit (worsening weakness, numbness, or coordination)
- Cauda equina syndrome signs (saddle anaesthesia, bladder/bowel dysfunction)
- Upper motor neuron signs inconsistent with musculoskeletal origin

### 2.2 Systemic Red Flags
- Unexplained weight loss
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
- The system output is REFER (to the appropriate medical specialist; emergencies to the ER)
- Documentation must specify the red flag identified and the referral destination

## 4. Decision Rule
`If Clinically_Significant_Red_Flag == TRUE → REFER (immediate)`

## Related Documents
- [Trial Window Limits](./trial-window-limits.md) — Red flags override trial window and prevent TRIAL initiation
- [Hypothesis-Driven Intervention](../models/hypothesis-driven-intervention.md) — Red flags invalidate the musculoskeletal hypothesis entirely
- [Exit Criteria for Stasis](./exit-criteria-stasis.md) — Red flags are distinct from stasis — they demand immediate action, not observation
- [Continuation Criteria](./continuation-criteria.md) — Red flags override continuation criteria regardless of objective improvement
