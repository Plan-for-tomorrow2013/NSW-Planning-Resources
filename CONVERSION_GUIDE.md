# NSW Planning Resources — Conversion Guide

This is the standard for converting source planning documents (LEPs, DCPs, SEPPs, codes)
into the markdown structure used in this repo. Follow this exactly so every document —
regardless of which council or session converted it — ends up queryable the same way.

## Top-level council index

Every council folder (e.g. `dcp/canterbury-bankstown/`) gets its own `_index.md` that
mirrors the council's own published chapter list exactly — same chapter numbers, same
chapter titles, same order. Get this list from the DCP's table of contents (usually visible
in Council's document navigation or the front matter of any chapter PDF) rather than
inferring it from whichever chapters happen to be converted so far.

This file does two jobs at once:
- **Entry point** — a reader (human or chatbot) starting from "what does this council's DCP
  cover" lands somewhere that matches the source structure, not an ad hoc grouping.
- **Progress tracker** — mark each chapter's status (not started / in progress / done) so
  it's obvious what's missing without cross-checking the folder tree. Don't create a folder
  for a chapter until there's a converted file to put in it — an empty folder implies
  something has started when it hasn't.

Don't assume every chapter follows the same internal pattern as the first one converted.
Check each chapter's own scope (LGA-split or council-wide, single section or many) before
deciding its folder shape — Chapter 5 splitting by former LGA doesn't mean Chapter 6 will.

## Folder structure

```
/{document-type}/{council}/{former-lga-or-scope}/
```

Examples:
- `/dcp/canterbury-bankstown/former-bankstown-lga/`
- `/dcp/cumberland/`  (single LGA, no former-LGA split needed)
- `/lep/parramatta/`
- `/sepp/sepp-exempt-complying/` (state-wide, no council folder)

Use `former-lga-or-scope` only where the source document itself splits by former LGA
(common post-amalgamation, e.g. Canterbury-Bankstown, Cumberland, Georges River). If the
document applies council-wide, omit that folder level.

## File naming

One file per **section** of the source document (not per clause — sections are usually
already well-scoped; splitting finer fragments cross-references unnecessarily).

`{NN}-{kebab-case-section-title}.md`

- Zero-pad the number (`01-`, `02-`, … `15-`) so files sort correctly in a plain directory
  listing.
- Keep the slug short but unambiguous — drop filler words ("in Residential Zones" →
  omit if the parent folder already scopes to residential).
- **Cap slugs at ~50 characters**, even when the source section title is long. Several
  folder levels deep (`dcp/{council}/{chapter}/{scope}/{sub-document}/{file}.md`) plus a
  user's own local repo path can exceed Windows' 260-character path limit, causing
  "Path too long" errors on extract/copy. Long section titles should be shortened to
  their key terms rather than transcribed in full — e.g. "Incentives for Conversion of
  First Floor Space to Residential Accommodation in Hurlstone Park Village Centre"
  → `19-hurlstone-park-first-floor-incentives.md`, not a verbatim slug of the whole
  title. The full title still belongs in the file's front matter and its `# Heading`,
  where length doesn't cause filesystem problems — only the filename needs trimming.

### When to nest a document in its own folder vs keep it as a flat file

Councils often publish DCP chapters as separate numbered sub-documents (e.g. "Chapter 5.1",
"Chapter 2.1", "Chapter 2.2") rather than one giant chapter file. Treat each numbered
sub-document (X.Y) as the conversion unit.

- **If the sub-document has 2+ internal sections** (like Chapter 5.1's 15 sections), give it
  its own folder named after the LGA/scope (e.g. `former-bankstown-lga/`), with one file per
  section inside, plus `_index.md`.
- **If the sub-document has only 1 internal section** (like Chapter 2.1's single "Site
  analysis plans" section), don't wrap it in its own folder — keep it as a single flat file
  named `{X.Y}-{kebab-case-title}.md` directly inside the LGA/scope folder (or `general/` if
  the chapter isn't LGA-specific). Forcing a folder around a one-section document just adds
  a click for no retrieval benefit.
- **Sibling sub-documents under the same chapter number** (2.1, 2.2, 2.3, 2.4 all under
  "Chapter 2 — Site Considerations") share a chapter grouping but don't need a shared
  subfolder unless the scope folder is getting crowded — a shared `_index.md` noting they're
  siblings is enough.

Every chapter/document folder also gets:
- `_index.md` — one-paragraph summary + a table linking every section file. This is what
  gets fed to the model first when it needs to know "what's in this chapter" before
  drilling into content.
- `appendices/_index.md` — if the source has maps, plans, or other non-text appendices,
  note what they are and what clauses reference them, even before they're converted to
  image assets. Never silently drop an appendix.

## Front matter schema

Every section file starts with this YAML block. Keep field names identical across all
documents — this is what makes cross-document filtering possible later.

```yaml
---
title: "Section N — Section Title"
council: <council name>
former_lga: <former LGA name, or omit if not applicable>
document_type: DCP | LEP | SEPP | Code
chapter: "<chapter number as printed>"
section: "<section number as printed>"
clause_range: "<first clause>-<last clause>"
effective_date: <YYYY-MM-DD, from source document date if known>
amended_date: <YYYY-MM-DD, if source shows an amendment date>
last_verified: <YYYY-MM-DD, the date this file was created/checked>
zones: [R2, R3, R4, ...]   # every zone this section's controls apply to
tags: [topic keywords, lowercase, kebab-case]
---
```

If a date or field genuinely isn't available in the source, omit the field rather than
guessing — a missing field is safer than a wrong one.

## Content rules

- **Preserve clause numbers exactly as printed**, including any numbering errors in the
  source (e.g. duplicate clause numbers). Add a short note flagging the anomaly rather than
  silently renumbering — silent renumbering breaks anyone cross-referencing the original
  PDF or citing a clause number to Council.
- **Convert tables to markdown tables.** Don't paraphrase table data into prose.
- **Preserve full clause text.** This is regulatory content the business relies on for
  compliance — summarising or lightly paraphrasing clauses is not acceptable here, unlike
  general web content.
- **Note but don't attempt to convert image-only content** (maps, figures, diagrams).
  Reference them by name/number in an inline note (`> See Figure 7a in the source PDF`) so
  a reader knows something is missing, and log them in the folder's `appendices/_index.md`
  or a `## Figures` section at the end of the file if they're referenced by specific clauses.
- **Cross-reference related sections** where the source does (e.g. Section 6 → Section 15 on
  basements) using relative markdown links.

## Quality check before committing

- [ ] Every clause number from the source appears in the output
- [ ] Every table converted, not summarised
- [ ] Front matter zones match what the section's setback/height clauses actually say
- [ ] Appendices/figures noted, not silently dropped
- [ ] `_index.md` table links to every section file and the links aren't broken
