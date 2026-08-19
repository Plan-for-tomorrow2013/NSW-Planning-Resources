Convert the planning document PDF at the path given in $ARGUMENTS into this repo's
markdown structure, following `CONVERSION_GUIDE.md` at the repo root exactly.

Steps:

1. Read `CONVERSION_GUIDE.md` in full before doing anything else — it defines the folder
   structure, file naming, front-matter schema, and content rules. Do not deviate from it.
2. Read the source PDF at the path in $ARGUMENTS.
3. Identify: the document type (DCP/LEP/SEPP/Code), the council, the former LGA if
   applicable, the chapter number/title, and the full list of sections.
4. Determine the target folder path per the guide's folder structure rules. If a folder
   for this council/LGA doesn't exist yet, create it.
5. Create `_index.md` for the chapter/document (or update it if converting an additional
   chapter into an existing council folder) with a summary and a table linking every
   section file.
6. Convert each section into its own file per the naming and front-matter rules. Preserve
   clause numbers, tables, and full clause text exactly — do not paraphrase or summarise
   regulatory content.
7. If the document has non-text appendices (maps, plans), create or update
   `appendices/_index.md` describing what's missing and which clauses reference them.
   Do not skip this step even if no images can be extracted.
8. Once all files are created, run through the "Quality check before committing" checklist
   in `CONVERSION_GUIDE.md` and report any items that failed, rather than silently
   proceeding.
9. Give a short summary: how many sections were converted, the folder path used, and
   anything flagged in the quality check (missing dates, ambiguous clause numbers,
   appendices not yet converted).

Do not commit or push to git — leave that to the user to review first.
