# Stage 3: Outline

Turn the locked scope, reading notes, and learning map into a clear article structure — section by section, with what each section needs to cover and where visual aids would help.

## Inputs
- L4 (working): `../02_scope/output/scope.md` — the locked thesis, angle, and scope boundaries from Stage 2
- L4 (working): `../01_research/output/research-brief.md` — the learning map from Stage 1
- L4 (working): `../01_research/output/reading-notes.md` — the author's notes from reading sources
- L3 (reference): `../../_config/writing-conventions.md` — length guidance and visual aid annotation format

## Process

Read all four inputs in full before writing anything.

**If `scope.md` is missing or empty**, stop and tell the author:
"Run Stage 2 first to lock down the article's scope, then run Stage 3."

**If `reading-notes.md` is missing or empty**, stop and tell the author:
"Add your reading notes to `stages/01_research/output/reading-notes.md` before running Stage 3. Paste in your notes freeform, or use `/summarize-source` to structure notes from sources you've read."

---

Build the outline as a structured document:

**Opening line**
One sentence: "This outline covers [topic] from [angle], making the case that [thesis]." Pull the angle and thesis from `scope.md`, not the original topic brief.

**Article arc**
3–5 sentences describing the overall shape of the article: what it establishes first, how it builds, and what it lands on. This is the narrative logic — not a list of sections, but the reason the sections are in this order.

**Sections**
For each section:
- **Section title** — a working title (the author will revise it)
- **Role in the arc** — one sentence on what this section does in the overall argument
- **What it needs to cover** — 2–5 bullet points of specific concepts, claims, or questions this section should address. Pull directly from the reading notes and scope document. Only include items that are **in scope**.
- **Visual aid** — if a visual would genuinely help comprehension, add a `[VISUAL: description]` callout per `writing-conventions.md`. Omit if no visual is needed.
- **Estimated length** — short (1–3 paragraphs) / medium (4–6) / long (7+), based on how much genuine explanation the content requires

Aim for 4–7 sections. Fewer for surface-depth topics; more only when the depth genuinely warrants it and each section has a distinct role. Respect the scope boundaries — do not outline sections for topics marked out of scope.

**Gaps**
List any in-scope items from `scope.md` that the reading notes don't adequately support. For each: name the item, describe what's missing, and suggest what type of source might fill it. If there are no gaps, write: "None — reading notes cover all in-scope items."

**Length estimate**
Total up the section estimates and give a rough word count range and read time. Flag if the estimate is outside the 750–3,750 word / 3–15 min range from `writing-conventions.md`.

---

Close the output with this note:

> **Next step:** Review this outline. If there are gaps listed above, decide whether to fill them before writing or address them in the article itself. When the structure makes sense to you, write your article and save it as `stages/04_editorial/draft.md`. Then run Stage 4.

## Outputs
- `outline.md` → output/
