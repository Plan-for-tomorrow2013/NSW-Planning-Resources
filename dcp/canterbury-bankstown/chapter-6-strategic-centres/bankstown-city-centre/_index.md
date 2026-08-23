---
title: "Canterbury-Bankstown DCP 2023 — Chapter 6.2 Bankstown City Centre — Index"
council: Canterbury-Bankstown
document_type: DCP
chapter: "6.2"
last_verified: 2026-08-23
---

## Chapter 6.2 — Strategic Centres: Bankstown City Centre

Cover page reads "May 2025, Final Version" (differs from the "AMENDMENT 8... August 2025" framing on the source filename supplied for conversion — see note below). Centre-specific sub-chapter, applies only to the Bankstown City Centre precinct — parallel to Chapter 6.3 (Campsie Town Centre). 221 pages across 6 top-level Sections, a "Part 5" of General Provisions, a Key Sites section, and an Appendix.

**Status: done.** All 7 top-level divisions converted.

| Top-level division | Folder/File | Status |
|---|---|---|
| Section 1 — Introduction | [section-1-introduction/](section-1-introduction/_index.md) | done (1.1–1.3, 3 of 3) |
| Section 2 — Understanding Place | [section-2-understanding-place/](section-2-understanding-place/_index.md) | done (2.1.1–2.1.9 + 2.2, 10 of 10) |
| Section 3 — Designing the Public Domain | [section-3-designing-public-domain/](section-3-designing-public-domain/_index.md) | done (3.1.1–3.1.3, 3.2, 3.3, 3.4.1, 3.4.2, 3.5 — 8 of 8) |
| Section 4 — Built Form | [section-4-built-form/](section-4-built-form/_index.md) | done (4.1.1, 4.2.1–4.2.6 + upper storey setbacks anomaly, 4.3, 4.4, 4.5.1–4.5.3, 4.6, 4.7, 4.8 — 16 files, all 14 numbered subsections) |
| Part 5 — General Provisions | [part-5-general-provisions.md](part-5-general-provisions.md) | done (5.1–5.13, 13 of 13 subsections, kept as a single flat file) |
| Section 6 — Key Sites | [section-6-key-sites/](section-6-key-sites/_index.md) | done (KS1–KS8 as flat files, KS9 Bankstown Central as its own 8-file subfolder — 9 of 9 key sites) |
| Appendix 1 | [appendix-1-definitions-figures.md](appendix-1-definitions-figures.md) | done (A1.1 Definitions + A1.2 full 97-entry Figures list, kept as a single flat file) |

## Notes

- **Date discrepancy**: the uploaded source file is named "...AMENDMENT_8...August_2025..." but the document's own cover page reads "May 2025, Final Version" with no "Amended" qualifier printed anywhere in the pages converted. Unlike 6.1 (which explicitly prints "Amended August 2025" on its own cover) and 6.3 ("Amended April 2025"), 6.2's cover page does not show an amendment date in the same format. Flagged rather than assumed — this may mean 6.2's "Amendment 8" filename refers to the LEP/DCP-wide amendment tranche rather than a chapter-specific amendment note, but that's not stated in the source text seen so far.
- **Three-tier structure**: 6.2 uses Objectives, Principles, *and* Controls (see [1.3](section-1-introduction/03-how-to-read-this-dcp.md)) — unlike 6.1 and 6.3, which use only Objectives and Controls. In practice not every subsection uses all three tiers — the eight Character Area subsections (2.1.2–2.1.9) use only Character statement + Principles, 2.2 (Connecting with Country) uses Objectives + a "Design Guidance" (G-numbered) tier instead of Controls, and Section 6's Key Sites (KS1–KS8) use unlettered "Design principles" only, without separate Objectives/Controls tiers. See each section's own `_index.md` for details.
- **Numbering resets**: within Section 4 (Built Form) and Section 6.9 (KS9 Bankstown Central) especially, Controls are numbered C1, C2... independently *within each numbered sub-topic* rather than running continuously through the whole top-level Section, unlike 6.1/6.3 where clause numbers ran continuously through each section. `clause_range` front matter for 6.2 files is therefore scoped to the specific sub-topic, not the whole Section.
- **Precedence**: per [1.1](section-1-introduction/01-application-of-this-dcp.md), this chapter's controls prevail over other DCP chapters (including 6.1) where inconsistent, for development in the Bankstown City Centre — same pattern as 6.3 for Campsie. Section 6.9 (KS9 Bankstown Central) further prevails over the rest of Chapter 6.2 where inconsistent, for development of the Bankstown Central site specifically.
- **Duplicated-controls pattern (systematic, not isolated)**: verbatim-duplicated control blocks under new numbers appeared twice in Section 3/4 — [3.1.3](section-3-designing-public-domain/03-laneways-shared-zones-service-lanes.md) C10–C12 duplicate C7–C9, and [4.2.5](section-4-built-form/07-building-separation-distance.md) C9–C12 duplicate C5–C8. Worth raising with Council as a possible document-wide export/drafting issue.
- **4.2.4 printed twice**: Ground Level Setbacks and Upper Storey Setbacks are both labelled "4.2.4" in the source. See [Section 4 index](section-4-built-form/_index.md) for detail.
- **Duplicate "6.9.7" numbering in KS9**: the source labels both the Controls under 6.9.6 Signage strategy/public art, and the separate Staging and implementation sub-section, as "6.9.7" — see [section-6-key-sites/ks9-bankstown-central/07-signage-public-art.md](section-6-key-sites/ks9-bankstown-central/07-signage-public-art.md).
- **KS2/KS3 street-name and address discrepancies**: "Richard Road" vs "Rickard Road" (KS2), "67-70" vs "67-69" Rickard Road (KS3) — see [section-6-key-sites/00-overview.md](section-6-key-sites/00-overview.md).
- **Page 181 text corruption**: KS7's design principles f–j had a garbled text layer in the source PDF and were transcribed from a rasterised page image — see [section-6-key-sites/07-ks7-8-14-west-terrace.md](section-6-key-sites/07-ks7-8-14-west-terrace.md).
- **"CWCF" acronym flag**: raised in [2.2 Connecting with Country](section-2-understanding-place/10-connecting-with-country.md), checked against Appendix 1 Definitions — **not resolved**, the term does not appear in A1.1. See [appendix-1-definitions-figures.md](appendix-1-definitions-figures.md) note.
- **Un-digitised lot-level and structure maps**: several Section 4 figures (33, 37, 40, 42) and several KS9 figures (81, 82, 83, 89–91, 96) assign specific controls to specific lots/precincts on maps that couldn't be reliably extracted as text — flagged as the top priority for image conversion across this chapter, since they're the figures most likely to be queried directly by address or precinct.

## Chapter-wide next step

With Chapter 6.2 now fully converted, remaining work in Chapter 6 (Strategic Centres) is done — 6.1, 6.2 and 6.3 are all complete. Update the Chapter 6 index and the top-level council index to reflect this (see conversion guide: "bump the chapter-level and top-level council index status lines").
