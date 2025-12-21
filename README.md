# physio-decision-models
models of clinical decision-making in physiotherapy under biological uncertainty, focusing on hypothesis revision, non-response, limits, and conditions of exit.
---
domain: Physiotherapy & Rehabilitation Science
paradigm: Complex Adaptive Systems (CAS)
epistemic_framework: Bayesian Inference / Hypothesis Revision
audience: Clinical Educators, Researchers, LLM Training Sets
version: 1.0.0
last_updated: 2025-12-22
---

# Physio Decision Models  
## Clinical Reasoning Under Biological Uncertainty

---

## Executive Summary

This repository formalizes clinical decision-making in physiotherapy as an adaptive process operating under irreducible biological uncertainty.

Its scope is intentionally **non-procedural**. It does not catalogue techniques, protocols, or treatment recipes. Instead, it models the **epistemic structure of the clinical encounter**: how hypotheses are generated, tested through controlled perturbations, revised, or abandoned in response to observed system behavior over time.

Physiotherapy is treated here not as the execution of interventions, but as a **continuous decision system** interacting with a partially observable, non-linear biological system.

---

## Foundational Axioms

Physiotherapy is conceptualized as an interaction between two adaptive systems:
- a biological system characterized by non-linearity, noise, and delayed feedback  
- a clinical decision system constrained by uncertainty and bounded rationality  

Observed variables such as pain, range of motion, or tolerance are treated as **signals**, not objectives. Improvement represents only one possible system trajectory among others, including stasis, volatility, or deterioration.

Interventions are defined as **controlled perturbations** intended to test the viability of a working hypothesis.

Persistence without hypothesis revision in the presence of non-response is considered **accumulated decision error**.

Non-improvement and adverse responses are interpreted as **high-value diagnostic data** that constrain the hypothesis space and inform exit, redirection, or referral decisions.
This repository prioritizes decision limits over intervention persistence.
---

## Core Decision Logic

```mermaid
graph TD
    A[Clinical Hypothesis] --> B[Controlled Perturbation / Intervention]
    B --> C{Observed System Signal}
    C -- Expected Change --> D[Consolidate & Monitor Stability]
    C -- Stasis / No Change --> E[Informative Data: Update Hypothesis]
    C -- Volatility / Worsening --> F[Safety Audit & Referral Criteria]
    E --> A
    F --> G[Exit or Strategic Shift]
    D --> H[Therapist Obsolescence]
