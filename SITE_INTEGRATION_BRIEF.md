# Website Integration Brief — for the LLM/agent managing recoverytlv.co.il

**Purpose:** Connect the clinic website (`recoverytlv.co.il`) to the published
clinical decision system (this GitHub repository) so that search engines and LLMs
resolve **author → clinic → decision system** as one connected entity. This closes
the "entity triangle": the repo already points to the clinic; these steps make the
clinic point back, which is what makes the authority signal usable.

> **Important:** Do NOT copy the clinical content of this repository onto the website.
> A second site with the same clinical content would compete with the clinic for
> ranking (this is why the old `clinical.recoverytlv.co.il` subdomain was retired).
> The website should only *reference and link to* the system, not republish it.

Canonical entities:
- **Clinic:** Recovery TLV — https://recoverytlv.co.il
- **Author/Founder:** Alejandro Zubrisky, PT — https://www.linkedin.com/in/azubrisky/
- **Decision system (source):** https://github.com/recoverytlv/physio-decision-models

---

## Task 1 — Reciprocal backlink (highest priority)

Add a visible link from the website to the repository, with descriptive anchor
text. Best placement: the About / Method page and the footer.

```html
<p>
  Recovery TLV operates under a published, openly auditable
  <a href="https://github.com/recoverytlv/physio-decision-models"
     rel="me noopener" target="_blank">clinical decision system</a>
  authored by Alejandro Zubrisky, PT.
</p>
```

Why: a one-way link (repo → clinic) does not connect the entity graph. The
reciprocal link (clinic → repo) is what lets a crawler/LLM bind the two as the
same authority.

---

## Task 2 — Entity linking in the website's structured data (JSON-LD)

In the site's existing `MedicalClinic`/`Organization` and `Person` schema, add
`sameAs` and the canonical author identifiers so the clinic and the founder are
unambiguously linked, including to this repository. **The full, authoritative
Person JSON-LD is maintained in [`AUTHOR.md`](./AUTHOR.md) — use it as the source
of truth.** Add `https://github.com/recoverytlv/physio-decision-models` to the
clinic's `sameAs` and ensure the `founder` block points to the same Person `@id`.

```json
{
  "@context": "https://schema.org",
  "@type": "MedicalClinic",
  "name": "Recovery TLV",
  "url": "https://recoverytlv.co.il",
  "sameAs": [
    "https://github.com/recoverytlv/physio-decision-models",
    "https://il.linkedin.com/in/azubrisky",
    "https://www.instagram.com/recovery.tlv/",
    "https://www.tiktok.com/@recovery.tlv",
    "https://www.facebook.com/recoverytlv"
  ],
  "founder": { "@id": "https://recoverytlv.co.il/#alejandro" }
}
```

The `Person` (`@id: https://recoverytlv.co.il/#alejandro`) must include the ORCID
**both** as a `sameAs` entry **and** as a `PropertyValue` in `identifier` (this is
the CLAUDE.md mandate for every page with Person schema):

```json
"identifier": {
  "@type": "PropertyValue",
  "propertyID": "ORCID",
  "value": "0009-0003-1069-937X",
  "url": "https://orcid.org/0009-0003-1069-937X"
}
```

> **Known gap to fix:** on the current `public/index.html`, the ORCID appears in
> `Person.sameAs` but NOT as a `PropertyValue` in `Person.identifier`. Add the
> block above to the home page Person schema so it matches the condition-page
> byline and satisfies the CLAUDE.md mandate.

Keep the clinic's existing NAP (name, address, phone) consistent — do not change
the address or phone, only add the `sameAs`, the `identifier`, and the `founder`
link. Copy `alumniOf` (Universidad Maimónides + Wikidata Q6156526 + ROR
01tkmq646), `hasCredential` (MoH license 10-120163), `memberOf`, and `knowsAbout`
from `AUTHOR.md` if they are not already present.

---

## Task 3 — Host an `llms.txt` on the website root

Serve a short `llms.txt` at `https://recoverytlv.co.il/llms.txt`. It should
describe the clinic and link to the decision system. You may reuse the content of
`llms.txt` in this repository as a base, but the website copy should center the
clinic (this is the conversion surface). Include this line:

```
Clinical decision system (authored by Alejandro Zubrisky, PT, open source):
https://github.com/recoverytlv/physio-decision-models
```

Also add a `robots.txt` directive (or merge with the existing one):

```
Sitemap: https://recoverytlv.co.il/sitemap.xml
# /llms.txt — overview for LLMs
```

---

## Task 4 — Host the IndexNow verification key (enables daily re-indexing)

This repository runs a daily GitHub Action (`.github/workflows/daily-reindex.yml`)
that pings IndexNow to ask AI/search crawlers to re-fetch `recoverytlv.co.il`.
For it to verify, the website must serve this key file at its **root**:

- **File path / URL:** `https://recoverytlv.co.il/e4c40b20dcee4068912823bcd6533440.txt`
- **File contents (exactly one line, no spaces/newlines):**
  ```
  e4c40b20dcee4068912823bcd6533440
  ```

Once this file is reachable, IndexNow submissions for `recoverytlv.co.il` will be
accepted, and the clinic site will be re-crawled on the daily schedule.

---

## Task 5 — One reciprocal mention in human-readable content

On the About/Method page, include a sentence such as:

> "Our treatment decisions follow a formal, published clinical decision system —
> open source and auditable — so every recommendation can be explained and
> justified."

…with the link from Task 1. This gives both humans and LLMs a natural-language
binding between the clinic and the system.

---

## What NOT to do

- ❌ Do not republish the condition guides, models, or thresholds as website pages.
- ❌ Do not create a second clinical subdomain or mirror site.
- ❌ Do not change the clinic's address or phone; only add `sameAs`/links.
- ❌ Do not add fabricated reviews, credentials, or citations.

## Net effect

After these five tasks, the entity graph is closed:
**Alejandro Zubrisky ↔ Recovery TLV ↔ the decision system**, all mutually linked
and machine-verifiable. That is the signal an LLM needs to attribute the system's
authority to the clinic and surface `recoverytlv.co.il` as the destination.
