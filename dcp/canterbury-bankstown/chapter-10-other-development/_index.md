---
title: "Canterbury-Bankstown DCP 2023 — Chapter 10: Other Development"
council: Canterbury-Bankstown
document_type: DCP
chapter: "10"
last_verified: 2026-09-03
---

# Chapter 10 — Other Development

Status: **DONE — 8 of 8 sub-chapters complete** (10.1, 10.2, 10.3, 10.4, 10.5, 10.6, 10.7, 10.8).

Chapter 10 groups together development controls for specific, mostly small-scale land uses
that don't have their own dedicated chapter elsewhere in the DCP — child care, schools,
home-based work, non-residential uses within residential zones, places of worship,
commercial land uses, sex services premises, and telecommunications facilities.

## Sub-chapters

The expected full chapter list below is taken from Council's own Chapter 10 navigation
page (a screenshot of Council's website, supplied alongside the source PDFs), cross-checked
against the source PDFs' own cover-page titles where available.

| Sub-chapter | Council nav label | Source PDF title (canonical) | Folder / file | Status |
|---|---|---|---|---|
| 10.1 | Child Care Centres | Centre-Based Child Care Facilities | [`general/10.1-centre-based-child-care-facilities/`](general/10.1-centre-based-child-care-facilities/_index.md) | Converted (8 of 8 sections) |
| 10.2 | Schools | Schools | [`general/10.2-schools/`](general/10.2-schools/_index.md) | Converted (9 of 9 sections) |
| 10.3 | Home Businesses | Home Businesses and Home Industries | [`general/10.3-home-businesses-and-home-industries.md`](general/10.3-home-businesses-and-home-industries.md) | Converted (flat file — 1 of 1 section) |
| 10.4 | Non Residential Land Uses | Non-Residential Land Uses in Residential Zones | [`general/10.4-non-residential-land-uses-in-residential-zones/`](general/10.4-non-residential-land-uses-in-residential-zones/_index.md) | Converted (6 of 6 sections; 1 figure not converted — see its `_index.md`) |
| 10.5 | Places of Public Worship | Places of Public Worship | [`general/10.5-places-of-public-worship/`](general/10.5-places-of-public-worship/_index.md) | Converted (9 of 9 sections; 1 of 3 appendices converted, 2 diagrams not converted) |
| 10.6 | Commercial Land Uses | Commercial Land Uses | [`general/10.6-commercial-land-uses/`](general/10.6-commercial-land-uses/_index.md) | Converted (4 of 4 sections) |
| 10.7 | Sex Services Premises | Sex Services Premises | [`general/10.7-sex-services-premises/`](general/10.7-sex-services-premises/_index.md) | Converted (12 of 12 sections) |
| 10.8 | Telecommunications Facilities | Telecommunications Facilities | [`general/10.8-telecommunications-facilities/`](general/10.8-telecommunications-facilities/_index.md) | Converted (3 of 3 sections; appendix converted in full) |

## Scope check

Each converted sub-chapter's own text was checked before deciding folder shape, the same
way as previous chapters:

- **10.1** — no "Application of this chapter" clause; applies council-wide across
  residential zones, split internally by zone (R2/R3 vs R4). No former-LGA content.
- **10.2** — no "Application of this chapter" clause; applies council-wide, split
  internally by zone only (R2/R3/R4 site-width and setback rules vs Council-determined
  Zone E1/MU1 rules). No former-LGA content.
- **10.3** — no zone or LGA wording at all; applies generally. Only one internal section,
  kept as a flat file.
- **10.4** — Section 1's explanation states it applies to Zone R2, R3 and R4 council-wide.
  Section 4 (Serviced Apartments) has an internal former-LGA setback split; clause 5.2 is
  former-Canterbury-LGA-specific.
- **10.5** — no "Application of this chapter" clause; applies council-wide, does not apply
  to schools except worship spaces within a school. Split internally by zone. Its
  **Appendix 1** (state/regional roads) is itself scoped to the former Bankstown LGA —
  handled as an appendix-level note (see 10.5's `_index.md`), not a document-level split.
- **10.6** — no LGA wording; applies council-wide across three distinct commercial land
  uses (amusement centres, massage services premises, restricted premises), split
  internally by zone only for restricted premises (200m exclusion from residential/RE1).
- **10.7** — no LGA wording; applies council-wide, using distance-based controls (from
  sensitive uses, other sex services premises, and state roads) rather than zone- or
  LGA-based controls.
- **10.8** — no LGA wording; applies council-wide, split internally by zone only (Zone E1
  height; Zone R2/R3/R4 domestic satellite dishes).

All eight sit under `general/`, consistent with Chapters 4, 8 and 9.

## Notes

- **Title mismatch between Council's navigation and the source PDFs**: Council's own
  Chapter 10 index page (screenshot) uses shorter labels than the PDFs' cover-page titles —
  e.g. "10.1 - Child Care Centres" vs the PDF's own "10.1 Centre-Based Child Care
  Facilities"; "10.4 - Non Residential Land Uses" vs "10.4 Non-Residential Land Uses in
  Residential Zones". For 10.2, 10.5, 10.6, 10.7 and 10.8 the navigation labels and source
  PDF cover titles match exactly. This repo's file titles and folder names use the source
  PDFs' own titles as canonical, with the navigation label recorded in the table above for
  cross-reference when a reader arrives via Council's website wording.
- **Amendment dates are not uniform across the chapter**: 10.1–10.5 and 10.8 are "Amended
  April 2025"; 10.6 and 10.7 are "Amended August 2024". No single "as at" date applies to
  Chapter 10 as a whole.
- Source anomalies specific to each converted sub-chapter (an internal former-LGA setback
  split and an unconverted diagram in 10.4; a self-referencing clause 4.5 and two
  unconverted diagrams plus a likely-duplicated roads appendix in 10.5; a possible
  duplicated roads dataset in 10.7; a recurring "Chapter 3.3" cross-reference used in both
  10.2 and 10.5 that does not match this repo's actual Chapter 3 numbering; and the
  flat-file treatment of 10.3) are detailed in each sub-chapter's own `_index.md`.

## Recommended follow-up (cross-chapter reconciliation, not yet done)

- **State/regional roads datasets**: Chapter 9.1's Appendix 1, 10.5's Appendix 1, and
  10.7's Section 2 state-roads table all cover overlapping ground (state and/or regional
  roads relevant to the former Bankstown LGA / Canterbury-Bankstown). Worth checking whether
  these are meant to be a single maintained dataset that has drifted, or are genuinely
  independent lists for different regulatory purposes.
- **"Chapter 3.3" cross-reference**: both 10.2 (clause 5.1) and 10.5 (clause 5.1) instruct
  applicants to comply with "Chapter 3.3 of this DCP" for energy efficiency — this repo's
  Chapter 3 index shows the sustainable-development content actually sits at 3.4, not 3.3.
  Worth confirming against the source Chapter 3 PDFs directly rather than assuming a typo.
- **Self-referencing clause 4.5 in 10.5** almost certainly should read "clauses 4.3 and
  4.4" rather than "clauses 4.5 and 4.6" — worth confirming with Council before treating this
  repo's flagged note as authoritative for citation purposes.
