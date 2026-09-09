---
title: "Chapter 11.16 — 1 Leicester St, Chester Hill (Chester Square)"
council: Canterbury-Bankstown
document_type: DCP
chapter: "11.16"
last_verified: 2026-09-09
---

# 11.16 — 1 Leicester Street, Chester Hill ("Chester Square")

Site-specific precinct DCP for the Chester Square site, 1 Leicester Street, Chester Hill
(bounded by Priam Street, Waldron Road, Frost Lane and Bent Street), providing detailed
provisions additional to the Canterbury-Bankstown Local Environmental Plan (CBLEP) 2023 for
a mixed-use redevelopment (retail, residential towers up to ~18 storeys/60m, a publicly
accessible open space of 2,000–2,800m², and a dedicated public community facility).

No former-LGA content — consistent with every other Chapter 11 sub-chapter, this sits under
`general/`. No internal zone, development-type or storey-transition split is stated either;
unusually for Chapter 11, **no zone code (e.g. R4, B4, E1) is stated anywhere in the supplied
text** — the source relies entirely on Figure 3 (site boundary) and the CBLEP for zoning,
rather than naming a zone in this chapter's own text. This is a difference from most other
Chapter 11 sub-chapters, which typically name their own zone at least once.

Cover-page date reads **"March 2026"** only — no day, and no "Amended" wording, and no June
2023 base date. This breaks the "June 2023 (Amended August 2024 / April 2025)" pattern shared
by every other converted Chapter 11 sub-chapter (11.1–11.14), echoing the way 11.14 broke the
pattern with "August 2025 (Final Version)". Per the conversion guide, a month/year-only date
with no amendment table is omitted from front matter (`effective_date`/`amended_date`) rather
than guessed. Worth checking whether 11.16 is a genuinely new chapter (not an amendment to a
pre-existing 2023 chapter) — unlike 11.1–11.15, nothing in the supplied text refers to an
original "June 2023" version of this specific chapter.

## Sections

18 numbered content sections (1.1–4.6) plus a Section 5 Appendix (5.1 Figures List, converted
in full as a table — see file 19). Kept in its own folder per the conversion guide's 2+
section rule.

| File | Section | Title |
|---|---|---|
| [01](01-explanation.md) | 1.1 | Explanation |
| [02](02-application-of-this-dcp.md) | 1.2 | Application of this DCP (incl. 1.2.1 How to read this DCP) |
| [03](03-vision-and-character.md) | 1.3 | Vision and Character |
| [04](04-design-excellence.md) | 1.4 | Design Excellence |
| [05](05-connecting-to-country.md) | 1.5 | Connecting to Country |
| [06](06-active-frontages-public-domain.md) | 2.1 | Active Frontages and improving the Public Domain (incl. 2.1.1 Ground floor frontage) |
| [07](07-public-art.md) | 2.2 | Public Art |
| [08](08-streets.md) | 2.3 | Streets (incl. 2.3.1 Frost Lane and Charles Place; 2.3.2 Priam, Bent and Leicester Streets, Sections A–D) |
| [09](09-publicly-accessible-open-space.md) | 2.4 | Publicly Accessible Open Space |
| [10](10-building-envelope-and-height.md) | 3.1 | Building Envelope and Height |
| [11](11-dwelling-mix-flexible-housing.md) | 3.2 | Dwelling Mix and Flexible Housing |
| [12](12-private-communal-space.md) | 3.3 | Private Communal Space |
| [13](13-public-community-facility.md) | 4.1 | Public Community Facility |
| [14](14-access-and-parking.md) | 4.2 | Access and Parking (incl. 4.2.1 Pedestrian Access; 4.2.2 Cycling) |
| [15](15-sustainability.md) | 4.3 | Sustainability |
| [16](16-waste-management.md) | 4.4 | Waste Management |
| [17](17-amenity.md) | 4.5 | Amenity (incl. 4.5.1 Solar Access; 4.5.2 Wind effects) |
| [18](18-landscaping.md) | 4.6 | Landscaping |
| [19](19-figures-list.md) | 5.1 | Figures List (converted in full — genuine text/tabular content, not an image) |

See [`appendices/_index.md`](appendices/_index.md) for all unconverted figures (maps,
diagrams, photos).

## Scope check

No former-LGA content. Site-specific precinct DCP for a single named site (Chester Square,
1 Leicester Street, Chester Hill), consistent with every other Chapter 11 sub-chapter. No
internal zone, development-type or storey-height-transition split like 11.4/11.6/11.10 —
building height instead varies by **block**, per Figure 25's storey map (2–18 storeys), which
is not paralleled by an equivalent enumerated list in the text controls (see file 10 and
`appendices/_index.md`).

Consistent with the rest of Chapter 11, 11.16 carries its own precedence-style statement, but
phrased as ordinary prose within 1.2 (Application of this DCP) rather than as a standalone
numbered clause: *"In case of any conflict between the controls in this DCP chapter and those
in another, the provisions of this DCP will prevail."* This is the same substantive effect as
the discrete precedence clauses seen in 11.1–11.14, just embedded in different wording.

## Anomalies and flags (not silently resolved)

- **"Definitions" part promised but never delivered.** The front-matter "Explore the design
  for Chester Square DCP" graphic (page 3 of the source PDF) lists five parts: Introduction,
  Public Domain, Built Form, General Provisions, and **Definitions**. The actual document
  (per its own Contents page, page 4) has only Sections 1–5 (Introduction, Public Domain,
  Built Form, General Provisions, **Appendix**) — there is no Definitions section anywhere in
  the 57-page source. This looks like boilerplate carried over from a template that wasn't
  fully populated for this chapter, rather than missing pages (the PDF's own pagination is
  otherwise complete and consistent, ending at the back cover, page 57).
- **No zone code stated anywhere in the chapter.** Unlike most other Chapter 11 sub-chapters
  (which cite at least one zone, e.g. 11.4's E1/R4, 11.9/11.12's hospital zones, 11.13's zone
  mix), 11.16 never names a zone for the Chester Square site in its own text — only the site
  boundary (Figure 3) and a generic reference to "the LEP." `zones:` is omitted from every
  section's front matter accordingly, per the conversion guide's instruction to omit rather
  than guess.
- **1.3 (Vision and Character) and 4.1 (Public Community Facility) both skip the Objectives
  tier** of the O→P→C hierarchy that 1.2.1 ("How to read this DCP") itself sets out — 1.3 has
  only a prose "Locality Statement" plus Principles (no Controls either); 4.1 has only
  Principles and Controls (no Objectives). See files 03 and 13.
- **3.3 (Private Communal Space) prints "Principles" before "Objectives"** — the only section
  in this sub-chapter (and, so far, in Chapter 11) where the printed order inverts the
  Objectives→Principles→Controls sequence set out in 1.2.1. Preserved in that order; see
  file 12.
- **1.5 (Connecting to Country) introduces "Design Guidance" (G1–G6)** in place of
  "Controls" — not matching the O/P/C hierarchy defined in 1.2.1, and not matching the O#/C#
  restart pattern seen in 11.13/11.14. A "G#" label was used once before in Chapter 11
  (11.13's Appendix A, restarting under each of its own four headings), but only inside an
  appendix — 11.16 is the first sub-chapter to use "G#" as a main-hierarchy label (alongside
  Objectives, replacing Controls) rather than as appendix-only content. See file 05.
- **1.5's clause G5 is apparently missing its own sub-list.** G5 introduces "the following
  design opportunities should be considered" but no list items follow before G6 begins —
  either a supply gap or a formatting loss in the source PDF. See file 05.
- **2.3.2's "Section D" (Leicester Street, page 27) has no accompanying Objective, Principle
  or Control text** — only a "Section D" label and Figure 17 (plan/section diagram). Sections
  A, B and C (Frost Lane; Priam/Bent commercial interface; Priam/Bent/Leicester Street design)
  each carry their own text alongside their figure; Section D does not. Possible incomplete
  supply, similar in kind to 11.5's and 11.6's previously-flagged incomplete-supply concerns.
  See file 08.
- **2.4's control C5 is internally contradictory as printed**: "Through site access is
  required 24 hours a day and must include DDA compliant ramps / lifts and must not rely on
  lifts, escalators or other mechanical modes of transport." This requires DDA-compliant
  lifts/ramps while also saying access must not rely on lifts or other mechanical modes —
  preserved verbatim rather than silently resolved. See file 09.
- **Figure 27's on-page caption ("Podium level setbacks Map") does not match its Figures List
  caption ("Ground level setbacks map")** — a minor label mismatch of the same kind already
  flagged elsewhere in this DCP (e.g. Chapter 4's Table-of-Contents/heading mismatches,
  Chapter 9.1's Section 2 heading mismatch). See file 10 and `appendices/_index.md`.
- **Figure 25 (Building height storeys map) is the sole source of the site's specific
  per-block maximum storeys (values from 2 up to 18 storeys across different blocks)** — no
  text control anywhere in Section 3.1 enumerates these figures; C1–C9 describe only general
  street-wall heights (2–3 storeys) and tower setback/footprint rules. This is the same
  "sole-source figure" pattern already flagged repeatedly elsewhere in Chapter 11 (e.g. 11.1's
  Figures 12.1.5/12.1.6, 11.10's Figure 2). See file 10 and `appendices/_index.md`.
- **An uncaptioned photograph (Aboriginal artefacts/tools, page 15, within 1.5 Connecting to
  Country) does not appear in the Section 5.1 Figures List at all** — every other photo and
  diagram in this chapter has a "Figure N." caption and a corresponding row in the Figures
  List; this one has neither. See file 05 and `appendices/_index.md`.
- **4.2.2 (Cycling) cites "Chapter 6.2 Bankstown City Centre Development Control Plan,
  Section 5.2.3"** and **4.5.1 (Solar Access) cites "Chapter 5.1 of the Canterbury Bankstown
  DCP 2023."** Chapters 5 and 6.2 are both already fully converted in this repo, so — unlike
  most of the Chapter 3.x cross-references flagged elsewhere in Chapter 11 (which cite
  chapters not yet converted, or not matching this repo's structure) — these two citations
  can be checked directly against existing content. Not yet reconciled in this pass; flagged
  for the cross-chapter reconciliation pass. See files 14 and 17.
- **4.4 (Waste Management) restarts its Objectives numbering (O1–O5, then O1–O3 again) under
  two sub-headings ("Construction" then "Operation")** rather than running one sequential O#
  count for the section — the same kind of nested-numbering-restart pattern already flagged
  for Chapter 8.2/8.3 and 11.13/11.14, but here affecting Objectives rather than Controls.
  See file 16.
- **Divider-page mini-Contents for Section 4 (page 44) labels 4.2 as "Access"**, while the
  master Contents page (page 4) and the section heading itself (page 46) both read "Access
  and Parking" — a minor title inconsistency of the same kind already seen elsewhere in this
  DCP (e.g. Chapter 9.1's ToC/heading mismatch).
- **No amendment table is supplied**, consistent with every other Chapter 11 sub-chapter, so
  the "March 2026" cover date cannot be cross-checked against a list of specific changes.

## Figures

38 numbered figures (Figure 1–38) plus one unnumbered/unlisted photograph (see above). Full
list converted verbatim as file 19 (`19-figures-list.md`) since the Figures List itself is
genuine text/tabular content, not an image. All 38 figures are maps, diagrams or photographs
and are not themselves converted to image assets — see `appendices/_index.md` for the full
breakdown of which figures carry sole-source numeric/spatial information (Figures 3, 8, 10,
19, 25, 26, 27, 28, 33) versus purely illustrative photographs.
