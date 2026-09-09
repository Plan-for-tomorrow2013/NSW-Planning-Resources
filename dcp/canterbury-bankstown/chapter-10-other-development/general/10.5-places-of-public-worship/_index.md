---
title: "10.5 Places of Public Worship"
council: Canterbury-Bankstown
document_type: DCP
chapter: "10.5"
last_verified: 2026-09-03
---

# 10.5 – Places of Public Worship

Canterbury-Bankstown DCP 2023, Chapter 10 (Other Development), sub-chapter 10.5. Source
PDF cover date: June 2023 (Amended April 2025).

Sets out development controls for places of public worship (new buildings, extensions,
and/or occupation of an existing building), covering site analysis, location and traffic
management (including required separation from sex services premises), site layout and
building envelopes (assembly area caps, height, setbacks, deep soil zones, sunlight access),
energy efficiency and urban design, acoustic privacy and management (including a mandatory
Neighbourhood Liaison Committee in the residential zones), open space and landscape,
safety and security, and site facilities/ancillary uses. Explicitly does **not** apply to
schools, except for places within a school used for regular public worship.

## Scope

No document-level former-LGA split. The explanation and objectives apply council-wide; the
only geographic/zone-based variation is by planning zone (R2/R3/R4 vs SP2/E4 vs E1/E3/MU1),
consistent with 10.1, 10.2, 10.3 and 10.4. Sits under `general/`.

One caveat: **Appendix 1** (state and regional roads) is itself scoped to the *former
Bankstown LGA* by its own heading — see the appendices index for how this is handled
(appendix-level note, not a document-level folder split).

## Sections

| Section | File | Status |
|---|---|---|
| 1 — Introduction | [`01-introduction.md`](01-introduction.md) | Converted |
| 2 — Site analysis | [`02-site-analysis.md`](02-site-analysis.md) | Converted |
| 3 — Location and traffic management | [`03-location-and-traffic-management.md`](03-location-and-traffic-management.md) | Converted |
| 4 — Site layout and building envelopes | [`04-site-layout-and-building-envelopes.md`](04-site-layout-and-building-envelopes.md) | Converted |
| 5 — Energy efficiency and urban design | [`05-energy-efficiency-and-urban-design.md`](05-energy-efficiency-and-urban-design.md) | Converted |
| 6 — Acoustic privacy and management | [`06-acoustic-privacy-and-management.md`](06-acoustic-privacy-and-management.md) | Converted |
| 7 — Open space and landscape | [`07-open-space-and-landscape.md`](07-open-space-and-landscape.md) | Converted |
| 8 — Safety and security | [`08-safety-and-security.md`](08-safety-and-security.md) | Converted |
| 9 — Site facilities and ancillary uses | [`09-site-facilities-and-ancillary-uses.md`](09-site-facilities-and-ancillary-uses.md) | Converted |

9 of 9 sections converted. Appendices: 1 of 3 converted in full (tabular data); 2 diagrams
not converted — see [`appendices/_index.md`](appendices/_index.md).

## Anomalies / notes flagged during conversion

- **Self-referencing clause 4.5**: "Despite clauses 4.5 and 4.6" almost certainly should
  read "Despite clauses 4.3 and 4.4" (the wall-height clauses it is meant to modify).
  Preserved verbatim, flagged inline in
  [`04-site-layout-and-building-envelopes.md`](04-site-layout-and-building-envelopes.md).
- **Boilerplate carried over from Schools**: Section 2 objective O1(e) reads "determine the
  enrolment numbers of schools over a long period of time" — places of public worship do not
  have enrolments; this looks like copy-paste boilerplate from the 10.2 Schools template.
  Flagged inline in [`02-site-analysis.md`](02-site-analysis.md).
- **"Chapter 3.3" cross-reference**: clause 5.1 refers to "Chapter 3.3 of this DCP" for
  energy efficiency — same numbering mismatch noted in 10.2 Schools clause 5.1; recurs
  identically here, so likely a shared drafting-template issue across Chapter 10 rather than
  an isolated error.
- **Two diagrams not converted**: Appendix 2 (assembly-area floor plan) and Appendix 3
  (maximum wall height diagram), plus the in-text Figure 4a (setback formula diagram) in
  Section 4. All three are described in text at the point they are referenced; see
  [`appendices/_index.md`](appendices/_index.md).
- **Appendix 1 scoped to former Bankstown LGA** within an otherwise council-wide
  sub-chapter — handled as an appendix-level note rather than a folder-level LGA split, per
  the conversion guide's principle that the LGA-split determination is made per source
  document/chapter, not per appendix. Also **appears to duplicate the equivalent appendix
  already converted in Chapter 9.1** (Industrial Precincts) — flagged for a future
  cross-chapter reconciliation pass (see top-level chapter notes).
- **Partial amendment date** ("Amended April 2025", no day, no amendment table) —
  `effective_date`/`amended_date` omitted from all section front matter per the conversion
  guide.
- No duplicate clause numbers found elsewhere in this sub-chapter.
