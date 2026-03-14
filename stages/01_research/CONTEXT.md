# Stage 1: Research

Build a learning map for the topic — a structured study guide that helps the author know what to read, what questions to answer, and what to watch for when reading sources.

## Inputs
- L4 (working): `../../setup/topic-brief.md` — topic, angle, thesis, audience, and depth preference for this run

## Process

Read `topic-brief.md` in full. Note the topic, angle, thesis (if given), audience, and depth preference before writing anything.

If the topic brief is blank or very sparse, produce the learning map anyway using reasonable assumptions, and note each assumption clearly at the top of the output.

---

Build the learning map as a structured document with these sections:

**1. Core concepts**
List the fundamental concepts the author needs to understand to write about this topic with confidence. For each concept, write one sentence: what it is and why it matters for this topic's angle. Only include concepts that are load-bearing for the article — skip background knowledge the audience likely already has.

**2. Sub-topics to explore**
List the distinct threads within the topic worth exploring separately. For each sub-topic:
- One sentence on what question it answers
- Whether it's central to the thesis or peripheral (peripheral = worth knowing but doesn't need to be in the article)
- The depth level at which it becomes useful: surface / medium / deep

Calibrate the list to the depth preference in the topic brief. A surface-level article doesn't need sub-topics that only matter at depth.

**3. Key questions**
List the specific questions the author should be able to answer after reading. These function as a test: if the author can answer all of them, they understand the topic well enough to write about it. Aim for 5–10 questions. Make them concrete — not "understand X" but "why does X behave differently from Y under condition Z?"

**4. Debates and open questions**
List significant debates, contested claims, or open problems in this topic:
- What the positions are (briefly)
- Why the debate exists
- Whether it's relevant to the author's angle

Omit this section if the topic has no meaningful debates — not every topic does.

**5. Common misconceptions**
List 2–4 things people commonly get wrong about this topic, especially things the author might encounter in sources. This helps the author read critically.

**6. Suggested source types**
Recommend kinds of sources worth reading — not specific URLs, but categories:
- Most reliable for core concepts (e.g. textbooks, foundational papers, official documentation)
- Most useful for context and debates (e.g. practitioner essays, retrospectives)
- Sources to treat with caution and why (e.g. introductory blog posts that over-simplify, advocacy writing with a position to defend)

**7. Scope note**
If the topic brief's angle or depth implies the article should stay narrower or broader than the learning map suggests, say so in one paragraph. This is a flag for the author, not a directive.

---

Close the output with this note:

> **Next step:** Go read. When you're done, create `stages/01_research/output/reading-notes.md` and paste in your notes, excerpts, or summaries from what you read. Then run Stage 2.
>
> Use `/summarize-source` to paste in an article or paper and get a structured summary formatted for your reading notes.
> Use `/gap-check` to check whether your notes cover all the key questions before outlining.

## Outputs
- `research-brief.md` → output/
