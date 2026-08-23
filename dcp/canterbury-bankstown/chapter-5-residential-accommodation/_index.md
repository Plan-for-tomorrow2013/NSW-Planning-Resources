---
title: "Chapter 5 — Residential Accommodation"
council: Canterbury-Bankstown
document_type: DCP
chapter: "5"
amended_date: 2026-03-12
last_verified: 2026-08-19
tags: [residential]
---

# Chapter 5 — Residential Accommodation

Canterbury-Bankstown DCP 2023, Chapter 5, sets design controls for residential accommodation
across the LGA. **This chapter is split by former LGA** — each side is a separate
pre-amalgamation council's own DCP grafted into the merged document, and **each retains its
own native clause-numbering style**:

| Sub-chapter | Former LGA | Numbering style | Status |
|---|---|---|---|
| [5.1](former-bankstown-lga/_index.md) | Bankstown | One Objectives list per section (O1–O8), then continuous clause numbers (e.g. 2.1–2.29) grouped under descriptive subheadings. No "C" labels. | done |
| [5.2](former-canterbury-lga/_index.md) | Canterbury | Objectives and controls restart their own `O1, O2…` / `C1, C2…` sequence at every numbered sub-clause (e.g. 2.1, 2.2, 2.3…). | done (10 of 10 sections) |

**Do not force these two sub-chapters to look the same.** Reconciling their structure would
mean silently renumbering clauses relative to the source PDFs, breaking citation back to
Council. If a reader finds the difference confusing, that's a genuine quirk of how Council
merged two legacy DCPs — noted here and in each sub-chapter's own `_index.md`, not smoothed
over.

## 5.2 (former Canterbury LGA) — known PDF defect and reconstruction status

This source PDF (`2026_03_12_-_DCP_2023_-_AMENDMENT_11_-_Chapter_5_2_-_Former_Canterbury_LGA_pdf.pdf`)
drops many of its "O1, O2…" and "C1, C2…" list labels from the text layer while still
rendering them visually on the page — confirmed by checking the PDF's actual text layer
(via `page.get_text("words")` in PyMuPDF) against rendered page images, not just by
re-running text extraction. Where every checked instance in the document is strictly
sequential with no gaps, missing labels have been reconstructed and flagged
`[RECONSTRUCTED-LABEL]` inline in the affected section files. **A number of these blocks
have not yet been individually spot-checked against the source PDF** — see
`former-canterbury-lga/_index.md` for the full section-by-section verification table and
list of separately-flagged source anomalies (duplicated clauses, inconsistent numeric
thresholds between sections, etc.) found during conversion.
