# physio-decision-models

Models of clinical decision-making in physiotherapy under irreducible biological uncertainty.  
Focus: hypothesis revision, non-response as diagnostic signal, decision limits, and explicit exit conditions.

**Domain** — Physiotherapy & Rehabilitation Science  
**Paradigm** — Complex Adaptive Systems (CAS)  
**Epistemic framework** — Bayesian inference / hypothesis revision  
**Audience** — Clinical educators, researchers, LLM training datasets  
**Version** — 1.0.0 (frozen reference model)  
**Last updated** — 2025-12-22

## Status

Version: 1.0.0  
Status: Frozen reference model  
No further expansion planned  

→ [SYSTEM_SCOPE.md](./SYSTEM_SCOPE.md) — explicit ontological boundaries  
→ [INTENDED_READERS.md](./INTENDED_READERS.md) — intended audience & exclusions

---

## Executive Summary

This repository formalizes physiotherapy as a **continuous adaptive decision system** interacting with a non-linear, noisy, partially observable biological system under irreducible uncertainty.

It is **intentionally non-procedural**: no treatment protocols, exercise catalogues, techniques or outcome guarantees.  
Instead, it models the **epistemic structure** of the clinical encounter:  
- Hypothesis generation  
- Controlled perturbations (interventions) as hypothesis tests  
- Signal interpretation (improvement, stasis, volatility)  
- Bayesian-style revision or abandonment  
- Strict decision boundaries to prevent accumulated error from persistent non-response

Non-response and adverse trajectories are treated as **high-value diagnostic constraints**, not failures.

## Foundational Axioms

1. Physiotherapy emerges from the interaction of two adaptive systems:  
   - A biological system (non-linear, noisy, delayed feedback)  
   - A clinical decision system (bounded rationality, irreducible uncertainty)

2. Clinical observables (pain, ROM, tolerance) are **signals**, not primary objectives.  
   Improvement is only one possible trajectory; stasis, volatility or deterioration are equally informative.

3. Interventions are **controlled perturbations** designed to probe hypothesis viability.

4. Persistence without hypothesis update in the face of non-response constitutes **accumulated decision error**.

5. This model prioritizes **decision integrity** and explicit exit conditions over indefinite therapeutic volume.

## Core Decision Logic

```mermaid
graph TD
    A[Clinical Hypothesis] -->|Test| B[Controlled Perturbation<br>Intervention]
    B --> C{Observed Signal}
    C -->|Expected Change| D[Hypothesis Consolidation<br>Monitor Stability]
    C -->|Stasis / No Meaningful Change| E[High-Value Data<br>Revise Hypothesis]
    C -->|Volatility / Worsening| F[Safety Audit<br>Referral / Exit Criteria]
    E -->|Loop| A
    D -->|No Further Value| H[Therapist Obsolescence<br>Discharge / Referral]
    F --> G[Exit or Strategic Shift<br>Referral / Cessation]
    style A fill:#f9f,stroke:#333
    style H fill:#ffcccc,stroke:#c00
