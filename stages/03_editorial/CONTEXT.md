# Stage 3: Editorial

Review the author's draft and give specific, located editorial notes. No rewrites. No prose suggestions. Flag what's structurally or conceptually unclear so the author can fix it in their own way.

## Inputs
- L4 (working): `draft.md` — the author's draft, placed in this stage's folder (not in output/)
- L4 (working): `../02_outline/output/outline.md` — the article structure from Stage 2
- L3 (reference): `../../_config/writing-conventions.md` — editorial criteria and what to flag

## Process

**If `draft.md` is missing or empty**, stop and tell the author:
"Write your article and save it as `stages/03_editorial/draft.md`, then run Stage 3."

Read all three inputs in full before writing any notes.

---

Produce editorial notes as a structured document:

**Header line**
One sentence: "Editorial notes for '[working title]' — approximately [word count] words, [read time] min read."

**Overall structure**
2–3 sentences: does the draft follow the outline's arc? Does the overall structure work? Note any major departures from the outline — not as problems, but as things the author should be aware of. Intentional departures are fine; the author should know when they've diverged.

**Section-by-section notes**
Work through the draft section by section, applying the editorial criteria from `writing-conventions.md`.

Only write a note when there's something to flag. If a section has no issues, skip it entirely — the absence of a note means the section is clear. Do not write "Section X looks good."

For each issue flagged:
- Location: section name and paragraph number
- Issue type: use the exact category names from `writing-conventions.md` (dead-end thought, meandering section, buried point, unexplained concept, conceptual gap, structural mismatch)
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
