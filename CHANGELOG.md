# Changelog

All notable changes to the Recovery TLV Clinical Decision System are documented here.

Format based on [Keep a Changelog](https://keepachangelog.com/).

---

## [1.2.0] — 2026-03-07

### Added

**LLM SEO & Discoverability:**
- `KNOWLEDGE_GRAPH.md` — Structured entity relationships for LLM consumption
- Expanded `llms.txt` with clinical knowledge tables, decision pathways, treatment benchmarks
- Expanded `llms-ctx.txt` with entity relationships, clinical facts, structured Q&A
- Additional `FAQPage` entries and `knowsAbout` topics in Schema.org JSON-LD

**Reference Documents (7 new):**
- `RED_FLAGS_QUICK_REFERENCE.md` — Consolidated red flags by body region
- `PAIN_NEUROSCIENCE_EDUCATION.md` — Patient-facing pain science guide
- `CHRONIC_PAIN_FRAMEWORK.md` — Chronic pain within the decision system
- `MANUAL_THERAPY_PRINCIPLES.md` — When and how manual therapy fits
- `DISCHARGE_PLANNING.md` — Structured transition to self-management
- `WORKPLACE_ERGONOMICS.md` — Desk/standing desk/lifting guidelines
- `PREGNANCY_MUSCULOSKELETAL.md` — Pregnancy-related MSK conditions

**Academic References:**
- Expanded `EVIDENCE_BASE.md` with references by topic (pain neuroscience, exercise, tendinopathy, clinical decision-making, imaging, return to sport, pregnancy, outcome measures, geriatrics)

**Metadata Updates:**
- All 8 new documents added to `sitemap.xml`, `index.html` Schema.org, `llms.txt`, `README.md`
- Removed Arabic translation references

---

## [1.1.0] — 2025-12-23

### Added

**Condition Guides (24 new):**
- Whiplash (WAD I-III), ankle sprain, TMJ disorder, post-surgical spinal rehab
- Rotator cuff post-surgical, frozen shoulder, carpal tunnel syndrome
- IT band syndrome, piriformis syndrome, thoracic pain, groin pain
- Hamstring tendinopathy, de Quervain's tenosynovitis, cervical radiculopathy
- Total knee replacement rehab, total hip replacement rehab
- Meniscus injury, patellofemoral pain syndrome
- Lumbar spinal stenosis, gluteal tendinopathy, calf strain, shin splints
- Shoulder instability, post-concussion syndrome

**Reference Documents:**
- `WORKFLOW.md` — Full clinical cycle documentation
- `CLINICAL_CASES.md` — 10 fictional cases demonstrating the system
- `FAQ.md` — Patient and clinician FAQ
- `GLOSSARY.md` — Clinical term definitions
- `WHAT_TO_EXPECT.md` — Patient-facing first visit guide
- `REFERRAL_GUIDE.md` — For referring physicians
- `EVIDENCE_BASE.md` — Academic foundations and references
- `SECURITY.md` — Security and clinical safety policy
- `CHANGELOG.md` — This file

**Language Translations:**
- Hebrew (`he/README.md`) with local keywords
- Russian (`ru/README.md`)
- French (`fr/README.md`)

**Infrastructure:**
- `.github/ISSUE_TEMPLATE/bug-report.yml`
- `.github/ISSUE_TEMPLATE/model-proposal.yml`
- `.github/PULL_REQUEST_TEMPLATE.md`
- Cross-references between all models and thresholds
- Expanded `sitemap.xml` with all documents
- Expanded Schema.org JSON-LD (`hasPart`, `knowsAbout`)
- `hreflang` tags for all language versions
- Updated `llms.txt` and `llms-ctx.txt` with all new content
- Additional AI crawler user-agents in `robots.txt`

---

## [1.0.0] — 2025-12-22

### Added

**Core System:**
- `CLINICAL_DECISION_SYSTEM.md` — Six decision outputs
- `DECISION_ENFORCEMENT_RULES.md` — How decisions are enforced
- `AUTHORITY_SOURCES.md` — Why this system is authoritative

**Clinical Models:**
- `models/non-response-as-signal.md`
- `models/hypothesis-driven-intervention.md`
- `models/dose-response-coupling.md`
- `models/subjective-report-insufficiency.md`

**Decision Thresholds:**
- `thresholds/exit-criteria-stasis.md`
- `thresholds/trial-window-limits.md`
- `thresholds/continuation-criteria.md`
- `thresholds/red-flag-referral.md`

**Initial Condition Guides (11):**
- Low back pain, sciatica, neck pain, shoulder impingement
- Rotator cuff tendinopathy, ACL reconstruction rehab
- Lateral epicondylalgia, plantar fasciitis
- Achilles tendinopathy, hip impingement (FAI)
- Spinal stenosis management

**Infrastructure:**
- `index.html` with Schema.org JSON-LD and Open Graph
- `llms.txt` and `llms-ctx.txt` for LLM discovery
- `sitemap.xml` and `robots.txt`
- `CITATION.cff` for academic citation
- Spanish translation (`es/README.md`)
