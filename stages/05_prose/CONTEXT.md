# Stage 5: Prose Review

Review the draft at the sentence and paragraph level. Flag structural problems in the prose — dead ends, buried points, repetition, unclear references, weak transitions. This stage is about how the article reads, not what it covers (that was Stage 4).

## Inputs
- L4 (working): `../04_editorial/draft.md` — the author's draft (same file as Stage 4, updated after conceptual review)
- L3 (reference): `../../_config/writing-conventions.md` — prose review criteria

## Process

**If `../04_editorial/draft.md` is missing or empty**, stop and tell the author:
"No draft found. Complete Stages 1–4 first."

Read both inputs in full before writing any notes. Do not reference the outline — this stage evaluates the draft on its own terms.

---

Produce prose notes as a structured document:

**Header line**
One sentence: "Prose notes for '[working title]' — [N] sections, [word count] words."

**Section-by-section notes**
Work through the draft section by section, paragraph by paragraph, applying the prose criteria from `writing-conventions.md`.

Only write a note when there's something to flag. If a section has no issues, skip it entirely — the absence of a note means the prose is clean. Do not write "Section X reads well."

For each issue flagged:
- Location: section name and paragraph number (and sentence number if relevant)
- Issue type: use the exact category names from `writing-conventions.md` (dead-end thought, meandering section, buried point, unexplained concept, echo/repetition, unclear referent, weak transition)
- One sentence describing the specific problem
- One sentence suggesting how the author might address it — but do not write the fix

**Closing line**
One sentence: "[N] notes above. Address what matters to you — these are observations, not requirements."

---

Do not rewrite or rephrase anything. Do not suggest alternative wording. Do not comment on voice or tone — the author's style is theirs. All feedback must point to a specific location and name a specific structural problem.

## Outputs
- `prose-notes.md` → output/
