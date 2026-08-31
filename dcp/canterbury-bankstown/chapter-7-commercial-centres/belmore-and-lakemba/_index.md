---
title: "Chapter 7.6 — Belmore and Lakemba Precinct"
council: Canterbury-Bankstown
document_type: DCP
chapter: "7.6"
effective_date: 2026-06-22
amended_date: 2026-06-22
last_verified: 2026-08-26
tags: [belmore, lakemba, area-specific-dcp, key-sites, complete, supersedes-7-3-sections-3-and-8, tree-canopy, public-domain, flood-controls, sustainability]
---

## Chapter 7.6 — Belmore and Lakemba Precinct

Standalone, area-specific DCP chapter for the Belmore and Lakemba Precinct — issued **Amendment 13** ("Final"). Replaces the former Section 3 (Belmore Local Centre) and Section 8 (Lakemba Local Centre) of Chapter 7.3 City East, which the current 7.3 Contents page explicitly marks "(Replaced by Chapter 7.6)" and which no longer contain any body text in the 7.3 PDF (see `../city-east/_index.md`). 142 pages: Introduction, Understanding Place, Public Domain Design, Building Design, General Provisions (including flood controls), Key Sites (4 named sites), and Appendices.

**Clause 1.1 (Application of this Chapter)** confirms the Precinct is comprised of the two local centres Belmore and Lakemba, and that this chapter **prevails over other CBDCP 2023 chapters to the extent of any inconsistency, except Chapter 4 Heritage** — the same precedence pattern confirmed directly in Chapter 7.7 (Punchbowl and Wiley Park) and (presumably, by template similarity) Chapter 7.5 (Canterbury).

**Status: complete — 7 of 7 sections converted.**

### Converted sections

| Section | Folder | Pages | Status |
|---|---|---|---|
| 1 — Introduction | [introduction/](introduction/_index.md) | 5–9 | **done** (3 of 3 sub-sections) |
| 2 — Understanding Place | [understanding-place/](understanding-place/_index.md) | 10–39 | **done** (10 of 10 files — 2.2 Character Areas split into overview + 7 per-area files) |
| 3 — Public domain design | [public-domain-design/](public-domain-design/_index.md) | 40–67 | **done** (6 of 6 sub-sections) |
| 4 — Building design | [building-design/](building-design/_index.md) | 68–101 | **done** (6 of 6 sub-sections — 4.2 The building envelope split into overview + 7 per-sub-section files) |
| 5 — General provisions | [general-provisions/](general-provisions/_index.md) | 102–120 | **done** (5 of 5 sub-sections — 5.4 Sustainability split into overview + 6 per-sub-section files) |
| 6 — Key Sites | [key-sites/](key-sites/_index.md) | 121–133 | **done** (5 of 5 sub-sections — overview + 4 named key sites) |
| 7 — Appendix | [appendices/](appendices/_index.md) | 134–142 | **done** (3 of 3 sub-sections — Definitions, Figures List, Table list) |

### Confirmed anomaly: amendment-date discrepancy (same pattern as 7.7)

The title page reads **"March 2026 Final"**, but the source filename indicates **Amendment 13, dated 22 June 2026**. This mirrors the confirmed-unresolved discrepancy in Chapter 7.7 (title page "March 2026 Final" vs. filename Amendment 14, dated April 2026). Not resolved here either — front matter above uses the filename date (2026-06-22) pending Council confirmation of which date is authoritative for citation purposes.

### Resolved: Figure 9 was never missing

An earlier session flagged a suspected gap ("Figures numbered sequentially 1–8 ... then jump to Figure 10 (page 16) — no Figure 9 appears in pages 1–39"). Cross-checking against the source's own Figures List (Section 7.2, converted in this session) and the page 15 caption directly confirms **Figure 9 ("Character areas map") does exist**, on page 15, within Section 2.2. This was a scanning miss in the earlier session, not a genuine numbering gap. See `appendices/02-figures-list.md` for the full, authoritative figure list (all 63 figures, cross-checked page by page).

### Confirmed anomaly: zone-name mismatch in Section 3.4, Control C10

Control C10 (green cover requirement for local centre development) refers to the **"B2 Local Centre zone"**, while the rest of Section 3.4 — including Table 2's canopy-coverage requirements — refers to the **"E1 Local Centre Zone"**. B2 is an older Standard Instrument LEP zone name; E1 is its current equivalent under the reformed commercial zone framework. Not resolved here — flagged in `public-domain-design/04-tree-canopy-green-cover-deep-soil.md` rather than silently corrected. Confirm with Council which zone C10 is meant to apply to before relying on it.

### Confirmed anomaly: duplicated controls, Section 5.4.3 vs 5.4.4

Section 5.4.4 (Water efficiency) Controls C5–C6 are verbatim duplicates of Section 5.4.3's Controls C4–C5, incorrectly referencing "energy target achievement" and NABERS inside a water-efficiency clause. Verified against the source page image (p.113) — the duplication exists in the source PDF itself, not a conversion artifact. Flagged in `general-provisions/sustainability/04-water-efficiency.md`, not silently corrected.

### Confirmed: Key Sites numbering matches Contents page (no anomaly)

An earlier session flagged this as needing a check, by analogy with Chapter 7.7 (where the Contents page numbered KS-4/5/6 one higher than the body headings). For 7.6, the Contents-page numbering (6.2–6.5 for KS-1 to KS-4) **matches** the body section headings exactly — no renumbering anomaly here. See `key-sites/_index.md`.

### Notable structural decisions

- **Sections split into their own subfolders** (each with a full internal Objectives/Principles/Controls treatment per sub-section, mirroring the precedent set by Section 2.2 Character Areas): `understanding-place/character-areas/` (2.2, 7 areas), `building-design/building-envelope/` (4.2, 7 sub-sections), `general-provisions/sustainability/` (5.4, 6 sub-sections).
- **Sections kept as single flat files despite having internal sub-headings** (because the sub-headings are short and/or tightly interdependent, and splitting further would fragment cross-references without adding retrieval value): 3.3 Streets/shared lanes/pedestrian links/arcades (8 named street visions), 4.3 Building interface (4.3.1 + 4.3.2), 5.5 Flood development controls (5.5.1–5.5.7).
- **Section 6 Key Sites**: each of the 4 named key-site files (6.2–6.5) contains only a Vision + Design Principles — no separate Objectives/Controls, since those are the general ones set out once in 6.1 and stated to apply to all key sites.
- **Section 7 Appendix**: 7.2 Figures List and 7.3 Table list were converted as their own files (not just folded into `appendices/_index.md`) since they are genuine numbered sub-sections of the source document, not just a conversion-repo index.

### Tables and complex content verified against page images

Tables 7–10 (5.4.2 — shading requirements and sun-angle tables) were cross-checked against rasterized page images (pp.110–111) because the raw PDF text layer mis-renders degree symbols (°) as trailing zero digits and merges some table columns. All other tables (1–6, 11) converted directly from the clean text layer.

Source file: `2026_06_22_-_DCP_2023_-_AMENDMENT_13_-_Chapter_7_6_-_Belmore_and_Lakemba_-_website.pdf`. Text layer is clean (fonts embedded, `pdftotext -layout` extracts cleanly) — no OCR needed.

### Quality check (per Conversion Guide)

- [x] Every clause number from the source appears in the output (Objectives, Principles, Controls numbered O/P/C throughout; anomalous/duplicated numbering preserved and flagged, not silently renumbered)
- [x] Every table converted, not summarised (11 of 11 tables, per Section 7.3's own table list)
- [x] Front matter zones match what the section's setback/height clauses actually say (zones populated only where a section names specific zones — e.g. 3.4, 5.1)
- [x] Appendices/figures noted, not silently dropped (all 63 figures logged inline per-section and consolidated in `appendices/02-figures-list.md`)
- [x] `_index.md` tables link to every section file at each folder level, and links use relative paths within the converted tree
