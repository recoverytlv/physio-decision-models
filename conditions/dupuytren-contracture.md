---
title: "Dupuytren's Contracture — Physiotherapy Scope"
type: clinical-decision-guide
system: "Recovery TLV Clinical Decision System"
version: 2.0.0
status: supporting-guide
license: MIT
author: "Alejandro Zubrisky, PT"
author_orcid: "0009-0003-1069-937X"
organization: "Recovery TLV, Tel Aviv, Israel"
summary: "Progressive fibroproliferative disorder of the palmar fascia causing finger flexion contracture. Physiotherapy does not reverse it; the role is hand function, post-procedural rehabilitation and timely referral."
decision_outputs: [DECLINE, DEFER, REFER, TRIAL, CONTINUE, DISCHARGE]
trial_window: "4 sessions"
continuation_threshold: "measurable change in the marker agreed at the first session, beyond measurement error"
red_flags:
  - "Rapidly progressing contracture → surgical/procedural evaluation"
  - "MCP contracture >30° or any PIP contracture — 'table top test' positive → surgical opinion"
  - "Contracture causing functional limitation (can't put hand in pocket, wash face, grip properly)"
  - "Suspected Dupuytren's diathesis (young onset, bilateral, family history, ectopic disease) — more aggressive, needs specialist monitoring"
canonical: "https://github.com/recoverytlv/physio-decision-models/blob/main/conditions/dupuytren-contracture.md"
clinic: "https://recoverytlv.co.il"
---

# Dupuytren's Contracture — Physiotherapy Scope

## Definition
Progressive fibroproliferative disorder of the palmar fascia causing flexion contracture of the fingers, most commonly ring and little fingers. Characterised by myofibroblast proliferation and pathological collagen deposition.

## Scope Boundaries
- **IN scope:** Pre-surgical optimization, post-surgical rehabilitation (fasciectomy, needle aponeurotomy, collagenase injection), splinting for contracture management, functional hand rehabilitation
- **OUT of scope:** Surgical decision-making, injection procedures

## Important Context
Dupuytren's has a strong hereditary component; heavy manual work and exposure to vibration are associated with a higher risk (Descatha 2011, PMID 21575231; Mathieu 2020, PMID 32061740). It cannot be "cured" by physiotherapy. The role of physiotherapy is to optimize hand function, manage post-procedural recovery, and maintain gains from surgical/procedural intervention.

## Red Flags → REFER
- Rapidly progressing contracture → surgical/procedural evaluation
- MCP contracture >30° or any PIP contracture — "table top test" positive → surgical opinion
- Contracture causing functional limitation (can't put hand in pocket, wash face, grip properly)
- Suspected Dupuytren's diathesis (young onset, bilateral, family history, ectopic disease) — more aggressive, needs specialist monitoring

## Clinical Hypothesis Framework

### Post-Fasciectomy Rehabilitation
- **Hypothesis:** Post-surgical edema, scarring, and stiffness limit functional recovery
- **Test:** Edema management, scar mobilization, progressive AROM/PROM, splinting protocol
- **Expected response:** Progressive ROM gains, reduced edema, improved grip strength over 6-12 weeks
- **If no response:** Consider wound complication, nerve injury, or recurrence → REFER back to surgeon

### Post-Needle Aponeurotomy / Collagenase
- **Hypothesis:** Extension gained from procedure needs to be maintained with exercise, and with splinting when indicated
- **Test:** Active exercise program and functional hand use; night extension splinting when extension is being lost or when the treating surgeon prescribes it
- **Expected response:** Maintained extension gains, improved functional hand use
- **If losing extension:** Start or review night splinting, consider recurrence

### Early/Mild Dupuytren's (No Procedure Done)
- **Hypothesis:** Physiotherapy can maintain hand function and monitor progression
- **Test:** Stretching, functional exercises, education about condition
- **Expected response:** Maintained function (note: physiotherapy does NOT reverse Dupuytren's)
- **Decision:** Monitor every 3-6 months. REFER for procedure when table top test positive

## Post-Surgical Splinting Protocol

| Phase | Timeframe | Splinting | Exercise |
|-------|-----------|-----------|----------|
| Phase 1 | 0-2 weeks | Per surgeon's protocol | Gentle AROM within comfort |
| Phase 2 | 2-6 weeks | Per surgeon's protocol; night splint if extension is being lost | Progressive AROM/PROM, scar massage, edema management |
| Phase 3 | 6-12 weeks | Night splint if extension is being lost | Grip strengthening, functional tasks, full ROM exercises |
| Phase 4 | 3-6 months | Night splint if needed | Full function, monitor for recurrence |

Splinting practice varies between surgeons, and the treating surgeon's protocol takes precedence. In a randomised trial, routine night splinting after fasciectomy or dermofasciectomy added no benefit to hand therapy alone (Jerosch-Herold et al. 2011, PMID 21693044); the timeline above is a guide, not a validated protocol.

## Trial Protocol (TRIAL)
| Session | Focus |
|---------|-------|
| 1 | Assessment: ROM deficit, functional limitation, procedure history, splint assessment |
| 2-3 | Targeted rehabilitation (scar, ROM, splinting, edema) |
| 4 | Re-evaluate: ROM gains, functional improvement |

## Decision Criteria

### CONTINUE if:
- Progressive ROM gains
- Improving grip strength
- Reducing edema
- Functional improvement documented

### DISCHARGE if:
- Maximum ROM achieved and stable
- Functional goals met
- Independent home program and splinting established

### REFER if:
- Early Dupuytren's with positive table top test → procedure evaluation
- Post-surgical complications (wound breakdown, nerve symptoms, infection signs)
- Rapid recurrence after procedure
- No ROM gains after 6 weeks of structured post-surgical rehab

## Cross-References
- [De Quervain's Tenosynovitis](./de-quervain-tenosynovitis.md) — Hand/wrist conditions
- [Carpal Tunnel Syndrome](./carpal-tunnel-syndrome.md) — May coexist
- [Trial Window Limits](../thresholds/trial-window-limits.md) — Post-surgical rehab follows the surgeon's protocol; progress is measured against the protocol stage instead of a session count
