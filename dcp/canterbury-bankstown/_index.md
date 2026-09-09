---
title: "Canterbury-Bankstown DCP 2023 — Chapter Index"
council: Canterbury-Bankstown
document_type: DCP
last_verified: 2026-09-09
---

## Canterbury-Bankstown DCP 2023

Folder structure mirrors Council's own DCP table of contents. Status reflects conversion into this repo, not the currency of the source document itself.

| Chapter | Folder | Status |
|---|---|---|
| 1 — Introduction | [chapter-1-introduction/](chapter-1-introduction/_index.md) | converted (1 of 1 supplied sub-chapter — 1.1; unconfirmed whether further sub-chapters 1.2+ exist, see chapter notes) |
| 2 — Site Considerations | [chapter-2-site-considerations/](chapter-2-site-considerations/_index.md) | converted (4 of 4 sub-chapters; source-set completeness still to be verified) |
| 3 — General Requirements | [chapter-3-general-requirements/](chapter-3-general-requirements/_index.md) | done (7 of 7 sub-chapters) |
| 4 — Heritage | [chapter-4-heritage/](chapter-4-heritage/_index.md) | done (4 of 4 sub-chapters) |
| 5 — Residential Accommodation | [chapter-5-residential-accommodation/](chapter-5-residential-accommodation/_index.md) | done (former Bankstown LGA + former Canterbury LGA both complete — see chapter notes for reconstructed-label spot-checks still needed) |
| 6 — Strategic Centres | [chapter-6-strategic-centres/](chapter-6-strategic-centres/_index.md) | done (6.1, 6.2 Bankstown City Centre, and 6.3 Campsie Town Centre complete) |
| 7 — Commercial Centres | [chapter-7-commercial-centres/](chapter-7-commercial-centres/_index.md) | **DONE — 7 of 7 sub-chapters complete** |
| 8 — Employment Lands | [chapter-8-employment-lands/](chapter-8-employment-lands/_index.md) | **DONE — 3 of 3 sub-chapters complete** |
| 9 — Industrial Precincts | [chapter-9-industrial-precincts/](chapter-9-industrial-precincts/_index.md) | converted (1 of 1 supplied sub-chapter — 9.1; unconfirmed whether further sub-chapters 9.2+ exist, see chapter notes) |
| 10 — Other Development | [chapter-10-other-development/](chapter-10-other-development/_index.md) | **DONE — 8 of 8 sub-chapters complete** |
| 11 — Key Development Sites | [chapter-11-key-development-sites/](chapter-11-key-development-sites/_index.md) | in progress (15 of 16 sub-chapters converted — 11.1 through 11.14 plus 11.16; only 11.15 not yet supplied; see chapter notes) |
| Supporting Guides | supporting-guides/ | not started |

### Notes
- **Chapter 1 (Introduction)** is now converted — 1.1 "Introduction and Administration" is council-wide (`general/` scope, not LGA-split), consistent with its "Land where this DCP applies" clause. Whether Chapter 1 has further sub-chapters (1.2, 1.3...) is still unconfirmed — nothing in the 1.1 source PDF lists further sub-chapters, but Council's own document navigation hasn't been separately checked. See `chapter-1-introduction/_index.md`. A discrepancy was also flagged between the "Amended March 2026" date on 1.1's cover/footers and the amendment table in its Section 3, which has no row naming Chapter 1.1 specifically — see `chapter-1-introduction/general/_index.md`.
- **Chapter 4 (Heritage)** is council-wide, not split by former LGA — all four sub-chapters (4.1–4.4) sit under `chapter-4-heritage/general/`. Chapter 4.3 has one Ashbury-HCA-specific section and one Hurlstone-Park-specific section internal to that single document; this is not a former-LGA folder split. Chapter 4.4 is a single-section sub-document kept as a flat file per the conversion guide, rather than its own folder. See `chapter-4-heritage/_index.md` for two follow-up documents needed (Heritage Guide; Heritage Conservation Area Character Statements) and each sub-chapter's own `_index.md` for source anomalies flagged during conversion (a duplicate clause label, an apparently incomplete clause, and minor cross-chapter wording differences).
- **Chapter 5** is the only chapter confirmed so far to split by former LGA. Don't assume other chapters split the same way — check each chapter's own "Application of this chapter" wording before deciding whether it needs an LGA-level subfolder. Chapter 3 was checked sub-chapter by sub-chapter during its conversion: only 3.4 (Sustainable Development) has an "Application of this chapter" section, and none of the seven Chapter 3 sub-chapters split by former LGA (see chapter-3-general-requirements/_index.md for the reasoning; Chapter 3.2 is confirmed by Chapter 11.10 to be titled "Parking" — see Chapter 11 notes below). Chapter 4 was likewise checked sub-chapter by sub-chapter and found not to split by former LGA. Chapters 7.5 and 7.6 were both checked and also do not split by former LGA — each defines its own single precinct/local-centre application area (Figure 1) with no LGA-based wording. Chapter 1.1 was checked the same way and applies council-wide. Chapter 8.1 was checked the same way and also applies council-wide, split internally by zone (E3/SP4) rather than by former LGA — see `chapter-8-employment-lands/_index.md`. All eight Chapter 10 sub-chapters (10.1–10.8) were checked the same way and also apply council-wide — see `chapter-10-other-development/_index.md`. **Chapter 11.1 through 11.10, plus 11.12, have all now been checked the same way** — none split by former LGA at all, since every Chapter 11 sub-chapter is a stand-alone, site-specific precinct rather than a topic applied broadly across the council; 11.4 and 11.6 do have internal splits, by zone and by development-type respectively, and 11.10 has an internal storey-height transition tied to the LEP's Height of Building Map, but none of these are former-LGA splits. See `chapter-11-key-development-sites/_index.md`.
- Folders for "not started" chapters are intentionally not created yet — create them only when there's a converted file to put in them, so an empty folder never implies work that hasn't happened.
- **Chapter 6 (Strategic Centres)** splits by **strategic centre**, not by former LGA. 6.1 (General Requirements) applies across both centres; 6.2 (Bankstown City Centre) and 6.3 (Campsie Town Centre) are centre-specific. All three sub-documents are converted. The 221-page 6.2 is structured as Sections 1—4, Part 5, Section 6 Key Sites, and Appendix 1; see its own `_index.md` for the full file map and source anomalies.
- **Chapter 7 (Commercial Centres) is now fully converted — 7 of 7 sub-chapters done.** It combines *four* different scope patterns in one chapter — see `chapter-7-commercial-centres/_index.md` for the full breakdown: 7.1 (General Requirements) is council-wide across all of Chapter 7 (like 6.1); 7.4 (Neighbourhood Centres) is council-wide but scoped to 'Area 1' land only; 7.2 (City West) and 7.3 (City East) split by geographic grouping with one boilerplate section per named centre; and 7.5/7.6/7.7 (Canterbury Local Centre / Belmore and Lakemba Precinct / Punchbowl and Wiley Park) are newer, much more detailed standalone "precinct DCP" chapters (Understanding Place, Public Domain Design, Building Design, General Provisions, Key Sites, Appendices, ~120–142 pages and 40–55 files each) that explicitly supersede older centre sections previously inside 7.3, each via its own clause-1.1 precedence wording. A cross-chapter reconciliation pass is recommended (not yet done) covering three patterns that turned up **independently in more than one of the precinct-DCP chapters**, suggesting shared drafting-template issues rather than isolated errors: (1) an amendment-date discrepancy between title page and filename, confirmed in both 7.6 and 7.7 but not 7.5; (2) a B2/E1 zone-name mismatch, confirmed in both 7.5 and 7.6, **and also found in Chapter 11.4**; (3) verbatim-duplicated controls between the water-efficiency and energy-efficiency sustainability sub-sections, confirmed in both 7.5 and 7.6, in the same two sub-sections (5.4.3/5.4.4) in each. Full anomaly lists are in `chapter-7-commercial-centres/_index.md` and each sub-chapter's own `_index.md`. One outstanding filename fix remains in 7.5 (`06-connecting-to-country.md` needs renaming to `10-connecting-to-country.md`) that couldn't be actioned without that file's actual content — see `chapter-7-commercial-centres/canterbury-local-centre/_index.md`. **This precedence-clause pattern recurs again in Chapter 11 — now confirmed in all eight converted sub-chapters, 11.1 through 11.8 — see below.**
- **Chapter 8 (Employment Lands) is now fully converted — 3 of 3 sub-chapters done.** All
  three sub-documents (8.1 General Requirements, 8.2 Canterbury Road Enterprise Corridor,
  8.3 Hume Highway Enterprise Corridor) were individually checked and confirmed
  council-wide (no former-LGA split), so all three sit under `chapter-8-employment-lands/general/`
  like Chapter 4 — 8.1 splits internally by zone (E3/SP4), while 8.2 and 8.3 are each
  scoped to a specific named road corridor rather than a former LGA. 8.1's own
  objectives/clauses (O4, O7, 2.7) refer to "the enterprise corridors," which reads like
  boilerplate — 8.2 and 8.3 are literally about enterprise *corridors*, so this is worth
  checking during a future cross-chapter reconciliation pass alongside the existing Chapter
  7 precinct-DCP wording issues. 8.2's development-control numbering restarts at "C1"
  within every numbered subsection rather than running sequentially (cite with the
  subsection, e.g. "5.3 C1"); 8.3's Section 6 (167 Hume Highway) follows the same pattern
  and is a large, structurally distinct site-specific mini-DCP closer in style to Chapter 7's
  newer precinct DCPs (7.5/7.6/7.7) and to Chapter 11 than to the rest of 8.3; it was
  split into its own subfolder with one file per numbered subsection (6.1–6.15). A
  few source typos were preserved and flagged inline rather than silently corrected (8.2
  clause 5.2 C10 "will not be support"; 8.2 clause 6.1 C4 "sites were a laneway"; 8.3 clause
  8.5's duplicated "from the from the"). See `chapter-8-employment-lands/_index.md` for the
  full breakdown.
- **Chapter 9 (Industrial Precincts)** has its first sub-chapter converted — **9.1 (General
  Requirements)**, checked the same way as the chapters above and confirmed council-wide
  (Zone E4 General Industrial), so it sits under `chapter-9-industrial-precincts/general/`
  like Chapters 4 and 8. Unlike Chapter 8.1's internal zone split, 9.1 has an internal
  **former-LGA** split limited to a single clause pair (2.2 former Bankstown / 2.3 former
  Canterbury street setbacks) — everything else in 9.1 is uniform. Two anomalies were
  flagged rather than resolved: a Table-of-Contents heading that doesn't match the printed
  in-document section heading for Section 2, and an unconverted figure (Figure 3a, a
  photograph of architectural elements — its text callout legend was preserved, the image
  was not). Appendix 1 (a state/regional-roads table for the former Bankstown LGA) was
  fully converted as a markdown table. Whether Chapter 9 has further sub-chapters (9.2,
  9.3, …) is unconfirmed — see `chapter-9-industrial-precincts/_index.md`.
- **Chapter 10 (Other Development) is now fully converted — 8 of 8 sub-chapters done**:
  **10.1** (Centre-Based Child Care Facilities), **10.2** (Schools), **10.3** (Home
  Businesses and Home Industries), **10.4** (Non-Residential Land Uses in Residential
  Zones), **10.5** (Places of Public Worship), **10.6** (Commercial Land Uses), **10.7**
  (Sex Services Premises), and **10.8** (Telecommunications Facilities). All eight sit
  under `chapter-10-other-development/general/` — 10.3 is a flat file (single section);
  10.4 has an internal former-LGA setback split (Section 4); 10.5 has a self-referencing
  clause anomaly, two unconverted diagrams, and an Appendix 1 scoped to the former
  Bankstown LGA despite the sub-chapter otherwise being council-wide; 10.7 has its own
  overlapping state-roads table; 10.2 and 10.5 both cite a "Chapter 3.3" cross-reference
  that doesn't match this repo's actual Chapter 3 structure (the same stray-cross-reference
  pattern now also seen in Chapter 11.4's "section F10.10" citation; Chapter 11.8's
  citation of Chapter 3.2 has since been confirmed correct — see the Chapter 11 note
  below — but its citation of Chapter 3.7 remains unverified);
  10.6/10.7 carry a different amendment date to the rest of the chapter (echoed by Chapter
  11.10 carrying a different amendment date to the rest of Chapter 11 — see below). See
  `chapter-10-other-development/_index.md` for the full breakdown and recommended
  cross-chapter reconciliation follow-ups.
- **Chapter 11 (Key Development Sites)** now has **eleven of sixteen** sub-chapters
  converted — **11.1** (149–171 Milton Street, Ashbury), **11.2** (Undercliffe Bridge
  Precinct, Earlwood), **11.3** (52–60 Roberts Road, Greenacre), **11.4** (Croydon
  Street Precinct, Lakemba), **11.5** (Former Riverlands Golf Course Site, Milperra),
  **11.6** (Former Potts Hill Reservoirs Site, Potts Hill), **11.7** (30–46 Auburn Road,
  Regents Park), **11.8** (20–21 Boorea Avenue, Lakemba), **11.9** (297–299 Canterbury
  Road, Revesby — a hospital), **11.10** (Chullora Marketplace, Greenacre) and **11.12**
  (445 Canterbury Road, Campsie — a hospital; **converted ahead of 11.11**, which
  remains not yet supplied). Each sub-chapter is a stand-alone, site-specific mini-DCP
  for one named site, structurally closer to Chapter 7's newer precinct DCPs (7.5–7.7)
  and Chapter 8.3 Section 6 than to the topic-based Chapters 1–10, and each carries its
  own precedence clause (controls prevail over other DCP controls where inconsistent,
  for applications on that site). None split by former LGA — 11.4 splits internally by
  **zone**, 11.6 splits internally by **development type** (per its own Land
  Application Map), and 11.10 has an internal storey-height transition tied to the
  LEP's Height of Building Map, but none of these are former-LGA splits. 11.2, 11.3,
  11.5, 11.7 and 11.8 are single-section flat files; 11.1 (17 sections), 11.4 (8
  sections), 11.6 (5 sections), 11.9 (6 sections), 11.10 (10 sections) and **11.12 (13
  sections)** each have their own subfolder with one file per section, per the
  conversion guide's 2+ section rule — 11.12 is now the **second-largest** Chapter 11
  sub-chapter by section count after 11.1. Several cross-chapter anomaly patterns
  already flagged for Chapter 7's precinct DCPs and Chapter 10 have recurred inside
  Chapter 11: a B2/E1 zone-name mismatch (11.4, matching 7.5/7.6), the general
  precedence-clause drafting pattern (all eleven Chapter 11 sub-chapters so far, with
  11.1 and 11.9 each also carrying a second, narrower precedence-type statement), a
  differing amendment date within the chapter (11.10 and **11.12** both read "Amended
  April 2025" versus 11.1–11.9's "Amended August 2024," matching the pattern already
  seen in 10.6/10.7), and a self-referencing clause number (11.10's clause 5.10,
  matching the pattern already seen in 10.5). **11.10 and 11.12 also share a naming
  inconsistency not found elsewhere in this DCP** — both mis-name the *State
  Environmental Planning Policy (Housing) 2021* as "State Environment Planning Policy"
  (missing "-al") — which, combined with their shared amendment date, suggests these two
  sub-chapters share a common drafting template distinct from 11.1–11.9. **11.5 is
  flagged as a possible incomplete supply** — four of its nine objectives (heritage,
  flood/contamination/bushfire, access, infrastructure) have no standalone numbered
  development control in the pages received, unlike every other Chapter 11 sub-chapter
  converted to date; worth confirming against Council's source before treating it as
  final. **11.6 introduces a structural anomaly**: its Sections 2–5 use unnumbered,
  sub-headed development controls rather than the sequential clause numbering (1.1, 1.2…)
  used by every other converted Chapter 11 sub-chapter, and its Land Application Map's own
  internal "Section" legend numbering doesn't align with the document's actual Section 1–5
  headings. **11.8 cited Chapter 3.2 and Chapter 3.7 of this DCP** for parking/traffic and
  landscaping controls respectively; **the Chapter 3.2 citation is now confirmed correct**
  — both 11.9 (clause 5.7) and 11.10 (clause 3.12, which explicitly names it "Chapter 3.2
  Parking") independently cite the same chapter for the same subject matter — **but
  Chapter 3.7 remains unverified**. **11.9 and 11.12 both restrict their own
  applicability to hospital development only** ("For other development types, the other
  parts/chapters of the DCP apply"), now a confirmed pattern for hospital sites
  specifically, and both require State Design Review Panel referral (11.9) or a Public
  Art Strategy informed by the Government Architect NSW's Connecting with Country
  framework (11.12). **11.12 additionally introduces a site-consolidation precondition**
  (six separate lots must be consolidated into one before redevelopment) not seen in any
  other Chapter 11 sub-chapter, and carries five likely source typos preserved verbatim.
  **11.10 introduces a staged/progressive-development mechanism** (an indicative concept
  plan covering the whole site) not seen elsewhere in Chapter 11, and carries the
  chapter's most detailed heritage controls (the site is a listed archaeological site of
  state heritage significance — the former Liebentritt's Pottery and Chullora Drive-in).
  **Update as of 11.16 (1 Leicester Street, Chester Hill — "Chester Square"): fifteen of
  sixteen sub-chapters are now converted (all of 11.1–11.14, plus 11.16); only 11.15
  (Marco Avenue) remains not yet supplied.** 11.16 introduces its own new anomalies —
  no zone code stated anywhere in its own text (unlike every other Chapter 11
  sub-chapter), a cover date ("March 2026") with no day and no relationship to a 2023
  base version, a new "Design Guidance G#" main-hierarchy label (distinct from 11.13's
  appendix-only use of "G#"), and two directly-checkable cross-references to the
  already-converted Chapters 5.1 and 6.2. This top-level paragraph is a summary only and
  was not kept fully in sync with every sub-chapter added after 11.12 — see
  `chapter-11-key-development-sites/_index.md` and, for full current detail,
  `chapter-11-key-development-sites/general/_index.md` for the authoritative site list,
  file map, and anomaly/citation/dating notes.
