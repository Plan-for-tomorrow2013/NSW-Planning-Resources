---
title: "11.14 — Riverwood Estate (Stage 1 DCP)"
council: Canterbury-Bankstown
document_type: DCP
chapter: "11.14"
last_verified: 2026-09-07
tags: [riverwood-estate, precinct-dcp, state-significant-precinct, structure-plan]
---

# 11.14 — Riverwood Estate

**This sub-chapter does not follow the pattern established by 11.1–11.12 and needs
deliberate confirmation from the repo owner before being treated as "just another Chapter
11 site."** See flags below.

## Structure and file map

Unlike 11.1–11.12 (simple sequential "Section 1, Section 2…" numbering with Objectives
O# / numbered clauses matching the section number), 11.14 is a full multi-part precinct
DCP with four top-level **Sections**, each containing its own numbered **sub-sections**
(1.1, 1.2… / 2.1, 2.2… / 3.1–3.7 / 4.1–4.4), and each sub-section using **O# (Objectives) /
C# (Controls)** numbering that restarts at 1 in every sub-section. One file has been created
per sub-section, following the same "sub-document with 2+ internal sections gets its own
folder, one file per section" rule used elsewhere in the guide — here applied one level down
(11.14 itself is the sub-document; its "sections" are 1.1, 1.2, 2.1, 3.1… etc.).

| Section | Sub-section | Title | File |
|---|---|---|---|
| 1 — Introduction | 1.1 | Name of this Plan | [`1.1-name-of-this-plan.md`](1.1-name-of-this-plan.md) |
| | 1.2 | Purpose of this Chapter | [`1.2-purpose-of-this-chapter.md`](1.2-purpose-of-this-chapter.md) |
| | 1.3 | Land to Which this DCP Applies | [`1.3-land-to-which-this-dcp-applies.md`](1.3-land-to-which-this-dcp-applies.md) |
| | 1.4 | Relationship to Other Planning Instruments and DCPs | [`1.4-relationship-to-other-planning-instruments.md`](1.4-relationship-to-other-planning-instruments.md) |
| 2 — Vision and Character | 2.1 | Vision | [`2.1-vision.md`](2.1-vision.md) |
| | 2.2 | Project Objectives | [`2.2-project-objectives.md`](2.2-project-objectives.md) |
| 3 — Structure Plan and Built Form | 3.1 | Structure Plan, Street and Block Layout | [`3.1-structure-plan-street-and-block-layout.md`](3.1-structure-plan-street-and-block-layout.md) |
| | 3.2 | Height | [`3.2-height.md`](3.2-height.md) |
| | 3.3 | Setbacks and Street Wall Heights | [`3.3-setbacks-and-street-wall-heights.md`](3.3-setbacks-and-street-wall-heights.md) |
| | 3.4 | Building Design | [`3.4-building-design.md`](3.4-building-design.md) |
| | 3.5 | Open Space and Landscaping | [`3.5-open-space-and-landscaping.md`](3.5-open-space-and-landscaping.md) |
| | 3.6 | Water Sensitive Urban Design and Stormwater Management | [`3.6-water-sensitive-urban-design-and-stormwater-management.md`](3.6-water-sensitive-urban-design-and-stormwater-management.md) |
| | 3.7 | Solar Access | [`3.7-solar-access.md`](3.7-solar-access.md) |
| 4 — General Provisions | 4.1 | Traffic, Access and Parking | [`4.1-traffic-access-and-parking.md`](4.1-traffic-access-and-parking.md) |
| | 4.2 | Sustainability | [`4.2-sustainability.md`](4.2-sustainability.md) |
| | 4.3 | Heritage (own folder — 3 sub-subsections) | [`4.3-heritage/_index.md`](4.3-heritage/_index.md) |
| | 4.4 | Waste | [`4.4-waste.md`](4.4-waste.md) |

Figures: [`appendices/_index.md`](appendices/_index.md) (Figures 1–9 — image-only, not
converted; largest figure set of any Chapter 11 sub-chapter so far).

## Flags for review — please confirm before treating this as final

1. **This is not a "Chapter 11 key development site" in the same sense as 11.1–11.12.**
   Every other converted Chapter 11 sub-chapter is a short, single-topic, site-specific
   precinct DCP for one development site (typically 6–19 numbered clause sections). 11.14
   is a full State Significant Precinct-style structure plan document covering an entire
   multi-block estate, with sections on vision, structure planning, sustainability
   benchmarks (Green Star, NABERS), and a three-part Aboriginal/European heritage and
   Connecting with Country framework — closer in scope and format to a mini-LEP/masterplan
   than to a single-site DCP chapter. **Recommend confirming with the repo owner whether
   this really belongs under `general/` alongside 11.1–11.13, or deserves treatment as its
   own top-level entity** (the source's own title is "Stage 1 Riverwood Estate Development
   Control Plan 2023," suggesting it may consider itself a free-standing DCP rather than a
   simple sub-chapter).
2. **Date/version mismatch.** The cover page is dated **August 2025, "Final Version"** —
   this postdates every other Chapter 11 amendment date seen so far (11.1–11.9: June 2023,
   amended August 2024; 11.10/11.12: June 2023, amended April 2025). Yet the document
   internally names itself "Stage 1 Riverwood Estate **Development Control Plan 2023**"
   (Section 1.1) — a 2023-dated title on an August-2025-dated final document. No
   `effective_date`/`amended_date` has been set in any file's front matter because of this
   ambiguity — flagging rather than guessing which date is authoritative.
3. **No page footer date string** in this source (unlike 11.1–11.13, which all carry a
   "June 2023 (Amended ...)" footer on every page) — the only date evidence is the cover
   page. This breaks the pattern used elsewhere in the chapter to derive dates.
4. **O#/C# numbering, not clause numbers.** All other Chapter 11 sub-chapters number
   development controls as clauses matching the section number (e.g. clause "3.1" in
   Section 3). 11.14 instead uses **Objectives (O1, O2…) and Controls (C1, C2…)**, each
   restarting from 1 within every sub-section (i.e., there are unrelated "C1"s in 1.4, 3.1,
   3.2, 3.3, etc.). This is a genuinely new internal-numbering pattern for Chapter 11 —
   distinct even from 11.6's "unnumbered sub-headed" pattern. Cross-references must always
   cite sub-section + control label together (e.g. "3.3 C3", not just "C3").
5. **No former-LGA or zone split found.** The document does not name a former-LGA split,
   and only implicitly references zone-like concepts (none of R2/R3/R4/etc. appear by
   code). Placed under `general/` consistent with the rest of Chapter 11, but this is a much
   larger and more self-contained document than the other `general/` sub-chapters, so the
   `general/` classification is offered provisionally (see flag 1).
6. **Cross-references to the parent "DCP 2023" are pervasive and mostly unqualified.**
   Unlike 11.1–11.12's specific "Chapter 3.2"/"Chapter 5.2"-style citations, 11.14 mostly
   just says "the DCP 2023" or "Section 5 of the DCP 2023" (3.7 C2) or "Chapter 3 of the DCP"
   (4.2 C9) without a specific chapter/section number to check — flagged inline in the
   relevant files rather than resolved.
7. **Aboriginal/European heritage structure (4.3) has its own locally-restarting C#/O#
   numbering across three sub-subsections** — see [`4.3-heritage/_index.md`](4.3-heritage/_index.md)
   for detail.
8. **Figures not converted** — 9 figures, the largest set of any Chapter 11 sub-chapter to
   date; one (Figure 9, Virginia Place section) contains extractable dimension data that
   could be tabulated in a future pass. See [`appendices/_index.md`](appendices/_index.md).
