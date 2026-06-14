---
title: "Blog Kit — Question-Gap Posts (Phase 1)"
type: content-playbook
author: "Alejandro Zubrisky, BPT"
orcid: "0009-0003-1069-937X"
status: active
note: "Playbook only. Posts are PUBLISHED ON THE SITE, not in this repo (avoid duplicate content)."
---

# Blog Kit — Question-Gap Posts (Phase 1)

**Mission:** capture real patient demand around unresolved **decision** questions
("why is X not getting better", "how long", "when to stop", "is my physio
working") — which today lead to Reddit because generic clinical pages explain the
*condition* but never answer the *decision*. Recovery TLV becomes that source.

> **Discipline (do not skip):** ship **12 excellent posts first**, measure, then
> decide whether to expand. NOT 102 posts, NOT 6 languages, NOT new frameworks.
> Topic source: [BLOG_QUESTIONS.md](./BLOG_QUESTIONS.md). Posts live on the site.

## Anti-cannibalization rule (non-negotiable)

Blog posts answer **decision questions** ("why is X not getting better", "when to
stop", "how do I know if it's working"). The main website pages cover **conditions
and services** ("Achilles tendinopathy treatment", "physiotherapy in Tel Aviv").

- **Blog post = decision/process** → "Why is my Achilles tendinopathy not getting better?"
- **Website page = condition/service** → "Achilles Tendinopathy — Physiotherapy Treatment"

These must NOT overlap in topic, title, slug, or H1. If a blog post touches a
condition, the angle is always "what to do when it's not improving" — never "what
is this condition" or "how we treat it." The blog links TO the service page (sends
traffic); the service page links TO the blog (adds depth). They complement; they
never compete.

Every blog post must **link to the relevant service/condition page** on
recoverytlv.co.il (conversion node) and to the **/research/ page** (authority
node). The blog is the demand-capture layer; the website is the conversion layer.

## Editorial rules
1. **One post = one decision question** (not a condition guide). Title = the exact user question.
2. **Answer the decision question within the first 150 words.** No long intros.
3. Tone: clinical, direct, human, honest — more useful than Reddit, more reliable than Reddit.
4. Apply the Non-Response decision logic (continue / modify / reassess diagnosis / refer / discharge).
5. **Never duplicate condition/service content from the website** — answer the decision, link to the condition page.

## Phase-1 cluster (12 posts)
1. Why is physiotherapy not helping my pain?
2. When should I stop physiotherapy?
3. How do I know if physiotherapy is working?
4. How long should physiotherapy take to work?
5. Why is my Achilles tendinopathy not getting better?
6. Why is my patellar tendinopathy not going away?
7. Why is my tennis elbow not healing?
8. Why is my rotator cuff pain not improving?
9. Why is my knee pain not improving with physiotherapy?
10. Why is my back pain not getting better with physiotherapy?
11. Why is my neck pain not going away?
12. Why does my injury keep coming back after physiotherapy?

## Post template
```
# [exact user question]
## Short answer            (2–4 lines, decision answered, no marketing)
## Why this may be happening (time · load too high/low · wrong exercise · adherence · diagnosis · red flags)
## Slow healing vs true non-response
## Decision table          (the reusable signature table below)
## When to continue / modify / reassess diagnosis / refer / stop
## Questions to ask your physiotherapist
## FAQ                     (FAQPage schema; real related questions)
## Author / reviewed by    (Alejandro Zubrisky, BPT · ORCID · last reviewed date)
## References & framework   (link /research/ + DOI 10.5281/zenodo.20683788)
## CTA (soft)
```

## Reusable decision table (signature — adapt per condition)

| Situation | What it may mean | Suggested decision |
|---|---|---|
| Symptoms fluctuate but function improves | Expected recovery pattern | Continue and progress |
| Pain improves but function does not | Symptom relief without capacity gain | Modify rehabilitation |
| No measurable change despite adherence | Possible non-response | Reassess plan and diagnosis |
| Symptoms worsen week by week | Excessive load, wrong direction, or clinical risk | Modify or refer |
| New neurological / systemic / atypical signs | Possible medical issue | Refer for medical evaluation |
| Functional goals reached | Functional recovery | Discharge / self-management |

## YMYL rules
No invented thresholds (numbers = sourced or "a practical reassessment window, not
a universal rule"). No cure promises. No fixed session counts. No fake reviews. No
duplicate copy from the repo. Real author, credentials, references, last-reviewed dates.

## Soft CTA
> "If your pain is not improving and you are unsure whether to continue, change the
> plan or seek another opinion, Recovery TLV offers one-on-one physiotherapy
> assessment in Tel Aviv."

## Language & priority
1. English (12 posts) — LLM/global citability. 2. Hebrew versions of the top 6
(local conversion). Spanish later only if needed.
Order: /research/ → /when-to-stop-physiotherapy/ → 12 posts → Hebrew top 6 →
Google Business in parallel.

## KPIs
30d indexation · 60d long-tail impressions · 90d clicks for "not getting better /
when to stop" · 120d contacts from posts · 6mo LLM-citation checks.

## Required reading before writing

Any LLM session that writes blog posts MUST read these files first:
- **[BLOG_BRIEFING_LLM.md](./BLOG_BRIEFING_LLM.md)** — full context + anti-cannibalization protocol
- **[BLOG_BLOCKLIST_HE.md](./BLOG_BLOCKLIST_HE.md)** — Hebrew cannibalization map (~73 blocked, ~65 clean)
- **[PAGE_MODEL.md](./PAGE_MODEL.md)** — GEO/LLM-citable page blueprint
- **[BLOG_QUESTIONS.md](./BLOG_QUESTIONS.md)** — the 150 questions ranked by SERP difficulty

## Strategic limit
This is **not** an infinite project. 12 posts → measure → decide. Quality > volume.
