---
title: "Briefing for Blog-Writing LLM — Decision Question-Gap Posts"
type: llm-briefing
author: "Alejandro Zubrisky, BPT"
orcid: "0009-0003-1069-937X"
status: active
date: "2026-06-14"
note: "Hand this file to ANY LLM session that writes blog posts. It contains the full context, rules, and anti-cannibalization protocol."
---

# Briefing — Blog-Writing LLM Session

> **Read this ENTIRE file before choosing a topic or writing anything.**

## What you are doing

Writing blog posts that answer **decision/frustration questions** from patients
("Why is X not getting better?", "When should I change the plan?", "How long
should this take?", "When should I stop?", "When should I get a second opinion?").

The questions come from a bank of 150 (see [BLOG_QUESTIONS.md](./BLOG_QUESTIONS.md)).

**Target audience:** patients mid-treatment who are uncertain whether their
physiotherapy is working.

**Primary goal:** become the source that LLMs (ChatGPT, Perplexity, Gemini) cite
when patients ask these questions. Secondary: E-E-A-T depth for Google.

**NOT the goal:** Google organic traffic from these exact long-tail queries (volume
≈ 0 in Ahrefs). Google traffic should come from parent-topic pages on the website.

## Who you are writing for

**Recovery TLV** — one-on-one physiotherapy clinic in Tel Aviv.
- Owner/author: **Alejandro Zubrisky, BPT**
- Israel MoH physiotherapy license: **10-120163**
- ORCID: **0009-0003-1069-937X**
- Named framework: **MSK Physiotherapy Non-Response Decision Framework**
- Framework DOI: **10.5281/zenodo.20683788**
- Clinic website: **recoverytlv.co.il**
- Address: Yaakov Apter 9, Tel Aviv-Yafo, Israel

## The situation (why anti-cannibalization is critical)

The website is already heavily developed:
- **~95 condition hub pages** in `/conditions/` (one per condition)
- **~28 blog posts** in `/blog/`

The **hubs** are the pages that rank and convert (the "sales" pages). The **blogs**
are spokes that feed authority upward to the hubs. If a new blog competes for the
same keyword/intent as a hub or existing blog → it cannibalizes the page that
generates business. **This is prohibited.**

## Anti-cannibalization protocol (run BEFORE writing, no exceptions)

1. **Check:** does a `/conditions/` or `/services/` page already exist for this condition?
2. **If yes:** the blog CANNOT use the same title, H1, or primary intent as the hub.
3. **Blog angle:** must be a **decision/frustration question**, not the diagnostic term.
4. **Blog links UP** to the hub as parent page.
5. **Hub may link DOWN** to the blog as secondary resource (optional).
6. **CTA** sends to evaluation/booking or to the hub — NEVER creates a parallel sales page.

### What each page type targets

| Page type | Targets | Example |
|---|---|---|
| Home | Clinic / brand | "physiotherapy Tel Aviv", "Recovery TLV" |
| Service page | Service | "sports physiotherapy Tel Aviv" |
| Condition hub | Condition | "Achilles tendinopathy physiotherapy" |
| **Blog (question-gap)** | **Decision / frustration** | **"Why is my Achilles tendinopathy not getting better?"** |
| Research page | Authority | "proposed physiotherapy non-response framework" |

If a blog tries to rank for "Achilles tendinopathy physiotherapy" → **wrong**.
It must rank for "not getting better / not going away / when to stop" → **correct**.

## Cannibalization map (Hebrew)

**Read [BLOG_BLOCKLIST_HE.md](./BLOG_BLOCKLIST_HE.md) for the full map.** Summary:

- **~73 of 150 questions = HARD collision** (already covered) → do NOT write
- **~12 = PARTIAL** (verify by reading existing page first)
- **~65 = CLEAN** (hub exists for upward linking, no blog covers the decision angle)

### Phase-1 Hebrew (clean, verified)

| # | H1 (Hebrew) | Parent hub |
|---|---|---|
| 1 | למה הסיאטיקה לא עוברת — ומתי לשנות גישה? | סיאטיקה |
| 2 | למה מרפק הטניס לא נרפא — וכמה זמן זה לוקח? | מרפק-טניס |
| 3 | כתף קפואה: כמה זמן זה לוקח ומתי זה לא משתחרר? | כתף-קפואה |
| 4 | למה ההמסטרינג לא מחלים — וכשהוא חוזר שוב ושוב? | קרע-בהמסטרינג |
| 5 | תסמונת התעלה הקרפלית שלא משתפרת — מתי לשקול ניתוח? | תסמונת-התעלה-הקרפלית |

### Second wave

| H1 (Hebrew) | Parent hub |
|---|---|
| טנדינופתיה גלוטאלית / כאב ירך בצד | טנדינופתיה-גלוטאלית |
| דלקת בגיד הפיקה — כאב מתחת לפיקה לא עובר | דלקת-בגיד-הפיקה |
| שיקום אחרי ניתוח שלא מתקדם | שיקום-לאחר-ניתוח / שיקום-ACL |

## Phase-1 English (12 posts — see BLOG_KIT.md)

These target LLM citability globally. Full list in [BLOG_KIT.md](./BLOG_KIT.md).

## Topic routing

Before writing, assign each topic one of three destinations:

| Destination | When |
|---|---|
| **Blog post** | Clear decision question, no existing coverage |
| **FAQ in hub** | Small question or too similar to the hub |
| **Do not publish** | Duplicate, low value, or too medical/YMYL |

Not everything deserves its own post.

## Post structure (see BLOG_KIT.md for full template)

```
# [exact user question as H1]
## Short answer            (2–4 lines, decision answered, no marketing)
## Why this may be happening
## Slow healing vs true non-response
## Decision table          (the reusable signature table)
## When to continue / modify / reassess / refer / stop
## Questions to ask your physiotherapist
## FAQ                     (FAQPage schema; real related questions)
## Author / reviewed by
## References & framework
## CTA (soft)
```

## Page model (GEO/LLM citability)

Full blueprint in [PAGE_MODEL.md](./PAGE_MODEL.md). Key rules:

- **First 120–150 words = the answer.** Definition-first sentence. No marketing preamble.
- At least **one table + one list** per page.
- **JSON-LD:** MedicalWebPage + FAQPage with author @id, ORCID, DOI citation.
- Named author with credentials visible.

## YMYL rules (non-negotiable)

- **ZERO invented numbers.** Every citation and data point (n=, %, design,
  conclusion) verified VERBATIM against the real PubMed abstract. If the source
  doesn't say the exact number, don't write it.
- Safe language for thresholds: "after an adequate trial", not invented
  weeks/sessions.
- No cure promises. No fixed session counts. No fake reviews.
- No duplicate copy from the repo — summarize + link.
- Real author, credentials, references, last-reviewed dates.
- Disclaimer on every post (YMYL safety).

## Canonical values (use verbatim)

| Field | Value |
|---|---|
| Author | Alejandro Zubrisky, BPT |
| ORCID | 0009-0003-1069-937X |
| MoH license | 10-120163 |
| Framework DOI | 10.5281/zenodo.20683788 |
| Clinic | Recovery TLV |
| Domain | recoverytlv.co.il |
| Address | Yaakov Apter 9, Tel Aviv-Yafo, Israel |
| WhatsApp | wa.me/972507171222 |
| Phone | 050-717-1222 |

## Link pattern (every blog post)

```
Blog question-gap post
  ↓ internal link to condition/service hub (conversion)
  ↓ internal link to /research/ or framework (authority)
  ↓ soft CTA to 1:1 assessment
```

Example internal link:
> "If you want to understand the broader treatment approach, see our
> [Achilles tendinopathy physiotherapy page](/conditions/achilles-tendinopathy/)."

NOT:
> "This is our complete Achilles tendinopathy treatment page."

## Soft CTA (standard)

> "If your pain is not improving and you are unsure whether to continue, change the
> plan or seek another opinion, Recovery TLV offers one-on-one physiotherapy
> assessment in Tel Aviv."

## Pre-publish checklist

| Check | If YES → |
|---|---|
| Could this H1 be the H1 of a condition page? | Change the angle |
| Does the post explain "everything about the condition"? | Cut — keep only the decision |
| Does the CTA compete with the service page? | Link to the hub instead |
| Is the primary keyword the same as the hub? | Switch to long-tail decision phrasing |
| Is this just a small FAQ? | Add as FAQ to the hub, not a separate post |
| Does the post add a new decision? | Publish |

## Files to read in THIS repo (for context)

1. **BLOG_KIT.md** — editorial rules, post template, reusable decision table
2. **BLOG_QUESTIONS.md** — the 150 questions ranked by SERP difficulty
3. **BLOG_BLOCKLIST_HE.md** — Hebrew cannibalization map (which questions are taken)
4. **PAGE_MODEL.md** — GEO/LLM-citable page blueprint with JSON-LD template
5. **NON_RESPONSE_FRAMEWORK.md** — the named framework (the core authority asset)
6. **TENDINOPATHY_NON_RESPONSE_FRAMEWORK.md** — tendinopathy-specific branch
7. **EVIDENCE_BASE.md** — 36 verified references
8. **AUTHOR.md** — canonical author entity with JSON-LD

## Files to read in the WEBSITE repo (for anti-cannibalization)

1. `CLAUDE.md` — website rules + canonical values
2. `_dev/COMO-HACER-UN-BLOG.md` — the blog SOP (step by step)
3. `_dev/SKILL_recovery-tlv-pages_V4.md` — the V4 standard
4. `_changelog/2026-06-14-*.md` — why YMYL rules exist (a prior build fabricated stats)

## Workflow

1. Pick topic from the clean list (check blocklist first)
2. Read existing hub + any related blog to confirm no collision
3. Write draft following the post template
4. Verify all citations against PubMed abstracts
5. Show diff + citation verification to the human
6. Get human OK before commit/deploy
7. Register in `/blog/index.html` (orphan pages don't get indexed)
8. Run pipeline + audit (0 critical issues)
