---
title: "Chapter 9.1 — General Requirements"
council: Canterbury-Bankstown
document_type: DCP
chapter: "9.1"
effective_date: 2023-06-01
amended_date: 2025-04-01
last_verified: 2026-09-02
zones: [E4]
tags: [industrial-precinct, general-industrial, e4]
---

# Chapter 9.1 — General Requirements

Applies council-wide to land in **Zone E4 General Industrial** (not split by former LGA at
the document level — see the "Application of this chapter" check in the chapter-level
`_index.md`). Sets out design and amenity controls for industrial precinct development:
site cover, street/side/rear setbacks, landscape and deep-soil requirements, employee
amenity areas, facade and roof design, crime-prevention/safety measures, environmental
management (noise and pollution), and site facilities (hazardous materials storage,
utilities, substations, food premises, front fences). Sourced from the June 2023 edition,
amended April 2025.

Two clauses (2.2 and 2.3) vary internally by former LGA — see Section 2 below — but this
does not amount to a document-level LGA split, so the sub-chapter sits under `general/`
alongside any future Chapter 9 sub-documents that also prove to be council-wide.

## Sections

| Section | File | Clauses |
|---|---|---|
| Section 1 — Introduction | [`01-introduction.md`](01-introduction.md) | Objectives O1–O5; desired character C1 |
| Section 2 — Building Form and Landscape | [`02-building-form-and-landscape.md`](02-building-form-and-landscape.md) | 2.1–2.16 |
| Section 3 — Building Design | [`03-building-design.md`](03-building-design.md) | 3.1–3.19 |
| Section 4 — Environmental Management | [`04-environmental-management.md`](04-environmental-management.md) | 4.1–4.2 |
| Section 5 — Site Facilities | [`05-site-facilities.md`](05-site-facilities.md) | 5.1–5.13 |
| Appendices | [`appendices/_index.md`](appendices/_index.md) | Appendix 1 (converted); Figure 3a (not converted — image) |

## Source anomalies flagged during conversion

1. **TOC/heading mismatch** — the source PDF's Table of Contents lists Section 2 as
   "Building envelopes and landscape", but the printed section heading itself reads
   "Building form and landscape". Not resolved silently; see the note at the top of
   `02-building-form-and-landscape.md`.
2. **Internal former-LGA split within a single clause pair** — clauses 2.2 (former
   Bankstown LGA) and 2.3 (former Canterbury LGA) set different street-setback minimums.
   This is the only LGA-dependent content in the chapter; everything else applies
   uniformly. Worth checking during a future cross-chapter reconciliation pass, alongside
   the similar internal zone-split pattern already flagged in Chapter 8.1 (E3/SP4).
3. **Figure 3a not converted** — see `appendices/_index.md`. The callout legend text is
   preserved in `03-building-design.md`; the photograph is not.
4. **No duplicate clause numbers or obvious source typos were found** in this sub-chapter
   (unlike some Chapter 7/8 sub-documents) — clauses run sequentially 2.1–2.16, 3.1–3.19,
   4.1–4.2, 5.1–5.13.
5. **Amendment date** — cover page and every footer consistently read "June 2023 (Amended
   April 2025)"; no discrepancy found here (contrast with the Chapter 1.1 date discrepancy
   noted elsewhere in this repo).

## Not yet verified

- Whether Chapter 9 has further sub-documents (9.2, 9.3, …) beyond this General
  Requirements chapter. Nothing in this source PDF lists further sub-chapters, but
  Council's own document navigation hasn't been separately checked — same caveat as noted
  for Chapter 1. See the chapter-level `_index.md`.
