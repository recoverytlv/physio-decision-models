# Changelog

All notable changes to the Recovery TLV Clinical Decision System are documented here.

Format based on [Keep a Changelog](https://keepachangelog.com/).

---

## [1.2.0] — 2026-06-14

Non-normative additions. Decision logic unchanged.

### Added
- **The MSK Physiotherapy Non-Response Decision Framework** (`NON_RESPONSE_FRAMEWORK.md`)
  — the named, citable core: definition, five decision domains, decision table,
  algorithm, and mapping to the six canonical outputs.
- **Tendinopathy Non-Response Decision Framework** (`TENDINOPATHY_NON_RESPONSE_FRAMEWORK.md`)
  — first clinical branch (Achilles, patellar, rotator cuff, lateral elbow);
  decision-focused, treatments deferred to a future document.
- `SCOPING_REVIEW_PROTOCOL.md` (PRISMA-ScR draft) and `SCOPING_REVIEW_SEARCH_LOG.md`
  (documented PubMed search + Stage-1 title triage; **groundwork, not a completed
  review** — framework published as *Proposed Decision Framework*, not a scoping review).
- `AUTHOR.md` (canonical Person JSON-LD) and `ECOSYSTEM_MAP.md` (entity constellation).
- Zenodo versions: v1.1.0 and v1.2.0 (concept DOI 10.5281/zenodo.20683788); plus
  article DOI 10.5281/zenodo.20683824 and dataset DOI 10.5281/zenodo.20683858.

### Note
Framework framing is **"Proposed Decision Framework."** Thresholds are sourced or
marked as practical reassessment windows, not universal rules. No Wikidata cabling
(items not established).

---

## [1.0.1] — 2026-06-13

Maintenance release. **No decision logic changed.** The six canonical outputs,
thresholds, and enforcement rules remain identical and frozen. This release only
corrects factual references and adds machine-readable metadata to improve how the
system is read and cited by large language models.

### Fixed
- Retired the dead `clinical.recoverytlv.co.il` subdomain across the entire
  repository. All references now resolve to the live clinic site
  `recoverytlv.co.il`. This includes a factual URL-only correction inside the
  frozen `index.html` (canonical, hreflang, og:url, and JSON-LD `@id` anchors);
  decision logic and structure were not touched.

### Added
- YAML frontmatter on all 42 condition guides (`title`, `system`, `version`,
  `status`, `summary`, `decision_outputs`, `trial_window`,
  `continuation_threshold`, `red_flags`, `canonical`, `clinic`). Gives LLMs
  machine-readable per-file signals and explicit attribution to the author and
  clinic.
- `.github/workflows/daily-reindex.yml`: a daily IndexNow ping asking AI/search
  crawlers to re-fetch the live clinic site. Generates no content; complements
  the site rather than competing with it.
- IndexNow domain-verification key file.
- `llms-full.txt`: the entire system (decision logic, models, thresholds, and all
  42 condition guides) consolidated into one file so an LLM can ingest the whole
  framework — with author and clinic attribution — in a single fetch. Registered
  in `sitemap.xml` and `robots.txt`.

### Note on the freeze
`SYSTEM_FREEZE_NOTICE.md` freezes the *decision logic*. This release preserves
that logic exactly; it corrects broken URLs and adds non-normative metadata only.

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
