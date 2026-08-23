---
title: "Canterbury-Bankstown DCP 2023 — Chapter 6.2 Bankstown City Centre — Section 4 Built Form — Index"
council: Canterbury-Bankstown
document_type: DCP
chapter: "6.2"
last_verified: 2026-08-22
---

## Section 4 — Built Form

| Sub-section | File | Status |
|---|---|---|
| 4.1.1 — Isolated sites | [01-minimum-lot-sizes-isolated-sites.md](01-minimum-lot-sizes-isolated-sites.md) | done |
| 4.2.1 — Building heights | [02-building-envelope-4-2-1-building-heights.md](02-building-envelope-4-2-1-building-heights.md) | done |
| 4.2.2 — Floor to floor height | [03-floor-to-floor-height.md](03-floor-to-floor-height.md) | done |
| 4.2.3 — Street wall | [04-street-wall.md](04-street-wall.md) | done |
| 4.2.4 — Ground level setbacks | [05-ground-level-setbacks.md](05-ground-level-setbacks.md) | done |
| Upper storey setbacks (printed 4.2.4 — numbering anomaly) | [06-upper-storey-setbacks.md](06-upper-storey-setbacks.md) | done |
| 4.2.5 — Building separation distance | [07-building-separation-distance.md](07-building-separation-distance.md) | done |
| 4.2.6 — Building floorplates | [08-building-floorplates.md](08-building-floorplates.md) | done |
| 4.3 — Residential ground floor frontage | [09-residential-ground-floor-frontage.md](09-residential-ground-floor-frontage.md) | done |
| 4.4 — Building interface with open space | [10-building-interface-open-space.md](10-building-interface-open-space.md) | done |
| 4.5.1 — Development interface with the public domain | [11-development-interface-public-domain.md](11-development-interface-public-domain.md) | done |
| 4.5.2 — Building awnings and interface with streets, plazas and squares | [12-building-awnings-interface.md](12-building-awnings-interface.md) | done |
| 4.5.3 — Active frontage design | [13-active-frontage-design.md](13-active-frontage-design.md) | done |
| 4.6 — Visual diversity, articulation and fine grain buildings | [14-visual-diversity-articulation-fine-grain.md](14-visual-diversity-articulation-fine-grain.md) | done |
| 4.7 — Materials and finishes | [15-materials-and-finishes.md](15-materials-and-finishes.md) | done |
| 4.8 — Rooftop and podium communal open space | [16-rooftop-podium-communal-open-space.md](16-rooftop-podium-communal-open-space.md) | done |

**Section 4 status: done (16 files covering all 14 numbered subsections, including the 4.2.4 duplicate-number anomaly as a separate file).**

### Notes

- **Significant numbering anomaly**: the source prints "4.2.4" twice — once for Ground Level Setbacks (pages 92–95) and again for Upper Storey Setbacks (pages 96–99). Everything downstream (4.2.5 Building separation distance, 4.2.6 Building floorplates) follows the sequence you'd expect if Upper Storey Setbacks were actually 4.2.5, but that's an inference — the source itself never corrects the duplicate "4.2.4" label. Flagged in detail in `06-upper-storey-setbacks.md`; this repo's filenames use positional slugs rather than asserting a corrected number.
- **Duplicated controls, second occurrence**: 4.2.5's C9–C12 are verbatim duplicates of C5–C8 — same exact pattern already found in [3.1.3](../section-3-designing-public-domain/03-laneways-shared-zones-service-lanes.md). Two independent occurrences of the identical duplication pattern suggests a systematic export/drafting issue in the source document rather than two unrelated typos — worth raising with Council directly.
- **Unrecoverable figure text**: Figure 32 (4.2.1, wind design guidelines) uses a custom/embedded font encoding on its source page that pdftotext cannot decode — flagged in `02-building-envelope-4-2-1-building-heights.md` rather than guessed at.
- **Un-digitised lot-level maps**: Figures 33, 37, 40 and 42 (maximum storeys, street wall heights, ground setbacks, upper storey setbacks) are large-format street maps assigning specific numeric controls to specific lots. None could be reliably extracted as structured text — each file flags this and recommends these four figures as the top priority for image conversion or manual digitisation, since they're the figures most likely to be asked about directly ("how tall can I build at X address").
- **Figures**: all figures for 4.1–4.3 logged in the chapter-level [`appendices/_index.md`](../../appendices/_index.md).
