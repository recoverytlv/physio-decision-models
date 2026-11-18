# Changelog

All notable changes to the Recovery TLV Clinical Decision System are documented here.

Format based on [Keep a Changelog](https://keepachangelog.com/).

---

## [2.0.1] — 2026-11-18

Packaging fix. No decision logic, threshold or clinical text changed.

### Removed
- `SITE_INTEGRATION_BRIEF.md`. The 1.3.0 entry below lists it as removed, but the file was still shipped in
  1.3.0 and 2.0.0. It held instructions for the clinic website, not clinical content.

## [2.0.0] — 2026-11-18

Decision-logic change (major version, as SYSTEM_FREEZE_NOTICE.md requires). The six canonical outputs are unchanged.

**Why:** the 3–5 session window and the fixed ≥10% threshold were author-defined numbers that no study validates,
and a fixed percentage can be smaller than the measurement error of the instrument (goniometry on a small range).
The author's clinical rule, already applied at the clinic, is simpler and states the measurement problem directly.

**What changed:**
- Trial window: **4 sessions**. One measurable marker (pain on a validated scale, function, mobility or strength) is
  agreed at the first session; the first session counts. A change counts only if it exceeds the instrument's
  measurement error (MDC) and, where published, its MCID. The fixed ≥10% threshold is removed.
- No measurable change after 4 sessions: treatment stops and the case is re-evaluated → ONE revised trial, or
  DISCHARGE, or REFER (advice in person to see the treating or family doctor; emergency signs → emergency department; a written
  summary only if the physician asks). A second failed
  trial → DISCHARGE or REFER.
- A revised trial may test a different hypothesis, or the same hypothesis with a documented change of dose,
  technique or adherence plan.
- Post-operative cases are measured against the stage of the rehabilitation protocol (stalled stage → the surgeon);
  warning signs or worsening → immediate referral, without waiting for the window to end.
- Chronic pain and older adults follow the same 4-session rule (no extended windows); the agreed marker is usually
  functional.
- Session length stated: 50–60 minutes, one-to-one. Contact e-mail and Ministry of Health verification URL updated.

## [1.3.0] — 2026-11-17

Scope correction and evidence audit. The six canonical outputs and the numeric thresholds (3–5 session
trial window; ≥10% objective change) are unchanged. Normative texts were corrected where they contradicted
each other (see *Corrected*); in particular, the end-of-trial rule now matches WORKFLOW.md and REFERRAL_GUIDE.md.
This release also removes guides for conditions the clinic does not treat, so that readers and language
models are not told otherwise.

Numbering note: commit `485ec55` was labelled "v1.0.2" by mistake. Versions 1.1.0 and 1.2.0 were deposited
on Zenodo in June 2026, so this release is **1.3.0**. Release 1.0.1 (2026-06-13) was a maintenance release
applied after 1.1.0; its number does not follow semantic ordering. Some condition guides present by 1.0.1
were added without a changelog entry.

### Removed
- `conditions/fibromyalgia.md`, `conditions/pelvic-floor-dysfunction.md` and `conditions/scoliosis.md`
  (adolescent idiopathic / Schroth) — not treated at this clinic.
- `conditions/post-concussion.md` and the concussion case — concussion (including its vestibular component)
  is not treated at this clinic; post-traumatic neck pain is covered by the whiplash and neck pain guides.
- `CLINICAL_CASES.md` fibromyalgia and concussion cases; remaining 13 cases renumbered 1–13.
- `TELEHEALTH_GUIDELINES.md` (the clinic does not provide telehealth) and `SITE_INTEGRATION_BRIEF.md`.
- `SCOPING_REVIEW_PROTOCOL.md` and `ECOSYSTEM_MAP.md` (present in the 1.2.0 deposit) are not part of this release.

### Restored
- `NON_RESPONSE_FRAMEWORK.md` and `TENDINOPATHY_NON_RESPONSE_FRAMEWORK.md` (from the 1.2.0 deposit), corrected and
  mapped to the six canonical outputs.

### Changed
- `PREGNANCY_MUSCULOSKELETAL.md` rewritten as a scope-and-referral note: musculoskeletal care during pregnancy
  and pelvic floor rehabilitation are referred; postpartum musculoskeletal care is in scope.
- `index.html`: booking, WhatsApp and phone links; practitioner credentials (MoH license 10-120163, ORCID);
  address normalised to Yaakov Apter 9, Tel Aviv (all files); neuromotor re-education removed from service lists.
- ACL return-to-sport strength criterion: handheld dynamometry (no isokinetic testing at this clinic).
- Case 10: aquatic exercise is self-managed at a community pool (the clinic has no pool).
- Indexes updated: `README.md`, `llms.txt`, `llms-ctx.txt`, `llms-full.txt`, `sitemap.xml`, `index.html`
  JSON-LD, `codemeta.json`, `.zenodo.json` (42 → 38 condition guides).

### Corrected (evidence audit 2026-10-22)
- Trial window and 10% threshold described as author-defined review points, not evidence-based cut-offs; the
  ≥10% criterion applies to ROM or another objective measure and must exceed the instrument's MDC.
- End-of-trial rule unified across normative and supporting files: documented hypothesis revision + ONE new TRIAL,
  or DISCHARGE, or REFER; a second failed TRIAL → DISCHARGE or REFER. Off-by-one in the trial-window rule, the
  stasis count (3 vs 2) and workflow session numbering fixed; DEFER described as a temporary hold; undefined
  "80% confidence" and "3 extensions" removed; documented clinician judgement allowed.
- Red flags: wording aligned with Henschke 2009 and Downie 2013; myelopathy → REFER; weight-loss criterion unified;
  imaging actions rewritten as referral to a physician.
- Outcome measures: published values corrected and sourced; unsourced goniometry MCID table removed; LSI ≥90% and
  Y-Balance 4 cm labelled as criteria/cut-offs; unverified thresholds labelled as guides.
- Attributions corrected (MCID origin, Croskerry, dose-response decoupling, Cook et al. 2018, fear of re-injury);
  bibliographic titles and pages corrected; "[verified]" defined as a bibliographic check against PubMed.
- Scope and metadata: neuromotor re-education removed from the in-scope list; telehealth references removed;
  "multi-LLM consensus validation" removed; guideline-prevails statement added; tendinopathy framework states that
  shockwave, injections and percutaneous electrolysis are outside the framework (shockwave and injections are not
  provided at this clinic); versions, dates and
  metadata aligned (README.md, CITATION.cff, codemeta.json, .zenodo.json).

---

## [1.2.0] — 2026-06-14

Entry reconstructed in 1.3.0 (it was missing). Files present in the 1.2.0 deposit and not recorded
elsewhere in this changelog:
- `NON_RESPONSE_FRAMEWORK.md` — the MSK Physiotherapy Non-Response Decision Framework (proposed).
- `TENDINOPATHY_NON_RESPONSE_FRAMEWORK.md` — tendinopathy branch of that framework.
- `SCOPING_REVIEW_PROTOCOL.md` and `ECOSYSTEM_MAP.md`.

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

## [1.1.0] — 2025-12-23 (deposited on Zenodo in June 2026)

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
