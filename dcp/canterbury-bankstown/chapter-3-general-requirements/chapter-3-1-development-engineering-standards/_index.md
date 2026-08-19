---
title: "Chapter 3.1 — Development Engineering Standards"
council: Canterbury-Bankstown
document_type: DCP
chapter: "3.1"
last_verified: 2026-08-18
tags: [development-engineering, civil-engineering, stormwater, drainage, on-site-detention]
---

Chapter 3.1 provides development engineering standards for civil engineering requirements, stormwater drainage systems, on-site detention systems and associated definitions. The chapter is converted as one file per source section.

| Section | Title | File | Clause range |
|---|---|---|---|
| 1 | Introduction | [01-introduction.md](01-introduction.md) | — |
| 2 | Civil engineering requirements | [02-civil-engineering-requirements.md](02-civil-engineering-requirements.md) | 2.1-2.4 |
| 3 | Stormwater drainage systems | [03-stormwater-drainage-systems.md](03-stormwater-drainage-systems.md) | 3.1-3.17 |
| 4 | On-site detention systems | [04-on-site-detention-systems.md](04-on-site-detention-systems.md) | 4.1-4.2 |
| 5 | Definitions | [05-definitions.md](05-definitions.md) | — |

### Source notes
- Source cover date: June 2023 (Amended March 2026). No exact day appears on the source cover.
  `effective_date` (2023-06-01) and `amended_date` (2026-03-01) are recorded at month precision
  — matching the convention used for the 2.2/2.3/2.4 conversion — rather than omitted entirely.
- No "Application of this chapter" wording appears in the source chapter.
- No named appendices appear in the source chapter.
- **Post-conversion fixes applied:**
  - Fixed a broken cross-reference in clause 3.17 (03-stormwater-drainage-systems.md), which
    linked to a flat file `2.2-flood-risk-management.md` that doesn't exist in this repo — 2.2
    was converted as a folder, so the link now correctly points to
    `../../chapter-2-site-considerations/2.2-flood-risk-management/_index.md`.
  - Merged doubled bold markdown spans in 05-definitions.md (e.g.
    `**Annual Exceedence Probability** **(AEP)**` → `**Annual Exceedence Probability (AEP)**`).
    Cosmetic only, no content change.
- **Confirmed, not fabricated:** the Chapter 3.2–3.7 titles listed in the parent
  [chapter-3-general-requirements/_index.md](../_index.md) were checked against the source
  PDF's own "Chapter 3 — General Requirements" navigation page and match exactly.
