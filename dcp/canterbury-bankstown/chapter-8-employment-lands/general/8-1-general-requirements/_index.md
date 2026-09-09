---
title: "Chapter 8.1 — General Requirements"
council: Canterbury-Bankstown
document_type: DCP
chapter: "8.1"
last_verified: 2026-09-01
status: converted
---

## Chapter 8.1 — General Requirements

June 2023 (Amended April 2025). Applies council-wide across the whole of Chapter 8
(Employment Lands) — Section 2 applies specifically to Zone E3 (Productivity Support
Precinct) and Section 3 applies specifically to Zone SP4 (Enterprise Precinct, the former
Potts Hill Reservoirs site); Sections 1 and 4 apply to both. No former-LGA split — confirmed
from the document's own explanatory text, which frames everything by zone (E3/SP4)
rather than by former Bankstown/Canterbury LGA.

| Section | File | Clause range |
|---|---|---|
| 1 — Introduction | [01-introduction.md](./01-introduction.md) | Objectives O1–O3 (no numbered clauses) |
| 2 — Productivity Support Precinct | [02-productivity-support-precinct.md](./02-productivity-support-precinct.md) | 2.1–2.40 |
| 3 — Enterprise Precinct | [03-enterprise-precinct.md](./03-enterprise-precinct.md) | 3.1–3.3 |
| 4 — Site Facilities | [04-site-facilities.md](./04-site-facilities.md) | 4.1–4.6 |

Figures: see [appendices/_index.md](./appendices/_index.md) (1 figure, not yet converted).

### Anomalies flagged during conversion

1. **No amendment/gazettal table in the source.** Unlike Chapter 1.1, this PDF has no
   revision-history section, so the "Amended April 2025" date on the cover/footers
   can't be cross-checked against a clause-level table. `effective_date`/`amended_date`
   front-matter fields were omitted rather than guessed at day-level precision — see
   the note at the top of `01-introduction.md`.
2. **Objective wording mismatch (Section 2).** Objectives O4 and O7 in Section 2
   (Productivity Support Precinct) both refer to "the enterprise corridors" rather than
   "the productivity support precinct," and clauses 2.7(a)/(b) do the same. This reads
   like boilerplate carried over from another chapter's drafting template rather than an
   error specific to this conversion — flagging rather than silently correcting, per the
   conversion guide. Worth checking whether the same "enterprise corridors" phrasing
   turns up in Chapter 7's precinct DCPs (7.5/7.6/7.7) when reconciling cross-chapter
   template issues, per the top-level index's existing note about that pattern.
3. **Section 2 residential/serviced-apartment provisions inside an employment-lands
   chapter.** Clauses 2.2(a), 2.22, 2.26, 2.32(a)–(f), and the full Serviced apartments
   subsection (2.36–2.40) all regulate residential dwellings, private open space, and
   serviced apartments even though this chapter's own Section 1 explanation describes
   the precinct as primarily commercial/urban-services land. This matches Section 1's
   own C1 desired-character note that "certain key development sites may accommodate
   certain residential uses only as part of mixed use development" — so it's consistent
   with the source, not an error, but worth a chatbot-facing note since a query like
   "residential rules in Chapter 8" would otherwise seem out of place for an employment
   lands chapter.
4. **Clause 3.2 incorporates an external document by reference** (the 2008 Potts Hill
   Reservoir Business Park Design Guidelines) that was not supplied for conversion —
   see `03-enterprise-precinct.md` and `appendices/_index.md`.
5. No duplicate or missing clause numbers were found (2.1–2.40, 3.1–3.3, 4.1–4.6 are
   all sequential and complete).
