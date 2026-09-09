---
title: "10.2 Schools"
council: Canterbury-Bankstown
document_type: DCP
chapter: "10.2"
last_verified: 2026-09-03
---

# 10.2 – Schools

Canterbury-Bankstown DCP 2023, Chapter 10 (Other Development), sub-chapter 10.2. Source
PDF cover date: June 2023 (Amended April 2025).

Sets out development controls for schools (government and non-government), covering site
analysis requirements, location and traffic management, site layout and building envelopes
(including site width, classroom density, setbacks, deep soil zones and free play areas),
energy efficiency and urban design, acoustic privacy, landscape, safety and security, and
site facilities.

## Scope

No "Application of this chapter" clause is present, and no wording anywhere in the source
splits this sub-chapter by former LGA. Controls apply council-wide, with internal variation
by **zone** only (e.g. Zone R2/R3/R4 site-width and setback rules vs Zone E1/MU1 rules
determined case-by-case by Council; the Neighbourhood Liaison Committee requirement in
6.5 is mandatory only in Zone R2). Consistent with the pattern established by 10.1, 10.3 and
10.4, this sub-document sits under `general/`.

## Sections

| Section | File | Status |
|---|---|---|
| 1 — Introduction | [`01-introduction.md`](01-introduction.md) | Converted |
| 2 — Site analysis | [`02-site-analysis.md`](02-site-analysis.md) | Converted |
| 3 — Location and traffic management | [`03-location-and-traffic-management.md`](03-location-and-traffic-management.md) | Converted |
| 4 — Site layout and building envelopes | [`04-site-layout-and-building-envelopes.md`](04-site-layout-and-building-envelopes.md) | Converted |
| 5 — Energy efficiency and urban design | [`05-energy-efficiency-and-urban-design.md`](05-energy-efficiency-and-urban-design.md) | Converted |
| 6 — Acoustic privacy and management | [`06-acoustic-privacy-and-management.md`](06-acoustic-privacy-and-management.md) | Converted |
| 7 — Landscape | [`07-landscape.md`](07-landscape.md) | Converted |
| 8 — Safety and security | [`08-safety-and-security.md`](08-safety-and-security.md) | Converted |
| 9 — Site facilities | [`09-site-facilities.md`](09-site-facilities.md) | Converted |

9 of 9 sections converted. No appendices or figures in the source (unlike 10.4/10.5/10.8,
this sub-chapter has no appendix).

## Anomalies / notes flagged during conversion

- **Partial amendment date**: cover page reads "June 2023 (Amended April 2025)" — no day
  is given and there is no amendment table to cross-check against, so `effective_date` and
  `amended_date` front-matter fields are omitted from every section file per the conversion
  guide, rather than guessing a day.
- **Cross-reference to "Chapter 3.3"**: clause 5.1 refers applicants to "Chapter 3.3 of this
  DCP" for energy efficiency requirements — this is Chapter 3 (General Requirements),
  sub-chapter 3.4 "Sustainable Development" per this repo's Chapter 3 index, not 3.3. This
  looks like a source numbering mismatch (worth checking against the actual printed Chapter
  3 PDF) rather than something to silently correct here — flagged, not resolved. The same
  cross-reference recurs in 10.5 clause 5.1 (Places of Public Worship), so it is not
  isolated to this sub-chapter.
- **Storey limit and Zone E1/MU1 setbacks are undefined numerically** (clauses 4.6, 4.10,
  4.13) — Council determines these case-by-case "based on the scale of the street and the
  surrounding buildings" rather than a fixed figure. This is a genuine discretionary control
  in the source, not an omission.
- No duplicate clause numbers or obvious typos were found in this sub-chapter (unlike some
  other Chapter 8/9 sub-documents already in this repo).
