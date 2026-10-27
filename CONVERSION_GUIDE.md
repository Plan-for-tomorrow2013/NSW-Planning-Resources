# NSW Planning Resources — Conversion Guide

This is the standard for converting source planning documents (LEPs, DCPs, SEPPs, codes)
into the markdown structure used in this repo. Follow this exactly so every document —
regardless of which council or session converted it — ends up queryable the same way.

Most of this guide was written against DCPs and applies to any document with numbered
chapters/sections (DCPs, codes, SEPPs). **LEPs follow the same top-level philosophy — a
top-level index, one file per unit of content, preserve-don't-resolve on anomalies — but have
enough structural differences (clauses instead of sections, a Land Use Table, Schedules, a
Dictionary) that they get their own section below: see "LEP-specific conventions." Read that
section in full before starting an LEP conversion; don't assume the DCP rules transfer
one-for-one.

## DCP folder layout (automatic DCP converter, from 26 Oct 2026)

DCPs are now converted by the automatic program (run_dcp_to_md), not by hand. The master
`dcp/` folder uses the same folder names as the drop folders, so at this level it looks the
same as what was dropped in. One folder per DCP:

```
dcp/
  bayside-development-control-plan/
    _index.md                      <- the DCP index (front matter + list of chapters)
    section-05-residential-mixed-use-developments/
      _index.md                    <- chapter index: front matter, short intro, any text before
                                      the first numbered heading, ordered list of section files
      01-5-1-1-fences-and-retaining-walls-general-controls.md
      02-5-1-2-....md              <- one file per numbered section, in PDF order
      images/                      <- pictures (GIF) used by this chapter
      <council's PDF file name>.pdf <- the chapter's own PDF (moved here on publish, one copy)
  parramatta-development-control-plan-2023/
    _index.md
    <chapter folders>/
    standalone-plans/
      <stand-alone plan slug>/     <- Wentworth Point, Homebush Bay West, Carter Street
        _index.md
        <chapter folders>/
```

- Section file name: `NN-<section number>-<title>.md`, e.g. `01-5-1-1-fences-and-retaining-walls.md`
  (NN is the order in the PDF; three digits when a chapter has more than 99 files).
- Split level: the deepest numbered heading level that is used at least twice and still gives
  sensible file sizes (typical file 1.5 KB or more, at most 250 files). Unnumbered
  sub-headings stay inside their section. A numbered heading with no text of its own goes into
  the next file. A chapter with no numbered headings keeps all its text in `_index.md`.
- Section front matter: `title`, `document_id` (`<dcp>/<chapter>/<section file>`),
  `register_id`, `current_from`, `authoritative_url`.
- Pictures, maps and figures are saved as GIF pictures and tables as markdown tables, in every
  chapter type. Objective/control tables have one row per objective or control (O1 | text,
  C1 | text), with a. / b. sub-items kept with their control.
- PDFs (from 26 Oct 2026, like the LEP): every PDF that became a chapter, supporting guide or stand-alone plan
  is MOVED (one copy, the council's file name) into its folder beside `_index.md`: split sections into their
  chapter folders, unsplit chapter PDFs into their chapter folder, supporting-guide PDFs into their guide folder,
  stand-alone plan PDFs into their plan (or plan chapter) folder. The chapter `_index.md` has `source_pdf:` in its
  front matter and a visible `Source PDF: [file](file)` link under the title. Web-only parts (Camden Part 1) have
  no PDF. `DCP-processed\<drop folder>\` is the untouched archive: `manifest.xlsx` and `original-whole-pdf\`
  (the council's whole PDF exactly as dropped; re-splitting reads it from there). Re-conversions and re-checks
  read a chapter's PDF from its dcp folder.
- canterbury-bankstown-development-control-plan-2023 and gilgandra-development-control-plan-2011
  were made by the older program: they were renamed to their drop-folder names but their
  contents (including `00-index.md`) are unchanged.

The sections below are the original hand-conversion rules. Where they show council-level
paths such as `dcp/canterbury-bankstown/` or `dcp/{council}/`, read them as
`dcp/<drop folder>/` for folders made by the automatic program.

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
- `/dcp/canterbury-bankstown/general/` (chapter applies council-wide, no former-LGA split)
- `/dcp/cumberland/`  (single LGA, no former-LGA split needed)
- `/lep/parramatta/`
- `/sepp/sepp-exempt-complying/` (state-wide, no council folder)

Every chapter folder gets a `{former-lga-or-scope}` level — always present, never omitted,
so the folder shape is predictable without checking each chapter individually:
- Where the source document splits by former LGA (common post-amalgamation, e.g.
  Canterbury-Bankstown, Cumberland, Georges River), name it after the former LGA, e.g.
  `former-bankstown-lga/`, `former-canterbury-lga/`.
- Where the document applies council-wide with no former-LGA split, use the literal
  folder name `general/` rather than omitting the level. This keeps every chapter's path
  the same shape (`{chapter}/{scope}/{sub-document}/{file}.md`) whether or not that
  chapter happens to split by LGA, and gives a place to note *why* it's council-wide (in
  that folder's own `_index.md`) rather than leaving the absence of a scope folder to be
  read as "nobody checked yet." Established by Chapter 4 (Heritage) and followed by
  Chapter 8 (Employment Lands, including its corridor-specific sub-chapters 8.2 and 8.3,
  which are scoped to a named road corridor rather than a former LGA but still council-wide
  in the LGA sense).

Use `former-lga-or-scope` only where the source document itself splits by former LGA, or
use `general/` where it applies council-wide — never omit this folder level.

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
  its own folder named after the LGA/scope (e.g. `former-bankstown-lga/`, or `general/`
  where council-wide), with one file per section inside, plus `_index.md`.
- **If the sub-document has only 1 internal section** (like Chapter 2.1's single "Site
  analysis plans" section), don't wrap it in its own folder — keep it as a single flat file
  named `{X.Y}-{kebab-case-title}.md` directly inside the LGA/scope folder (or `general/` if
  the chapter isn't LGA-specific). Forcing a folder around a one-section document just adds
  a click for no retrieval benefit.
- **Sibling sub-documents under the same chapter number** (2.1, 2.2, 2.3, 2.4 all under
  "Chapter 2 — Site Considerations") share a chapter grouping but don't need a shared
  subfolder unless the scope folder is getting crowded — a shared `_index.md` noting they're
  siblings is enough.
- **The same "2+ internal sections gets its own folder" logic applies recursively** where a
  single numbered section is itself large and multi-part enough to function as its own
  mini sub-document (e.g. a site-specific precinct DCP embedded as one section of a larger
  chapter). Give that section its own folder with one file per subsection, rather than
  forcing a large multi-part section into a single file. See Chapter 8.3 Section 6 (167
  Hume Highway) for a worked example.

Every chapter/document folder also gets:
- `_index.md` — one-paragraph summary + a table linking every section file. This is what
  gets fed to the model first when it needs to know "what's in this chapter" before
  drilling into content.
- `appendices/_index.md` — if the source has maps, plans, or other non-text appendices,
  note what they are and what clauses reference them, even before they're converted to
  image assets. Never silently drop an appendix. If an appendix is genuine tabular/text
  data (e.g. a species list) rather than an image, convert it in full as its own file
  instead of only logging it here.

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
guessing — a missing field is safer than a wrong one. This includes partial dates: if the
source only gives a month/year (e.g. "Amended April 2025") with no day and no amendment
table to cross-check against, omit `effective_date`/`amended_date` entirely rather than
guessing a day.

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
- **Preserve source typos verbatim, flagged inline** (e.g. "will not be support[ed]",
  duplicated words like "from the from the") rather than silently correcting them —
  correct where it aids readability but always note that the source had an error.
- **Where a document's own clauses restart local numbering** (e.g. "C1" repeating inside
  every numbered subsection, rather than one sequential count for the whole document),
  flag this explicitly in the sub-document's `_index.md` so cross-references always cite
  the subsection along with the clause label.

## LEP-specific conventions

Standard Instrument LEPs (every NSW council's LEP since ~2010 uses the same template, the
*Standard Instrument (Local Environmental Plans) Order*) have a consistent structure that's
different enough from DCPs to need its own rules. This section was written converting
Gilgandra LEP 2011 — extend it, don't contradict it, if a later LEP reveals a new edge case.

### Folder structure

```
/lep/{council}/{part-slug}/{file}.md
/lep/{council}/schedule-{N}-{kebab-case-title}.md   (or a folder, if the schedule is large)
/lep/{council}/dictionary/{letter}.md
```

LEPs are **not LGA-split** the way some DCP chapters are — an LEP is one instrument covering
the whole council area (occasionally with a handful of site-specific savings clauses), so
there's no `general/`-vs-`former-lga/` scope folder layer here. Go straight from
`/lep/{council}/` into part folders.

A council can have more than one LEP in force at once (e.g. a principal LEP plus a separate
LEP for a specific precinct). Where that happens, each LEP gets its own folder under
`/lep/{council}/`, named after the LEP itself (e.g. `/lep/gilgandra/gilgandra-lep-2011/`,
`/lep/gilgandra/gilgandra-town-centre-lep-2015/`), with the top-level `/lep/{council}/_index.md`
listing which LEPs exist and what each covers — don't assume a council has only one.

### Top-level index

Same job as the DCP council index (entry point + progress tracker), but mirrors the LEP's own
**Contents** page: Parts in order, then Schedules in order, then the Dictionary. Note the
LEP's title exactly as printed (e.g. "Gilgandra Local Environmental Plan 2011") and its
official instrument number if shown (e.g. "[2011-641]").

### Where to get the source, and the "current version" trap

LEPs are published and kept up to date on the NSW legislation website
(legislation.nsw.gov.au). A PDF pulled from that site is **the consolidated version as currently
in force**, not the instrument as originally made — it silently folds in every amendment up
to the access date. This is a real difference from most DCP conversions, where the source PDF
is a single dated council document.

### Prefer XML (or HTML) over PDF when both are available

This is the single most important lesson from converting Gilgandra LEP 2011: **when a source
document is available from legislation.nsw.gov.au in both PDF and XML (or HTML) form, use the
XML.** This isn't specific to LEPs — it applies to any legislation.nsw.gov.au instrument
(SEPPs, Acts, regulations) and likely to other jurisdictions' structured-legislation
publishers too.

**Why PDF is the weaker source.** A PDF has no structure — it's characters positioned on a
page. Every boundary Claude needs (where one clause ends and the next begins, where a
sub-clause's numbering restarts, where a Note ends, where a dictionary entry ends) has to be
*inferred* from typographic proxies: blank lines, indentation, page breaks. Page breaks in
particular fall mid-sentence with no visual marker beyond the text simply stopping and
resuming 40 lines later — reconstructing the original sentence means guessing where the cut
was, and a plausible guess is still a guess. On Gilgandra's LEP, PDF-based extraction produced
two classes of real error, both traceable directly to this inference problem:
- The Dictionary (a 300+ term glossary with no numbering, only paragraph breaks) had several
  terms mis-split into two entries, because the pattern "*term* has the same meaning as in
  [Act]. Note: the term is defined as follows— *term* means..." looks, from blank-line
  spacing alone, exactly like two separate entries.
  One entry also had a Note inserted mid-list, in a way that confused the same paragraph-based
  heuristics.
- 13 dictionary terms were missed entirely because the regex used to detect "this paragraph
  starts a new term" didn't match their particular phrasing.

**Why XML is the stronger source.** Every clause, sub-clause, list item, note, table cell, and
dictionary entry is an explicit tagged element with a stable ID — `<tier type="subclause"
id="sec.5.10-ssec.9" status="repealed">`, `<defterm id="dict-def.relic">`, and so on. There is
no inference step: a clause is repealed because an attribute says so, not because the word
"Repealed" was pattern-matched from running text; a dictionary entry's boundary is a tag, not
a guessed paragraph break. This eliminates the exact failure class described above. XML
exports from legislation.nsw.gov.au also carry two things a PDF doesn't: a **Table of
amending instruments** and a **Table of amendments** (which clauses each instrument touched)
— genuinely useful provenance that has no PDF equivalent, worth converting into its own
reference file (see Gilgandra's `amendment-history.md`).

**What this looks like in practice**: parse the XML with a real XML parser (e.g. Python's
`lxml`, in recovery mode — legislation.nsw.gov.au XML is well-formed but large and sometimes
has minor irregularities recovery mode handles gracefully), write a small set of recursive
render functions keyed on element type (`tier`/`level`/`block`/`txt`/`list`/`note`/`table`/
`defterm`/`repealed`), and generate every file from that render pass rather than hand-copying
prose. This is not "scraping" — it's parsing a document already in hand, and it produces far
higher-fidelity output than transcription from a PDF, with less total effort once the
render functions exist, since they apply uniformly across the whole instrument.

**Reference implementation**: `tools/xml_to_md.py` is a working, tested converter for
legislation.nsw.gov.au LEP XML (`python tools/xml_to_md.py file.xml -o outdir`). It handles every
gotcha above and was regression-checked against the Gilgandra and Canterbury-Bankstown
conversions (177/178 Canterbury-Bankstown clause bodies came out byte-identical to the hand-built
versions; the one difference was Schedule 4, which the tool correctly makes a folder because its
Parts contain tables). A common mistake when writing such a tool from scratch is to search for
tags by name (e.g. BeautifulSoup `find_all("clause")`): this schema has no `<clause>`, `<part>` or
`<subclause>` tags at all, only `<level type="clause">` / `<tier type="subclause">`, so name
lookups silently match nothing and the output degrades to unstructured text.
Hand-added annotations (anomaly notes, cross-reference links to a DCP) are NOT produced by the
tool and are lost if you regenerate over a folder that carries them; re-apply them afterwards.

**Getting the XML**: legislation.nsw.gov.au's live pages are commonly protected by bot
detection that blocks direct fetches (including Claude's own web-fetch tooling). Don't attempt
to route around this with a scripted/automated fetch — the same detection applies regardless
of what's making the request, and building something designed to look like a browser risks
violating the site's terms of service. Check the site for an official bulk-download or API
path first (many legislation registers provide one precisely so people don't need to scrape).
Failing that, ask the person to download the file manually (the site does serve it to a normal
browser session) and upload it — a manual one-off download is a completely different thing
from an automated scraper.

- Record the **access/currency statement** the site prints (e.g. "Current version for 1 July
  2026 to date (accessed 21 August 2026)") in the top-level `_index.md`, verbatim, so anyone
  querying this content later knows how current it is and can check for newer amendments.
- Don't backdate `effective_date` to the LEP's original making/commencement date as printed
  in clause 1.1AA unless a specific clause's text is actually unchanged since then — for an
  amended clause, the text in front of you is the amended text, not the original. Where the
  source doesn't give you a per-clause amendment date (it usually won't), it's safer to use
  the document's stated currency date as `last_verified` and omit `effective_date` /
  `amended_date` entirely, per the existing "omit rather than guess" rule.
- Flag this in the top-level index as an open item: the person may want to know this LEP will
  drift out of date and should periodically be re-pulled and re-diffed, in a way a static DCP
  PDF doesn't.

### Clause numbering and file naming

LEP clauses are numbered `{part}.{clause}`, and clauses inserted later by amendment get a
letter suffix rather than renumbering everything after them — e.g. `1.1AA`, `4.1AA`, `5.9AA`.
**Preserve these exactly**, suffix and all; don't renumber to close the gaps and don't treat
the suffix as a typo.

- One file per clause, same "don't split finer than the source's own units, don't cram
  multiple units into one file" logic as DCP sections. A Part with many short clauses (Part 1,
  Part 3) is a flat `general`-style folder of one-file-per-clause; a Part with unusually many
  or unusually long clauses (Part 5 in a typical LEP, which can run 25+ clauses) still gets one
  file per clause — Parts don't get the DCP's "combine short sub-sections into one file"
  treatment, because each clause is independently numbered, cited, and amended, unlike a
  DCP's unnumbered sub-headings.
- File name: zero-padded source order + kebab-case clause title, same as DCP sections, e.g.
  `04-erection-of-dwelling-houses-on-land-in-certain-rural-and-conservation-zones.md` for
  clause 4.2A. Store the actual clause number (`4.2A`) in front matter, not just in the
  filename.
- **Some Standard Instrument LEPs (particularly larger urban councils') nest an extra level
  or two inside a Part**: `Part → Division → Clause`, or even `Part → Division →
  Subdivision → Clause`, where Divisions/Subdivisions are real structural units in the
  source (e.g. named precincts with their own site-specific clauses), not something this
  guide's folder conventions invented. Mirror that nesting with a folder per Division/
  Subdivision, each with its own `_index.md`, exactly like a DCP chapter's own nested
  sub-documents.
- **Path length is a real, not theoretical, constraint here — check it before treating a
  conversion as finished.** Combine deep nesting (Part/Division/Subdivision/Clause, 4 levels)
  with a long, spelled-out clause title (LEP clause titles run long — "Development at
  134-140 Brighton Avenue, Campsie" or worse) and the result can exceed Windows' 260-character
  path limit once the person's own local folder path is added on top, producing a literal
  copy-time failure ("Error 0x80010135: Path too long"), not just an ugly path. This bit a
  real conversion (Canterbury-Bankstown LEP 2023's Part 6) even though each individual
  folder/file name looked reasonable in isolation — it was the sum across four nested levels
  that broke the limit. Budget for this **before** generating files, not after: cap clause
  filename slugs at **40 characters** (tighter than a DCP chapter's ~50, because LEPs nest at
  least as deep and their own clause titles tend to run longer), and if a Part nests
  Divisions/Subdivisions, use short abbreviated folder names (`div-2-belmore-and-lakemba`,
  `sub-4-publicly-accessible`, not the full spelled-out title) — the complete, unabbreviated
  title still belongs in the file's front matter and its heading, exactly as this guide
  already says for long DCP section titles; only the filename/foldername needs trimming.
  After generating, spot-check the single longest path in the whole conversion (e.g. `find
  lep/{council} -name "*.md" | awk '{{ print length, $0 }}' | sort -rn | head`) and confirm it
  stays comfortably under 200 characters measured from the repo's own root, leaving headroom
  for however deep the person's own local folder happens to be.
- **Repealed clauses** (shown in the source as e.g. "5.9AA (Repealed)" or "6.1 (Repealed)")
  get a row in that Part's index noting "(Repealed)" but **no content file** — there's no
  substantive text to convert, and creating an empty file to hold a number violates this
  guide's existing rule against empty files. The index row is what stops a repealed clause
  from looking like a missed one.
- **"[Not adopted]" clauses** are different from repealed clauses and need different
  treatment. A Standard Instrument LEP's numbered clauses (especially 4.3 Height of
  buildings, 4.4 Floor space ratio, 4.5 Calculation of floor space ratio and site area) are
  a fixed template; a council that hasn't switched a particular standard on prints
  "[Not adopted]" under that clause heading instead of the template text. Unlike a repealed
  clause, this is live, meaningful information ("this LEP currently imposes no height
  limit") that someone querying the LEP needs to be told, not a historical artifact to
  summarise away — so a "[Not adopted]" clause **does get its own file**, stating
  "[Not adopted]" plainly, with a short note explaining what that means for anyone
  expecting to find an actual standard there.

### Front matter additions for LEP clauses

Use the same schema as DCP sections, with these LEP-specific adjustments:
- `document_type: LEP`
- `part`: the Part number and name as printed (e.g. `"5 — Miscellaneous provisions"`)
- `clause`: the clause number as printed, suffix included (e.g. `"5.9AA"`)
- `chapter` / `section` fields don't apply to LEPs — omit them rather than force-fitting a
  DCP field name onto a different structural unit.
- `zones`: still applies — many Part 4/5/7 clauses apply only to specific zones (e.g. "4.2A
  Erection of dwelling houses on land in certain rural and conservation zones"); read the
  clause's own applicability wording rather than assuming from the clause title.

### Nested sub-clause numbering

LEP clauses nest sub-provisions as `(1)`, `(2)`… then `(a)`, `(b)`… then `(i)`, `(ii)`…,
which is a different convention from the DCP's `a.`, `b.`, `i.`, `ii.` lettering. **Preserve
the source's own bracketing style** (numbers-then-letters-then-romans, all in round brackets)
rather than converting it to the DCP's lettering style — a reader cross-referencing "clause
4.2A(2)(b)" against this file needs the same bracket style to find it.

### Notes

Clause 1.5 of every Standard Instrument LEP states "Notes in this Plan are provided for
guidance and do not form part of this Plan." Convert "Note." blocks anyway (they're genuinely
useful for a chatbot answering questions), but as a clearly marked block (e.g. a markdown
blockquote headed "Note:") so it's visually distinct from the operative clause text, matching
this guide's existing convention of flagging non-operative content inline.

### Land Use Table (Part 2)

Every Standard Instrument LEP has a Land Use Table organised by zone (e.g. Zone RU1, Zone
R1, Zone E1…), each with: zone objectives, a list of land uses "permitted without consent," a
list "permitted with consent," and a list of land uses that are prohibited (implicitly:
anything not listed in the first two lists). This table is usually as long as or longer than
any single DCP chapter, so it gets its own subfolder under Part 2's folder, one file per zone:

```
/lep/{council}/part-2-permitted-or-prohibited-development/land-use-table/{zone-code}-{zone-name}.md
```

Within each zone's file:
- Convert the objectives as a lettered/bulleted list exactly as printed.
- Convert "permitted without consent" and "permitted with consent" as their own lists —
  **alphabetise or reorder nothing**; these lists are often already alphabetical in the
  source but preserve the source order regardless, since consistency with the legal
  instrument matters more than tidiness.
- The prohibited-uses list, where the LEP states it explicitly (some do, some just say "any
  other development not specified in item 2 or 3"), should be converted verbatim rather than
  computed by the converter — don't generate a "prohibited" list by inference from what's
  missing out of the permitted lists, since that's the kind of derived content this guide
  generally avoids (compare: never inventing a missing list item elsewhere in this guide).
- Record the zone code and full zone name in front matter (`zone_code: RU1`,
  `zone: "Primary Production"`) so cross-document zone filtering (e.g. matching a DCP
  chapter's `zones:` field to this LEP's land use table) works without string-matching on
  differently-formatted zone labels.

### Schedules

Convert each Schedule as its own file or folder (mirroring the DCP's "2+ items gets a
folder" rule) directly under `/lep/{council}/`, not nested inside a Part folder — Schedules
sit alongside Parts in the LEP's own Contents page, not underneath them.

- **Schedule 5 (Environmental Heritage)** deserves particular care: it's the authoritative
  list of every heritage item and heritage conservation area referenced by a DCP's heritage
  chapter (see e.g. `dcp/<drop folder>/chapter-12-non-indigenous-heritage/`). Convert its table
  (typically: item name, address, property description, significance level, item number) in
  full as a real markdown table, and cross-link it from the DCP heritage chapter's own
  `_index.md` once both exist — this is exactly the kind of cross-document link this repo
  exists to make possible.
- Site-specific schedules (Schedule 1 Additional permitted uses, Schedule 4 Classification
  and reclassification of public land) are tables keyed by lot/DP or location — convert in
  full; don't summarise "see the schedule for details," since the whole point of converting
  it is so a chatbot doesn't have to say that.

### Dictionary

The Dictionary defines every term used in the LEP and is typically alphabetical, one term per
entry, and can run to 40+ pages — far larger than any other single part of the instrument.
Splitting it into one file per Part-2-style "section" doesn't apply (there's no numbering);
instead:

- Split into one file per starting letter: `/lep/{council}/dictionary/a.md`,
  `dictionary/b.md`, etc. Skip letters with no entries rather than creating empty files.
  Where a letter has very few entries, still give it its own file — consistency of retrieval
  ("look up the D file for any D-term") matters more than avoiding a couple of small files.
- Convert every entry in full, including any "Note." explaining or cross-referencing the
  term (LEP dictionary notes very often point to a related term — "X is a type of Y, see the
  definition of that term in this Dictionary" — convert that pointer as a relative markdown
  link to the term's own entry where practical).
- Each file's front matter: `document_type: LEP`, plus `dictionary_range: "A"` (or the
  relevant letter/range) instead of `clause`/`section`.
- A term that's itself defined as "has the same meaning as in the Act" (very common) should
  be converted with that phrase preserved verbatim, plus its "Note." (which usually then
  states what the Act's definition actually is) — don't chase down and inline the Act's
  definition yourself if the LEP's own note doesn't already give it.

## Quality check before committing

- [ ] Every clause number from the source appears in the output
- [ ] Every table converted, not summarised
- [ ] Front matter zones match what the section's setback/height clauses actually say
- [ ] Appendices/figures noted, not silently dropped
- [ ] `_index.md` table links to every section file and the links aren't broken
- [ ] Scope folder (`former-{lga}/` or `general/`) is present and justified in that folder's
      own `_index.md`, based on the source's own wording rather than assumed from a
      sibling chapter (DCPs only — LEPs don't use this layer, see "LEP-specific conventions")

### LEP-specific quality check

- [ ] Repealed clauses are noted in the Part's index table and have no content file
- [ ] Clause number suffixes (AA, A, etc.) preserved exactly, not renumbered
- [ ] Sub-clause bracketing preserved as (1)/(a)/(i), not converted to DCP-style lettering
- [ ] Land Use Table converted one file per zone, with objectives/permitted-without-consent/
      permitted-with-consent as separate lists in source order, and no inferred/computed
      prohibited-use list
- [ ] Dictionary split one file per letter, every entry (including "Note." pointers) converted
- [ ] Top-level index records the source's currency/access-date statement verbatim
- [ ] Longest file path in the conversion checked and kept well under 200 characters from
      the repo root, with extra caution (shorter slugs, abbreviated Division/Subdivision
      folder names) whenever a Part nests more than the usual `Part/scope/file` depth
