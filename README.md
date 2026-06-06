# CCA-F Exam Prep — Claude Code Skill

A repeatable system for passing the Anthropic **Claude Certified Architect – Foundations (CCA-F)** exam.

## What this is

A Claude Code (or Cowork) skill that runs a learner through CCA-F prep using a validated study system:

- **Explain → Feynman → Quiz → Notes** loop per concept
- **Spaced-repetition** learning log (intervals based on recall confidence)
- **Distractor-pattern library** (19 named patterns — the most reusable artifact)
- **Session opener** that surfaces what's due before any new teaching

Originally built and validated by the author: **5 days from start of study to sitting the exam** (913/1000 on the official practice exam, full pass on the real exam).

## Install

### Cowork / Claude Desktop

Open Cowork → Customize sidebar → upload this skill folder as a zip.

Then in any chat: *"let's study CCA-F"* — the skill auto-activates.

### Claude Code

Drop this folder into `.claude/skills/` of a project, or `~/.claude/skills/` for personal use.

## How a learner uses it

Once installed, start a session by saying:

- *"let's study CCA-F"*
- *"CCA-F prep"*
- *"continue my Claude Cert study"*

The skill will:

1. Check what reviews are due today
2. Drill any open watch-list items
3. Teach the next concept using the 4-step loop
4. Update your notes and learning log

Your study files live at `.tmp/cca-f-study/`. They're created automatically on first use from the templates in this skill.

## What's inside

```
cca-f-exam-prep/
├── SKILL.md                       — main instructions for Claude
├── README.md                      — this file
├── reference/
│   ├── exam-blueprint.md          — domains, weights, exam structure
│   ├── study-method.md            — the 4-step per-concept loop
│   ├── spaced-rep-rules.md        — interval rules
│   ├── distractor-pattern-library.md — 19 named patterns
│   ├── session-opener.md          — how every session starts
│   └── quiz-format.md             — scenario MCQ format + tagging
└── templates/
    ├── domain-notes-template.md   — per-domain notes skeleton
    └── learning-log-template.md   — spaced-rep log skeleton
```

## Requirements

- Access to the official Anthropic CCA-F Certification Exam Guide PDF (the skill treats this as the spine)
- A learner who wants to be pushed, not coddled
- ~1 hour per session, ~2 weeks total (varies with prior Claude experience)

## What the learner walks away with

- Per-domain study notes with consolidated learnings
- A spaced-repetition log that surfaces what to review and when
- A growing distractor-pattern library (starts with 19, grows as new patterns are named during study)
- A pass on the exam

## Adapting it

The skill is CCA-F-specific by design. The *method* (Explain → Feynman → Quiz → Notes + spaced rep + named distractor library) is generic and can be lifted into any cert prep — but this skill bundles the CCA-F-specific blueprint, sample-question references, and pattern library.

## Credit

Built and validated by Abi (CodeFreeIQ) — sat the CCA-F exam on 2026-05-30, **5 days from start of study**. Pass confirmed 2026-06-06.