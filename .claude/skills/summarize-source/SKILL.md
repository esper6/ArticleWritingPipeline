---
name: summarize-source
description: Paste in an article, paper, or thread and get a structured summary formatted for the reading notes file
user-invocable: true
---

Summarize a source and format the result for reading-notes.md.

1. Read `stages/01_research/output/research-brief.md` to understand the current topic's key questions and sub-topics.
2. Ask the user to paste the source material (or provide it in $ARGUMENTS if they already have).
3. Produce a structured summary with these sections:
   - **Source:** title, author, type (article / paper / documentation / other), and URL or reference if known
   - **Key claims:** 3–7 bullet points of the main arguments or findings
   - **Evidence and support:** what the source uses to back its claims (data, examples, citations, reasoning)
   - **Relevance to this article:** which key questions from the research brief this source helps answer — be specific
   - **Gaps or caveats:** anything the source doesn't cover, oversimplifies, or where it has a clear bias
4. Tell the user: "Copy this into `stages/01_research/output/reading-notes.md`. Run `/gap-check` when you've added all your sources to see what's still missing."
