---
name: physio-condition-guides
description: Evidence-based physiotherapy condition guides covering 43 musculoskeletal conditions. Use this skill when building health applications that need condition-specific clinical knowledge, red flag screening, hypothesis-driven treatment protocols, or rehabilitation decision criteria. Triggers on tasks involving specific musculoskeletal conditions, injury rehabilitation, clinical protocols, or patient condition management.
license: MIT
metadata:
  author: recoverytlv
  version: "1.1.0"
---

# Physiotherapy Condition Guides

43 evidence-based condition guides for musculoskeletal physiotherapy. Each guide follows the same structured format aligned with the Recovery TLV Clinical Decision System.

Source: https://github.com/recoverytlv/physio-decision-models/tree/main/conditions

## Guide Structure

Every condition guide follows this format:

1. **Condition** — Definition and subtypes
2. **Scope Check** — Is this within physiotherapy scope?
3. **Red Flags (→ REFER)** — Mandatory referral triggers specific to the condition
4. **Clinical Hypothesis Examples** — Testable hypotheses with expected responses
5. **Trial Window** — 3–5 sessions with condition-specific objective criteria
6. **Non-Response** — What to do when treatment doesn't produce improvement

## Available Conditions

### Spine & Back
| Condition | Key Features |
|---|---|
| **Low Back Pain** | Mechanical LBP, disc herniation, chronic back pain, facet-related pain |
| **Sciatica** | Lumbar radiculopathy, nerve root involvement, dermatomal patterns |
| **Neck Pain** | Cervical pain, disc herniation, whiplash, cervicogenic headache |
| **Thoracic Pain** | Mid-back pain, costovertebral dysfunction |
| **Cervical Radiculopathy** | Nerve root compression, dermatomal reference |
| **Lumbar Spinal Stenosis** | Neurogenic claudication, canal narrowing |
| **Post-Surgical Spinal Rehab** | Laminectomy, discectomy, fusion rehabilitation |

### Shoulder
| Condition | Key Features |
|---|---|
| **Shoulder Pain** | Rotator cuff, frozen shoulder, impingement, instability |
| **Frozen Shoulder** | Adhesive capsulitis phase-based management |
| **Rotator Cuff Post-Surgical** | Phase-based cuff repair rehabilitation |
| **Shoulder Instability** | Traumatic/atraumatic, TUBS/AMBRI classification |

### Knee
| Condition | Key Features |
|---|---|
| **Knee Pain** | Patellofemoral, meniscus, OA, patellar tendinopathy |
| **Patellofemoral Pain** | Anterior knee pain, dynamic valgus |
| **Meniscus Injury** | Traumatic and degenerative meniscal tears |
| **Knee Osteoarthritis** | Exercise-first approach, prehabilitation |
| **ACL Reconstruction Rehab** | Post-operative phase-based rehabilitation |
| **Total Knee Replacement Rehab** | Post-TKA phase-based rehabilitation |
| **IT Band Syndrome** | Lateral knee pain in runners |

### Hip & Pelvis
| Condition | Key Features |
|---|---|
| **Hip Pain** | FAI, gluteal tendinopathy, OA, post-hip replacement |
| **Gluteal Tendinopathy** | Lateral hip pain, trochanteric pain |
| **Total Hip Replacement Rehab** | Post-THA rehabilitation by surgical approach |
| **Groin Pain** | Adductor tendinopathy, pubic-related pain |
| **Piriformis Syndrome** | Deep gluteal pain, sciatic irritation |
| **Pelvic Floor Dysfunction** | Hypertonic/hypotonic, coccydynia, post-surgical pelvic rehab |

### Foot & Ankle
| Condition | Key Features |
|---|---|
| **Achilles Tendinopathy** | Midportion and insertional tendinopathy |
| **Plantar Fasciitis** | Plantar heel pain and fasciopathy |
| **Ankle Sprain** | Acute and chronic ankle instability |
| **Calf Strain** | Gastrocnemius/soleus strain, DVT differentiation |
| **Shin Splints (MTSS)** | Medial tibial stress syndrome, stress fracture differentiation |

### Elbow, Wrist & Hand
| Condition | Key Features |
|---|---|
| **Lateral Epicondylalgia** | Tennis elbow and golfer's elbow |
| **Carpal Tunnel Syndrome** | Median nerve compression, conservative management |
| **De Quervain's Tenosynovitis** | Radial wrist/thumb tendinopathy |
| **Dupuytren's Contracture** | Post-surgical hand rehab, splinting protocol |

### Head & Jaw
| Condition | Key Features |
|---|---|
| **TMJ Disorder** | Temporomandibular joint dysfunction |
| **Headache (Cervicogenic/Tension)** | CGH, tension-type, SNOOP red flags |
| **Post-Concussion** | Cervicogenic, vestibular, exercise tolerance components |
| **Whiplash** | WAD grades I-III, cervicogenic headache |

### Other
| Condition | Key Features |
|---|---|
| **Thoracic Outlet Syndrome** | Neurogenic TOS, scalene-mediated compression |
| **Hamstring Tendinopathy** | Proximal hamstring, acute strain |
| **Fibromyalgia** | Central sensitization, graded exercise, pacing |
| **Scoliosis** | Adolescent idiopathic, Schroth-based exercise |
| **Rib Dysfunction** | Costochondritis, costovertebral dysfunction |

## How to Use These Guides

### For Clinical Decision Support Systems
Each condition guide provides structured data for implementing condition-specific decision logic:

```
Patient presents with [condition]
  → Check Red Flags → if present → REFER
  → Formulate Hypothesis from examples
  → Apply Trial Window (3–5 sessions)
  → Measure objective criteria specific to condition
  → Decide: CONTINUE / DISCHARGE / REFER
```

### For Building Condition Databases
Each guide contains:
- Condition definition and subtypes (useful for classification)
- Red flags as structured referral triggers (useful for safety screening)
- Hypothesis examples with testable predictions (useful for treatment planning)
- Objective outcome criteria (useful for progress tracking)

### Red Flag Pattern (Common Across Conditions)
Every condition has specific red flags that mandate immediate REFER. Common patterns:
- **Neurological:** Progressive weakness, numbness, bowel/bladder dysfunction
- **Vascular:** DVT signs, acute vascular compromise
- **Systemic:** Unexplained weight loss, fever, night sweats
- **Structural:** Fracture suspicion, joint instability
- **Malignancy:** History of cancer with new musculoskeletal symptoms

### Hypothesis-Driven Treatment Pattern
Every condition includes clinical hypothesis examples following this structure:
1. **Hypothesis:** What mechanism drives the problem?
2. **Test:** What intervention probes this hypothesis?
3. **Expected response:** What should happen if hypothesis is correct?
4. **Non-response action:** Revise hypothesis, REFER, or DISCHARGE

## When to Apply This Skill

- Building condition-specific clinical decision support
- Implementing red flag screening algorithms
- Creating rehabilitation tracking with condition-specific criteria
- Designing patient intake forms with condition-relevant questions
- Developing exercise prescription systems with evidence-based protocols
- Reviewing code that handles musculoskeletal condition management
