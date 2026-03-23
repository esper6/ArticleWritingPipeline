# Stage 4: Conceptual Review

Check whether the draft covers the outline's points and whether the overall arc holds. This stage is about what the article says, not how it says it. Prose-level feedback happens in Stage 5.

## Inputs
- L4 (working): `draft.md` — the author's draft, placed in this stage's folder (not in output/)
- L4 (working): `../03_outline/output/outline.md` — the article structure from Stage 3
- L3 (reference): `../../_config/writing-conventions.md` — conceptual review criteria

## Process

**If `draft.md` is missing or empty**, stop and tell the author:
"Write your article and save it as `stages/04_editorial/draft.md`, then run Stage 4."

Read all three inputs in full before writing any notes.

---

Produce editorial notes as a structured document:

**Header line**
One sentence: "Editorial notes for '[working title]' — approximately [word count] words, [read time] min read."

**Overall structure**
2–3 sentences: does the draft follow the outline's arc? Does the overall structure work? Note any major departures from the outline — not as problems, but as things the author should be aware of. Intentional departures are fine; the author should know when they've diverged.

**Section-by-section notes**
Work through the draft section by section, applying only the conceptual criteria from `writing-conventions.md`: conceptual gap and structural mismatch.

Only write a note when there's something to flag. If a section has no issues, skip it entirely — the absence of a note means the section is clear. Do not write "Section X looks good."

For each issue flagged:
- Location: section name and paragraph number
- Issue type: use the exact category names from `writing-conventions.md` (conceptual gap, structural mismatch)
- One sentence describing the specific problem
- One sentence suggesting how the author might address it — but do not write the fix

**Conceptual coverage check**
Compare the draft against the "What it needs to cover" bullets in the outline. For each bullet that doesn't appear in the draft, flag it as a question: "The outline included [X]. It doesn't appear in the draft — was this intentional?"

If all outline bullets are covered, write: "All key points from the outline are present in the draft."

**Visual aids**
List any `[VISUAL: ...]` callouts from the outline that don't appear in the draft. For each: "The outline recommended a visual for [description]. Not in draft — include if relevant."

If all visual callouts are accounted for, omit this section.

**Closing line**
One sentence: "[N] notes above. Address what matters to you — these are observations, not requirements."

---

Do not rewrite or rephrase anything. All feedback must be observations and questions. The author's voice is theirs.

## Outputs
- `editorial-notes.md` → output/
