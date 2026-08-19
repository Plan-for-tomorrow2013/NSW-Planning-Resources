---
title: "Chapter 2.2 — Flood Risk Management"
council: Canterbury-Bankstown
document_type: DCP
chapter: "2.2"
effective_date: 2023-06-01
amended_date: 2025-04-01
last_verified: 2026-08-18
scope: dual-lga (see note below)
---

# Chapter 2.2 — Flood Risk Management

Provides objectives and development controls for flood-liable land across Canterbury-Bankstown,
supporting the Canterbury-Bankstown Local Environmental Plan 2023 and the *Floodplain
Development Manual* (NSW Government).

## ⚠️ Structural flag: this single sub-document covers two former LGAs differently

Unlike Chapter 5 (which splits into separate `former-bankstown-lga/` and
`former-canterbury-lga/` sub-documents per the Conversion Guide's LGA-split pattern), **Chapter
2.2 is one PDF, one sub-document number (2.2), with a single continuous section numbering
(Sections 1–10)** — but the document itself states a hard scope split partway through:

- **Sections 1–8** apply only to flood liable land in the **former Bankstown LGA** (stated explicitly in Section 1's "Land to which sections 1–8 apply").
- **Sections 9–10** apply only to land in the **former Canterbury LGA** (stated explicitly in Section 9's "Land to which sections 9–10 apply").

This doesn't match either pattern the Conversion Guide anticipates (a chapter that's wholly
council-wide, or a chapter that's split into separate former-LGA sub-documents). I've resolved
it as follows, but flagging for confirmation rather than treating it as settled:

- Kept **one folder, one file-per-section**, matching the source PDF's own structure (a single continuous Section 1–10 numbering), rather than forcing an artificial folder split.
- Recorded `former_lga: Bankstown` in the front matter of files 01–08, and `former_lga: Canterbury` in files 09–10, so downstream filtering/retrieval by LGA still works correctly despite the shared folder.
- Called this out at the top of both Section 1 and Section 9's files themselves, not just here, since a reader/chatbot landing directly on one of those files without seeing this index also needs the scope boundary to be obvious.

**Please confirm this treatment is what you want** — the alternative would be to physically
split this into `2.2-flood-risk-management/former-bankstown-lga/` (Sections 1–8) and
`2.2-flood-risk-management/former-canterbury-lga/` (Sections 9–10) sub-folders, matching
Chapter 5's precedent more literally. I didn't do that by default because Sections 1–8 share
Schedules 1–5 (Section 6) as common machinery, and splitting would mean either duplicating the
schedules into both LGA folders or awkwardly orphaning them — the source document's own
structure (schedules living centrally, referenced by the Bankstown-scoped sections) argued for
keeping it as one folder.

## Section 6 note

Section 6 ("Schedules") is ~43 pages covering six distinct schedules (1, 2, 3, 4A, 4B, 4C, 5)
that are each their own self-contained document with their own "SCHEDULE X" heading in the
source. Rather than one oversized `06-schedules.md` file, each schedule is its own file
(`06-schedule-1-...md` through `06-schedule-5-...md`), all sharing the `06-` prefix to preserve
their position in the source's Section ordering.

## Files

| Section | File | Status |
|---|---|---|
| 1 — Flood risk management in the former Bankstown LGA | [01-flood-risk-management-former-bankstown-lga.md](01-flood-risk-management-former-bankstown-lga.md) | ✅ converted |
| 2 — Criteria for determining applications | [02-criteria-for-determining-applications.md](02-criteria-for-determining-applications.md) | ✅ converted |
| 3 — Development controls | [03-development-controls.md](03-development-controls.md) | ✅ converted |
| 4 — Special considerations | [04-special-considerations.md](04-special-considerations.md) | ✅ converted |
| 5 — Fencing | [05-fencing.md](05-fencing.md) | ✅ converted |
| 6 — Schedule 1: Flood compatible materials | [06-schedule-1-flood-compatible-materials.md](06-schedule-1-flood-compatible-materials.md) | ✅ converted |
| 6 — Schedule 2: Land use categories | [06-schedule-2-land-use-categories.md](06-schedule-2-land-use-categories.md) | ✅ converted |
| 6 — Schedule 3: Georges River floodplain | [06-schedule-3-georges-river-floodplain.md](06-schedule-3-georges-river-floodplain.md) | ✅ converted — ⚠️ matrix needs visual verification |
| 6 — Schedule 4A: Carinya Road matrix | [06-schedule-4a-carinya-road-matrix.md](06-schedule-4a-carinya-road-matrix.md) | ✅ converted — ⚠️ matrix needs visual verification |
| 6 — Schedule 4B: Carinya Road residential controls | [06-schedule-4b-carinya-road-residential-controls.md](06-schedule-4b-carinya-road-residential-controls.md) | ✅ converted |
| 6 — Schedule 4C: Carinya Road subdivision controls | [06-schedule-4c-carinya-road-subdivision-controls.md](06-schedule-4c-carinya-road-subdivision-controls.md) | ✅ converted |
| 6 — Schedule 5: Stormwater catchments | [06-schedule-5-stormwater-catchments.md](06-schedule-5-stormwater-catchments.md) | ✅ converted — ⚠️ matrix needs visual verification |
| 7 — Explanatory notes on lodging applications | [07-explanatory-notes-lodging-applications.md](07-explanatory-notes-lodging-applications.md) | ✅ converted |
| 8 — Definitions | [08-definitions.md](08-definitions.md) | ✅ converted — ⚠️ contains a duplicate definition preserved verbatim |
| 9 — Flood risk management in the former Canterbury LGA | [09-flood-risk-management-former-canterbury-lga.md](09-flood-risk-management-former-canterbury-lga.md) | ✅ converted |
| 10 — Flood risk management | [10-flood-risk-management.md](10-flood-risk-management.md) | ✅ converted |
| Appendices (maps/figures index) | [appendices/_index.md](appendices/_index.md) | ✅ tracked, images not yet converted |

## Other flags

- **Amendment date precision:** source cover page reads "June 2023 (Amended April 2025)" — no day-level date given, so `amended_date` is recorded at month precision (2025-04-01).
- **Duplicate definition** in Section 8: "high hazard flood fringe areas" is defined twice with different wording — preserved verbatim, not merged.
- **Three colour-coded planning matrices** (Schedules 3, 4A, 5) were extracted as flattened text; column alignment should be visually re-checked against the source PDF before being used for a determination — see the ⚠️ notes in those files.
- **Schedule 4C, Note 1** flags a Council/Lands Department negotiation over "Reserve Road" access status that reads as unresolved/in-progress in the source text — worth confirming current status.
