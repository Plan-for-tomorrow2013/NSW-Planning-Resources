---
title: "11.1 — 149–171 Milton Street, Ashbury"
council: Canterbury-Bankstown
document_type: DCP
chapter: "11"
section: "11.1"
last_verified: 2026-09-04
tags: [key-development-site, milton-street, ashbury, precedence-clause, heritage-conservation-area, wh-wagener-oval]
---

# 11.1 — 149–171 Milton Street, Ashbury

*June 2023 (Amended August 2024)*

A stand-alone, site-specific precinct DCP for the Milton Street Precinct, Ashbury (Lots A, B
and C DP 30778, bounded by Milton Street, Trevenar Street, Yabsley Avenue and WH
Wagener Oval). Currently industrial/commercial land and surface carparking; the chapter
sets controls for its redevelopment into a residential precinct grading from low-scale
terraces on Milton Street up to taller buildings along the WH Wagener Oval edge, with a
new road connecting Milton Street to the oval.

Like 11.2, 11.3 and 11.4, this sub-chapter carries its own precedence clause: the
development controls of Chapter 11.1 prevail over other DCP controls where there is an
inconsistency, for applications on this site (stated in Section 1; a second, narrower
precedence statement specific to waste controls also appears in Section 17).

**No former-LGA split.** The chapter has no "Application of this chapter" wording tied to
former Bankstown/Canterbury LGA boundaries — it is scoped entirely to this one precinct,
consistent with the other Chapter 11 sub-chapters and the corridor-/precinct-specific
sub-chapters already seen in Chapters 7 and 8. Sits under `general/`.

**17 internal sections** — unlike 11.2 (a single-section flat file), 11.1 has 2+ internal
sections and so gets its own folder with one file per section, per the conversion guide.

## Sections

| # | Section | File | Status |
|---|---|---|---|
| 1 | Introduction | [`01-introduction.md`](01-introduction.md) | Converted |
| 2 | Siting the development | [`02-siting-development.md`](02-siting-development.md) | Converted |
| 3 | Building height and density | [`03-building-height-density.md`](03-building-height-density.md) | Converted |
| 4 | Setbacks | [`04-setbacks.md`](04-setbacks.md) | Converted |
| 5 | Upper level setbacks | [`05-upper-level-setbacks.md`](05-upper-level-setbacks.md) | Converted |
| 6 | Building separation | [`06-building-separation.md`](06-building-separation.md) | Converted |
| 7 | View corridors | [`07-view-corridors.md`](07-view-corridors.md) | Converted |
| 8 | Building depth | [`08-building-depth.md`](08-building-depth.md) | Converted |
| 9 | Deep soil zones | [`09-deep-soil-zones.md`](09-deep-soil-zones.md) | Converted |
| 10 | Communal open space | [`10-communal-open-space.md`](10-communal-open-space.md) | Converted |
| 11 | Vehicular and pedestrian entries | [`11-vehicular-pedestrian-entries.md`](11-vehicular-pedestrian-entries.md) | Converted |
| 12 | New road | [`12-new-road.md`](12-new-road.md) | Converted |
| 13 | Basement parking | [`13-basement-parking.md`](13-basement-parking.md) | Converted |
| 14 | Excavation | [`14-excavation.md`](14-excavation.md) | Converted |
| 15 | Drainage | [`15-drainage.md`](15-drainage.md) | Converted |
| 16 | Tree retention | [`16-tree-retention.md`](16-tree-retention.md) | Converted |
| 17 | Waste management | [`17-waste-management.md`](17-waste-management.md) | Converted |

10 of 10 figures logged (all unconverted, image-only) — see
[`appendices/_index.md`](appendices/_index.md).

## Anomalies and notes flagged during conversion

- **Amendment date has no day**, only "Amended August 2024" on the cover/footers, with no
  amendment table in Section 1 to cross-check against — `amended_date` omitted from all
  section front matter per the conversion guide.
- **Figures 12.1.5 and 12.1.6 carry the operative numeric setback/separation dimensions**
  for individual buildings, not restated in clause text — see the stronger caveat in
  `appendices/_index.md`. This is the same pattern flagged for 11.2's Figure 1b.
- **Zones not stated for this site in the supplied text.** Unlike 11.4 (which explicitly
  states E1/R4 zoning), the 11.1 source PDF does not state the site's own zone — only that
  it is adjacent to Zone R2 (used as the sight-line benchmark in Figure 12.1.4/control 3.6).
  `zones` field omitted from front matter rather than guessed; worth checking against the
  LEP zoning map in a future pass.
- **Clause 9.5** reads "tree planning" — likely a source typo for "tree planting", preserved
  verbatim and flagged inline.
- **Clause 17.8** describes the recycling-collection carting route using wording that
  duplicates 17.6's *bulky waste* carting-route clause almost verbatim ("from the bulky
  storage area(s)") — possible drafting carry-over rather than a genuine cross-reference to
  bulky waste; flagged inline in Section 17 rather than silently corrected.
- **Two precedence clauses in one sub-chapter**: the chapter-level clause in Section 1, and
  a second, waste-specific precedence statement in Section 17's Explanation. Both preserved
  and distinguished — see the note in `17-waste-management.md`.
- This is the **third** Chapter 11 precedence-clause sub-chapter after 11.2 and 11.4 (and
  now 11.3) — consistent with the pattern already flagged for Chapter 7's newer precinct
  DCPs and Chapter 8.3 Section 6. Worth including in the same future cross-chapter
  reconciliation pass.
