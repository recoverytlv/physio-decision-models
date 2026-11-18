---
title: "Carpal Tunnel Syndrome"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 1.3.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Compression neuropathy of the median nerve at the carpal tunnel. Symptoms include numbness and tingling in the thumb, index, middle, and radial half of the ring finger, with possible weakness of thumb opposition and grip strength."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "3-5 sessions"
continuation_threshold: ">=10% objective functional improvement"
red_flags:
  - "Thenar muscle wasting (atrophy of the thumb muscles)"
  - "Constant numbness (loss of protective sensation)"
  - "Progressive motor weakness (difficulty gripping, dropping objects frequently)"
  - "Symptoms not responding to 6–8 weeks of conservative management"
  - "Bilateral CTS with systemic symptoms (consider hypothyroidism, diabetes, rheumatoid arthritis)"
  - "Symptoms inconsistent with median nerve distribution (consider cervical radiculopathy, thoracic outlet syndrome, or double crush syndrome)"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/carpal-tunnel-syndrome.md"
clinic: "https://recoverytlv.co.il"
---

# Carpal Tunnel Syndrome

## Condition
Compression neuropathy of the median nerve at the carpal tunnel. Symptoms include numbness and tingling in the thumb, index, middle, and radial half of the ring finger, with possible weakness of thumb opposition and grip strength.

## Scope Check
Mild to moderate carpal tunnel syndrome is within physiotherapy scope for conservative management. Severe CTS (constant numbness, thenar muscle wasting, failed conservative treatment) requires surgical consultation (REFER).

## Red Flags (→ REFER)
- Thenar muscle wasting (atrophy of the thumb muscles)
- Constant numbness (loss of protective sensation)
- Progressive motor weakness (difficulty gripping, dropping objects frequently)
- Symptoms not responding to 6–8 weeks of conservative management
- Bilateral CTS with systemic symptoms (consider hypothyroidism, diabetes, rheumatoid arthritis)
- Symptoms inconsistent with median nerve distribution (consider cervical radiculopathy, thoracic outlet syndrome, or double crush syndrome)

## Clinical Hypothesis Examples
- **Mechanical compression — wrist position:** Sustained wrist flexion or extension during work/sleep compresses the carpal tunnel. Tested with ergonomic modification, wrist splinting (neutral position), and activity modification. Expected response: reduced nocturnal symptoms and improved daytime function within 3–5 sessions.
- **Neural mobility restriction:** Restricted median nerve gliding contributing to symptoms. Tested with median nerve glides and neurodynamic mobilization. Expected response: improved nerve tension test tolerance and reduced distal symptoms.
- **Cervical contribution (double crush):** Cervical radiculopathy or thoracic outlet syndrome contributing to or mimicking CTS. Tested with cervical treatment and upper limb neurodynamics. Expected response: if cervical-driven, distal symptoms improve with proximal treatment.
- **Tendon and tenosynovial load:** Thickening of the flexor tenosynovium (non-inflammatory fibrosis of the subsynovial connective tissue; Ettema 2004, PMID 15252093) raising carpal tunnel pressure. Tested with activity modification and tendon gliding exercises. Expected response: reduced Phalen's and Tinel's test provocation.

## Trial Window
3–5 sessions. Objective criteria:
- Reduced frequency or intensity of nocturnal symptoms
- Improved grip strength (measured with dynamometer)
- Improved Phalen's or Tinel's test response
- Improved functional capacity (writing, gripping, typing)

## Non-Response
If no objective criterion is met by the end of the trial window (3–5 sessions), revise the hypothesis once or refer. Symptoms that have not responded after 6–8 weeks of conservative management are referred for nerve conduction studies (NCS/EMG) and surgical consultation. Persistent motor deficit or sensory loss should not be managed conservatively beyond the trial window.

## Related Documents
- [Lateral Epicondylalgia](lateral-epicondylalgia.md)
- [Neck Pain](neck-pain.md)
- [Non-Response as Signal](../models/non-response-as-signal.md)
- [Red Flag Referral](../thresholds/red-flag-referral.md)
