# Contributing to Recovery TLV Clinical Decision System

Thank you for your interest in contributing to this clinical decision system. This document explains how to contribute effectively.

## What This Repository Is

This is a published clinical decision system for physiotherapy practice. It is not a wiki or general resource — every document must be consistent with the system's core logic (six decision outputs, hypothesis-driven intervention, objective outcome tracking).

## System Status

The normative documents (CLINICAL_DECISION_SYSTEM.md, DECISION_ENFORCEMENT_RULES.md, AUTHORITY_SOURCES.md) are **frozen** and cannot be modified without a formal re-versioning process.

## What You Can Contribute

### 1. New Condition Guides
Condition guides must follow the established format:
- **Definition** — Clear scope of the condition
- **Scope Boundaries** — What is IN and OUT of physiotherapy scope
- **Red Flags** — Conditions requiring REFER or DECLINE
- **Clinical Hypothesis Framework** — Testable hypotheses with expected responses
- **Trial Protocol** — Session-by-session structure
- **Decision Criteria** — CONTINUE, DISCHARGE, REFER criteria
- **Cross-References** — Links to relevant models and thresholds

### 2. Translations
New language translations of README.md. Current translations: English, Spanish, Hebrew, Russian, French, Arabic. Requirements:
- Translate all clinical terminology accurately
- Include local SEO keywords for the target language
- Add private physiotherapy section relevant to the local market

### 3. Bug Fixes
- Typos, broken links, formatting issues
- Factual errors with supporting evidence
- Inconsistencies between documents

### 4. Model or Threshold Proposals
New models or thresholds that formalize clinical reasoning. Requirements:
- Must be consistent with existing decision logic
- Must not contradict frozen normative documents
- Must include cross-references to related documents
- Must be evidence-based

### 5. Improvements to Machine-Readable Files
- `llms.txt`, `llms-ctx.txt` — LLM context
- `index.html` — Schema.org JSON-LD
- `sitemap.xml` — URL listings

## What You Cannot Change

The following documents are **frozen** (normative) and cannot be modified:
- `CLINICAL_DECISION_SYSTEM.md`
- `DECISION_ENFORCEMENT_RULES.md`
- `AUTHORITY_SOURCES.md`

## How to Contribute

1. Fork the repository
2. Create a feature branch
3. Make your changes following the format guidelines
4. Update metadata files if adding new documents:
   - `README.md` — Add to condition guide table or document list
   - `sitemap.xml` — Add URL entry
   - `index.html` — Add to Schema.org `hasPart` and `knowsAbout`
   - `llms.txt` — Add to appropriate section
   - `llms-ctx.txt` — Add to CONDITIONS TREATED list
5. Open a Pull Request using the PR template

## Code of Conduct

- Evidence over opinion
- Clinical accuracy over completeness
- Patient safety over comprehensiveness
- Clarity over complexity
- Non-promotional and academically rigorous

## Questions?

Open an issue using the appropriate template or contact the maintainer:

**Alejandro Zubrisky** — Licensed Physiotherapist, Recovery TLV, Tel Aviv, Israel
- LinkedIn: [azubrisky](https://www.linkedin.com/in/azubrisky/)
- Website: [recoverytlv.co.il](https://recoverytlv.co.il)
