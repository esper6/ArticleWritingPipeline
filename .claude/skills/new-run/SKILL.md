---
name: new-run
description: Clear all stage outputs and reset the topic brief so the pipeline can be run on a new topic
user-invocable: true
---

Start the pipeline fresh for a new article topic.

1. List every file currently in any stage output/ folder (all stages/0N_*/output/ folders), excluding .gitkeep files. Also note whether setup/topic-brief.md has content filled in.

2. Summarize what will be erased:
   - All stage output files (research-brief.md, reading-notes.md, outline, editorial notes, etc.)
   - The topic brief content (replaced with a blank template)

3. Ask the user to confirm: "This will delete [list files] and reset topic-brief.md. Proceed?"

4. If confirmed:
   a. Delete all output files except .gitkeep files
   b. Rewrite setup/topic-brief.md with this blank template exactly:

```
# Topic Brief

Fill this in before each run. The more specific your angle and thesis, the more focused the learning map and outline will be. Leave any section blank — Stage 1 will note what's missing and make reasonable assumptions.

---

## Topic
<!-- What is the subject you want to write about?
     Examples:
       "The attention mechanism in transformer models"
       "Why most companies fail at building internal tools"
       "What Gödel's incompleteness theorems actually say and don't say" -->


## Angle
<!-- What specific lens or perspective do you want to take on this topic?
     Examples:
       "Focus on the intuition behind why attention works, not the full history"
       "From the perspective of a developer who has tried and failed at this"
       "Aimed at someone who knows basic logic but hasn't studied computability" -->


## Thesis (if you have one)
<!-- What's the core claim the article makes?
     Leave blank if you don't have one yet — the research stage often helps surface it.
     Examples:
       "Attention works because it decomposes the problem differently, not because it's 'smarter'"
       "Internal tools fail because the incentive to maintain them disappears once they work" -->


## Audience
<!-- Who is this for? What do they already know?
     Examples:
       "Technically literate readers who don't work in ML"
       "People in the industry who know the problem but haven't said, there are many"
       "Primarily myself — writing to solidify my understanding" -->


## Depth preference
<!-- How deeply do you want to go? Affects how the learning map is scoped.
     Surface  — introduce the topic and key concepts, no technical detail
     Medium   — explain the mechanisms, cover key debates, some technical depth where it matters
     Deep     — go into the weeds: how it works, where it breaks, edge cases and exceptions -->


## Prior knowledge or context
<!-- What do you already know? What have you already read on this topic?
     Stage 1 uses this to avoid covering ground you've already covered.
     Leave blank if you're starting fresh. -->
```

5. Tell the user the pipeline is reset. Remind them to fill in setup/topic-brief.md, then run /run-stage 1 when ready.
