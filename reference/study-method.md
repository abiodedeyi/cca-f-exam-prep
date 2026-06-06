# Study Method — Per-Concept 4-Step Loop

For every task statement / concept, run this loop in order. Do not skip steps. Do not let the learner skip steps.

## Step 1: Explanation

Teach the concept clearly. A good explanation includes:

- **A simple definition in the learner's frame** — not the official guide's verbatim text
- **An analogy** that anchors the underlying mechanism (e.g., "lock vs. sign" for programmatic enforcement, "drawer labels" for tool descriptions)
- **The official mechanism with exact names** — when the guide uses a specific term (a parameter name, a config key, a flag), use that exact term
- **Anti-patterns the exam dangles as distractors** — name them with their pattern from `distractor-pattern-library.md`
- **Cross-domain connections** — "this echoes Concept X.Y from Domain N because…"

Cite the official guide as the spine. If you need a detail that isn't in the guide, verify it against primary Anthropic docs before stating it as fact. Never fabricate.

## Step 2: Feynman Test (open recall)

Ask the learner to explain, *in their own words, with no options and no looking up*, the key parts of the concept. Usually three questions:

1. **The core mechanism** — what is it, how does it work
2. **A specific failure mode or distractor pattern** — name a way it goes wrong
3. **A cross-domain connection or named principle** — tie it to something they already know

After they answer:

- **Be honest about gaps.** State plainly what they nailed and what they missed.
- **Fill in missing pieces precisely.** Don't paraphrase — use the official names for the mechanisms and parameters.
- **Sharpen vague answers.** "Right idea, but the precise framing is…"

The learner does NOT get to claim "I had that, I just didn't say it." If they didn't say it, they didn't have it. That's the whole point of open recall.

## Step 3: Quiz (exam-style MCQ)

Pose ONE scenario-based MCQ per concept. See `quiz-format.md` for the exact format. Required elements:

- A realistic scenario (2-3 sentences with concrete details — percentages, numbers, file paths)
- Four answer options — three are plausible distractors
- Ask the learner to (a) pick a letter, (b) give a one-line "why", (c) **tag each distractor with a named pattern**

Critical:

- **Vary the position of the correct answer across the curriculum.** Don't always make A correct. Distribute across A/B/C/D.
- **Each distractor maps to a named pattern** from the library. If you can't think of one, you've designed a weak distractor — rewrite it.
- **The bonus tagging is non-negotiable** — gently push back when the learner skips it. The exam IS multiple choice; tagging is how you eliminate distractors fast under time pressure.

## Step 4: Notes

Consolidate the concept into the learner's domain notes file. Append a `Final Notes (consolidated)` section under the task-statement heading with:

- The concept's definition, mechanism, and trigger phrase if applicable
- Fixes / right answers for the canonical scenarios
- Distractor watch — which patterns the exam dangles around this concept
- Quiz result (question summary, learner's answer, your confidence rating)
- Cross-domain echoes

Mark the task-statement checkbox done.

Add a row to `learning-log.md` for this concept with its next review date (per `spaced-rep-rules.md`).

## When the learner is going fast

If a learner is breezing through (clean Feynman + correct quiz + accurate tags every concept), continue the pace but **don't dilute the rigor**. They're still going to encounter their first wall — the goal is to find it before exam day, not after.

## When the learner is struggling

If they're missing repeatedly:

- Slow down. Re-teach with a different analogy.
- Drop the next-due interval to Weak (1 day) for the affected concept.
- Don't move to the next concept until the current one is at least Hesitant.
- Be encouraging about the system working as designed — catching gaps IS the value.