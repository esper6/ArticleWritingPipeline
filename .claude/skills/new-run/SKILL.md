---
name: new-run
description: Archive all stage content and topic brief as a zip, clear stages, and reset for a new topic
user-invocable: true
---

Start the pipeline fresh for a new article topic. Archive everything from the current run as a zip before clearing.

## What gets archived

Everything in `stages/` and `setup/topic-brief.md` **except** structural files that are part of the repo skeleton:
- `stages/*/CONTEXT.md`
- `stages/*/ARCHITECTURE.md`
- `stages/*/README.md`
- `stages/*/output/.gitkeep`

All other files — user-supplied (PDFs, drafts, reading notes) and pipeline-generated (research brief, scope, outline, editorial notes, prose notes) — go into the archive. This preserves a complete snapshot of the run.

## Steps

1. Scan `stages/` and `setup/topic-brief.md`. List every non-structural file that will be archived. If there are no files to archive (empty pipeline), tell the user and stop.

2. Summarize what will happen:
   - **Archived** to `archive/YYYY-MM-DD_HHMMSS.zip`: list all files that will be included
   - **Cleared**: all non-structural files in `stages/` deleted
   - **Reset**: `setup/topic-brief.md` replaced with blank template

3. Ask the user to confirm: "This will archive [N] files to `archive/YYYY-MM-DD_HHMMSS.zip`, clear all stages, and reset topic-brief.md. Proceed?"

4. If confirmed:
   a. Create the `archive/` directory if it doesn't exist
   b. Collect all non-structural files into a temporary staging folder (preserving their paths relative to the project root), then zip it. Use `powershell.exe -Command "Compress-Archive ..."` to create the zip (this is a Windows environment without `zip` CLI). The zip file goes to `archive/YYYY-MM-DD_HHMMSS.zip`. Clean up the temporary staging folder after zipping.
   c. Verify the zip was created and is non-empty
   d. Delete all non-structural files from `stages/` (everything except CONTEXT.md, ARCHITECTURE.md, README.md, and output/.gitkeep). If a file can't be deleted (locked by another process), note it to the user but continue.
   e. Delete all files in `stages/*/output/` except `.gitkeep`
   f. Rewrite `setup/topic-brief.md` with this blank template exactly:

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

5. Tell the user the pipeline is reset. Remind them to fill in `setup/topic-brief.md`, then run `/run-stage 1` when ready.
