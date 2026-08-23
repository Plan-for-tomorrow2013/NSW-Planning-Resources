---
title: "Canterbury-Bankstown DCP 2023 — Chapter 6.1 General Requirements — Index"
council: Canterbury-Bankstown
document_type: DCP
chapter: "6.1"
last_verified: 2026-08-22
---

## Chapter 6.1 — Strategic Centres: General Requirements

June 2023 (Amended August 2025). Applies generally across both strategic centres (Bankstown and Campsie) — see Section 1's explanation, which frames the whole sub-chapter around *Connective City 2036*'s two strategic centres without any LGA or centre-specific split. Kept as `general/` per the same pattern used for Chapter 4 (Heritage).

| Section | File | Status |
|---|---|---|
| 1 — Introduction | [01-introduction.md](01-introduction.md) | done |
| 2 — Active street frontages | [02-active-street-frontages.md](02-active-street-frontages.md) | done |
| 3 — Facade design | [03-facade-design.md](03-facade-design.md) | done |
| 4 — Corner buildings | [04-corner-buildings.md](04-corner-buildings.md) | done |
| 5 — Roof design | [05-roof-design.md](05-roof-design.md) | done |
| 6 — Materials and finishes | [06-materials-and-finishes.md](06-materials-and-finishes.md) | done |
| 7 — Awning design | [07-awning-design.md](07-awning-design.md) | done |
| 8 — General design and amenity | [08-general-design-and-amenity.md](08-general-design-and-amenity.md) | done |

### Notes

- **Source date**: the cover page reads "June 2023 (Amended August 2025)" — only month/year given, no exact day, so `effective_date`/`amended_date` front-matter fields were omitted from all section files per the conversion guide's "omit rather than guess" rule. The source date line is noted as plain text at the top of each file instead.
- **Section 5 heading discrepancy**: the source's own table of contents lists "Section 5 – Roof design" (singular) but the section heading on the page itself reads "SECTION 5–ROOF DESIGNS" (plural). Flagged in `05-roof-design.md`, not silently normalised.
- **Clause 5.6 formatting anomaly**: two unnumbered paragraphs of explanatory/definitional text sit directly under clause 5.6 with no clause number of their own — inconsistent with the rest of the section's numbering pattern. Flagged in `05-roof-design.md` rather than assigning them a clause number that isn't in the source.
- **Figure 7b caption inconsistency**: caption states awnings should cover "up to 40-50% of secondary built frontage," while clause 7.2's operative text sets a 40% *minimum*. Flagged in `07-awning-design.md`.
- **Figures**: all figures referenced in these sections (1a, 2a, 3a, 3b, 4a–4c, 7a, 7b) are noted inline and logged in the chapter-level [`appendices/_index.md`](../appendices/_index.md) — none have been converted to image assets yet.
- **Zones**: only Section 8 (clause 8.19) names explicit zone codes (R2, R3, R4) in the source text. No other section in this sub-chapter names a zone code, so `zones` front matter was omitted elsewhere rather than inferred from context (e.g. E1, which appears in Chapter 6.3 but not in 6.1's own text).
