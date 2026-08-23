---
title: "Chapter 7.3 — City East"
council: Canterbury-Bankstown
document_type: DCP
chapter: "7.3"
effective_date: 2023-06-01
amended_date: 2026-04-24
last_verified: 2026-08-23
tags: [city-east, belfield, canterbury, croydon-park, earlwood, hurlstone-park, narwee, roselands]
---

## Chapter 7.3 — City East

Covers seven currently-active local/village/small-village centres in the eastern part of the LGA: Belfield, Canterbury, Croydon Park, Earlwood, Hurlstone Park, Narwee and Roselands, plus a chapter-wide Section 13 (Lanes). This is a **scope split by named centre within a geographic grouping** ("City East"), not a former-LGA split — a third pattern for this repo, alongside Chapter 5's former-LGA split and Chapter 6's strategic-centre split. Chapter 7.2 (City West) follows the same "geographic grouping, one section per centre" pattern for the western centres — see its own `_index.md` once converted.

Status: **done (9 of 9 currently-content-bearing sections)** — see anomalies below regarding four sections with no content in the source, and one further live conflict.

| Section | File | Summary |
|---|---|---|
| 1 — Introduction | [01-introduction.md](01-introduction.md) | Centres hierarchy, objectives O1–O6; flags a stale reference to Belmore/Lakemba/Punchbowl/Wiley Park |
| 2 — Belfield Small Village Centre | [02-belfield-small-village-centre.md](02-belfield-small-village-centre.md) | Structure plan, E1 front/side/rear setbacks, 18m min frontage |
| ~~3 — Belmore Local Centre~~ | *not present in source — see anomalies* | Replaced by Chapter 7.6 |
| 4 — Canterbury Local Centre | [04-canterbury-local-centre.md](04-canterbury-local-centre.md) | Riverfront precinct, 1,500m² min lot, Market Lane, public domain figures — **see conflict note below** |
| 5 — Croydon Park Small Village Centre | [05-croydon-park-small-village-centre.md](05-croydon-park-small-village-centre.md) | Structure plan, standard E1 setbacks |
| 6 — Earlwood Local Centre | [06-earlwood-local-centre.md](06-earlwood-local-centre.md) | Structure plan, standard E1 setbacks |
| 7 — Hurlstone Park Small Village Centre | [07-hurlstone-park-small-village-centre.md](07-hurlstone-park-small-village-centre.md) | Structure plan, heritage deferral to Chapter 4, standard E1 setbacks |
| ~~8 — Lakemba Local Centre~~ | *not present in source — see anomalies* | Replaced by Chapter 7.6 |
| 9 — Narwee Village Centre | [09-narwee-village-centre.md](09-narwee-village-centre.md) | Structure plan, standard E1 setbacks |
| ~~10 — Punchbowl Village Centre~~ | *not present in source — see anomalies* | Replaced by Chapter 7.7 |
| 11 — Roselands Village Centre | [11-roselands-village-centre.md](11-roselands-village-centre.md) | Structure plan, car park height/setback, traffic and access controls, standard E1 setbacks |
| ~~12 — Wiley Park Village Centre~~ | *not present in source — see anomalies* | Replaced by Chapter 7.7 |
| 13 — Lanes | [13-lanes.md](13-lanes.md) | 6m lane reservation, subdivision/dedication, developer contribution |

### Source anomalies / notes

- **Sections 3, 8, 10, 12 (Belmore, Lakemba, Punchbowl, Wiley Park) contain no content.** The Contents page marks them "(Replaced by Chapter 7.6)" / "(Replaced by Chapter 7.7)" and the PDF body skips straight from Section 2 to Section 4, and has no Sections 8, 10 or 12 at all. No stub files were created for these — see `chapter-7-commercial-centres/belmore-and-lakemba/` and `chapter-7-commercial-centres/punchbowl-and-wiley-park/` (7.6 and 7.7) instead.
- **Section 1's explanatory text was not updated to match**: it still lists Belmore, Lakemba, Punchbowl and Wiley Park as centres "the centres in" this chapter covers, even though those sections have been removed and replaced by standalone chapters. Flagged in `01-introduction.md` rather than silently dropped.
- **Section 4 (Canterbury Local Centre) is superseded by standalone Chapter 7.5 — resolved via 7.5's own precedence clause, but 7.3's Contents page is stale.** A full standalone chapter, **Chapter 7.5 Canterbury Local Centre** (122 pages: Introduction, Understanding Place, Designing the Public Domain, Building Design, General Provisions, Key Sites, Appendices — structurally similar in scope/ambition to Chapter 6.2 Bankstown City Centre), was issued via **Amendment 12 (dated March 2026)**. Chapter 7.3 was itself re-amended after that — **Amendment 14 (dated April 2026)** — and in that later amendment, Section 4's brief ~5-page Canterbury content is still fully present, with no "(Replaced by Chapter 7.5)" notice on the Contents page (unlike the other four superseded sections, which do carry that notice). Read in isolation this looks like an unresolved duplicate. **It isn't**: Chapter 7.5 clause 1.1 ("Application of this Chapter") states in terms — *"Where there is an inconsistency between the controls in this Chapter and other Chapters in the CBDCP 2023 in relation to development in the Local Centre, this chapter prevails to the extent of the inconsistency except in respect of Chapter 4 Heritage."* So **Chapter 7.5 governs Canterbury Local Centre land wherever it conflicts with this Section 4**, by the source's own precedence rule — Council simply never updated 7.3's Contents page/explanatory text to add the "(Replaced by Chapter 7.6)"-style notice that Belmore/Lakemba/Punchbowl/Wiley Park received. `04-canterbury-local-centre.md` has been converted as printed (it's still live text in the current 7.3 PDF and may still apply to any edge-of-precinct land not covered by 7.5's Figure 1 application map), with a pointer to this resolution at the top of the file.
- No duplicate clause numbers spotted within the sections that were converted. Clause numbering restarts per section (e.g. 2.1–2.13, 4.1–4.15, 5.1–5.13) and is otherwise sequential and consistent with the equivalent sections in 7.2/7.4/7.6/7.7 boilerplate.
- Figures 1a, 2a–2c, 4a–4f, 5a–5c, 6a–6c, 7a–7c, 9a–9c, 11a–11c, 13a–13c are referenced but not yet converted to image assets — logged individually in each section file.
