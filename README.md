# Article Writing Pipeline

This workspace helps you research, outline, and write deeply-considered articles on topics you care about. The pipeline builds your learning map, shapes your outline, and gives editorial feedback on your draft. You do all the writing — the output is a personally written article, not a generated one. Understanding is the point; publishing is the byproduct.

---

## Before you run anything

Complete the one-time setup before your first run: read `setup/configure.md` and follow the checklist there. It takes five minutes and only needs to happen once.

---

## How it works each time

1. Fill in `setup/topic-brief.md` with your topic, angle, and thesis
2. Run the stages in order

| Stage | What the pipeline does | What you do after |
|---|---|---|
| 1 — Research | Builds a learning map: key concepts, questions to answer, debates to understand, source types to read | Go read. Paste your notes into `stages/01_research/output/reading-notes.md` |
| 2 — Outline | Turns your reading notes into a section-by-section article structure with visual aid callouts | Review the outline, fill any remaining gaps, then write your article and save it as `stages/03_editorial/draft.md` |
| 3 — Editorial | Reviews your draft for gaps, dead-end thoughts, and structural issues — notes only, no rewrites | Read the notes and revise where it matters to you |

---

## What you get at the end

`stages/03_editorial/output/editorial-notes.md` — specific, located feedback on your draft. You decide what to act on.

---

## Files

| File | What it's for |
|---|---|
| `setup/configure.md` | One-time setup checklist |
| `setup/topic-brief.md` | Fill in before each run |
| `_config/writing-conventions.md` | Editorial criteria, length guidance, visual aid format — edit to change how the pipeline behaves |
| `stages/01_research/output/research-brief.md` | Learning map produced by Stage 1 |
| `stages/01_research/output/reading-notes.md` | Your notes from reading — you create and fill this between Stage 1 and Stage 2 |
| `stages/02_outline/output/outline.md` | Article structure produced by Stage 2 |
| `stages/03_editorial/draft.md` | Your article — you write this and place it here before running Stage 3 |
| `stages/03_editorial/output/editorial-notes.md` | Editorial feedback produced by Stage 3 |

---

## Skills

| Skill | What it does |
|---|---|
| `/run-stage [N]` | Run a specific stage of this pipeline |
| `/pipeline-status` | Show which stages are done and what's next |
| `/reset-stage [N]` | Clear a stage's output so you can re-run it |
| `/summarize-source` | Paste in an article, paper, or thread — get a structured summary formatted for your reading notes |
| `/gap-check` | Check whether your reading notes cover all the key questions from the research brief |

### Typical flow

```
Fill in setup/topic-brief.md

/run-stage 1    → review research-brief.md
                → go read sources
                → paste notes into stages/01_research/output/reading-notes.md

/gap-check      → (optional) confirm your notes cover the key questions

/run-stage 2    → review outline.md, confirm the structure makes sense
                → write your article
                → save it as stages/03_editorial/draft.md

/run-stage 3    → review editorial-notes.md
                → revise your draft as you see fit
```

### If something needs rework

```
/reset-stage [N]    → edit the intake or previous output
/run-stage [N]      → re-run the stage
```

### Conditional skills

These aren't included by default. Add them if you find you need them:

| Skill | When it's useful | How to add |
|---|---|---|
| `/retry-with-note` | When a stage output misses the mark and you want to re-run with a one-time redirect, without editing the stage contract permanently | Create `.claude/skills/retry-with-note/SKILL.md` and ask your agent to generate it using the domain skill template from the MWP skills catalog |
| `/headline-variants` | When you want title options after writing — not for SEO, just to find the framing that best reflects what the article actually says | Create `.claude/skills/headline-variants/SKILL.md` and ask your agent to generate it |
