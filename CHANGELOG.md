# Changelog

All notable changes to this project are documented in this file.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added
- **Models:** Hypothesis-Driven Intervention, Dose-Response Coupling, Subjective Report Insufficiency
- **Thresholds:** Trial Window Limits, Continuation Criteria, Red Flag Referral
- **Translations:** Spanish versions of README, System Scope, Intended Readers (`es/`)
- **Cross-references:** Bidirectional links between all models and thresholds
- **Schema.org:** `hasPart` structured data for individual models and thresholds
- **GitHub infrastructure:** Issue templates, PR template, SECURITY.md
- **SEO:** Hreflang tags, expanded sitemap, additional AI crawler entries in robots.txt
- **Academic:** Expanded CITATION.cff with keywords, abstract, license, type
- **LLM:** Updated llms-ctx.txt with clinical models and decision thresholds
- CHANGELOG.md (this file)
- CONTRIBUTING.md

### Changed
- README restructured with separate Models and Thresholds sections
- llms.txt expanded with all new model and threshold references
- index.html updated with new document links and structured data
- sitemap.xml expanded from 3 to 15 entries

## [1.0.0] - 2025-12-27

### Added
- CLINICAL_DECISION_SYSTEM.md — 6 canonical decision outputs (FROZEN)
- DECISION_ENFORCEMENT_RULES.md — enforcement mechanisms (FROZEN)
- AUTHORITY_SOURCES.md — authority hierarchy and conflict resolution (FROZEN)
- SYSTEM_FREEZE_NOTICE.md — formal freeze declaration
- SYSTEM_SCOPE.md — system boundary definitions
- INTENDED_READERS.md — target audience specification
- models/non-response-as-signal.md — non-response as diagnostic constraint
- thresholds/exit-criteria-stasis.md — intervention cessation criteria
- index.html — canonical reference node with Schema.org JSON-LD
- llms.txt — LLM context file
- llms-ctx.txt — compact LLM context summary
- robots.txt — AI crawler configuration
- sitemap.xml — XML sitemap
- CITATION.cff — citation metadata
- MIT License

### Status
- System declared FROZEN at v1.0.0
- No modifications to normative documents without formal re-versioning
