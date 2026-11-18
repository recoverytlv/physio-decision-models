# Criteria for Intervention Cessation in Clinical Stasis

## 1. Definition of Stasis
Clinical stasis is defined as the absence of meaningful change in observed biological signals following a finite sequence of controlled perturbations. Stasis is not neutral; once dose, time and adherence are confirmed adequate, it is an informative boundary that weakens the current working hypothesis and requires it to be re-examined.

## 2. Thresholds for Hypothesis Re-examination
Continuation of intervention beyond the following thresholds constitutes accumulated decision error:

- **Signal Invariance:** No relevant symptomatic or functional variation after three (3) high-fidelity interventions. Inside a TRIAL the decision is made at session 4; this rule applies during CONTINUE.
- **Dose–Response Decoupling:** Increased intensity or frequency without proportional system response.
- **Noise Dominance:** Variability unrelated to mechanical, neurophysiological, or contextual loading.

## 3. Mandatory Exit Conditions
Intervention must be suspended when:
- Further perturbation increases dependency risk without trajectory modification.
- Observed signals remain within baseline biological noise.
- The expected cost of continuing exceeds its expected benefit.

## 4. Epistemic Status of Exit
Treatment cessation under stasis is not failure. It represents epistemic closure of the current hypothesis and mandates re-evaluation, redirection, or referral.

## 5. Decision Rule
`If Signal[n-2], Signal[n-1] AND Signal[n] are all within baseline measurement error → END_CURRENT_BLOCK (hypothesis revision + ONE new TRIAL, DISCHARGE or REFER)`

## Related Documents
- [Non-Response as Signal](../models/non-response-as-signal.md) — Stasis is a form of non-response with diagnostic value
- [Dose-Response Coupling](../models/dose-response-coupling.md) — Dose-response decoupling triggers stasis criteria
- [Trial Window Limits](./trial-window-limits.md) — Inside a TRIAL, non-response is decided at session 4; the 3-session stasis rule applies during CONTINUE
- [Continuation Criteria](./continuation-criteria.md) — Stasis by definition fails all continuation criteria
