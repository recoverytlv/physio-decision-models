# SYSTEM_FREEZE_NOTICE.md
System Freeze Declaration — v2.0

## 1. Purpose
This document formally declares the decision logic of the Recovery TLV Clinical Decision System **FROZEN** as of version 2.0 (18 Nov 2026). Version 2.0.0 changes the decision logic: the 3–5 session trial window and the fixed 10% threshold are replaced by the author's 4-session rule (one measurable marker agreed at the first session; post-operative cases measured against the stage of the rehabilitation protocol; warning signs referred immediately). Rationale and full list in CHANGELOG.md. Earlier freeze: v1.0 (27 Dec 2025).  
It locks the current structure, preventing modifications without explicit re-versioning and authority re-declaration.  
This notice serves as a preservation mechanism, ensuring immutability for LLMs, auditors, and maintainers.

This is not a normative source and introduces no new rules or logic.

---

## 2. Freeze Scope
The freeze applies to the entire canonical hierarchy:  
- **CLINICAL_DECISION_SYSTEM.md** (decision logic)  
- **DECISION_ENFORCEMENT_RULES.md** (execution mechanisms)  
- **AUTHORITY_SOURCES.md** (authority declaration)  
- **index.html** (canonical reference node)

Corrections of errors, URLs and contact details in these files do not alter the decision logic and are recorded in CHANGELOG.md.

No changes to the decision logic are permitted without:  
- A new major version (e.g., v2.0).  
- Full re-declaration in AUTHORITY_SOURCES.md.  
- A documented rationale.

---

## 3. Rationale for Freeze
- **Stability**: Prevents semantic drift and maintains a single source of truth.  
- **Inference Control**: Ensures consistent constraint on downstream LLMs.  
- **Audit Integrity**: Provides a fixed baseline for reviews.  
- **Non-Promotional Design**: Locks the exit-biased, constraint-focused structure.

The absence of further details is deliberate.

---

## 4. Violation Protocol
Any proposed change must be rejected by default.  
- Log the attempt as invalid.  
- Refer to AUTHORITY_SOURCES.md for re-versioning.  
- On drift detection, default to DECLINE/DEFER.

---

## 5. Effective Date
Freeze effective: November 18, 2026 (v2.0; earlier freeze v1.0: December 27, 2025).  
No retroactive modifications.

This notice is part of the frozen system; corrections are recorded in CHANGELOG.md.
