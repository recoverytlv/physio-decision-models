# Ecosystem Map — Recovery TLV Entity Constellation

The goal: every property in the "universe" of Alejandro Zubrisky / Recovery TLV
links to the others and uses identical identity (name, NAP, ORCID), so search
engines and LLMs resolve them as **one trusted entity** and surface the clinic.

> **Golden rule:** every node must (1) use the same Name + Address + Phone (NAP),
> (2) link to at least the **website** and **GitHub**, and (3) carry the **ORCID**
> where the platform allows. Convergence = entity consensus = citation.

## One entity, two facets (bind them everywhere)

Recovery TLV (the clinic/brand) and Alejandro Zubrisky (the person/author) are
**one entity in two facets**, joined by the **framework** he authored and the
clinic applies. Every node should express both, using this canonical binding
statement (verbatim, adapted to length):

> **EN:** Recovery TLV is the Tel Aviv musculoskeletal physiotherapy clinic of
> Alejandro Zubrisky, BPT — physiotherapist and author of the *MSK Physiotherapy
> Non-Response Decision Framework*. The clinic applies the framework it publishes:
> objective, auditable decisions on when to continue, modify, refer, or stop
> treatment.

> **ES:** Recovery TLV es la clínica de fisioterapia musculoesquelética en Tel
> Aviv de Alejandro Zubrisky, BPT — fisioterapeuta y autor del *Marco de decisión
> ante no-respuesta en fisioterapia musculoesquelética*. La clínica aplica el
> marco que publica: decisiones objetivas y auditables sobre cuándo continuar,
> modificar, derivar o detener el tratamiento.

Binding mechanics in schema: `Person.worksFor` = clinic; `MedicalClinic.founder`
= person `@id`; both carry mutual `sameAs`; the framework is the shared asset both
reference (repo + DOI).

## The constellation

```
                         ┌─────────────────────────┐
                         │   GOOGLE BUSINESS /      │  ← #1 for "recommend a clinic"
                         │   GOOGLE MAPS  (local)   │
                         └────────────┬────────────┘
                                      │
        AUTHORITY                     │                    REACH
   ┌───────────────┐        ┌─────────▼──────────┐    ┌───────────────┐
   │ GitHub repo   │◄──────►│  WEBSITE           │◄──►│ LinkedIn /    │
   │ (credential)  │        │  recoverytlv.co.il │    │ IG / TikTok / │
   │ Zenodo DOIs   │◄──────►│  (CONVERSION HUB)  │◄──►│ Facebook      │
   │ ORCID         │        └─────────┬──────────┘    └───────────────┘
   │ Software Her. │                  │
   └───────────────┘        ┌─────────▼──────────┐
                            │ DIRECTORIES +       │
                            │ MoH registry        │
                            │ (local citations)   │
                            └─────────────────────┘
```

## Node-by-node

| Node | Canonical URL | Role | Status | Action |
|---|---|---|---|---|
| **Website** | https://recoverytlv.co.il | Conversion hub | live | Apply `SITE_INTEGRATION_BRIEF.md` (links, schema, llms.txt, GEO) |
| **Author page** | https://recoverytlv.co.il/about/alejandro-zubrisky/ | Person entity | live | ORCID as `identifier` + `sameAs` to all nodes |
| **GitHub repo** | https://github.com/recoverytlv/physio-decision-models | Authority/credential | optimized ✅ | Set repo topics + description + website link |
| **GitHub org** | https://github.com/recoverytlv | Brand profile | live | Org README linking clinic |
| **Google Business / Maps** | (claim/verify) | Local recommendation | **TODO** ⭐ | Verify, complete, collect reviews, link website |
| **Zenodo — system** | https://doi.org/10.5281/zenodo.20683788 | Academic DOI | published ✅ | — |
| **Zenodo — article** | https://doi.org/10.5281/zenodo.20683824 | Academic DOI #2 | published ✅ | — |
| **Zenodo — dataset** | https://doi.org/10.5281/zenodo.20683858 | Academic DOI #3 | published ✅ | — |
| **ORCID** | https://orcid.org/0009-0003-1069-937X | Author hub | rich; `works:0` | Add the 2 DOIs (auto via DataCite) |
| **Software Heritage** | archived ✅ | Code archive | done ✅ | — |
| **MoH registry** | https://practitioners.health.gov.il/Practitioners/10 | Official credential | live | Reference as `sameAs` everywhere |
| **LinkedIn** | https://il.linkedin.com/in/azubrisky | Reach | live | Bio links to website + repo |
| **Instagram** | https://www.instagram.com/recovery.tlv/ | Reach | live | Link in bio → website |
| **TikTok** | https://www.tiktok.com/@recovery.tlv | Reach | live | Link in bio → website |
| **Facebook** | https://www.facebook.com/recoverytlv | Reach | live | About → website |
| **Wikidata** | Q140078695 / Q140078796 | Knowledge graph | empty | After DOIs: populate carefully (P356 DOI, P496 ORCID) |
| **Maimónides** | Wikidata Q6156526 · ROR 01tkmq646 | Education anchor | — | Cite in `alumniOf` |

## Identity constants (use these EXACTLY everywhere)

```
Name:      Recovery TLV
Person:    Alejandro Zubrisky, BPT
Address:   Yaakov Apter 9, Tel Aviv, Israel, 6936209
Phone:     +972-50-717-1222
Email:     tlvphysio@gmail.com
Website:   https://recoverytlv.co.il
ORCID:     0009-0003-1069-937X
MoH lic.:  10-120163
Geo:       32.1051161, 34.7900481
```

## Priority order (highest real return first)

1. **Google Business Profile** — verify + reviews (the local recommendation engine)
2. **Bing Webmaster Tools** for the website (ChatGPT's index)
3. **Website** — apply `SITE_INTEGRATION_BRIEF.md` (links back + schema + GEO)
4. **ORCID** — add the 2 DOIs
5. **Social bios + directories** — consistent NAP + website link
6. **Wikidata** — only after the DOIs have propagated
