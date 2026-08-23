---
title: "Chapter 7 — Commercial Centres"
council: Canterbury-Bankstown
document_type: DCP
chapter: "7"
last_verified: 2026-08-23
tags: [commercial-centres, chapter-index]
---

## Chapter 7 — Commercial Centres

Council's own Contents screenshot lists seven numbered sub-chapters:

| Sub-chapter | Folder | Status |
|---|---|---|
| 7.1 — General Requirements | [general/](general/_index.md) | **done** (9 of 9 sections) |
| 7.2 — City West (Bass Hill, Birrong, Chester Hill, Condell Park, East Hills, Georges Hall, Greenacre, Padstow, Panania, Revesby, Sefton, Yagoona) | [city-west/](city-west/_index.md) | not started (page map ready) |
| 7.3 — City East (Belfield, Canterbury, Croydon Park, Earlwood, Hurlstone Park, Narwee, Roselands) | [city-east/](city-east/_index.md) | **done** (9 of 9 currently-content-bearing sections — see anomalies) |
| 7.4 — Neighbourhood Centres | [neighbourhood-centres/](neighbourhood-centres/_index.md) | **done** (3 of 3 sections) |
| 7.5 — Canterbury Local Centre | [canterbury-local-centre/](canterbury-local-centre/_index.md) | not started (page map ready) |
| 7.6 — Belmore and Lakemba | [belmore-and-lakemba/](belmore-and-lakemba/_index.md) | not started (page map ready) |
| 7.7 — Punchbowl and Wiley Park | [punchbowl-and-wiley-park/](punchbowl-and-wiley-park/_index.md) | not started (page map ready) |

**Overall chapter status: in progress — 3 of 7 sub-chapters fully converted (7.1, 7.3, 7.4); 4 of 7 scaffolded with page maps for resuming (7.2, 7.5, 7.6, 7.7).**

### How this chapter is structured (four distinct scope patterns in one chapter)

- **7.1 General Requirements** — council-wide design controls applying to *every* commercial centre in the chapter (active frontages, facades, bulk, corner buildings, roofs, materials, awnings, general amenity). Analogous to Chapter 6.1's role for Strategic Centres.
- **7.4 Neighbourhood Centres** — council-wide, but scoped specifically to centres identified as 'Area 1' on the Land Zoning Map (storey limits, setbacks) — a distinct policy layer from 7.1, not a duplicate of it.
- **7.2 City West / 7.3 City East** — split by geographic grouping (not former LGA), each containing one boilerplate section per named local/village/small-village centre (near-identical E1-zone setback controls, differing mainly in structure-plan figures and the occasional bespoke clause set, as seen with Roselands in 7.3).
- **7.5 Canterbury Local Centre / 7.6 Belmore and Lakemba / 7.7 Punchbowl and Wiley Park** — a newer, much more detailed "precinct DCP" template (Understanding Place, Public Domain Design, Building Design, General Provisions, Key Sites, Appendices) issued as standalone chapters between March–June 2026, each **explicitly superseding** the older brief centre sections that used to live inside 7.3 (Canterbury/Belmore/Lakemba/Punchbowl/Wiley Park), via each new chapter's own clause 1.1 precedence wording ("this chapter prevails ... except in respect of Chapter 4 Heritage").

### Cross-chapter notes and anomalies (see each sub-chapter's own `_index.md` for full detail)

- **7.3's Contents page is only partly up to date.** It correctly flags Belmore, Lakemba, Punchbowl and Wiley Park as "(Replaced by Chapter 7.6)" / "(Replaced by Chapter 7.7)", with those sections' body content actually removed from the PDF — but it does **not** flag Section 4 (Canterbury Local Centre) as replaced, even though standalone Chapter 7.5 (issued *before* 7.3's most recent amendment) governs Canterbury by its own precedence clause. Section 4's stale content is still fully printed in 7.3 and has been converted as-is, with a prominent pointer to Chapter 7.5. See `city-east/_index.md`.
- **7.3's own Section 1 introduction is stale too** — it still names Belmore, Lakemba, Punchbowl and Wiley Park as centres "the centres in" 7.3 covers, despite those sections having been removed.
- **Two amendment-date discrepancies spotted (not yet resolved) in 7.6 and 7.7**: each chapter's title page reads "March 2026 Final", but the source filenames indicate later amendment dates (7.6: June 2026, Amendment 13; 7.7: April 2026, Amendment 14). Flagged in each sub-chapter's `_index.md`; confirm the correct `amended_date` front-matter value when those sub-chapters are actually converted.
- **7.2 City West has not been checked for the same kind of supersession** that happened to Belmore/Lakemba/Canterbury/Punchbowl/Wiley Park in 7.3 — none of its 12 centres carry a "(Replaced by...)" notice on its Contents page as of the source PDF read for this pass, but that should be re-confirmed if a City West sub-chapter conversion is picked up later, in case a similar standalone chapter has since been issued for one of those centres too.

### Recommended order for resuming

1. **7.2 City West** — smallest of the four not-started items (108pp) and structurally identical to the already-converted 7.3, so fastest to finish and gets the "old template" fully covered.
2. **7.5 Canterbury Local Centre** — highest practical value, since it's the currently-governing document for a centre this repo already has (superseded) content for.
3. **7.6 Belmore and Lakemba**, then **7.7 Punchbowl and Wiley Park** — same "precinct DCP" template as 7.5, convert once that template's section-splitting approach is proven out on 7.5.
