---
title: "Citable Page Model — How to build a page LLMs & Google cite (GEO)"
type: page-blueprint
author: "Alejandro Zubrisky, BPT"
orcid: "0009-0003-1069-937X"
status: active
---

# Citable Page Model (LLM / Google / GEO)

How to build each question-gap page so AI engines and Google **extract and cite
it**. Every rule below maps to a measured GEO citation factor.

## 1. URL & title
- **Slug** = the question, kebab-case: `/why-is-my-achilles-tendinopathy-not-getting-better/`
- **H1** = the exact user question (verbatim — matches the query).
- **`<title>`** = question + brand: "Why is my Achilles tendinopathy not getting better? | Recovery TLV"
- **Meta description** = the 1-sentence direct answer (not marketing).

## 2. The extractable answer (most important)
- **First 120–150 words = the answer**, opening with a **definition-style sentence**
  ("X is …" / "You should … when …"). LLMs lift this as the canonical answer.
- Plain language, direct, honest. No long intro, no marketing preamble.

## 3. Structure (machine-readable)
- One **unique H1**; logical **H2 → H3** hierarchy (each H2 = a sub-question).
- At least **one table** and **one list** per page (cited pages overwhelmingly have these).
- A **TL;DR / "Short answer"** block near the top.
- A **decision table** (the reusable signature) — tables are highly extractable.
- An **FAQ** block of real related questions.

## 4. E-E-A-T (trust signals — visible + in schema)
- **Named author** with bio: *Alejandro Zubrisky, BPT*.
- **Credentials visible**: ORCID `0009-0003-1069-937X`, Israel MoH license `10-120163`.
- **Published date + "Last reviewed" date** (freshness).
- **Inline references** to real sources + link to the open framework (DOI).
- **Disclaimer** (YMYL safety).

## 5. Structured data (JSON-LD) — paste & adapt per page

```json
{
  "@context": "https://schema.org",
  "@type": ["MedicalWebPage", "FAQPage"],
  "url": "https://recoverytlv.co.il/why-is-my-achilles-tendinopathy-not-getting-better/",
  "name": "Why is my Achilles tendinopathy not getting better?",
  "headline": "Why is my Achilles tendinopathy not getting better?",
  "datePublished": "2026-06-14",
  "dateModified": "2026-06-14",
  "inLanguage": "en",
  "about": { "@type": "MedicalCondition", "name": "Achilles tendinopathy" },
  "author": {
    "@type": "Person",
    "@id": "https://recoverytlv.co.il/#alejandro",
    "name": "Alejandro Zubrisky",
    "honorificSuffix": "BPT",
    "identifier": {
      "@type": "PropertyValue", "propertyID": "ORCID",
      "value": "0009-0003-1069-937X", "url": "https://orcid.org/0009-0003-1069-937X"
    }
  },
  "reviewedBy": { "@id": "https://recoverytlv.co.il/#alejandro" },
  "publisher": { "@type": "MedicalClinic", "name": "Recovery TLV", "url": "https://recoverytlv.co.il" },
  "isPartOf": { "@type": "WebSite", "url": "https://recoverytlv.co.il" },
  "citation": {
    "@type": "CreativeWork",
    "name": "MSK Physiotherapy Non-Response Decision Framework",
    "identifier": "https://doi.org/10.5281/zenodo.20683788"
  },
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Why is my Achilles tendinopathy not getting better?",
      "acceptedAnswer": { "@type": "Answer", "text": "<the 120–150 word direct answer>" }
    },
    {
      "@type": "Question",
      "name": "How long does Achilles tendinopathy take to heal?",
      "acceptedAnswer": { "@type": "Answer", "text": "<real, sourced or marked-as-window answer>" }
    }
  ]
}
```

## 6. Internal links
- Link to **/research/** (author + framework + DOI).
- Link to the relevant **condition/service page** (conversion).
- Cross-link sibling question-gap posts (topic cluster).

## 7. Honesty / YMYL (non-negotiable)
- No invented thresholds — numbers sourced or "a practical reassessment window, not
  a universal rule".
- No cure promises, no fixed session counts, no fake reviews.
- Do not duplicate the repo's clinical guides verbatim — summarise + link.

## 8. Soft CTA (end)
> "If your pain is not improving and you are unsure whether to continue, change the
> plan or seek another opinion, Recovery TLV offers one-on-one physiotherapy
> assessment in Tel Aviv."

## 9. Technical / discoverability
- Add to **sitemap.xml**; submit to **Google Search Console** + **Bing Webmaster**
  (Bing = ChatGPT's index) + **IndexNow** ping.
- Fast, mobile-friendly, crawlable (no JS-only content for the answer).
- Keep the page updated (bump `dateModified` on real edits).

## Why this gets cited
LLMs/Google cite a page when it (1) answers a real question, (2) does so clearly
and first (definition-first), (3) is structured for extraction (tables/lists/FAQ),
(4) is credible (named author + credentials + dates + references), and (5) is
discoverable (indexed). This model satisfies all five.
