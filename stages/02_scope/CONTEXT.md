# Stage 2: Scope

Distill the author's reading notes and research brief into a clear thesis, angle, and article scope — the decisions that need to be locked before an outline can be built.

## Inputs
- L4 (working): `../01_research/output/research-brief.md` — the learning map from Stage 1
- L4 (working): `../01_research/output/reading-notes.md` — the author's notes from reading sources
- L4 (working): `../../setup/topic-brief.md` — the original topic, angle, thesis, and audience

## Process

Read all three inputs in full before writing anything.

**If `reading-notes.md` is missing or empty**, stop and tell the author:
"Add your reading notes to `stages/01_research/output/reading-notes.md` before running Stage 2. Paste in your notes freeform, or use `/summarize-source` to structure notes from sources you've read."

---

Build the scope document as a structured set of decisions:

**1. Thesis**
State the article's core claim in one sentence. If the topic brief already has a thesis, sharpen it using what the author learned from reading. If not, propose one based on the strongest thread in the reading notes. Mark it clearly as either **refined** (from the topic brief) or **proposed** (new, based on reading).

**2. Angle**
One paragraph describing the specific lens the article takes. This is not the topic — it's what makes this article different from every other article on the same topic. Ground it in what the reading notes revealed, not just the original brief.

**3. Scope boundaries**
Two lists:

- **In scope** — the specific sub-topics, questions, and concepts this article will cover. Pull from the research brief's sub-topics and key questions, filtered by what the reading notes actually support. Each item gets one sentence explaining why it earns space in the article.
- **Out of scope** — things the reader might expect to see but that this article deliberately excludes. Each item gets one sentence explaining why it's cut (tangential to the thesis, insufficiently supported by reading, better suited to a separate piece, etc.).

**4. Audience contract**
2–3 sentences describing what the reader will walk away understanding. This is the promise the article makes — every section in the outline should serve it.

**5. Open questions for the author**
List any decisions the scope depends on that only the author can make. Examples: "The reading notes cover both X and Y in depth — which thread do you want to lead with?" or "The thesis could go either direction on [debate] — which side are you arguing?" Keep to 0–3 questions. If there are none, omit this section.

---

Close the output with this note:

> **Next step:** Review the scope above. Adjust anything that doesn't match your intent — this is your article, not the pipeline's. When the scope feels right, run Stage 3 to generate the outline.

## Outputs
- `scope.md` → output/
