---
title: "Canterbury-Bankstown DCP 2023 — Chapter 5.2: Former Canterbury LGA"
council: Canterbury-Bankstown
former_lga: Canterbury
document_type: DCP
chapter: "5.2"
chapter_title: Residential Accommodation
effective_date: 2023-06-01
amended_date: 2026-03-12
last_verified: 2026-08-19
source_document: 2026_03_12_-_DCP_2023_-_AMENDMENT_11_-_Chapter_5_2_-_Former_Canterbury_LGA_pdf.pdf
zones: [R2, R3, R4, E1, E3]
tags: [dcp, residential, canterbury-bankstown, canterbury]
---

# Chapter 5.2 — Residential Accommodation (Former Canterbury LGA)

This chapter of the Canterbury-Bankstown DCP 2023 applies to residential accommodation
within the former Canterbury Local Government Area. It sits alongside the
Canterbury-Bankstown LEP 2023, which sets zones, lot sizes, floor space ratios and building
heights; this DCP chapter adds detailed design controls (setbacks, storey limits, landscape,
privacy, parking, etc.) for each housing type.

**Numbering style**: unlike its sibling 5.1 (former Bankstown LGA), this source document
restarts its own `O1, O2…` Objectives sequence and `C1, C2…` Development controls sequence
at every numbered sub-clause (e.g. 2.1, 2.2, 2.3…), rather than using one Objectives list per
whole section with continuously-numbered clauses. This is a genuine difference in the two
former councils' original DCPs, not a conversion inconsistency — see the Chapter 5 `_index.md`.

**Known PDF defect — reconstructed labels**: this source PDF drops many "O#"/"C#" list
labels from its text layer while still rendering them visually on the page (confirmed
against PyMuPDF word-level text extraction cross-checked with rendered page images — a
genuine export defect, not an extraction failure). Where every checked instance is strictly
sequential with no gaps, missing labels have been reconstructed and flagged
`[RECONSTRUCTED-LABEL]` inline. **Please manually spot-check flagged blocks against the
source PDF**, especially those marked "not verified against a page image" in the
per-section notes below.

## Sections in this chapter — ALL CONVERTED

| # | Section | File | Zones |
|---|---------|------|-------|
| 1 | Introduction | [01-introduction.md](01-introduction.md) | R2, R3, R4 |
| 2 | Dwelling houses and outbuildings | [02-dwelling-houses-and-outbuildings.md](02-dwelling-houses-and-outbuildings.md) | R2 |
| 3 | Dual occupancies and semi-detached dwellings | [03-dual-occupancies-semi-detached.md](03-dual-occupancies-semi-detached.md) | R2 |
| 4 | Multi dwelling housing and attached dwellings | [04-multi-dwelling-housing-attached-dwellings.md](04-multi-dwelling-housing-attached-dwellings.md) | R3, R4 |
| 5 | Residential flat buildings | [05-residential-flat-buildings.md](05-residential-flat-buildings.md) | R3, R4 |
| 6 | Shop top housing | [06-shop-top-housing.md](06-shop-top-housing.md) | E1, E3, R4 |
| 7 | Secondary dwellings | [07-secondary-dwellings.md](07-secondary-dwellings.md) | R2 |
| 8 | Boarding houses | [08-boarding-houses.md](08-boarding-houses.md) | R2, R3, R4, E1, E3 |
| 9 | Livable housing | [09-livable-housing.md](09-livable-housing.md) | R2, R3, R4 |
| 10 | Solar light reflectivity (glare) | [10-solar-light-reflectivity-glare.md](10-solar-light-reflectivity-glare.md) | R3, R4 |

## Reconstruction verification status

Blocks marked ✅ were individually checked against a rendered image of the source PDF page.
Everything else follows the same sequential-reconstruction rule but has **not** been visually
spot-checked — please prioritise checking these against the source PDF, per the workflow
agreed with the repo owner.

| Section | Reconstructed blocks | Verified? |
|---|---|---|
| 2.5 Height (C1–C11) | Yes | Verified against page 10 |
| 2.9 Roof design (C1–C7) | Yes | Verified against page 17 |
| 2.10, 2.13, 2.15 | Yes | Not verified |
| 3.2, 3.5, 3.6, 3.7, 3.9, 3.10, 3.13 | Yes | Not verified |
| 4.1, 4.6, 4.7, 4.8, 4.10, 4.13 | Yes | Not verified |
| 5.2.2, 5.2.3, 5.2.4 (partial), 5.2.6, 5.2.7, 5.2.13, 5.2.15, 5.3.1-5.3.4, 5.3.6, 5.3.7, 5.3.14, 5.3.15 | Yes | Not verified |
| 6.2.1, 6.2.3, 6.2.4, 6.2.6, 6.2.9 (entries only), 6.2.10, 6.2.11 (O1), 6.2.13 (controls), 6.3.1, 6.3.3, 6.3.4, 6.3.5, 6.3.6, 6.3.7, 6.3.10 (O), 6.3.11, 6.3.12 (O1) | Yes | Not verified |
| 7 (all objectives) | Yes | Not verified |
| 8.1, 8.3, 8.5, 8.8, 8.12 (O1) | Yes | Not verified |

## Conversion-process correction (not a source anomaly)

- **Section 6, clause 6.3.13**: the automated first-pass label-reconstruction script used
  earlier in this conversion mis-parsed the boundary between an Objectives block and the
  following Development controls list, producing a nonsensical run of 19 fake "objectives"
  that swallowed an entire controls list and even a following section heading. This was
  caught during manual review and rewritten correctly by hand using the actual source
  structure. Flagged here as a reminder that the automated first pass was a starting point
  only, not a substitute for reading each section before finalising it.

## Source anomalies flagged during conversion (not silently resolved)

- **3.9 / 4.10 / 5.2.11 / 5.3.10 (Roof design)**: source repeats "Relate roof design to the
  desired built form and context." a second time in each of these near-identical roof-design
  blocks. In 3.9 and 4.10 the duplicate has no printed clause number (not counted as a
  separate control). In 5.2.11 and 4.5, by contrast, the duplicate **does** have its own
  printed clause number (C10, duplicating C8/C3 respectively) — preserved as printed since
  it's a genuine distinct source citation, not a reconstruction choice.
- **3.13 (Visual privacy)**: source duplicates an entire control paragraph verbatim
  (re-lettered) immediately after itself. Flagged, not double-numbered.
- **4.12 (Solar access), clause C6** and **8 (Visual privacy), clause C3**: specify different
  numeric thresholds (2 hours vs 3 hours for clothes-drying sunlight in 4.12; 1.6m vs 1.5m
  window sill height in Section 8) than the equivalent clauses elsewhere in this chapter.
  Preserved as printed — may be intentional or drafting inconsistencies; worth asking
  Council either way.
- **5.2.10 clause C28(b)/(c)** and **5.3.3 / 5.2.3 "Consolidate communal open space..."**:
  minor duplicated sub-items/sentences within the source, noted inline where they occur.
- Several minor spelling/typo corrections noted inline where they occurred throughout
  (e.g. "circustance" -> "circumstance"; a stray "+" in "substations+"; "seperation" ->
  "separation").
- **Section 5**: the source's own internal "5.1 / 5.2 / 5.3" sub-numbering (General
  objectives / SEPP applications / Non-SEPP applications) is unrelated to this repo's
  Chapter 5.1 (former Bankstown) / 5.2 (former Canterbury) split — flagged prominently at
  the top of `05-residential-flat-buildings.md` to avoid confusion. Section 6 (Shop top
  housing) has the same internal 6.1/6.2/6.3 pattern.
- **5.3.9 and 5.3.10**: rather than re-transcribing ~600 near-identical lines a second time,
  these point back to 5.2.10 and 5.2.11 respectively (which are, on inspection, identical in
  substance) with a note to split them back out if a future amendment makes them diverge.

## Follow-up needed

- **Reconstructed-label blocks not yet verified against page images** (table above) — the
  single largest remaining task for whoever reviews this conversion.
- The DCP references a **Landscape Guide**, a **Heritage Guide**, and the **Apartment Design
  Guide (ADG)** made under the *State Environmental Planning Policy (Housing) 2021* — none
  are yet in this repo. Section 5 and 6 in particular defer heavily to the ADG for SEPP
  applications (balconies, building separation, solar access, ceiling heights) rather than
  giving their own numeric controls, so a chatbot answering questions about SEPP-application
  residential flat buildings or shop top housing will hit a wall without it.
- **Chapters 3, 6, 7 and 8** are referenced by cross-reference tables in Section 8
  (Boarding houses) and elsewhere, but chapters 6–8 are not yet converted in this repo
  (see the top-level `_index.md`).

## Appendices (not yet converted)

Figures 1 and 2 in Section 2 (dwelling houses) and Section 3 (dual occupancies) are
basement-parking-arrangement diagrams referenced by specific clauses (2.16 C5/C6; 3.16 C5).
Image content, not text — not converted here. Add `appendices/_index.md` when these figures
are sourced, following the same pattern as Chapter 5.1's `appendices/_index.md`.
