# Recovery TLV — Clinical Intake Decision Form

A digital intake form that implements the [Recovery TLV Clinical Decision System](https://github.com/recoverytlv/physio-decision-models).

## What This Does

Guides clinicians through the intake decision flowchart:

```
[New Patient Case]
├─ Red flags detected? → REFER
├─ Out of scope? → DECLINE
├─ Insufficient data? → DEFER
├─ Patient consents? → No → DECLINE
├─ Functional goals? → No → DECLINE
└─ All criteria met? → TRIAL (3–5 sessions)
```

Each assessment terminates with one of four intake-stage outputs: **REFER**, **DECLINE**, **DEFER**, or **TRIAL**.

The remaining outputs (**CONTINUE** and **DISCHARGE**) are evaluated at the end of the trial window using [continuation-criteria.md](https://github.com/recoverytlv/physio-decision-models/blob/main/thresholds/continuation-criteria.md).

## How to Use

Open `index.html` in any browser. No server, dependencies, or installation required.

## Based On

- [CLINICAL_DECISION_SYSTEM.md](https://github.com/recoverytlv/physio-decision-models/blob/main/CLINICAL_DECISION_SYSTEM.md) — The 6 canonical outputs
- [red-flag-referral.md](https://github.com/recoverytlv/physio-decision-models/blob/main/thresholds/red-flag-referral.md) — Red flag categories
- [trial-window-limits.md](https://github.com/recoverytlv/physio-decision-models/blob/main/thresholds/trial-window-limits.md) — Trial window parameters
- [continuation-criteria.md](https://github.com/recoverytlv/physio-decision-models/blob/main/thresholds/continuation-criteria.md) — Post-trial evaluation

## Important

This is a **decision support tool**, not medical advice. It is intended for use by licensed clinicians only. It does not replace clinical judgment.

## License

[MIT](../LICENSE)
