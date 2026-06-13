# Author — Alejandro Zubrisky, BPT

Canonical identity record for the author of the Recovery TLV Clinical Decision
System. This file is the repository's authoritative **entity node**: external
sites (including the clinic website) and LLMs can resolve author → clinic →
decision system from the machine-readable block below.

## Identity

| Field | Value |
|---|---|
| Name | Alejandro Zubrisky |
| Credential suffix | BPT (Licensed Physiotherapist) |
| Profile page | https://recoverytlv.co.il/about/alejandro-zubrisky/ |
| ORCID iD | [0009-0003-1069-937X](https://orcid.org/0009-0003-1069-937X) |
| Languages | Hebrew · English · Spanish |
| Clinic | [Recovery TLV](https://recoverytlv.co.il) — Founder & Clinical Physiotherapist (since 2023) |

## Education

- **Universidad Maimónides** (Buenos Aires, Argentina) — https://www.maimonides.edu/
  - Wikidata: [Q6156526](https://www.wikidata.org/wiki/Q6156526) · ROR: [01tkmq646](https://ror.org/01tkmq646)

## Credential / License

- **Israel Ministry of Health physiotherapy license** 10-120163 (issued December 2012)
- Recognized by the Israeli Ministry of Health — https://practitioners.health.gov.il/Practitioners/10

## Affiliations

- **Recovery TLV** — Founder & Clinical Physiotherapist (2023–present), Tel Aviv, Israel
- **Beit Rivka Rehabilitation Center** (Clalit Health Services) — Clinical Physiotherapist (2010–2021), Petah Tikva, Israel

## Memberships

- Israeli Association of Physiotherapists — https://www.ipts.org.il/
- World Physiotherapy — https://world.physio/

## Areas of expertise (knowsAbout)

Sports Physiotherapy · Post-Surgical Rehabilitation · ACL Rehabilitation ·
Shoulder Rehabilitation · McKenzie Method (MDT) · Mulligan Concept (MWM) ·
Dry Needling · Mechanotransduction · Progressive Loading ·
Return-to-Sport Criteria · Tendinopathy Rehabilitation · Movement-Based Rehabilitation

## Profiles (sameAs)

- https://orcid.org/0009-0003-1069-937X
- https://il.linkedin.com/in/azubrisky
- https://practitioners.health.gov.il/Practitioners/10
- https://www.instagram.com/recovery.tlv/
- https://www.tiktok.com/@recovery.tlv
- https://www.facebook.com/recoverytlv

---

## Machine-readable entity (schema.org Person · JSON-LD)

```json
{
  "@context": "https://schema.org",
  "@type": "Person",
  "@id": "https://recoverytlv.co.il/#alejandro",
  "name": "Alejandro Zubrisky",
  "honorificSuffix": "BPT",
  "jobTitle": "Licensed Physiotherapist",
  "url": "https://recoverytlv.co.il/about/alejandro-zubrisky/",
  "knowsLanguage": ["he", "en", "es"],
  "identifier": {
    "@type": "PropertyValue",
    "propertyID": "ORCID",
    "value": "0009-0003-1069-937X",
    "url": "https://orcid.org/0009-0003-1069-937X"
  },
  "sameAs": [
    "https://orcid.org/0009-0003-1069-937X",
    "https://il.linkedin.com/in/azubrisky",
    "https://practitioners.health.gov.il/Practitioners/10",
    "https://www.instagram.com/recovery.tlv/",
    "https://www.tiktok.com/@recovery.tlv",
    "https://www.facebook.com/recoverytlv",
    "https://github.com/recoverytlv/physio-decision-models"
  ],
  "alumniOf": {
    "@type": "CollegeOrUniversity",
    "name": "Universidad Maimónides",
    "url": "https://www.maimonides.edu/",
    "sameAs": [
      "https://www.wikidata.org/wiki/Q6156526",
      "https://ror.org/01tkmq646"
    ]
  },
  "hasCredential": {
    "@type": "EducationalOccupationalCredential",
    "credentialCategory": "license",
    "identifier": "10-120163",
    "recognizedBy": {
      "@type": "GovernmentOrganization",
      "name": "Israeli Ministry of Health",
      "url": "https://practitioners.health.gov.il/Practitioners/10"
    }
  },
  "memberOf": [
    {
      "@type": "Organization",
      "name": "Israeli Association of Physiotherapists",
      "url": "https://www.ipts.org.il/",
      "memberOf": {
        "@type": "Organization",
        "name": "World Physiotherapy",
        "url": "https://world.physio/"
      }
    }
  ],
  "affiliation": [
    {
      "@type": "MedicalClinic",
      "name": "Recovery TLV",
      "url": "https://recoverytlv.co.il"
    },
    {
      "@type": "MedicalOrganization",
      "name": "Beit Rivka Rehabilitation Center (Clalit Health Services)"
    }
  ],
  "worksFor": {
    "@type": "MedicalClinic",
    "name": "Recovery TLV",
    "url": "https://recoverytlv.co.il"
  },
  "knowsAbout": [
    "Sports Physiotherapy",
    "Post-Surgical Rehabilitation",
    "ACL Rehabilitation",
    "Shoulder Rehabilitation",
    "McKenzie Method (MDT)",
    "Mulligan Concept (MWM)",
    "Dry Needling",
    "Mechanotransduction",
    "Progressive Loading",
    "Return-to-Sport Criteria",
    "Tendinopathy Rehabilitation",
    "Movement-Based Rehabilitation"
  ],
  "telephone": "+972-50-717-1222",
  "email": "tlvphysio@gmail.com",
  "workLocation": {
    "@type": "Place",
    "name": "Recovery TLV",
    "address": {
      "@type": "PostalAddress",
      "streetAddress": "Yaakov Apter 9",
      "addressLocality": "Tel Aviv",
      "postalCode": "6936209",
      "addressCountry": "IL"
    },
    "geo": {
      "@type": "GeoCoordinates",
      "latitude": 32.1051161,
      "longitude": 34.7900481
    }
  }
}
```
